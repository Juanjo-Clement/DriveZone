# DriveZone

**A Full-Stack Automotive E-Commerce Platform**

DriveZone is an academic full-stack e-commerce project focused on the automotive industry. It provides a digital shopping experience where users can explore automotive products, manage a shopping cart, configure delivery and payment preferences, and simulate the checkout process.

The project is built with a modern web technology stack, combining a Next.js frontend with a NestJS backend.

> **Project status:** This project is currently under development. Some features are implemented as demonstrations using mock data and browser local storage. It is not yet a production-ready e-commerce platform.

## Technologies

### Frontend
- Next.js 16
- React 19
- TypeScript
- Tailwind CSS 4

### Backend
- NestJS 12
- TypeScript
- Node.js
- Vitest

## Features

### Product Catalog
- Automotive product catalog.
- Product categories, including tires, oils, batteries, and wheels.
- Product search and filtering.
- Price and rating sorting.
- Product details and inventory information.

### Shopping Experience
- Shopping cart management.
- Quantity updates and product removal.
- Cart persistence using browser local storage.
- Checkout interface.
- Shipping method selection.
- Address and payment method management.

### User Interface
- Login and registration interfaces.
- User profile and account settings.
- Favorites.
- Order history.
- Customer support interface.
- Responsive, automotive-inspired design.

### Backend Modules
The NestJS application is organized into the following modules:

- Authentication
- Inventory
- Shopping Cart
- Orders
- Reviews
- Support
- Favorites
- Payments

## Project Structure

```text
DriveZone/
├── drivezone-frontend-main/
│   ├── app/
│   ├── context/
│   ├── public/
│   └── package.json
│
├── drivezone-backend-main/
│   ├── src/
│   │   ├── auth/
│   │   ├── inventory/
│   │   ├── cart/
│   │   ├── orders/
│   │   ├── reviews/
│   │   ├── support/
│   │   ├── favorites/
│   │   └── payments/
│   └── package.json
│
├── .gitignore
└── README.md
```

## Getting Started

### Prerequisites
- Node.js
- npm

### 1. Clone the repository

```bash
git clone https://github.com/Juanjo-Clement/DriveZone.git
cd DriveZone
```

### 2. Set up the backend

```bash
cd drivezone-backend-main
npm install
npm run start:dev
```

The backend runs by default at:

`http://localhost:3001`

### 3. Set up the frontend

Open a second terminal:

```bash
cd drivezone-frontend-main
npm install
npm run dev
```

The frontend runs at:

`http://localhost:3000`

### Environment Configuration

The frontend supports an optional environment variable to configure the backend URL:

```env
NEXT_PUBLIC_API_URL=http://localhost:3001
```

Create a `.env.local` file inside the frontend directory if you need to override the default API URL.

Do not commit environment files or private credentials.

## Current Development Status

DriveZone is an evolving academic project. The following limitations should be considered:

- Backend inventory, authentication, and cart services currently use in-memory data.
- The frontend shopping cart and checkout process rely on browser local storage.
- Authentication endpoints return demonstration responses and do not implement production-grade authentication.
- The registration form is currently a frontend demonstration.
- Google and Apple sign-in interfaces do not yet provide complete OAuth integration.
- The checkout flow simulates order creation and does not process real payments.
- Persistent database integration and production deployment remain future development goals.

## Academic Project

DriveZone was developed as an academic software engineering project, with a focus on full-stack development, modular architecture, user interface design, and e-commerce workflows.

**Contributors:** Add the project team members here.

---

*DriveZone — Automotive shopping, reimagined.*