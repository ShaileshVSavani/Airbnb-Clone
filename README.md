Here's a comprehensive `README.md` file for Airbnb clone project:

---

# Airbnb Clone

An Airbnb clone app built with a modern full-stack implementation using **Next.js 13 App Router** and technologies like **React**, **Tailwind CSS**, **Prisma**, **MongoDB**, and **NextAuth**. This application replicates key features of Airbnb, offering a seamless user experience for property listing, searching, booking, and managing reservations.

## Project Overview

This project is a full-stack implementation of an Airbnb-like platform, providing a rich feature set for users to browse properties, book stays, and manage their listings. It uses cutting-edge technologies to ensure a responsive and dynamic experience.

---

## Key Features

- **Responsive Design**: Built with Tailwind CSS for seamless rendering on all screen sizes.
- **Authentication**:
  - Credential-based login
  - Social logins via Google and GitHub
- **Advanced Search**:
  - Search by category, date range, map location, guests, rooms, and bathrooms.
  - Excludes properties with existing reservations in the selected date range.
- **Reservation Management**:
  - Booking and cancellation for guests.
  - Owners can manage and cancel bookings.
- **Property Management**:
  - Add, edit, and delete property listings.
  - Real-time pricing calculation.
- **Favorites System**: Save favorite properties for quick access.
- **Image Upload**: Upload property images using Cloudinary CDN.
- **Interactive Calendar**: Implemented using `react-date-range`.
- **Shareable Filters**: Share URL filters for categories, locations, and date ranges.

---

## Live Demo

Check out the live demo of the deployed application:  
[Airbnb Clone Live Demo]()

---

## Installation Instructions

Follow these steps to set up and run the project locally:

### Prerequisites

- Node.js version 14.x or higher
- MongoDB instance (local or cloud)
- Accounts for Google and GitHub OAuth for authentication.

### Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/ShaileshVSavani/Airbnb-Clone.git
   cd Airbnb
   ```

2. **Install Dependencies**
   ```bash
   npm install
   ```

3. **Set Up Environment Variables**
   Create a `.env` file in the root directory and configure the following variables:
   ```env
   DATABASE_URL=<Your MongoDB connection string>
   GOOGLE_CLIENT_ID=<Your Google OAuth Client ID>
   GOOGLE_CLIENT_SECRET=<Your Google OAuth Client Secret>
   GITHUB_ID=<Your GitHub OAuth ID>
   GITHUB_SECRET=<Your GitHub OAuth Secret>
   NEXTAUTH_SECRET=<A random secret string>
   NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME=<cloudinary cloud name>
   ```

4. **Set Up Prisma**
   Push the database schema to your MongoDB instance:
   ```bash
   npx prisma db push
   ```

5. **Start the Development Server**
   ```bash
   npm run dev
   ```
   The application will run at `http://localhost:3000`.

---

## Technologies Used

- **Frontend**:
  - [Next.js 13](https://nextjs.org/) (React Framework)
  - [React](https://reactjs.org/) (UI Library)
  - [Tailwind CSS](https://tailwindcss.com/) (Styling)

- **Backend**:
  - [NextAuth](https://next-auth.js.org/) (Authentication)
  - [Prisma](https://www.prisma.io/) (ORM for MongoDB)
  - [MongoDB](https://www.mongodb.com/) (Database)

- **Third-Party Libraries**:
  - [Cloudinary](https://cloudinary.com/) (Image Uploads)
  - [React Hook Form](https://react-hook-form.com/) (Form Validation)
  - [React Date Range](https://github.com/hypeserver/react-date-range) (Calendar)
  - [React Toast](https://react-hot-toast.com/) (Notifications)
  - [React Leaflet](https://react-leaflet.js.org/) (Map Integration)
  - [Zustand](https://zustand-demo.pmnd.rs/) (State Management)

- **Utilities**:
  - [ESLint](https://eslint.org/) (Linting)
  - [TypeScript](https://www.typescriptlang.org/) (Type Checking)

---

