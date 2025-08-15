# CyberEdt - Cybersecurity Education Platform

## Overview

CyberEdt is a comprehensive cybersecurity education platform focused on creating a cyber-aware India through awareness programs, training modules, and cutting-edge security solutions. The application serves as a landing page and course management system for cybersecurity education, featuring course catalogs, contact forms, and interactive UI components.

The platform emphasizes accessibility and user engagement with modern web technologies, providing a dark-themed cybersecurity aesthetic with interactive animations and responsive design.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript for type safety and modern component development
- **Routing**: Wouter for lightweight client-side routing
- **Styling**: Tailwind CSS with custom cybersecurity-themed design system using CSS variables
- **UI Components**: shadcn/ui component library built on Radix UI primitives for accessibility
- **State Management**: TanStack Query for server state management and data fetching
- **Build Tool**: Vite for fast development and optimized production builds

### Backend Architecture
- **Server**: Express.js with TypeScript for the API layer
- **Database ORM**: Drizzle ORM for type-safe database operations
- **Database**: PostgreSQL (configured for Neon Database) for data persistence
- **Storage Pattern**: Repository pattern with interface-based storage abstraction
- **Session Management**: connect-pg-simple for PostgreSQL-backed sessions

### Data Storage Solutions
- **Primary Database**: PostgreSQL with Drizzle ORM for schema management
- **Schema Design**: User-centric with username/password authentication
- **Migrations**: Drizzle Kit for database schema migrations and version control
- **Development Storage**: In-memory storage implementation for development/testing

### Authentication and Authorization
- **User Model**: Simple username/password authentication system
- **Session Storage**: PostgreSQL-backed sessions for persistence
- **Password Security**: Basic password storage (extensible for bcrypt hashing)

### External Dependencies
- **Database Hosting**: Neon Database (serverless PostgreSQL)
- **Font Integration**: Google Fonts (Poppins, custom font stack)
- **Icon System**: Font Awesome for consistent iconography
- **Development Tools**: Replit-specific tooling for hot reloading and error handling
- **Form Handling**: React Hook Form with Zod validation for type-safe form management
- **Animation Libraries**: Custom CSS animations with Intersection Observer API for scroll-based reveals

### Key Design Patterns
- **Component Architecture**: Modular React components with proper separation of concerns
- **Custom Hooks**: Reusable logic for scroll animations, counters, and form handling
- **Theme System**: CSS custom properties for consistent theming and dark mode support
- **Responsive Design**: Mobile-first approach with Tailwind CSS breakpoints
- **Error Handling**: Centralized error handling with toast notifications
- **Development Experience**: Hot reloading, TypeScript checking, and integrated development tools