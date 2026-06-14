# WD-001: Online Gaming Website

**Category:** Web Development


## Context

GameSphere Digital Solutions Pvt. Ltd. is a Bengaluru-based web development and digital entertainment company seeking to launch a centralized browser-based gaming portal called GameSphere. The platform will allow casual gamers across India to discover, play, and compete in HTML5 games without downloading any software. The immediate use case is an MVP launch targeting desktop and mobile users, with the goal of validating user engagement through profile management, leaderboards, and achievement systems. This project is a fully functional web application, not a prototype or design mockup.

This milestone covers end-to-end development and deployment of the gaming portal. The platform is NOT a game development project - embedded games may use freely available HTML5 game libraries. The deployment target is a standard web host accessible via a public URL.


## Project Information

| Field | Details |
|---|---|
| Project ID | WD-001 |
| Category | Web Development |
| Project Type | Online Gaming Portal |
| Client / Brand | GameSphere Digital Solutions Pvt. Ltd. |
| Platform / Medium | Responsive Web Application (Desktop, Tablet, Mobile) |
| Deliverable Type | Source code (.zip) + Deployed live URL + Documentation (.md) |
| Primary Goal | Launch a fully functional gaming portal where users can register, play HTML5 games, track scores, earn badges, and compete on leaderboards |


## Main Goal

Deliver a complete, deployed online gaming website for GameSphere Digital Solutions that enables user registration and authentication, a browsable and searchable game catalog with at least 6 embedded HTML5 games, score tracking per game, achievement badges, a favorites system, leaderboards, and an admin dashboard for platform management.

1. User-facing gaming portal with authentication, game catalog, leaderboard, and achievement system
2. Admin dashboard for managing users, games, and platform content
3. Deployed live URL with full source code and README documentation


## About GameSphere Digital Solutions Pvt. Ltd.

GameSphere Digital Solutions Pvt. Ltd. is a web development and digital entertainment company based in Bengaluru, Karnataka, India. The company specializes in creating innovative web applications, interactive platforms, and digital entertainment solutions. With expertise in modern web technologies, UI design, and scalable system development, they deliver secure, responsive, and high-performance digital products.

**Brand tone:** Modern, engaging, energetic, accessible
**Brand line / tagline:** `Play. Compete. Conquer.`


## Requirements

The freelancer will build a fully functional responsive online gaming portal with user authentication, game catalog, embedded HTML5 games, score tracking, badges, leaderboards, favorites, and an admin dashboard.

### Core Features

1. Users can register with email and password and log in and log out securely.
2. Authenticated users can browse a catalog of at least 6 embedded HTML5 games.
3. Each game must display a title, thumbnail image, short description, and genre tag.
4. Users can search the game catalog by game title using a live search input field.
5. Users can filter the game catalog by genre using a dropdown or tab selector.
6. Each game opens inside a dedicated game page that embeds the playable HTML5 game in an iframe or canvas element.
7. The platform records and displays a high score per user per game, updated automatically when a new session score exceeds the stored score.
8. Users can mark any game as a favorite and view all favorites in a dedicated Favorites page.
9. The platform displays a leaderboard per game showing the top 10 users ranked by high score.
10. Users can view their profile page showing username, avatar upload option, total games played, total score, and earned badges.
11. Achievement badges are awarded automatically based on the following triggers and must not require manual assignment.

### Achievement Badges (Minimum 5 Required)

| Badge Name | Trigger |
|---|---|
| First Win | User submits their first game score |
| High Roller | User achieves a score above 1000 in any single game session |
| Game Explorer | User plays 3 or more different games |
| Favorite Collector | User adds 5 or more games to favorites |
| Leaderboard Legend | User appears in the top 3 of any game leaderboard |

### Admin Dashboard

- Admin can view a list of all registered users with username and registration date.
- Admin can add a new game by entering title, description, genre, thumbnail URL, and game embed URL.
- Admin can remove an existing game from the catalog.
- Admin can deactivate a user account, preventing login without deleting the account.
- Admin dashboard is protected behind a separate admin login and is not accessible to regular users.

### User Profile

- Profile page displays the user's username, avatar (default placeholder if none uploaded), total games played count, cumulative total score across all games, and list of earned badges.
- Users can upload a profile avatar image (JPEG or PNG, max 2 MB).
- Users can change their display username from the profile page without changing their login email.

### Leaderboard

