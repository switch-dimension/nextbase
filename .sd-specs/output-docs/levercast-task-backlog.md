# Levercast Task Backlog

## Concise Suggested MVP for First Sprint

The MVP for the first sprint will focus on building out the front-end UI with placeholder components. A user will be able to see the three-column layout and interact with static components. Authentication and AI-powered content generation will be deferred.

- **UI:** Implement the three-column layout for desktop (Input, Editors, Previews) with placeholder components and basic client-side state.
- **Project Setup:** Basic Next.js project setup.
- **Database:** Defer database setup until authentication is implemented.
- **API:** Defer API creation until the backend and content generation phase.

## Concise Task Backlog

### Epic: Project Setup
- [x] **Task:** Initialize Next.js project with TypeScript and Tailwind CSS.
- [x] **Task:** Configure ESLint and Prettier for consistent code quality.
- [x] **Task:** Set up project structure, organizing components, and API routes.

### Epic: UI Scaffolding & Design
- [x] **Task:** Design and build the three-column UI layout with placeholder components.
- [ ] **Task:** Create the text input component for capturing raw content ideas.
- [ ] **Task:** Create the editor components for the LinkedIn and Twitter posts.
- [ ] **Task:** Create the preview components that mimic the look o LinkedIn and Twitter posts.
- [ ] **Task:** Implement the client-side state management for real-time updates between editors and previews (using mock data).

### Epic: User Authentication
- [ ] **Task:** Integrate Clerk for user sign-up, sign-in, and session management.
- [ ] **Task:** Build the UI components for the authentication flow (sign-in page, user profile button).
- [ ] **Task:** Set up Prisma with a SQLite database and define the initial schema to store user data references.
- [ ] **Task:** Implement the server-side logic to handle the OAuth flow for connecting LinkedIn.
- [ ] **Task:** Implement the server-side logic to handle the OAuth flow for connecting Twitter.
- [ ] **Task:** Protect API routes and frontend pages, ensuring they require authentication.

### Epic: Backend & Content Generation
- [ ] **Task:** Implement the `/api/generate` API route.
- [ ] **Task:** Integrate the backend with a third-party LLM service (e.g., OpenAI, Anthropic).
- [ ] **Task:** Connect the frontend UI to the `/api/generate` endpoint to replace mock data with live data.

### Epic: Content Publishing
- [ ] **Task:** Implement the `/api/publish` API route.
- [ ] **Task:** Add logic to retrieve the user's stored OAuth tokens from Clerk on the backend.
- [ ] **Task:** Integrate with the LinkedIn API to publish content.
- [ ] **Task:** Integrate with the Twitter API to publish content.
- [ ] **Task:** Create the "Publish" buttons in the UI and connect them to the publish API.

### Epic: UI/UX & Feature Refinements
- [ ] **Task:** Implement a fully responsive design that adapts the three-column layout to a stacked view on mobile.
- [ ] **Task:** Add voice-to-text input functionality to the input component.
- [ ] **Task:** Implement image handling for attaching images to posts.
- [ ] **Task:** Develop the functionality for users to create and manage their own AI generation templates.
- [ ] **Task:** Conduct a full accessibility audit and implement necessary improvements (WCAG AA).

### Epic: Deployment & Testing
- [ ] **Task:** Write unit tests for critical components and API routes.
- [ ] **Task:** Write end-to-end tests covering the primary user flow from idea generation to publishing.
- [ ] **Task:** Configure a CI/CD pipeline for automated testing and deployment.
- [ ] **Task:** Deploy the application to a suitable hosting provider (e.g., Vercel, Netlify).
