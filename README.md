# Real Estate Rental Application

A full-stack real estate rental platform built with Next.js, Node.js, and Prisma, designed to streamline the property rental process for both property managers and tenants. The app allowed users to search for properties, apply for leases, manage their rental history, and for managers to list, update, and oversee properties and tenant applications.


## 🌟 Features

### For Tenants

- 🏠 Browse available properties with advanced search filters
- 📍 Interactive map integration for property locations
- ❤️ Save favorite properties
- 📝 Submit rental applications online
- 📊 Track application status
- 🏢 Manage current residences and lease information

### For Property Managers

- 📈 Property listing management
- 📋 Application review system
- 🏘️ Property portfolio overview
- 📊 Tenant management
- ⚙️ Account settings and preferences

## 🛠️ Technology Stack

### Frontend (Client)

- Next.js 14
- TypeScript
- Redux for state management
- Tailwind CSS for styling
- Shadcn UI components
- React Hook Form for form handling

### Backend (Server)

- Node.js
- Express.js
- Prisma ORM
- PostgreSQL database
- TypeScript
- JWT authentication

## 🚀 Getting Started

### Prerequisites

- Node.js (v18 or higher)
- PostgreSQL database
- npm or yarn package manager

### Installation

1. Clone the repository

```bash
git clone https://github.com/MohammadShabazuddin/Real_Estate_Rental_App.git
cd Real_Estate_Rental_App
```

2. Install dependencies for both client and server

```bash
# Install client dependencies
cd client
npm install

# Install server dependencies
cd ../server
npm install
```

3. Set up environment variables

```bash
# Client (.env.local)
NEXT_PUBLIC_API_URL=http://localhost:5000
NEXT_PUBLIC_MAPBOX_TOKEN=your_mapbox_token

# Server (.env)
DATABASE_URL="postgresql://user:password@localhost:5432/real_estate_db"
JWT_SECRET=your_jwt_secret
PORT=5000
```

4. Set up the database

```bash
cd server
npx prisma migrate dev
npx prisma db seed
```

5. Start the development servers

```bash
# Start the backend server
cd server
npm run dev

# Start the frontend development server
cd client
npm run dev
```

## 📁 Project Structure

```
├── client/                 # Frontend Next.js application
│   ├── src/
│   │   ├── app/           # Next.js app router
│   │   ├── components/    # Reusable components
│   │   ├── lib/          # Utility functions
│   │   └── state/        # Redux store and API
│   └── public/           # Static assets
│
└── server/                # Backend Node.js application
    ├── src/
    │   ├── controllers/  # Route controllers
    │   ├── middleware/   # Custom middleware
    │   └── routes/      # API routes
    └── prisma/          # Database schema and migrations
```

## 🔐 Authentication

The application uses JWT (JSON Web Tokens) for authentication. Users can sign up and log in as either property managers or tenants, with different permissions and access levels for each role.

## 🎨 UI/UX Features

- Responsive design for all screen sizes
- Modern and clean user interface
- Interactive property search with real-time filtering
- Intuitive navigation and user flow
- Dark mode support
- Loading states and animations

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 👥 Authors

- Mohammad Shabazuddin
