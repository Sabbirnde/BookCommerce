# BookCommerce

A modern e-commerce platform for books with admin dashboard and email marketing capabilities.

## Features

- Browse books by categories (new and old books)
- Shopping cart and wishlist functionality
- User authentication and profile management
- Admin dashboard for product management
- Email marketing campaigns
- Customer support system
- Order management and payment processing

## Development

To work on this project locally:

```sh
# Clone the repository
git clone https://github.com/Sabbirnde/BookCommerce.git
cd BookCommerce

# Install dependencies
npm install

# Start the development server
npm run dev
```

The application will be available at http://localhost:8080

## Project Structure

```
src/
├── components/         # Reusable UI components
├── pages/             # Application pages
├── contexts/          # React contexts (Auth, etc.)
├── hooks/             # Custom React hooks
├── lib/               # Utilities and data
├── integrations/      # Third-party integrations
└── assets/           # Static assets
```

## Technologies Used

- Vite
- TypeScript
- React
- shadcn-ui
- Tailwind CSS
- Supabase for backend services
- React Router for navigation
- Zustand for state management

## Build for Production

```sh
npm run build
```

The built application will be in the `dist` folder.

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request
