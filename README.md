# BookCommerce

A modern, full-featured e-commerce platform for books built with React, TypeScript, Vite frontend and PHP MySQL backend. Features a comprehensive admin dashboard, email marketing capabilities, and seamless customer experience.

## ✨ Architecture

**Frontend:** React + TypeScript + Vite + Tailwind CSS  
**Backend:** PHP + MySQL + JWT Authentication  
**Deployment:** Apache/Nginx + MySQL Server

## ✨ Features

### Customer Features
- 📚 Browse books by categories (new and old books)
- 🛒 Shopping cart with persistent state
- ❤️ Wishlist functionality
- 👤 User authentication and profile management
- 🔍 Advanced search functionality
- 📱 Responsive design for all devices
- 💳 Secure payment processing
- 📦 Order tracking and management

### Admin Features
- 🎛️ Comprehensive admin dashboard
- 📊 Analytics and reporting
- 📧 Email marketing campaigns
- 👥 Customer management
- 📋 Product management
- 💬 Customer support system
- 📈 Sales tracking

### Technical Features
- ⚡ Fast performance with Vite
- 🎨 Modern UI with shadcn/ui components
- 🌐 Real-time data with Supabase
- 🔒 Secure authentication
- 📱 Mobile-first responsive design

## 🚀 Quick Start

### Prerequisites
- Node.js 18+ (for frontend)
- PHP 7.4+ (for backend)
- MySQL 8.0+ (database)
- Apache or Nginx web server
- npm or pnpm (recommended)

### Installation

**Frontend Setup:**
```bash
# Clone the repository
git clone https://github.com/Sabbirnde/BookCommerce.git
cd BookCommerce

# Install frontend dependencies (recommended: use pnpm for better Windows compatibility)
pnpm install
# or
npm install
```

**Backend Setup:**
```bash
# Configure database credentials
# Edit backend/config/database.php with your MySQL credentials

# Set up the database
cd backend
php setup.php

# Configure web server virtual host pointing to project root
# Example for Apache: DocumentRoot should point to BookCommerce directory
```

**Start the Application:**
```bash
# Start frontend development server
pnpm run dev
# or
npm run dev

# Backend runs on your web server (Apache/Nginx)
# API accessible at: http://localhost/BookCommerce/backend/api
```

The frontend will be available at **http://localhost:8080**
The backend API will be available at **http://localhost/BookCommerce/backend/api**

### 🛠️ Troubleshooting Installation Issues

If you encounter permission issues on Windows with npm, try:

1. **Use pnpm (recommended)**:
   ```bash
   npm install -g pnpm
   pnpm install
   pnpm run dev
   ```

2. **Alternative npm approaches**:
   ```bash
   npm cache clean --force
   npm install --force
   ```

## 📁 Project Structure

```
BookCommerce/
├── public/                 # Static assets
│   ├── lovable-uploads/   # Image assets
│   └── ...
├── src/                   # Frontend React application
│   ├── assets/            # Static assets (images, etc.)
│   ├── components/        # Reusable UI components
│   │   ├── admin/         # Admin-specific components
│   │   ├── analytics/     # Analytics components
│   │   ├── email-marketing/  # Email marketing components
│   │   └── ui/            # shadcn/ui components
│   ├── contexts/          # React contexts (Auth, etc.)
│   ├── hooks/             # Custom React hooks
│   ├── integrations/      # Third-party integrations
│   ├── lib/               # Utilities, stores, and data
│   │   ├── bookData.ts    # Book data management
│   │   ├── cartStore.ts   # Shopping cart state
│   │   └── wishlistStore.ts # Wishlist state
│   ├── pages/             # Application pages
│   └── ...
├── backend/               # PHP Backend API
│   ├── api/               # API endpoints
│   │   ├── auth.php       # Authentication
│   │   ├── books.php      # Book management
│   │   ├── cart.php       # Shopping cart
│   │   └── index.php      # API router
│   ├── config/            # Configuration
│   │   ├── config.php     # General config
│   │   └── database.php   # Database config
│   ├── models/            # Data models
│   │   ├── User.php       # User model
│   │   ├── Book.php       # Book model
│   │   ├── Category.php   # Category model
│   │   └── Cart.php       # Cart model
│   ├── middleware/        # Authentication middleware
│   ├── utils/             # Utility classes
│   └── setup.php          # Database setup script
├── database/              # Database schema and migrations
│   └── migrations/        # SQL migration files
└── ...
```

## 🛠️ Technologies Used

