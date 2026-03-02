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

