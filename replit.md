# Overview

This is a Flask-based personal website for an Automation & AI Consultant. The application serves as a professional portfolio and contact platform, featuring a single-page design with sections for services, about information, and contact functionality. The site is designed to showcase expertise in workflow automation, AI integration, and systems optimization while providing a way for potential clients to get in touch.

# User Preferences

Preferred communication style: Simple, everyday language.

# System Architecture

## Frontend Architecture
- **Single Page Application**: Uses a traditional server-rendered approach with Flask templates
- **Bootstrap 5 Framework**: Provides responsive design and pre-built UI components
- **Static Asset Structure**: CSS and JavaScript files organized in Flask's standard static folder structure
- **Template Engine**: Jinja2 templating for server-side rendering

## Backend Architecture
- **Flask Framework**: Lightweight Python web framework for handling HTTP requests and responses
- **MVC Pattern**: Follows Model-View-Controller pattern with routes in app.py, templates for views, and basic form processing logic
- **Session Management**: Uses Flask's built-in session handling with configurable secret key
- **Error Handling**: Implements try-catch blocks for form processing with user-friendly error messages
- **Logging**: Uses Python's logging module for debugging and monitoring form submissions

## Form Processing
- **Contact Form Handler**: POST endpoint at `/contact` for processing contact form submissions
- **Basic Validation**: Server-side validation for required fields and email format
- **Flash Messaging**: Uses Flask's flash messaging system for user feedback
- **Redirect Pattern**: Implements Post-Redirect-Get pattern to prevent form resubmission

## Static Assets
- **CSS Architecture**: Custom CSS with CSS variables for theming and consistent styling
- **JavaScript Enhancement**: Client-side smooth scrolling and active navigation highlighting
- **External Dependencies**: Bootstrap, Font Awesome, and Google Fonts loaded via CDN

# External Dependencies

## Frontend Libraries
- **Bootstrap 5.3.0**: UI framework for responsive design and components
- **Font Awesome 6.4.0**: Icon library for visual elements
- **Google Fonts (Inter)**: Typography system for consistent font rendering

## Python Dependencies
- **Flask**: Core web framework for handling HTTP requests and templating
- **Python Standard Library**: datetime, os, and logging modules for basic functionality

## Development Environment
- **Environment Variables**: Uses `SESSION_SECRET` environment variable for session security
- **Debug Mode**: Configured for development with debug=True and detailed logging
- **Host Configuration**: Set up to run on all interfaces (0.0.0.0) on port 5000

## Missing Integrations
- **Database**: Currently logs contact form submissions only; no persistent data storage
- **Email Service**: Contact forms are logged but not sent via email
- **Analytics**: No web analytics or tracking integration implemented