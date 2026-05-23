# NEON VIBE

NEON VIBE is a futuristic AI-powered social entertainment platform that enables creators and users to experience an immersive, cyberpunk-inspired world through responsive UI, real-time features, and AI interactions.

---

## 🌌 Features

- **Dark Neon Cyberpunk Design**
- **Responsive & Mobile-First UI**
- **AI Companion System** (Personalized virtual assistant)
- **Secure Authentication** with Supabase
- **Realtime Messaging** + Anonymous Mode
- **Creator Subscriptions** + **Fan Tipping** (Powered by Stripe)
- **User Profiles** + Dashboard for insights
- **Scalable Architecture**
- **Smooth Animations** using Framer Motion
- **Vercel Deployable** (Production-ready)

---

## 🏗️ Tech Stack

- Frontend: Next.js + TailwindCSS + Framer Motion
- Realtime Backend: Supabase
- Database: PostgreSQL (via Supabase)
- Payment Integration: Stripe
- Deployment: Vercel

---

## 🗂️ Folder Structure

```plaintext
neon-vibe/
├── public/                     # Static assets (e.g., images, fonts)
├── src/                        # Main source code
│   ├── components/            # Reusable UI components
│   ├── pages/                 # Next.js pages
│   │   ├── api/              # API routes
│   │   ├── dashboard/        # Creator and user dashboards
│   │   ├── auth/             # Authentication pages
│   │   ├── messaging/        # Realtime chat pages
│   │   └── ...
│   ├── styles/               # TailwindCSS custom styles
│   ├── utils/                # Utility functions
│   ├── config/               # Configuration files (e.g., base URLs, Stripe setup)
│   └── context/              # Global state/context providers
├── supabase/                  # Supabase-related schema/queries
├── .env.example               # Example environment variables
├── next.config.js             # Next.js configuration
├── tailwind.config.js         # TailwindCSS configuration
└── vercel.json                # Vercel deployment configuration
```

---

## 📜 Setup Instructions

1. **Clone the Repository**

```bash
git clone https://github.com/lamhouk/neon-vibe.git
cd neon-vibe
```

2. **Install Dependencies**

Make sure you have `npm` installed, then:

```bash
npm install
```

3. **Set Up Environment Variables**

Create a `.env.local` file and populate it with the following credentials:

```plaintext
NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_public_anon_key
SUPABASE_SERVICE_ROLE_KEY=your_service_role_key
STRIPE_SECRET_KEY=your_stripe_secret_key
STRIPE_WEBHOOK_SECRET=your_stripe_webhook_secret
NEXT_PUBLIC_BASE_URL=your_base_url
```

4. **Database Setup**

Head over to your [Supabase dashboard](https://app.supabase.io/):

- Create a new project.
- Import the database schema provided in `supabase/schema.sql`.

Run the following command to start the development environment:

```bash
npm run dev
```

Access it at `http://localhost:3000`.

---

## 🚀 Deployment (Vercel)

1. Install the [Vercel CLI](https://vercel.com/cli):

```bash
npm install -g vercel
```

2. Login to Vercel:

```bash
vercel login
```

3. Deploy the app:

```bash
vercel
```

Follow the Vercel prompts to configure your project.

---

## 🛠 Roadmap
- Multi-language support
- Advanced analytics for creators
- NFT integration for tipping
