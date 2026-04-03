# LUXE - Premium Fashion E-Commerce Platform

A modern, luxury fashion e-commerce frontend inspired by Zara, built with Next.js, React, TypeScript, and Tailwind CSS. Features smooth animations, editorial-style design, and premium UX patterns.

## 🎯 Features

### Pages
- **Home** - Editorial hero with scroll-triggered storytelling sections and category showcase
- **Products** - Filterable product grid with advanced filtering (category, price, color, size)
- **Product Detail** - Detailed product view with image gallery, size/color selection, and reviews
- **Cart** - Shopping cart management with quantity controls and order summary
- **Checkout** - Multi-step checkout process (shipping & payment information)
- **Auth** - Login and registration with form validation

### Design & UX
- ✨ Smooth Framer Motion animations throughout
- 📱 Fully responsive design (mobile, tablet, desktop)
- 🎨 Luxury color palette with custom Tailwind theme
- 📸 Lazy-loading images with skeleton loaders
- 🔄 Page transitions with smooth fades and slides
- 🎭 Hover animations on images and interactive elements
- ⌨️ Keyboard accessible forms and navigation
- 📊 Performance optimized with Next.js Image component

### Features
- Shopping cart with Zustand state management
- Product filtering by category, price, color, size
- Sort products by newest, price, and popularity
- Form validation with error handling
- Secure checkout flow
- User authentication system
- Mock product data with real-like details
- Premium micro-interactions everywhere

## 🛠 Tech Stack

- **Framework**: Next.js 14
- **Language**: TypeScript
- **Styling**: Tailwind CSS 3
- **Animations**: Framer Motion 10
- **State Management**: Zustand
- **HTTP Client**: Axios
- **Icons**: Lucide React
- **Intersection Observer**: react-intersection-observer

## 📦 Installation

### Prerequisites
- Node.js 18+ 
- npm or yarn

### Setup

1. **Navigate to project directory**
   ```bash
   cd clothingbrand
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Run development server**
   ```bash
   npm run dev
   ```

4. **Open browser**
   ```
   http://localhost:3000
   ```

## 📁 Project Structure

```
clothingbrand/
├── app/                          # Next.js app directory
│   ├── layout.tsx               # Root layout with navbar & footer
│   ├── globals.css              # Global styles & utilities
│   ├── page.tsx                 # Home page
│   ├── products/
│   │   ├── page.tsx            # Product listing
│   │   └── [id]/page.tsx       # Product detail
│   ├── cart/page.tsx            # Shopping cart
│   ├── checkout/page.tsx        # Checkout process
│   └── auth/page.tsx            # Login/Register
├── components/
│   ├── layout/
│   │   ├── Navbar.tsx          # Header navigation
│   │   ├── Footer.tsx          # Footer component
│   │   └── PageTransition.tsx  # Page animation wrapper
│   ├── common/
│   │   ├── Button.tsx          # Reusable button component
│   │   ├── ProductCard.tsx     # Product card with hover effects
│   │   ├── SkeletonLoader.tsx  # Loading skeleton UI
│   │   └── ImageGallery.tsx    # Product image carousel
│   └── features/
│       ├── HeroSection.tsx     # Full-screen hero
│       ├── CategoryGrid.tsx    # Category showcase
│       ├── ProductGrid.tsx     # Product listing grid
│       └── ScrollStorySection.tsx # Editorial story section
├── store/
│   ├── cart.ts                 # Zustand cart store
│   └── auth.ts                 # Zustand auth store
├── lib/
│   ├── utils.ts                # Utility functions
│   └── mockData.ts             # Sample product data
├── types/
│   └── index.ts                # TypeScript type definitions
└── [config files]
    ├── next.config.js
    ├── tailwind.config.ts
    ├── postcss.config.js
    ├── tsconfig.json
    └── package.json
