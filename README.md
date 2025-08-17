# BookCommerce

A modern, full-featured e-commerce platform for books built with React, TypeScript, and Vite. Features a comprehensive admin dashboard, email marketing capabilities, and seamless customer experience.

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
- Node.js 18+ 
- npm or pnpm (recommended)

### Installation

```bash
# Clone the repository
git clone https://github.com/Sabbirnde/BookCommerce.git
cd BookCommerce

# Install dependencies (recommended: use pnpm for better Windows compatibility)
pnpm install
# or
npm install

# Start the development server
pnpm run dev
# or
npm run dev
```

The application will be available at **http://localhost:8080**

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
├── src/
│   ├── assets/            # Static assets (images, etc.)
│   ├── components/        # Reusable UI components
│   │   ├── admin/         # Admin-specific components
│   │   ├── analytics/     # Analytics components
│   │   ├── email-marketing/  # Email marketing components
│   │   └── ui/            # shadcn/ui components
│   ├── contexts/          # React contexts (Auth, etc.)
│   ├── hooks/             # Custom React hooks
│   ├── integrations/      # Third-party integrations
│   │   └── supabase/      # Supabase configuration
│   ├── lib/               # Utilities, stores, and data
│   │   ├── bookData.ts    # Book data management
│   │   ├── cartStore.ts   # Shopping cart state
│   │   └── wishlistStore.ts # Wishlist state
│   ├── pages/             # Application pages
│   └── ...
├── supabase/              # Supabase configuration
│   ├── functions/         # Edge functions
│   └── migrations/        # Database migrations
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

### Backend & Services
- **🏢 Supabase** - Backend-as-a-Service
  - Authentication
  - Database (PostgreSQL)
  - Real-time subscriptions
  - Edge functions

### Development Tools
- **📋 ESLint** - Code linting
- **🎯 TypeScript ESLint** - TypeScript-specific linting
- **🔧 PostCSS** - CSS processing
- **📦 pnpm/npm** - Package management

## 🏗️ Available Scripts

```bash
# Development
pnpm run dev          # Start development server

# Building
pnpm run build        # Build for production
pnpm run build:dev    # Build in development mode

# Code Quality
pnpm run lint         # Run ESLint
pnpm run preview      # Preview production build
```

## 🚀 Deployment

### Build for Production

```bash
pnpm run build
# or
npm run build
```

The built application will be in the `dist` folder.

### Preview Production Build

```bash
pnpm run preview
# or
npm run preview
```

## 🤝 Contributing

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
