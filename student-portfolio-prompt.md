# MASTER PROMPT — Modern Student Portfolio Website

## 1. ROLE

Act as a **Senior Frontend Architect, UI/UX Designer, and Professional Portfolio Website Builder**, specializing in lightweight, accessible, responsive websites.

Your responsibility is to design and implement a modern personal portfolio for a high-school student preparing for college admissions.

You must demonstrate expertise in:

- HTML5, CSS3, CSS Custom Properties, and Vanilla JavaScript
- Modern editorial web design and responsive layouts
- Light/Dark theme architecture
- Accessibility, performance, and SEO
- Student academic portfolios and college application storytelling
- GitHub Pages and static website deployment

**Important:** This is a student portfolio, NOT a corporate résumé, developer portfolio, or business website.

---

## 2. CONTEXT

### 2.1 Project Overview

Build a modern, professional, visually engaging portfolio website for a high-school student.

**Primary purpose:**

Create a centralized digital identity showcasing the student's academic journey, interests, leadership, extracurricular activities, research, community service, and projects.

**Target audience:**

- College admissions representatives
- University program coordinators
- Scholarship committees
- Internship and research mentors
- School counselors and teachers
- Nonprofit organizations
- Professional networking connections

### 2.2 Student Profile

Use the following as initial context, but keep all content editable and configurable.

- Student Name: [STUDENT_NAME]
- School: Legacy Ranch High School
- Grade: 11
- Graduation Year: [GRADUATION_YEAR]
- Location: Texas, USA
- Intended College Majors: Finance, Business, Economics, or related disciplines
- Academic GPA: [CURRENT_GPA]
- Class Rank: [CURRENT_CLASS_RANK]
- Interests: Entrepreneurship, financial literacy, technology, soccer, community service, and leadership

Additional profile areas:

- DECA participation
- National Honor Society (NHS)
- National Technical Honor Society (NTHS)
- Soccer player
- Certified youth soccer referee
- Community volunteering
- Financial literacy workshops
- Student-led passion projects
- Research and academic interests

**Content integrity rule:** Do not invent awards, GPA values, research publications, leadership titles, volunteering hours, or project outcomes. Use clear placeholders until verified information is supplied.

### 2.3 Visual References

Two reference screenshots will be attached.

**Reference 1 — About Page**

Reproduce the visual language:

- Spacious editorial layout
- Large elegant serif headings
- Italic emphasis within headings
- Two-column composition
- Narrative content on the left
- Compact information cards on the right
- Subtle background grid
- Minimal borders and generous whitespace
- Small uppercase section labels

**Reference 2 — Selected Work Page**

Use its visual structure for projects and research:

- Asymmetric card grid
- One prominent featured card
- Multiple secondary project cards
- Subtle card borders
- Minimal line-art icons
- Compact category labels
- Project summaries and metadata
- Hover interactions

Do not copy branding, logos, names, or written content from the reference website.

Use the screenshots as design inspiration, not as content sources.

### 2.4 Design System

Create a cohesive, minimal, modern design.

**Light Theme**

- Background: `#F5F7FA`
- Cards: `#FFFFFF`
- Primary text: `#171B22`
- Secondary text: `#64748B`
- Accent blue: `#2563EB`
- Subtle border: `#DDE3EC`

**Dark Theme**

- Background: `#101827`
- Cards: `#1C293B`
- Primary text: `#F8FAFC`
- Secondary text: `#94A3B8`
- Accent blue: `#60A5FA`
- Border: `#334155`

**Typography**

- Display headings: Playfair Display or similar editorial serif
- Body text: Inter or similar modern sans-serif
- Labels/metadata: Monospace
- Heading emphasis: Italic serif with accent blue
- Body text: Readable, balanced, high contrast

**Visual characteristics**

- Subtle grid background
- Rounded cards
- Thin borders
- Restrained shadows
- Elegant spacing
- Minimal blue accents
- No excessive gradients
- No flashy animations
- No generic corporate dashboard styling

---

## 3. INSTRUCTIONS

### 3.1 Mandatory Technology Stack

Build using:

- HTML5
- CSS3
- CSS Custom Properties
- Vanilla JavaScript (ES6+)
- Google Fonts (with fallback fonts)
- Font Awesome or inline SVG icons

**Strict constraints:**

- No React
- No Vue
- No Angular
- No TypeScript
- No Node.js
- No npm
- No Vite/Webpack
- No build process
- No backend
- No database
- No Tailwind or Bootstrap
- No jQuery

The initial implementation must be a **single, self-contained `index.html` file** containing HTML, CSS, and JavaScript.

External font/icon CDNs are optional enhancements, not runtime requirements.

The core website must function when opened directly using `file://` and when hosted on any static HTTP server.

Do not use JavaScript module imports, cross-origin fetch requests, or local JSON fetches that would break under `file://`.

### 3.2 Light/Dark Theme

Implement a fully functional theme switcher.

Requirements:

