# ARTISAN - Art & Crafts Platform

A web-based platform designed to showcase and explore different forms of paintings and artwork. Artisan provides an interactive space where art enthusiasts can discover creative works, explore different artistic categories, and manage their own artwork collections.

**Live Demo:** [Artisan](https://sa-artisan.web.app/)

**Frontend Repository:** [Artisan](https://github.com/Arefin40/Artisan)

**Backend Repository:** [Artisan Server](https://github.com/Arefin40/Artisan-server)

**Backend API:** [Artisan API](https://artisan-server.vercel.app/)

## Tech Stack

**Prerequisites** 
Make sure you have the following installed:

- Git
- Node.js 18+
- pnpm
- MongoDB Atlas Account
- Firebase Account

**Frontend**
- React 18 - Component-based UI development
- Vite 5 - Fast development server and build tool
- JavaScript - Application logic
- Tailwind CSS v3 - Responsive styling
- React Router DOM - Client-side routing and private routes
- Firebase Authentication - User authentication
- React Hook Form - Form handling and validation
- Axios - HTTP requests and API communication
- Swiper - Responsive sliders and carousels
- React Hot Toast - Notifications and user feedback
- React Awesome Reveal - UI animations
- React Simple Typewriter - Text animations
- Emotion React - Styling support

**Backend**
- Node.js - Server-side JavaScript runtime
- Express.js - REST API development
- MongoDB - Database management and artwork storage
- CORS - Cross-origin resource sharing
- dotenv - Environment variable management
- Nodemon - Automatic server restarting during development

**Hosting**
- Firebase Hosting - Frontend deployment
- Vercel - Backend deployment

## Key Features

- User registration and login with Firebase Authentication.
- Explore paintings through different categories, including Landscape, Portrait, Watercolor, Oil Painting, Charcoal Sketching, and Cartoon Drawing.
- View detailed artwork information with images and descriptions.
- Add new paintings and artwork to the platform.
- Update and delete previously added artwork.
- Manage personal artwork collections through private routes.
- Filter personal artwork based on customization availability.
- Responsive interface for mobile, tablet, and desktop devices.
- Dark and light theme switching.
- Interactive sliders, animations, and loading indicators.

**Problems Solved**

- Lack of a dedicated platform for showcasing different forms of paintings and artwork.
- Difficulty discovering artwork from different artistic categories.
- Limited opportunities for artists to display and manage their creative collections.
- Inconvenient artwork management without centralized CRUD functionality.
- Difficulty organizing and filtering personal artwork collections.
- Inconsistent browsing experiences across different screen sizes.

## Run Locally

**1. Clone the frontend repository**

```bash
git clone https://github.com/Arefin40/Artisan.git
cd Artisan
```

**2. Install frontend dependencies**

```bash
pnpm install
```

**3. Configure Firebase and frontend environment variables**

Create a `.env.local` file in the frontend root directory.

```env
APP_API_URL=http://localhost:3000

APP_API_KEY=your_firebase_api_key
APP_AUTH_DOMAIN=your_firebase_auth_domain
APP_PROJECT_ID=your_firebase_project_id
APP_STORAGE_BUCKET=your_firebase_storage_bucket
APP_MESSAGING_SENDER_ID=your_messaging_sender_id
APP_APP_ID=your_firebase_app_id
```

Replace the placeholder values with your Firebase project credentials.

**4. Clone and configure the backend**

Open another terminal:

```bash
git clone https://github.com/Arefin40/Artisan-server.git
cd Artisan-server
pnpm install
```

Create a `.env` file in the backend root directory:

```env
PORT=3000
MONGO_DB_URI=your_mongodb_connection_string
```

Configure your MongoDB connection string before starting the server.

**5. Start the backend server**

```bash
pnpm run serve
```

The backend will run at `http://localhost:3000`.

**6. Start the frontend development server**

Return to the frontend terminal:

```bash
pnpm run dev
```

Visit: `http://localhost:5173`

**7. Production build**

```bash
pnpm run build
pnpm run preview
```

**Note:** Some artwork CRUD operations currently reference the deployed backend URL directly. For complete local CRUD testing, update those API references in `AddPainting.jsx`, `UpdatePainting.jsx`, and `MyArtsAndCrafts.jsx` to use the local backend URL.

## Challenges Faced During Development

- One of the major challenges was managing user authentication and restricting access to personal artwork management features. Firebase Authentication and React Router private routes helped maintain authentication-based navigation and prevent unauthorized access to protected frontend pages.

- Creating a responsive and interactive gallery experience was also challenging because of the image-heavy nature of the platform. Tailwind CSS, Swiper, and React Awesome Reveal helped create responsive layouts, interactive sliders, and smooth visual animations.

**Live Demo:** https://sa-artisan.web.app/

**ARTISAN - Bringing Creativity and Art Together.**
