# ARVIN Trade - E-commerce Platform

## Overview

ARVIN Trade is a comprehensive e-commerce platform built as a full-stack web application. The system allows users to buy and sell products online with features including user authentication, product management, real-time chat, notifications, and payment processing. The platform is designed with a modern tech stack using React for the frontend, Express.js for the backend, and PostgreSQL for data persistence.

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript
- **Styling**: Tailwind CSS with shadcn/ui component library
- **State Management**: Zustand for client-side state, React Query for server state
- **Build Tool**: Vite for development and production builds
- **UI Components**: Radix UI primitives with custom styling

### Backend Architecture
- **Runtime**: Node.js with Express.js framework
- **Language**: TypeScript with ES modules
- **API Design**: RESTful API architecture
- **Middleware**: Express middleware for logging, JSON parsing, and error handling

### Database Architecture
- **Database**: PostgreSQL with Neon serverless hosting
- **ORM**: Drizzle ORM for type-safe database operations
- **Schema Management**: Drizzle Kit for migrations and schema management
- **Connection**: WebSocket-based connection via Neon serverless

## Key Components

### Authentication System
- **Provider**: Supabase Auth for user management
- **State Management**: Zustand store for authentication state
- **Session Management**: Automatic session handling with persistent login

### Product Management
- **Upload System**: Multi-step product creation with image upload
- **Category System**: Predefined product categories
- **Status Management**: Pending/approved/rejected workflow for products
- **Stock Management**: Inventory tracking system

### Communication Features
- **Real-time Chat**: Direct messaging between buyers and sellers
- **Notifications**: System-wide notification system
- **Admin Panel**: Product approval and user management interface

### Payment System
- **Top-up Functionality**: User balance management
- **Transaction History**: Complete audit trail of all transactions
- **Subscription Model**: Premium user features

### User Interface
- **Responsive Design**: Mobile-first approach with bottom navigation
- **Component Library**: shadcn/ui for consistent UI components
- **Layout System**: Header, content, and bottom navigation structure
- **Theme Support**: CSS custom properties for theming

## Data Flow

1. **User Registration/Login**: Users authenticate through Supabase Auth
2. **Product Creation**: Sellers upload products which enter pending status
3. **Admin Approval**: Admins review and approve/reject products
4. **Product Discovery**: Buyers browse approved products
5. **Communication**: Direct chat between buyers and sellers
6. **Transaction Processing**: Payment handling and order management
7. **Notification System**: Real-time updates for important events

## External Dependencies

### Core Dependencies
- **Supabase**: Authentication and real-time features
- **Neon Database**: PostgreSQL hosting
- **Radix UI**: Accessible UI primitives
- **React Query**: Server state management
- **Date-fns**: Date manipulation utilities

### Development Tools
- **Vite**: Build tool and development server
- **TypeScript**: Type safety and developer experience
- **Tailwind CSS**: Utility-first CSS framework
- **ESBuild**: Fast JavaScript bundling

## Deployment Strategy

### Development Environment
- **Local Development**: Vite dev server with hot module replacement
- **Database**: Neon serverless PostgreSQL
- **Build Process**: TypeScript compilation with Vite

### Production Environment
- **Backend Build**: ESBuild for Node.js server bundling
- **Frontend Build**: Vite static asset generation
- **Database Migrations**: Drizzle Kit for schema updates
- **Environment Variables**: DATABASE_URL for database connection

### File Structure
- **Client**: React frontend in `/client` directory
- **Server**: Express backend in `/server` directory
- **Shared**: Common types and schemas in `/shared` directory
- **Database**: Schema definitions and migrations

## Changelog
- July 06, 2025. Initial setup

## User Preferences

Preferred communication style: Simple, everyday language.