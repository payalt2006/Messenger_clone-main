# ConvoX

### Real-Time Full Stack Messaging Platform

ConvoX is a fully responsive, real-time chat application built using **Next.js 13**, **MongoDB**, **Tailwind CSS**, **Pusher**, **NextAuth**, and **Cloudinary**.

The project demonstrates full-stack web development by combining authentication, real-time messaging, cloud storage, and modern UI design into a scalable messaging platform.

---

## Preview

<p align="center">
  <img src="public/images/Screenshot (84).png" alt="ConvoX Preview">
</p>

<p align="center">
  <img src="public/images/Screenshot (85).png" alt="ConvoX Preview">
</p>

<p align="center">
  <img src="public/images/Screenshot (88).png" alt="ConvoX Preview">
</p>

<p align="center">
  <img src="public/images/Screenshot (89).png" alt="ConvoX Preview">
</p>

## White Theme Interface

<p align="center">
  <img src="public/images/Screenshot (90).png" alt="ConvoX White Theme">
</p>

---

## Features

### Real-Time Messaging

* Instant message delivery powered by **Pusher**
* Live conversation updates
* Smooth and synchronized chat experience

### Group Conversations

* Create and manage group chats
* Collaborate and communicate seamlessly

### Secure Authentication

* Authentication powered by **NextAuth**
* Login using:

  * Google
  * GitHub

### Media Sharing

* Upload and share images
* Cloud-based storage with **Cloudinary**

### Chat Management

* Delete unwanted messages
* Manage conversations efficiently

### Dynamic Themes

* Switch between:

  * Light Mode
  * Dark Mode

### Responsive Design

Optimized for:

* Desktop
* Tablet
* Mobile devices

---

## Tech Stack

### Frontend

* Next.js 13
* React 18
* Tailwind CSS
* TypeScript

### Backend & Database

* MongoDB Atlas
* Prisma ORM

### Services & Integrations

* Pusher
* NextAuth
* Cloudinary

---

## Architecture Overview

ConvoX follows a full-stack real-time communication workflow.

### 1. Authentication Layer

Users securely authenticate using:

* Google OAuth
* GitHub OAuth
* NextAuth session management

### 2. Real-Time Communication

Pusher handles:

* Instant message delivery
* Live chat synchronization
* Real-time updates

### 3. Database Layer

MongoDB stores:

* User data
* Conversations
* Messages
* Chat metadata

Prisma manages schema and database operations.

### 4. Media Upload System

Cloudinary provides:

* Image hosting
* Cloud storage
* Optimized delivery

---

## Getting Started

Follow these steps to run ConvoX locally.

## Prerequisites

Make sure the following are installed:

* Node.js (14 or higher)
* Yarn Package Manager

---

## Installation

### Clone Repository

```bash
git clone https://github.com/himanshutatawat/Messenger_clone.git
cd ConvoX
```

### Install Dependencies

```bash
yarn install
```

---

## Environment Configuration

Create a **.env.local** file and add:

```env
DATABASE_URL=your_mongodb_connection_string
NEXTAUTH_URL=http://localhost:3020
NEXTAUTH_SECRET=your_nextauth_secret

GITHUB_ID=your_github_client_id
GITHUB_SECRET=your_github_client_secret

GOOGLE_ID=your_google_client_id
GOOGLE_SECRET=your_google_client_secret

CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_UPLOAD_PRESET=your_cloudinary_upload_preset

PUSHER_APP_ID=your_pusher_app_id
PUSHER_KEY=your_pusher_key
PUSHER_SECRET=your_pusher_secret
PUSHER_CLUSTER=your_pusher_cluster
```

---

## Database Setup

### MongoDB Atlas Setup

1. Create a MongoDB Atlas account
2. Create a cluster
3. Create a database user
4. Allow IP access:

```text
0.0.0.0/0
```

5. Copy your MongoDB connection string
6. Replace `<password>` with your database password

---

## Prisma Setup

Initialize Prisma and sync schema:

```bash
yarn prisma db push
yarn prisma generate
```

---

## Running ConvoX

### Development Mode

Start development server:

```bash
yarn dev
```

Open:

```text
http://localhost:3020
```

### Production Mode

Build application:

```bash
yarn build
```

Run production server:

```bash
yarn start
```

---

## Available Commands

| Command              | Description              |
| -------------------- | ------------------------ |
| yarn dev             | Start development server |
| yarn build           | Build production app     |
| yarn start           | Run production server    |
| yarn prisma db push  | Push schema to database  |
| yarn prisma generate | Generate Prisma client   |

---

## Key Highlights

ConvoX showcases experience with:

* Full Stack Development
* Next.js Applications
* Real-Time Systems
* Authentication & OAuth
* Database Design
* Cloud Media Integration
* Responsive UI Development

---

## Future Improvements

Planned enhancements include:

* Voice and video calling
* Typing indicators
* Read receipts
* Push notifications
* End-to-end encryption
* Message reactions

---

## Author

Built as a **Full Stack Next.js Messaging Platform** to explore scalable real-time communication and modern web development practices.
