# Portfolio Site Plan

## Plan Overview

Building a beautiful, interactive portfolio site to showcase Noam Shvacher's professional achievements and attract recruiters. The site will prominently feature key wins (30% latency reduction, 100,000+ RPS microservices systems, visual testing automation platform) with compelling visual design, smooth interactions, and clear calls-to-action. Target audience: senior-level tech recruiters and hiring managers.

## Goal

Create a modern, responsive portfolio website that:
- Presents a professional profile with avatar (media/noam.png)
- Highlights key career wins and technical achievements
- Includes smooth animations and interactive elements
- Optimizes for recruiter engagement and conversion
- Loads fast and works across all devices

**Development Approach:**
- **AI-Driven Development**: Leverage cutting-edge AI tools (Claude Code, Gemini, Copilot) to accelerate development cycles, enhance code quality, and demonstrate proficiency with modern AI development practices—directly reflecting the "AI-Driven Development" achievement on your CV
- **Spec-Driven Design**: Follow comprehensive specification documents before implementation; every feature has a clear spec defining requirements, acceptance criteria, and edge cases. This methodology ensures quality and maintainability while showcasing disciplined engineering practices to recruiters

## Acceptance Criteria

- Site loads in < 2s on 4G, passes Lighthouse 90+ on all metrics
- Responsive design: pixel-perfect on mobile, tablet, desktop
- Hero section immediately communicates seniority (Senior Backend Engineer, key metrics)
- "Key Wins" section is visually stunning and persuasive with metrics and outcomes
- Interactive timeline of career progression (IDF → MoonActive → Applitools)
- Tech stack clearly organized by category (Languages, Platforms, Infrastructure)
- All CTAs (LinkedIn, GitHub, Email) are 1-click accessible
- Smooth animations and transitions that feel polished, not distracting
- SEO-friendly with proper meta tags and structured data
- **Development Process Documented**: GitHub repo includes clear specs, commits follow Conventional Commits, AI usage is documented (demonstrates spec-driven + AI-driven methodology to recruiters)

## Context

This portfolio is the primary digital front door for recruiter engagement. The design should immediately establish competence and attention to detail through visual polish. The narrative arc should clearly position Noam as a senior engineer who has:
1. Worked at massive scale (100,000+ RPS)
2. Driven performance wins (30% latency reduction)
3. Led core product development (AI-powered testing platform)
4. Excelled in high-pressure environments (IDF, gaming, YC-backed startup)

The site should feel modern without being trendy—professional but with personality.

## Execution Steps

### Phase 1: Foundation & Design

[ ] - Set up project structure (Next.js/React, Tailwind, TypeScript)
Verify: `npm run dev` starts dev server on localhost:3000 without errors. Project structure includes components/, pages/, public/, styles/ directories.

[ ] - Create layout components (Header, Footer, Hero section, Container)
Verify: All layout components render without errors. Header includes nav links. Footer includes contact info and social links. Both are responsive on mobile/tablet/desktop.

[ ] - Design and implement Hero section with profile image and headline
Verify: Hero displays profile picture (media/noam.png), headline "Senior Backend Engineer", subtitle with key metrics visible. Responsive on all breakpoints. Image loads without distortion.

### Phase 2: Content & Sections

[ ] - Build "Key Wins" section showcasing 3-4 major achievements with metrics
   - Win 1: 30% latency reduction at Applitools (Redis + CDN optimization)
   - Win 2: 100,000+ RPS microservices system at MoonActive
   - Win 3: Visual testing automation platform (Autonomous team lead)
   - Win 4: AI-driven development with Claude Code
Verify: Each win displays title, brief description, key metric, and icon/visual indicator. Layout is 2x2 grid on desktop, stacked on mobile. Animations feel smooth and professional.

[ ] - Build interactive career timeline (IDF → MoonActive → Applitools)
Verify: Timeline shows three major roles with dates, company logos, and key responsibilities. Clicking/hovering on each role reveals detailed tech stack and achievements. Works smoothly on mobile.

[ ] - Build skills section organized by category (Languages, Platforms, Infrastructure, Certificates)
Verify: Skills are grouped logically. Each skill renders as a tag/badge with hover effects. Responsive grid layout. No visual clutter.

### Phase 3: Technical Details

[ ] - Add CV download button and contact CTAs
Verify: CV download link points to the actual CV PDF or provides a way to download. Email link opens mailto: correctly. All CTAs have hover states and are accessible via keyboard.

[ ] - Implement social links (GitHub, LinkedIn) with icons
Verify: Links open in new tabs. Icons display correctly. Hover states are clear. All links are working and point to correct profiles.

[ ] - Add smooth scroll behavior and page transitions
Verify: Navigation links scroll to sections smoothly. Page feels responsive and polished. No janky animations.

### Phase 4: Polish & Performance

[ ] - Optimize images (profile picture, company logos, icons)
Verify: All images load quickly. No layout shift. Images are served in modern formats (WebP with fallback).

[ ] - Performance optimization and SEO
Verify: Lighthouse scores: Performance 90+, Best Practices 95+, SEO 100. Meta tags include title, description. Open Graph tags for social sharing.

### Phase 5: Deployment & Testing

[ ] - Set up deployment on Google Firebase Hosting
Verify: Site is live on Firebase Hosting (auto-generated URL or custom domain). HTTPS enabled. Deploy script is set up (`npm run build && firebase deploy`).

[ ] - Final QA across browsers and devices
Verify: Testing on Chrome, Safari, Firefox on desktop, iPhone, Android tablet. All features work. No console errors. Loading time < 2s on 4G.

[ ] - Final review with user
Verify: User approves design, messaging, and performance. All contact information is correct and working.

## Key Design Principles

- **Hierarchy**: Key wins and metrics jump out immediately
- **Minimalist**: Clean spacing, strategic use of color
- **Interactive**: Subtle animations show technical sophistication without being distracting
- **Fast**: Optimized images, minimal JavaScript, lazy loading where appropriate
- **Mobile-first**: Responsive design starts with mobile, scales up beautifully

## Tech Stack Recommendation

- **Framework**: Next.js 14+ (App Router) with TypeScript
- **Styling**: Tailwind CSS (speed + modern design)
- **Icons**: Heroicons or similar
- **Animations**: Framer Motion (smooth, performant) or CSS-only where possible
- **Hosting**: Google Firebase Hosting (integrates with GCP ecosystem, fast deployment, free tier)
- **SEO**: Next.js built-in support + next-seo package

## Success Metrics

After launch:
- Recruiters can find and contact you within 10 seconds
- Site generates positive first impression (design, performance)
- Clear narrative of career progression and technical excellence
- Key achievements are memorable and quantifiable
