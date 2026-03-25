# Car Marketplace - Buy & Sell Cars

A full-featured web application for buying and selling cars with user accounts, wishlist functionality, and invoice generation.

## Features

- **User Authentication**: Register and login system with secure password hashing
- **Car Listings**: Browse available cars with filtering options
- **Sell Cars**: Create and manage your car listings
- **Buy Cars**: Purchase cars with a simple checkout process
- **Wishlist**: Save favorite cars to your wishlist
- **Dashboard**: Manage your listings and view purchase history
- **Invoice Generation**: Generate professional invoices/bills for purchases

## Tech Stack

- **Frontend**: Next.js 14, React, TypeScript, Tailwind CSS
- **Backend**: Next.js API Routes
- **Authentication**: JWT tokens with httpOnly cookies
- **Data Storage**: JSON file-based storage (easily migratable to database)

## Getting Started

### Installation

1. Install dependencies:
```bash
npm install
```

2. Run the development server:
```bash
npm run dev
```

3. Open [http://localhost:3000](http://localhost:3000) in your browser

## Project Structure

```
├── app/
│   ├── api/              # API routes
│   │   ├── auth/         # Authentication endpoints
│   │   ├── cars/         # Car CRUD operations
│   │   ├── wishlist/     # Wishlist management
│   │   ├── purchases/    # Purchase history
│   │   └── invoice/      # Invoice generation
│   ├── cars/             # Car listing pages
│   ├── dashboard/        # User dashboard
│   ├── wishlist/         # Wishlist page
│   ├── sell/             # Sell car page
│   ├── login/            # Login page
│   ├── register/         # Registration page
│   └── invoice/          # Invoice display page
├── components/           # React components
├── lib/                  # Utility functions
│   ├── auth.ts          # Authentication utilities
│   └── data.ts          # Data storage utilities
└── data/                 # JSON data files (auto-generated)
```

## Usage

1. **Register**: Create a new account
2. **Login**: Sign in to your account
3. **Browse**: View available cars on the homepage or browse page
4. **Sell**: List your car for sale from the dashboard
5. **Buy**: Purchase cars and receive an invoice
6. **Wishlist**: Save cars you're interested in
7. **Dashboard**: Manage your listings and view purchase history

## Environment Variables

Create a `.env.local` file for production:

```
JWT_SECRET=your-secret-key-here
```

## Notes

- Data is stored in JSON files in the `data/` directory
- For production, consider migrating to a database (MongoDB, PostgreSQL, etc.)
- Images are currently URL-based; consider implementing file upload for production
- The application uses JWT tokens stored in httpOnly cookies for security

## License

MIT

