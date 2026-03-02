# INFNOVA Academy

An online learning platform built with Next.js, featuring a modern course catalog with real-time API integration.

## Overview

INFNOVA Academy is a full-stack web application that allows users to explore, search, and view detailed information about technology courses. The platform features a clean, intuitive interface with a vibrant orange color scheme and integrates with a real API for course data.

## Features

- **Course Listing Page** - Browse all available courses with search and filter functionality
- **Course Detail Page** - View comprehensive course information including instructor profile, syllabus, and enrollment details
- **Search Functionality** - Search courses by title, instructor, or description in real-time
- **Difficulty Filtering** - Filter courses by level (Beginner, Intermediate, Advanced)
- **Responsive Design** - Fully responsive for mobile, tablet, and desktop devices
- **Real API Integration** - Fetches live course data from INFNOVA API
- **Loading States** - Beautiful skeleton loaders during data fetching
- **Error Handling** - Graceful error messages with retry functionality
- **Navigation** - Header with logo, navigation links, and authentication buttons
- **Footer** - Comprehensive footer with Quick Links and Support sections

## Tech Stack

- **Framework**: Next.js 16 with App Router
- **Language**: TypeScript
- **Styling**: Tailwind CSS v4
- **UI Components**: shadcn/ui
- **Icons**: Lucide React
- **API**: INFNOVA Course API (https://infnova-course-api.vercel.app)
- **Image Optimization**: Next.js Image component
- **Deployment**: Vercel

## Project Structure

```
infnova-academy/
├── app/
│   ├── page.tsx                 # Home page with hero and courses listing
│   ├── courses/
│   │   └── [id]/
│   │       └── page.tsx         # Course detail page
│   ├── about/
│   │   └── page.tsx             # About page
│   ├── contact/
│   │   └── page.tsx             # Contact page
│   ├── layout.tsx               # Root layout
│   └── globals.css              # Global styles and design tokens
├── components/
│   ├── header.tsx               # Navigation header
│   ├── footer.tsx               # Footer component
│   ├── courses-content.tsx       # Courses listing with search/filter
│   ├── course-detail-content.tsx # Course detail layout
│   ├── course-card.tsx           # Individual course card
│   ├── level-badge.tsx           # Difficulty level badge
│   └── course-skeleton.tsx       # Loading skeleton
├── lib/
│   ├── api.ts                   # API integration and data fetching
│   ├── types.ts                 # TypeScript type definitions
│   └── utils.ts                 # Utility functions
├── public/
│   └── logo.png                 # INFNOVA logo
└── package.json                 # Dependencies

```

## Getting Started

### Prerequisites

- Node.js 18+ and npm/pnpm
- Git
- Code editor (VS Code recommended)

### Installation

1. **Clone the repository:**
```bash
git clone https://github.com/maryagetu/infnova-academy.git
cd infnova-academy
```

2. **Install dependencies:**
```bash
npm install
# or
pnpm install
```

3. **Run development server:**
```bash
npm run dev
# or
pnpm dev
```

4. **Open in browser:**
Navigate to `http://localhost:3000`

## API Integration

The application fetches course data from the INFNOVA API:

**Base URL:** `https://infnova-course-api.vercel.app`

**Endpoints:**
- `GET /api/courses` - Get all courses
- `GET /api/courses/:id` - Get course by ID

**Features:**
- Server-side data fetching with caching (1 hour)
- Automatic data transformation and mapping
- Error handling with user-friendly messages
- Loading states with skeleton loaders

## Pages

### Home Page (`/`)
- Orange hero banner with "Explore Our Courses" tagline
- Search bar for course search
- Difficulty level filters
- Course grid with cards showing course details
- Loading states and error handling

### Course Detail Page (`/courses/[id]`)
- Orange gradient hero section with course image
- Course title, category, and metadata (instructor, duration, enrollment, rating)
- "What You'll Learn" section with two-column layout
- Course description and syllabus
- Enrollment sidebar with buttons
- Instructor profile section
- "This course includes" checklist

### About Page (`/about`)
- Company information and mission
- Vision statement
- Key statistics
- Why choose INFNOVA

### Contact Page (`/contact`)
- Contact form
- Business hours and location
- Phone and email information
- Social media links

## Color Scheme

- **Primary Color (Orange)**: `oklch(0.58 0.25 36.5)` - Used for buttons, badges, links
- **Background**: Light background with dark navy footer
- **Text**: Professional dark text on light backgrounds
- **Accents**: Green checkmarks, yellow ratings

## Deployment

### Deploy to Vercel

1. **Push to GitHub:**
```bash
git add .
git commit -m "Initial commit"
git push origin main
```

2. **Deploy on Vercel:**
- Go to vercel.com
- Click "Add New" → "Project"
- Select your GitHub repository
- Vercel auto-detects Next.js settings
- Click "Deploy"

3. **Get your live URL:**
```
https://infnova-academy.vercel.app
```

## Development

### Running Locally
```bash
npm run dev
```
- Starts dev server at `http://localhost:3000`
- Hot reload on file changes
- Open DevTools (F12) to view console logs for debugging

### Building for Production
```bash
npm run build
npm run start
```

### Linting
```bash
npm run lint
```

## Environment Variables

No environment variables required for basic functionality. The API base URL is hardcoded but can be made configurable by adding to `.env.local`:

```env
NEXT_PUBLIC_API_BASE_URL=https://infnova-course-api.vercel.app
```

## Features Implemented

✅ Real API data integration
✅ Search and filter functionality
✅ Course detail pages with dynamic routing
✅ Responsive mobile-first design
✅ Loading states and error handling
✅ Professional UI with orange branding
✅ INFNOVA logo and navigation
✅ Server-side data fetching with caching
✅ Type-safe TypeScript implementation
✅ SEO optimized with metadata

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Performance

- Server-side rendering for faster initial loads
- Image optimization with Next.js Image component
- CSS caching with Tailwind CSS
- API response caching (1 hour)
- Skeleton loaders for better perceived performance

## Future Enhancements

- User authentication and enrollment
- Student progress tracking
- Course reviews and ratings
- Payment integration
- Certificate generation
- Email notifications
- Admin dashboard

## Contributing

Feel free to fork this repository and submit pull requests for any improvements.

## License

MIT License - feel free to use this project for personal or commercial purposes.

## Support

For issues or questions, contact INFNOVA Academy support or visit our contact page.

## Links

- **Live Site**: https://infnova-academy.vercel.app
- **GitHub Repository**: https://github.com/maryagetu/infnova-academy
- **API Documentation**: https://infnova-course-api.vercel.app

---

Built with Next.js and Tailwind CSS by INFNOVA Academy Team