- Default to the system's preferred color scheme for first-time visitors
- Allow manual Light/Dark selection
- Persist user selection in `localStorage`
- Use CSS Custom Properties for all theme colors
- Prevent unnecessary flashes of the wrong theme
- Ensure every component supports both themes
- Maintain readable contrast
- Provide accessible toggle labels
- Gracefully handle unavailable browser storage

### 3.3 Responsive Design

Support:

- Desktop: 1440px and larger
- Laptop: 1024px
- Tablet: 768px
- Mobile: 375px and smaller

Use CSS Grid and Flexbox.

Requirements:

- Responsive navigation
- Mobile hamburger menu
- Flexible card grids
- Readable text sizing
- No horizontal scrolling
- Touch-friendly interactions
- Appropriate image sizing
- Accessible focus states

### 3.4 Website Navigation

Create a clean sticky header.

Suggested navigation:

Home | About | Academics | Activities | Projects | Articles | Contact

Use dropdowns or in-page subsections where appropriate.

Avoid overcrowding the navigation with every content category.

Navigation should support smooth scrolling, active section indicators, and mobile menu functionality.

### 3.5 Content Management

Since this is a static HTML portfolio, use a centralized JavaScript data object to manage repeatable content.

Example:

```javascript
const portfolioData = {
  student: {},
  academics: {},
  interests: [],
  activities: [],
  volunteering: [],
  sports: [],
  awards: [],
  research: [],
  passionProjects: [],
  projects: [],
  articles: [],
  socialLinks: {}
};
```

Render repeatable cards dynamically from the data object using Vanilla JavaScript.

Keep the content structure easy for a nontechnical student to update.

Provide comments explaining where to add or modify content.

Use safe DOM rendering practices. Avoid injecting untrusted user content directly into `innerHTML`.

### 3.6 Content Presentation Principles

- Highlight student growth, curiosity, initiative, and measurable impact.
- Focus on authentic accomplishments rather than exaggerated marketing language.
- Present academics factually.
- Differentiate completed projects from ongoing or planned initiatives.
- Showcase community impact through verified outcomes.
- Use concise, professional, student-appropriate writing.
- Avoid generic corporate phrases.
- Do not create fictional testimonials or statistics.

---

## 4. TASKS

### TASK 1 — Build Home / Hero Section

Create a visually distinctive landing section.

Include placeholders for:

- Student name
- Student portrait
- Short personal headline
- Grade and school
- Intended majors
- Brief personal introduction
- Key academic or leadership highlights

Suggested headline style:

**"Learning with purpose. Building with curiosity."**

CTA buttons:

- Explore My Work
- About Me
- Connect

Use editorial serif typography with italic blue emphasis.

### TASK 2 — About Me

Follow Reference Screenshot 1.

Left column:

- Personal introduction
- Academic journey
- Interests and motivations
- College and career aspirations
- Leadership philosophy
- Community involvement

Right column cards:

- Areas of Interest
- Student Snapshot
- Leadership & Activities
- Social / Community Footprint

Use placeholder content initially.

### TASK 3 — Academics

Create a structured academic profile.

Include:

- High school name
- Current grade
- Graduation year
- Unweighted GPA
- Weighted GPA
- Class rank
- AP courses
- AP exam scores
- Relevant coursework
- Academic interests
- Certifications

Use elegant information cards and compact tables.

Do not invent missing academic information.

Make GPA and rank easy to update each semester.

### TASK 4 — Research & Academic Interests

Build an interactive research portal.

Categories:

- Business
- Finance
- Economics
- Entrepreneurship
- Technology
- Other Academic Research

Features:

- Search by title or keyword
- Category filtering
- Featured research cards
- Research status labels
- Abstract/summary
- Publication date, when available
- External resource links
- Optional PDF links

Use placeholder entries clearly marked as examples.

### TASK 5 — Leadership & Extracurricular Activities

Create activity cards for:

- DECA
- NHS
- NTHS
- School clubs
- Leadership roles
- Competitions
- Student initiatives
- Mentoring activities

Each card should support:

- Activity name
- Organization
- Role
- Duration
- Description
- Responsibilities
- Achievements
- Evidence or external links

### TASK 6 — Community Impact & Volunteering

Showcase student-led service activities.

Support:

- Organization name
- Volunteer role
- Activity description
- Verified service hours
- Date or duration
- Community beneficiaries
- Measurable outcomes
- Photos or documentation

Possible categories:

- Financial literacy workshops
- Community book drives
- Animal welfare volunteering
- Youth mentoring
- Community support programs

Avoid unverified impact metrics.

### TASK 7 — Sports & Athletics

Create a section for athletic involvement.

Include:

- Soccer participation
- Team experience
- Youth referee certification
- Referee experience
- Athletic achievements
- Sports leadership
- Sports education initiatives

Support photos, certificates, and relevant links.

### TASK 8 — Awards & Recognition

Build a responsive awards grid.

Include:

- Academic honors
- NHS / NTHS recognition
- DECA awards, if verified
- Competition awards
- Certifications
- Community recognition

Each award should support:

- Award title
- Issuing organization
- Date
- Description
- Supporting link or image

### TASK 9 — Passion Projects

Follow Reference Screenshot 2 for the visual layout.

Potential categories:

