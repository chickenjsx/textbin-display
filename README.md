# Textbin

**The secure platform for dumping your ideas instantly.**

**This repository is for display purposes only. It helps me preserve the integrity and ownership of the code’s intellectual property.**

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


## 📧 Support

For support or questions, contact us at contact@textbin.app

## 🔗 Links

- **Live App**: [textbin.app](https://textbin.app)
- **GitHub**: [github.com/chickenjsx/textbin](https://github.com/chickenjsx/textbin)

---

Built with ❤️ by the Textbin team
