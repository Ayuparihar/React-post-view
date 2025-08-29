# Rest Express Application

## Overview

This is a full-stack web application built with React frontend and Express.js backend. The application features a posts dashboard that displays, paginates, and allows management of blog posts. It uses a modern tech stack including Drizzle ORM for database operations, shadcn/ui for UI components, and TanStack Query for state management.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript and Vite for fast development and building
- **UI Library**: shadcn/ui components built on top of Radix UI primitives for accessible, customizable components
- **Styling**: Tailwind CSS with CSS variables for theming and responsive design
- **State Management**: TanStack Query (React Query) for server state management and caching
- **Routing**: Wouter for lightweight client-side routing
- **Form Handling**: React Hook Form with Zod resolvers for type-safe form validation

### Backend Architecture
- **Framework**: Express.js with TypeScript for the REST API server
- **Database ORM**: Drizzle ORM configured for PostgreSQL with type-safe database operations
- **Development Tools**: Custom Vite integration for development mode with hot module replacement
- **Error Handling**: Centralized error handling middleware with proper HTTP status codes
- **Request Logging**: Custom middleware for API request logging with response time tracking

### Data Storage
- **Database**: PostgreSQL (configured via Drizzle) with Neon Database serverless integration
- **ORM**: Drizzle ORM provides type-safe database queries and migrations
- **Schema**: Shared schema definitions between frontend and backend using Zod for validation
- **Memory Storage**: Fallback in-memory storage implementation for development/testing

### Authentication & Authorization
- **Session Management**: PostgreSQL session store using connect-pg-simple
- **Storage Interface**: Abstracted storage layer with user management capabilities
- **Security**: Prepared for authentication implementation with user creation and retrieval methods

### External Dependencies
- **Database**: Neon Database serverless PostgreSQL for production data storage
- **UI Components**: Radix UI primitives for accessible component foundations
- **Development**: Modern development tools and hot module replacement for fast iteration
- **Build Tools**: Vite for frontend bundling and esbuild for backend compilation
- **Styling**: Google Fonts integration for typography (Inter, DM Sans, Fira Code, Geist Mono)
- **Icons**: Lucide React for consistent iconography throughout the application

The application follows a clean separation of concerns with a modular component structure, type-safe API communications, and a scalable database architecture that can easily transition from development to production environments.