- Financial Literacy for Teens
- Student-led Community Book Drive
- Donation Tracking Platform
- Entrepreneurship Initiatives
- Educational Tools

Each project card should include:

- Project title
- Problem statement
- Student's role
- Target audience
- Proposed solution
- Project status
- Technologies or tools used
- Verified impact
- GitHub/demo link
- Optional images

Visually distinguish:

- Idea
- Planning
- In Progress
- Completed

Do not represent an idea as a completed project.

### TASK 10 — Other Projects

Create cards for:

- Coding projects
- Websites
- Applications
- Academic experiments
- Business simulations
- School assignments worth showcasing

Include technology tags, descriptions, dates, and links.

### TASK 11 — Articles & Blog

Build a searchable article gallery.

Categories:

- Financial Literacy
- Business Principles
- Entrepreneurship
- Student Leadership
- Personal Learning
- Technology
- Community Service

Each article card should support:

- Title
- Category
- Publication date
- Short excerpt
- Reading time
- Article link

Support external LinkedIn articles and locally hosted HTML articles.

Do not require a backend or content management system.

### TASK 12 — Contact & Social Links

Include:

- LinkedIn
- GitHub
- Professional/student email
- Optional educational social channels

Use accessible external links.

Avoid publishing sensitive personal information such as home address, personal phone number, or private school records.

Do not expose private student contact information without explicit approval.

---

## 5. INTERACTIVE FUNCTIONALITY

Implement with Vanilla JavaScript:

1. Light/Dark theme toggle
2. Mobile navigation menu
3. Smooth scrolling
4. Active navigation indicator
5. Project category filters
6. Research search and filtering
7. Article category filtering
8. Expandable project details, where useful
9. Back-to-top control
10. Keyboard-accessible interactions

All controls must work without a backend.

No decorative or nonfunctional buttons.

---

## 6. PERFORMANCE & QUALITY REQUIREMENTS

Prioritize:

- Lightweight HTML/CSS/JS
- Minimal external dependencies
- Fast first render
- Semantic HTML5
- Accessible color contrast
- Keyboard navigation
- Proper image alt text
- Lazy loading for noncritical images
- Reduced-motion preferences
- Basic SEO metadata
- Open Graph metadata
- Responsive layout stability

Do not load large animation libraries or unnecessary JavaScript.

Use CSS animations only when they meaningfully improve usability.

---

## 7. DELIVERABLES

### Phase 1 — Prototype

Generate:

**`index.html`**

Requirements:

- Complete working HTML document
- Embedded CSS
- Embedded Vanilla JavaScript
- Fully working theme toggle
- Responsive navigation
- All required portfolio sections
- Placeholder student data
- Interactive research/project filtering
- Functional local `file://` support
- GitHub Pages compatibility

The output must be actual working code, not pseudocode.

### Phase 2 — Review

After generating the prototype:

- Explain major design decisions briefly
- Identify placeholder content
- Provide instructions to preview locally
- Ask for feedback on layout, typography, colors, navigation, and sections

Do not proceed with major redesigns without review.

### Phase 3 — Content Integration

Only after prototype approval:

- Replace placeholders with verified student information
- Add actual photographs and certificates
- Add project links and research documents
- Add articles and external profiles
- Optimize final content for college admissions audiences

### Phase 4 — Deployment

After approval:

- Prepare GitHub Pages deployment
- Verify static hosting compatibility
- Check mobile responsiveness
- Review accessibility and SEO
- Provide concise publishing instructions

---

## 8. ACCEPTANCE CRITERIA

The prototype is complete only when:

- [ ] It visually reflects the attached reference screenshots.
- [ ] It uses modern blue accents rather than orange.
- [ ] It has elegant serif headings and readable body typography.
- [ ] Both Light and Dark themes work across every section.
- [ ] Theme preference persists across page reloads.
- [ ] It is responsive on mobile, tablet, and desktop.
- [ ] Navigation works correctly.
- [ ] Research and project filtering works.
- [ ] All student portfolio sections exist.
- [ ] Content placeholders are clearly identified.
- [ ] No student accomplishments are fabricated.
- [ ] It works by opening `index.html` directly.
- [ ] It requires no Node.js, npm, or build process.
- [ ] It can be hosted on GitHub Pages.
- [ ] No unnecessary frameworks or dependencies are introduced.

---

## 9. IMPORTANT EXECUTION RULES

1. First inspect the attached screenshots and identify the shared visual design system.
2. Follow the reference layout closely while adapting it to a student portfolio.
3. Build the initial website using placeholders.
4. Do not ask for every content detail before generating the prototype.
5. Use sensible design defaults when information is missing.
6. Prioritize design quality, readability, and simplicity over feature quantity.
7. Do not generate a reusable Claude Skill, agent, or automation.
8. Do not create unnecessary files.
9. Do not introduce frameworks without approval.
10. Stop after delivering the first working prototype and wait for my review.

**FINAL INSTRUCTION:**

Create a beautiful, production-quality, lightweight student portfolio that feels like a premium modern editorial website—not a generic student résumé template.

Start with the attached visual references, implement the complete working `index.html`, and make it ready for visual review.