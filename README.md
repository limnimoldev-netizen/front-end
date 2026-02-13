# Nuxt Minimal Starter

Look at the [Nuxt documentation](https://nuxt.com/docs/getting-started/introduction) to learn more.

## Setup

Make sure to install dependencies:

```bash
# npm
npm install

# pnpm
pnpm install

# yarn
yarn install

# bun
bun install
```

## Development Server

Start the development server on `http://localhost:3000`:

```bash
# npm
npm run dev

# pnpm
pnpm dev

# yarn
yarn dev

# bun
bun run dev
```

## Production

Build the application for production:

```bash
# npm
npm run build

# pnpm
pnpm build

# yarn
yarn build

# bun
bun run build
```

Locally preview production build:

```bash
# npm
npm run preview

# pnpm
pnpm preview

# yarn
yarn preview

# bun
bun run preview
```

Check out the [deployment documentation](https://nuxt.com/docs/getting-started/deployment) for more information.



# FoxTech Dev 

## Requirements

Ensure you have the follwing software versions installed on system:

-   **PHP**: 8.3
-   **Composer**: 2.7.7 
-   **Node.js**: 22.x
-   **Laravel**:11.x
-   **Tailwind**: 3.x

...

## Installation Instructions

Follow these steps to set up the peoject :



##   Frontend

The frontend is built using **Nuxt 3** and follows a modular structure for better scalability and maintenance.

```bash
frontend/

│
├── assets/          # Images, fonts, and global styles
├── components/      # Reusable Vue components
├── composables/     # Reusable logic (Vue composables)
├── layouts/         # Page layouts
├── middleware/      # Route middleware
├── pages/           # Application routes (file-based routing)
├── plugins/         # Nuxt plugins
├── public/          # Static files
├── server/          # Server-side API (Nitro)
├── stores/          # Pinia state management
├── utils/           # Helper functions
│
├── app.vue          # Main application component
├── nuxt.config.ts   # Nuxt configuration
└── package.json     # Project dependencies





Here the most you should do



```bash
assets/
│
├── css/            # Global stylesheets
│   └── main.css
│
├── images/         # Project images
│   ├── logo.png
│   └── banner.jpg
│
├── fonts/          # Custom fonts
│   └── roboto.ttf
│
└── scss/           # SCSS/SASS files (optional)
    └── variables.scss


```bash
components/
│
├── common/          # Shared UI components
│   ├── Button.vue
│   ├── Input.vue
│   └── Modal.vue
│
├── layout/          # Layout-related components
│   ├── Navbar.vue
│   ├── Sidebar.vue
│   └── Footer.vue
│
├── auth/            # Authentication components
│   ├── LoginForm.vue
│   └── RegisterForm.vue
│
└── dashboard/       # Dashboard widgets
    ├── StatsCard.vue
    └── ChartBox.vue


```bash
pages/
│
├── index.vue          # Home page (/)
├── login.vue          # Login page (/login)
├── register.vue       # Register page (/register)
├── about.vue          # About page (/about)
│
├── dashboard/
│   ├── index.vue      # Dashboard (/dashboard)
│   ├── profile.vue    # Profile (/dashboard/profile)
│   └── settings.vue   # Dashboard Settings
│
└── posts/
    ├── index.vue      # Posts list (/posts)
    └── [id].vue       # Post detail (/posts/:id)

    
# 🌐 PeopleCore

> 👨‍💻 Full Stack Developer  
> Building People-Centered Digital Solutions

# 🌟 PeopleCore

> Full Stack Developer | Web Engineer  
> Nuxt • Laravel • API • Database