- Global leaderboard page shows the top 10 users ranked by cumulative total score across all games.
- Per-game leaderboard shows top 10 users by that game's high score.
- Both leaderboards display rank number, username, avatar thumbnail, and score.


## Technical Requirements

- **Frontend Framework:** React.js (v18 or later) or Next.js (v14 or later)
- **Backend Framework:** Node.js with Express.js OR Django (Python)
- **Database:** PostgreSQL or MongoDB
- **Authentication:** JWT-based session authentication with secure token storage; no OAuth required
- **Hosting:** Deployed to a publicly accessible URL (Vercel, Render, Railway, or equivalent free-tier host)
- **Language:** JavaScript / TypeScript (frontend); JavaScript or Python (backend)
- **Resolution / Responsive:** Fully responsive at 320 px (mobile), 768 px (tablet), and 1280 px (desktop)
- **Browser Support:** Chrome, Firefox, Edge, Safari — latest two versions each
- **Code quality:** Clean, commented, organized by feature folder

### Allowed Tech Stack

1. React.js or Next.js (frontend)
2. Node.js + Express.js or Django (backend)
3. PostgreSQL or MongoDB (database)
4. Tailwind CSS or plain CSS/SCSS (styling)
5. Free-tier cloud hosting with public URL

### Not Allowed

- Paid plugins, premium themes, or proprietary libraries requiring a license
- Firebase or Supabase as the sole backend (custom API required)
- Server-side rendering only without any client-side interactivity
- Games developed from scratch — use freely available HTML5 games or open-source game embeds


## Visual and Technical Specs

### Dimensions / Sizing

- **Breakpoints:** 320 px (mobile min), 768 px (tablet), 1280 px (desktop)
- **Game iframe / embed area:** Minimum 600 × 400 px on desktop; scales proportionally on smaller screens
- **Thumbnail images:** 300 × 200 px minimum per game card
- **Avatar image display size:** 80 × 80 px circular crop

### Colors (Suggested — Developer May Adjust)

| Purpose | Color Name | Hex |
|---|---|---|
| Primary | Dark Navy | `#0F172A` |
| Accent | Electric Blue | `#3B82F6` |
| Highlight | Amber | `#F59E0B` |
| Background | Deep Gray | `#1E293B` |
| Text | Off White | `#F8FAFC` |

### Typography

| Usage | Font | Notes |
|---|---|---|
| Headings | Inter Bold or Poppins Bold | Weight 700 |
| Body | Inter Regular | Weight 400 |
| Score / Numbers | Roboto Mono | Monospace for score display |


## Folder Structure

```
gamesphere/
  client/
    src/
      components/
      pages/
      hooks/
      context/
      assets/
  server/
    routes/
    controllers/
    models/
    middleware/
    config/
  docs/
    README.md
  .env.example
```


## Deliverables

| S.no. | Item | Format | Notes |
|---|---|---|---|
| 01 | Complete source code | `.zip` | Organized per folder structure above |
| 02 | Deployed live URL | Public URL | Must be accessible without login for catalog browsing |
| 03 | README documentation | `.md` | Setup, env variables, local run, admin credentials |
| 04 | .env.example file | `.env.example` | All required environment variable keys with placeholder values |
| 05 | Admin login credentials | Listed in README | Default admin username and password |
| 06 | Screenshot gallery | `.png` | Minimum 5 screenshots: home, catalog, game page, profile, admin dashboard |

### File Naming Convention

```
GAMESPHERE_[item-name]_v1.0_[YYYY-MM-DD].[ext]
```

**Example:** `GAMESPHERE_source-code_v1.0_2026-06-01.zip`

Rules:
- Use uppercase prefix, kebab-case for item name
- No spaces
- No alternate naming structures

### Folder Structure (Delivered ZIP)

```
GAMESPHERE_source-code_v1.0_[date]/
  client/
  server/
  docs/
    README.md
  .env.example
  screenshots/
    01_home.png
    02_catalog.png
    03_game-page.png
    04_profile.png
    05_admin.png
```


## Scope Boundaries

### DO
- Build a complete, deployed gaming portal accessible via a public URL
- Embed at least 6 existing freely available HTML5 games
- Implement all 5 achievement badges with automatic trigger logic
- Include full admin dashboard with user and game management
- Use free-tier hosting so the URL remains live through the review period

