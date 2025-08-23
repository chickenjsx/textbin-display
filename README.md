# Textbin

**The secure platform for dumping your ideas instantly.**

**This repository is for display purposes only. It helps me preserve the integrity and ownership of the code’s intellectual property.
**
Textbin is a modern, secure note-taking application that lets you quickly capture thoughts, ideas, code snippets, and any text-based content without the hassle of creating files or emailing yourself. Built with Next.js and featuring end-to-end encryption, Textbin is your digital brain dump.

## 🚀 Features

- **Instant Text Dumping** - No setup required, just start typing
- **Auto-Save Magic** - Everything saves automatically, never lose an idea
- **Cross-Device Access** - Your notes follow you everywhere
- **Secure Encryption** - 256-bit encryption with zero-knowledge architecture
- **Easy Sharing** - Turn any note into a shareable link instantly
- **Search & Filter** - Find your notes quickly with powerful search
- **Tag System** - Organize notes with custom tags
- **Premium Features** - Advanced features with subscription model
- **Dark/Light Themes** - Customizable interface themes

## 🛠️ Tech Stack

- **Frontend**: Next.js 14 (App Router)
- **Database**: PostgreSQL with Prisma ORM
- **Authentication**: Custom auth system with JWT
- **Payments**: Stripe integration
- **Encryption**: Client-side encryption for note content
- **Styling**: Tailwind CSS with custom CSS variables
- **Deployment**: Vercel-ready

## 🏗️ Project Structure

```
textbin/
├── app/                    # Next.js app directory
│   ├── api/               # API routes
│   │   ├── auth/          # Authentication endpoints
│   │   ├── notes/         # Note CRUD operations
│   │   ├── stripe/        # Payment processing
│   │   └── share/         # Note sharing functionality
│   ├── components/        # Reusable React components
│   ├── contexts/          # React contexts (Auth, Notes, Theme, etc.)
│   ├── hooks/             # Custom React hooks
│   ├── lib/               # Utility libraries
│   └── [pages]/           # App pages
├── prisma/                # Database schema and migrations
└── public/                # Static assets
```

## 🚦 Getting Started

### Prerequisites

- Node.js 18+
- PostgreSQL database
- Stripe account (for payments)

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/chickenjsx/textbin.git
   cd textbin
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Set up environment variables**
   Create a `.env.local` file in the root directory:

   ```env
   # Database
   DATABASE_URL="postgresql://username:password@localhost:5432/textbin"

   # Authentication
   JWT_SECRET="your-jwt-secret-key"

   # Stripe
   STRIPE_SECRET_KEY="sk_test_..."
   STRIPE_PUBLISHABLE_KEY="pk_test_..."
   STRIPE_WEBHOOK_SECRET="whsec_..."

   # App URL
   NEXT_PUBLIC_APP_URL="http://localhost:3000"
   ```

4. **Set up the database**

   ```bash
   npx prisma generate
   npx prisma db push
   ```

5. **Run the development server**

   ```bash
   npm run dev
   ```

6. **Open your browser**
   Navigate to [http://localhost:3000](http://localhost:3000)

## 📊 Database Schema

The application uses Prisma with PostgreSQL. Key models include:

- **User** - User accounts and authentication
- **Note** - Encrypted note storage
- **SharedNote** - Public note sharing
- **Subscription** - Premium subscription management

Run migrations:

```bash
npx prisma migrate dev
```

## 🔐 Security Features

- **Client-side Encryption** - Notes are encrypted before sending to server
- **Zero-knowledge Architecture** - Server cannot read note contents
- **Secure Authentication** - JWT-based auth with secure sessions
- **HTTPS Only** - All communications encrypted in transit
- **Data Privacy** - User data remains private and secure

## 💳 Payment Integration

Textbin integrates with Stripe for subscription management:

- Free tier with basic features
- Premium subscriptions with advanced features
- Secure payment processing
- Subscription management portal
- Webhook handling for payment events

## 🎨 Theming

The app supports custom themes using CSS variables:

- `--background` - Main background color
- `--foreground` - Primary text color
- `--accent` - Brand accent color
- `--surface` - Card/surface backgrounds
- `--border` - Border colors
- `--muted` - Muted text colors

## 📱 Pages & Features

- **/** - Landing page with hero and pricing
- **/signup** - User registration
- **/login** - User authentication
- **/mine** - User's private notes dashboard
- **/new** - Create new notes
- **/share/[id]** - Public note sharing
- **/account** - Account management
- **/pricing** - Subscription plans
- **/about-us** - About page with FAQ

## 🚀 Deployment

### Deploy to Vercel

1. **Connect your repository to Vercel**
2. **Set environment variables in Vercel dashboard**
3. **Deploy**

The app is optimized for Vercel deployment with proper build configurations.

### Environment Setup

Ensure all environment variables are set in your deployment platform:

- Database connection string
- JWT secrets
- Stripe configuration
- App URL

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📧 Support

For support or questions, contact us at contact@textbin.app

## 🔗 Links

- **Live App**: [textbin.app](https://textbin.app)
- **GitHub**: [github.com/chickenjsx/textbin](https://github.com/chickenjsx/textbin)

---

Built with ❤️ by the Textbin team