```

## 🎨 Design System

### Colors
- **Luxury Neutral**: #fafafa to #212121 (luxury-50 to luxury-950)
- **Accent Gold**: #d4af37 for premium highlights
- **Accent Platinum**: #e8e8e8 for subtle highlights
- **Accent Rose**: #f0e6e6 for feminine tones

### Typography
- **Display**: Bodoni Moda (serif, elegant)
- **Headings**: Georgia (serif)
- **Body**: System fonts (san-serif)

### Spacing & Layout
- Max width: 1280px (7xl)
- Section padding: 64-128px
- Grid gaps: 16-24px
- Uses CSS Grid and Flexbox

## 🚀 Performance

- Optimized images with Next.js Image component
- Lazy loading for below-the-fold content
- Skeleton loaders for better perceived performance
- CSS animations using transform/opacity (GPU accelerated)
- Code splitting and chunking by Next.js
- Static generation where possible

## 📱 Responsive Design

Breakpoints:
- **Mobile**: < 640px (sm)
- **Tablet**: 640px - 1024px (md)
- **Desktop**: 1024px+ (lg)

## 🔧 Available Scripts

```bash
# Development server
npm run dev

# Production build
npm run build

# Start production server
npm start

# Type checking
npm run type-check

# Linting
npm run lint
```

## 🎯 Key Features to Explore

### 1. Smooth Animations
- Hero section scroll animation
- Product card hover effects
- Image gallery transitions
- Page fade-in animations
- Section reveal on scroll

### 2. Cart Management
- Add/remove items
- Quantity management
- Real-time price calculation
- Persistent state with Zustand

### 3. Product Filtering
- By category (Women, Men, Accessories)
- By price range
- By color options
- By available sizes
- Sort by newest, price, popularity

### 4. Checkout Flow
- Multi-step form validation
- Shipping address form
- Credit card payment form
- Order summary
- Confirmation page

### 5. User Authentication
- Login form
- Registration form
- Form validation with helpful errors
- Mock authentication flow

## 🎨 Customization

### Add New Products
Edit `lib/mockData.ts`:
```typescript
export const mockProducts: Product[] = [
  {
    id: 'unique-id',
    name: 'Product Name',
    category: 'women',
    price: 299,
    // ... other properties
  },
]
```

### Modify Colors
Edit `tailwind.config.ts` in the `theme.extend.colors` section.

### Change Typography
Update font imports and `theme.extend.fontFamily` in `tailwind.config.ts`.

## 📊 Mock Data

The project includes mock product data with realistic details:
- 8 sample products across categories
- Real product imagery from Unsplash
- Price variations and discounts
- Multiple colors and sizes
- Product descriptions and care instructions

## 🔐 Security Notes

This is a frontend-only project with mock backend. For production:
1. Implement real API endpoints
2. Add authentication with JWT
3. Use environment variables for API keys
4. Implement payment processing (Stripe, etc.)
5. Add HTTPS enforcement
6. Implement CSRF protection

## 📝 License

This project is provided as-is for educational and commercial use.

## 🎓 Learning Resources

- [Next.js Documentation](https://nextjs.org/docs)
- [Tailwind CSS](https://tailwindcss.com/docs)
- [Framer Motion](https://www.framer.com/motion/)
- [TypeScript](https://www.typescriptlang.org/docs/)
- [Zustand](https://github.com/pmndrs/zustand)

## ✨ Premium Features Implemented

1. **Editorial Style Design** - Magazine-like layout with large typography
2. **Micro-interactions** - Hover effects, loading states, transitions
3. **Luxury Color Palette** - Neutral blacks, whites, golds
4. **High-quality Images** - Elegant product photography
5. **Smooth Animations** - Professional page transitions
6. **Search & Filter** - Advanced product discovery
7. **Cart Persistence** - State management with Zustand
8. **Form Validation** - Real-time error messages
9. **Responsive Grid** - Adapts to all screen sizes
10. **Trust Signals** - Security badges, free shipping info

## 🚀 Getting Started

```bash
# Install Node.js 18+
# Navigate to project
cd clothingbrand

# Install dependencies
npm install

# Start development
npm run dev

# Visit http://localhost:3000
```

---

**Built with ❤️ for luxury fashion e-commerce**