### DO NOT
- Develop original HTML5 games from scratch
- Implement real-money payments, subscriptions, or in-app purchases
- Build native mobile apps (iOS or Android)
- Add multiplayer real-time game functionality
- Implement social login (Google, Facebook OAuth)
- Use a frontend-only setup with no backend API


## Tool Requirements

- **Required tools:** Any modern code editor; Node.js v18+ or Python 3.10+; PostgreSQL or MongoDB
- **Acceptable alternatives:** Next.js instead of React + Express, Django REST Framework instead of Express
- **Forbidden:** No-code builders (Webflow, Bubble, Wix), Firebase as the sole backend, paid hosting plans


## Quality Control / Pre-Submission Checklist

Before submitting, confirm all of the following:

1. [ ] The live URL is publicly accessible and all 6 games load and are playable.
2. [ ] New user registration and login work without errors.
3. [ ] High scores update correctly after a game session ends.
4. [ ] All 5 achievement badges trigger automatically based on their defined conditions.
5. [ ] Favorites page shows only games marked by the logged-in user.
6. [ ] Global and per-game leaderboards display correct rankings.
7. [ ] Admin dashboard allows adding, removing games and deactivating users.
8. [ ] The website is fully usable on a 375 px wide mobile screen.
9. [ ] README contains all environment variables and setup steps.
10. [ ] All files follow the required naming convention and folder structure.


## Acceptance Checklist

1. [ ] Live URL is accessible and returns a functioning homepage without login errors.
2. [ ] Registering a new account with email and password succeeds and logs the user in.
3. [ ] At least 6 games appear in the catalog, each with title, thumbnail, description, and genre tag.
4. [ ] Searching by a game title filters the catalog in real time.
5. [ ] Filtering by genre shows only games of that genre.
6. [ ] A game opens and is playable on the game detail page.
7. [ ] A score submitted after gameplay appears on the per-game leaderboard.
8. [ ] Marking a game as favorite adds it to the Favorites page and removing it removes it.
9. [ ] The profile page shows total games played, total score, and earned badges.
10. [ ] All 5 badges trigger automatically when their conditions are met.
11. [ ] Admin can add a new game and it appears in the catalog immediately.
12. [ ] Admin can deactivate a user and that user cannot log in afterward.
13. [ ] The site renders without horizontal scroll on a 375 px wide screen.
14. [ ] Source code ZIP matches the required folder structure.
15. [ ] README lists all environment variables and default admin credentials.


## Evaluation Criteria

- Catalog completeness: all 6 games are present, playable, and correctly tagged
- Authentication security: JWT tokens are stored securely; no plain-text passwords in the database
- Score tracking accuracy: high scores update only when a new session score exceeds the stored value
- Badge automation: all 5 badges fire on the correct trigger without any manual admin action
- Leaderboard correctness: rankings are ordered by score descending; ties show equal rank
- Responsive fidelity: no broken layouts or overflow at 375 px, 768 px, and 1280 px
- Admin dashboard functionality: game add/remove and user deactivation work as specified
- Code quality: files are organized per the required folder structure with comments on non-obvious logic
- Documentation completeness: README enables a new developer to run the project locally from scratch


## Developer's Choices

| Decision | Accepted Options |
|---|---|
| Frontend framework | React.js v18+, Next.js v14+ |
| Backend framework | Node.js + Express.js, Django + DRF |
| Database | PostgreSQL, MongoDB |
| CSS approach | Tailwind CSS, plain CSS, SCSS |
| HTML5 game source | Open-source game libraries, freely embeddable third-party games |
| Hosting platform | Vercel, Render, Railway, Netlify, or equivalent free-tier |


## Delivery Terms

- **Revisions included:** 1 round of minor revisions
- **Allowed revision types:** Bug fixes, broken game embeds, missing badge triggers, leaderboard sorting errors
- **What does not count as a revision:** Adding new games beyond the 6 required, redesigning the UI, adding features outside this brief
- **Delivery method:** ZIP under 500 MB via transfer link valid 7 or more days, plus a live URL that remains accessible for 14 days after delivery


## Final Goal

Success means a real user can open the GameSphere URL on their phone or desktop, create an account, browse a catalog of six or more playable HTML5 games, compete for leaderboard rankings, collect achievement badges, and save favorites to their profile — all without any guidance beyond the interface itself. The admin can log into a separate dashboard and manage the game catalog and user accounts. The source code is clean enough that a new developer can clone the repository, follow the README, and run the project locally within thirty minutes.