### Frontend
- **⚡ Vite** - Build tool and development server
- **⚛️ React 18** - UI library
- **📘 TypeScript** - Type safety
- **🎨 Tailwind CSS** - Utility-first CSS framework
- **🧩 shadcn/ui** - Modern UI components
- **🚦 React Router** - Client-side routing
- **🗂️ Zustand** - Lightweight state management

### Backend & Database
- **🐘 PHP 7.4+** - Server-side scripting language
- **🗄️ MySQL 8.0+** - Relational database
- **🔐 JWT Authentication** - Secure token-based auth
- **🌐 RESTful API** - Clean API architecture
- **🔒 PDO** - Secure database abstraction layer

### Infrastructure
- **🖥️ Apache/Nginx** - Web server
- **🔧 XAMPP/WAMP** - Local development stack

### Development Tools
- **📋 ESLint** - Code linting
- **🎯 TypeScript ESLint** - TypeScript-specific linting
- **🔧 PostCSS** - CSS processing
- **📦 pnpm/npm** - Package management

## 🏗️ Available Scripts

```bash
# Frontend Development
pnpm run dev          # Start frontend development server
pnpm run build        # Build frontend for production
pnpm run build:dev    # Build frontend in development mode
pnpm run lint         # Run ESLint
pnpm run preview      # Preview production build

# Backend Development
php -S localhost:8000 # Start PHP development server (alternative)
# Note: Recommended to use Apache/Nginx with virtual host

# Database
mysql -u root -p      # Connect to MySQL
# Then run: SOURCE database/migrations/001_create_bookcommerce_schema.sql
```

## 🚀 Deployment

### Frontend Deployment
```bash
pnpm run build
# or
npm run build
```
The built frontend will be in the `dist` folder.

### Backend Deployment
1. Upload the `backend` folder to your web server
2. Create a MySQL database and import the schema
3. Configure database credentials in `backend/config/database.php`
4. Run `php backend/setup.php` to initialize the database
5. Set up virtual host or configure web server to serve the API
6. Update CORS settings in `backend/config/config.php`

### Full Stack Deployment
- **Frontend**: Deploy to Netlify, Vercel, or serve from the same server
- **Backend**: Deploy to shared hosting, VPS, or cloud server with PHP/MySQL
- **Database**: MySQL on the same server or managed database service

### Environment Configuration
- Update API endpoints in frontend code to point to your backend URL
- Configure CORS in backend to allow your frontend domain
- Use HTTPS in production for secure API communication

## 🔗 API Documentation

The backend provides a comprehensive RESTful API:

### Authentication Endpoints
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login  
- `GET /api/auth/profile` - Get user profile
- `PUT /api/auth/profile` - Update user profile

### Book Management
- `GET /api/books` - Get all books (with filters)
- `GET /api/books/featured` - Get featured books
- `GET /api/books/{id}` - Get book by ID
- `POST /api/books` - Create book (admin only)
- `PUT /api/books/{id}` - Update book (admin only)

### Shopping Cart
- `GET /api/cart` - Get cart items
- `POST /api/cart/add` - Add item to cart
- `PUT /api/cart/update` - Update cart item
- `DELETE /api/cart/remove` - Remove cart item

### Categories
- `GET /api/categories` - Get all categories

**Default Credentials:**
- Admin: `admin@bookcommerce.com` / `password`
- Customer: `john@example.com` / `password`

For complete API documentation, see [`backend/README.md`](backend/README.md)

We welcome contributions! Please follow these steps:

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/amazing-feature`)
3. **Commit** your changes (`git commit -m 'Add some amazing feature'`)
4. **Push** to the branch (`git push origin feature/amazing-feature`)
5. **Open** a Pull Request

### Development Guidelines
- Follow TypeScript best practices
- Use existing UI components from shadcn/ui when possible
- Maintain consistent code style (ESLint will help)
- Write meaningful commit messages
- Test your changes thoroughly

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Built with [Vite](https://vitejs.dev/)
- UI components from [shadcn/ui](https://ui.shadcn.com/)
- Backend powered by [Supabase](https://supabase.com/)
- Icons from [Lucide React](https://lucide.dev/)

## 📞 Support

If you have any questions or run into issues:

1. Check the [Issues](https://github.com/Sabbirnde/BookCommerce/issues) page
2. Create a new issue if your problem isn't already reported
3. Provide as much detail as possible including your OS, Node.js version, and error messages

---

**Happy coding!** 🚀📚
