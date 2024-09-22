# Messaging Service Prototype

# Name - Abdul Mannan
# University - Indian Institute of Technology (Indian School of Mines) Dhanbad
# Department - Environmental Engineering

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Technology Stack](#technology-stack)
- [Why These Technologies?](#why-these-technologies)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Environment Variables](#environment-variables)
  - [Running the Application](#running-the-application)
- [Real-Time Communication](#real-time-communication)
- [Security Considerations](#security-considerations)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Overview

The **Messaging Service Prototype** is a scalable, responsive, and real-time messaging application designed to replicate and enhance the core functionalities of modern messaging platforms. It supports real-time messaging, voice and video calls, media sharing, and seamless user authentication. This prototype serves as a robust foundation for building a full-featured messaging platform capable of handling high traffic and delivering an exceptional user experience.

## Features

- **Authentication & Signup**
  - Social Login with Google and GitHub via OAuth.
  - Email-based signup with verification using Nodemailer.
  - Session management using JWT stored in HTTP-only cookies.

- **Messaging**
  - One-to-One and Group Chats.
  - Media Support for text, images, and voice messages.
  - Real-Time Updates powered by Pusher.
  - Search functionality for messages and contacts.

- **Notifications**
  - Real-Time Notifications for messages, events, and call requests.
  - Web Push Notifications for offline alerts.

- **Voice & Video Calls**
  - Real-Time Voice and Video Communication using ZegoCloud.
  - Call Management including invitations, acceptance, and termination.

- **User Interface**
  - Support for Dark Mode and Light Mode.
  - Mobile-First Responsive Design.

## Technology Stack

### Frontend and Backend

- **Framework**: [Next.js](https://nextjs.org/) - Server-side rendering and API routes.
- **Language**: [TypeScript](https://www.typescriptlang.org/) - Enhanced JavaScript with type safety.
- **Styling**: [Tailwind CSS](https://tailwindcss.com/) or [Styled Components](https://styled-components.com/) - Utility-first and component-based styling.

### Database and Storage

- **Primary Database**: [MongoDB](https://www.mongodb.com/) - NoSQL database for flexible data storage.
- **ORM**: [Prisma](https://www.prisma.io/) - Type-safe ORM for database interactions.
- **File Storage**: [Cloudinary](https://cloudinary.com/) - Cloud-based media storage and CDN.

### Real-Time Services

- **Messaging**: [Pusher](https://pusher.com/) - Real-time WebSocket connections for instant messaging.
- **Voice & Video Calls**: [ZegoCloud](https://www.zegocloud.com/) - Real-time communication SDK.

### Authentication

- **Library**: [NextAuth.js](https://next-auth.js.org/) - Authentication for Next.js applications.
- **Email Service**: [Nodemailer](https://nodemailer.com/) - Sending verification emails.

## Why These Technologies?

- **Next.js**: Provides a robust framework for building both frontend and backend within a single application, leveraging server-side rendering for performance and SEO benefits.
  
- **TypeScript**: Enhances code quality and maintainability with static type checking, reducing runtime errors and improving developer experience.

- **Tailwind CSS / Styled Components**: Offers flexibility in styling. Tailwind provides utility-first classes for rapid UI development, while Styled Components allow for scoped, component-based styling.

- **MongoDB & Prisma**: MongoDB's schema-less nature accommodates dynamic data structures, ideal for messaging data. Prisma offers a type-safe ORM experience, simplifying database operations.

- **Pusher**: Facilitates real-time communication with minimal setup, enabling instant message delivery and updates.

- **ZegoCloud**: Provides reliable and scalable voice and video call functionalities, essential for real-time communication features.

- **Cloudinary**: Manages media uploads, storage, and delivery efficiently with built-in CDN capabilities, enhancing media handling performance.

- **NextAuth.js & Nodemailer**: Simplifies authentication flows, supporting multiple providers and secure email-based signup processes.

## Getting Started

### Prerequisites

Ensure you have the following installed on your machine:

- [Node.js](https://nodejs.org/) (v14 or higher)
- [npm](https://www.npmjs.com/) or [Yarn](https://yarnpkg.com/)
- [MongoDB](https://www.mongodb.com/) instance (local or cloud-based)
- Cloudinary account for media storage
- Pusher account for real-time messaging
- ZegoCloud account for voice and video calls

### Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/abdul1mannan/iby-intern.git
   cd iby-intern
   
2. **Install Dependencies**
   
    ```bash
   npm install

3. **Create a .env file**

DATABASE_URL=
NEXTAUTH_SECRET=
GITHUB_ID=
GITHUB_SECRET=
GOOGLE_CLIENT_ID=
GOOGLE_CLIENT_SECRET=
OAUTH_CLIENT_ID=
OAUTH_CLIENT_SECRET=
OAUTH_REFRESH_TOKEN=
MAIL_USERNAME=
MAIL_PASSWORD=
NEXTAUTH_URL=
NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME=
NEXT_PUBLIC_CLOUDINARY_UPLOAD_PRESET=
NEXT_PUBLIC_PUSHER_APP_KEY=
PUSHER_APP_ID=
PUSHER_SECRET=
NEXT_PUBLIC_PUSHER_CLUSTER=
NEXT_PUBLIC_ZEGOCLOUD_APP_ID=
NEXT_PUBLIC_ZEGOCLOUD_SERVER_SECRET=
NEXT_PUBLIC_BASE_URL=

4. **Start the Development Server**
     ```bash
   npm run dev
  
