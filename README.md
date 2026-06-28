# Unslopme
> **Created by TheMankou**

A unified, multi-agent configuration framework designed to wake AI up, purge statistical-mean defaults, and strip out generic AI slop from your codebases, landing pages, styling, and copy.
Compatible with VS Code (Cursor, Windsurf, Cline, Roo Code), Claude Code / Claude CLI, Google Antigravity, and GitHub Copilot.

## Why does this exist?
When you ask an AI model to build a layout or write text without feeding it explicit visual or linguistic constraints, it doesn't choose—it averages. It pulls from the absolute dead-center statistical mean of modern SaaS patterns. The result is AI Slop: identical bento grids, indigo-to-purple dark mode glows, predictable staggered animations, and a vocabulary flooded with repetitive, algorithmic keywords.
`unslopme` sets a hard, aggressive system-level boundary that forces AI models to drop the boilerplate and write code with human intent.

## Installation & Setup

### Google Antigravity & Claude Code
This repository is natively formatted as an Antigravity/Claude skill. 
- You can simply install or link this entire repository directly as a skill. The `SKILL.md` file at the root will automatically be recognized and triggered when you use the `@unslopme` command.

### Cursor, Windsurf, Cline & GitHub Copilot
To use this inside your specific IDE:
1. Copy the core `SKILL.md` file from this repository into the root of your project workspace.
2. Open the `templates/` directory in this repository and copy the pointer file for your specific tool (e.g. `.cursorrules`, `.clinerules`, `.windsurfdoc`, or `copilot-instructions.md`) into your project root.
3. These pointer files will ensure your AI agent reads `SKILL.md` before generating code.

## Usage
Once installed, use the trigger phrase whenever your AI agent starts outputting generic design or code:
> **User:** `@unslopme build a feature section for my landing page showing our API speeds`

The underlying agent will read the manifesto ruleset, skip the bento grids, skip the purple radial backgrounds, drop the generic copywriting, and write custom, performance-focused layout code.

## Contributing
Found a new piece of AI slop popping up in modern frontier models? Submit a PR to update `SKILL.md` and keep the filters sharp!
License: MIT

---

### The Master Appendix: Every AI Slop Cliché (Complete List)

#### Layout & Visual Architecture
* **The Centered Hero + Status Pill Combo:** A tiny, rounded badge containing an emoji (e.g., "✨ Introducing v2.0") floating directly above a massive, perfectly centered $H1$ containing generic text like "Scale Without Limits".
* **Reflexive Bento Grid Overkill:** Slicing up feature sections into asymmetrical rectangular grid boxes filled with flat icons, short copy, and meaningless charts, completely ignoring whether the features make logical sense in that structure.
* **The Symmetrical Dual-CTA Fold:** Forcing two identically proportioned primary buttons next to each other in the hero section—one high-contrast filled, one outlined—violating visual hierarchy because the AI cannot commit to a single target user path.
* **The "Wall of Shame" Logo Cloud:** A faded, monochrome row of tech logos (usually Stripe, Vercel, and Supabase) directly below the hero section accompanied by an unearned caption like "Trusted by forward-thinking teams".
* **The Floating Dashboard Mockup:** Dropping a generic, slightly angled, or isometric screenshot of a fictional application dashboard immediately beneath the main call-to-action.
* **The Falsified Stats Strip:** A horizontal banner boasting completely arbitrary success metrics: "99.9% Uptime", "10M+ Queries", "500% ROI Increase".
* **The Left-Only Border Card Accent:** Relying on a thick, colorful left-side border (`border-l-4 border-indigo-500`) on every grid card to force a layout structure instead of utilizing real semantic separation or spacing.
* **The Reflexive "Rule of Three" Feature Row:** Defaulting to a flat, horizontal row of exactly three feature or pricing cards simply because it looks mathematically tidy, regardless of actual content constraints.
* **The Left-Aligned Title / Centered Content Split:** Starting a section with a clean, left-aligned title block, but nesting a perfectly centered grid directly beneath it, breaking the page's vertical alignment rhythm.
* **Absolute Card Layering Shortcuts:** To simulate visual depth, stacking absolute layers (`absolute -top-4 -right-4`) containing cropped, blurred graphic elements that clip text on mobile or interact unpredictably with scrolling containers.
* **The Reflexive "Most Popular" Pricing Tier:** Automatically generating a 3-column pricing table where the middle tier is popped out, scaled up, and labeled "Most Popular" without any business logic to support it.
* **The Sparkle & Rocket Monoculture:** Over-relying on the 🚀, ✨, and ⚡ emojis to represent every single feature instead of using custom SVG geometry.

#### Tailwind, CSS, & Styling Clichés
* **The Indigo-to-Purple Dark Mode Glow:** Automatically defaulting to a pitch-black or deeply saturated gray background (`#0b0b0f`) mixed with a massive, soft radial gradient blending dark blue, indigo, and purple floating aimlessly behind containers.
* **The Lazy 1px Gray Border:** Placing a uniform, semi-transparent gray border around every card, button, layout block, and dropdown instead of using white space, elevation shadows, or subtle background shifts.
* **Corner Radius Monoculture:** Hardcoding a single, uniform mathematical roundness (usually `border-radius: 16px` or `rounded-2xl`) globally across all inputs, buttons, cards, and containers, flattening the visual hierarchy.
* **Overdone Grid & Dotted Overlays:** Masking lazy design layouts by throwing subtle CSS background grid patterns or dotted structures underneath elements to force a pseudo "engineering-focused" or "cyberpunk" look.
* **Backdrop Blur Abuse:** Applying `backdrop-blur-md` and semi-transparent backgrounds (`bg-white/10` or `bg-black/40`) to every navbar, dropdown, modal, and card, creating muddy overlapping artifacts.
* **The Rotating Gradient Border:** Wrapping interactive elements or priority cards in an infinite animation loop where a high-contrast gradient rotates around the perimeter of the container.
* **The Double-Nested Radius Error:** Forgetting to adjust padding offsets when nesting containers, resulting in identical corner radii on both the outer card and the inner element, making the corners look warped and broken.
* **The Neon Accent Flashbang:** Using highly saturated, uncalibrated primary colors (like pure green `#00FF00` or bright magenta `#FF00FF`) for subtle tag labels, which creates jagged visual artifacts along text edges on dark modes.
* **Unchecked Text Inversion:** Blanket-setting global dark text classes (`text-zinc-900`) on a section container that was manually styled with a dark background, rendering the text completely invisible.
* **Infinitely Looping Shimmer Buttons:** Attaching an animated, angled gradient streak that infinitely loops across the background of primary CTA buttons, adding visual noise and diluting user focus.
* **The Default Palette Crutch:** Relying exclusively on unmodified base Tailwind colors (e.g., raw `blue-500` or `indigo-600`) without defining a custom, brand-specific color palette or altering lightness/saturation.
* **The Excessive Soft Shadow:** Throwing massive, blurry `shadow-2xl` dropshadows on every single interactive card instead of relying on borders or subtle elevation.

#### Typography & Micro-Spacing Tells
* **The "Inter / Geist / Space Grotesk" Monoculture:** Setting an entire page in a single neutral sans-serif variable font with no intentional font pairing or structural variation, making the text look entirely generic.
* **The Random Editorial Italic:** Dropping a single serif italic word into the middle of a massive sans-serif headline just to look trendy or editorial.
* **Zero Display Kerning:** Outputting large display headings (above 36px or 48px) without setting micro-spacing tight tracking properties like `tracking-tight` or `tracking-tighter`, leaving large letters looking bloated and uncomfortably wide.
* **Static Line-Height Defaults:** Using standard body line-height ratios (`leading-normal` or `leading-relaxed`) for massive display titles, which causes headlines to break across lines with giant, empty gaps of white space.
* **The "Vibe-Check" Single Font Weight:** Styling an entire page utilizing a single heavy font weight (`font-semibold` or `font-bold`) for labels, tags, body descriptions, and inputs alike, destroying reading hierarchy.

#### Micro-Interactions & Animation Traps
* **The Infinite Staggered Fade-In Cascade:** Throwing framer-motion or GSAP scroll animations on every single text block, card, and icon on the page, forcing them to drift upward by 20px as you scroll. This adds input latency and disrupts reading.
* **The `hover:scale-105` Reflex:** Attaching active scale transitions to every single interactive block or image on the screen, causing layout shaking if the containers are tight.
* **Unconstrained Marquee Loops:** Splicing in an infinite horizontal sliding marquee for partner logos or testimonials that runs at a high frame rate, killing CPU and battery cycles on mobile browsers because it lacks hardware-acceleration properties.
* **Rigid Spring Physics Overuse:** Applying identical spring bounce physics (stiffness: 100, damping: 10) to every single dropdown, modal slide, and tooltip, making minor utility panels bounce around unnecessarily.

#### Architectural, Logic, & Code Slop
* **Immaculate READMEs, Zero Error Handling:** Generating perfectly formatted Markdown repository files complete with clean directory trees, but leaving the actual codebase entirely devoid of try/catch blocks, input validation, or edge-case safety.
* **The Global Component Multiplier:** Creating distinct files for tiny variations of the exact same element (e.g., `PrimaryButton.tsx`, `SecondaryButton.tsx`, `HeroButton.tsx`) instead of utilizing configurable component variants or props.
* **The Hardcoded Client/Server Boundary Panic:** Slapping `'use client'` at the absolute top of every single layout or page file in Next.js applications just to bypass an immediate state error, breaking server-side rendering benefits.
* **The Phantom useEffect Dependency Loop:** Writing complex layout or data states with empty dependency arrays `[]` or omitting critical variables, causing endless component re-renders that kill browser performance silently.
* **Inline Tailwind Bloat:** Generating single files with unreadable strings of 40+ utility classes packed into individual elements instead of breaking styling into reusable layout tokens or components.
* **Arbitrary z-index Spam:** Fixing overlapping visibility bugs by dropping random, massive layers onto components (`z-50`, `z-[9999]`) rather than cleaning up the DOM stacking context.
* **The Multi-State Flag Trap:** Controlling a single UI view by managing multiple, contradictory boolean states simultaneously (e.g., `const [isLoading, setIsLoading] = useState(false)` running right alongside `isError` and `isSuccess`), leading to broken, simultaneous rendering states.
* **The JSON.parse Crash Hazard:** Directly handling raw API payloads or LocalStorage data inside a `JSON.parse()` wrapper without a try/catch safety net, allowing an invalid data string to crash the entire application runtime.
* **The Inline Function Re-allocation:** Dropping raw anonymous arrow functions directly into rendering loops inside heavy scroll lists (`onClick={() => handleSelection(item.id)}`), forcing the JavaScript engine to wastefully re-allocate memory on every render cycle.
* **The Redundant `w-full w-full` Duplication:** Stacking duplicate or redundant sizing classes onto a single DOM element out of layout panic (e.g., `class="w-full max-w-full min-w-full flex-1"`).
* **The Over-Sanitized React Key String:** Defaulting to completely random, generated string concatenations or array index templates for database elements instead of referencing proper database IDs (`key={\`card-item-fallback-id-${index}-${item.title}\`}`).
* **The Empty Clean-up Wrapper Loop:** Generating layout component return hooks stuffed with nested, empty layout blocks, fragments, or zero-utility wrappers (`<div><div><div><Component/></div></div></div>`) because it struggled to safely resolve a flex block or layout error.
* **The Premature Optimization Trap:** Reflexively wrapping every single React function in `useCallback` and every variable in `useMemo` when there are zero actual performance bottlenecks, creating unreadable code.

#### Responsive & Mobile Design Failures
* **The Desktop-First `hidden md:block` Escape Route:** Hiding complex or broken responsive components entirely on mobile screens, replacing rich interactive sections with a lazy, flat text bullet list for mobile users.
* **The Locked Viewport Clip:** Forcing layout containers into absolute pixel heights (`h-[800px]`) that clip text content on smaller mobile devices, breaking native touch scrolling.
* **The Tiny Thumb Target:** Rendering tightly packed rows of utility buttons or pagination links that drop well below the standard 44x44px minimum touch target size, making the interface a nightmare to navigate on mobile.
* **The Unchecked Horizontal Overflow:** Letting wide code syntax blocks, tables, or nested bento boxes spill off the right side of mobile viewports, introducing horizontal layout wobble.

#### API & Data-Handling Illusions
* **The Hardcoded fetch Endpoint String:** Dropping absolute local paths like `fetch('http://localhost:3000/api/users')` deep within frontend UI component code, ensuring the build immediately crashes in production.
* **The Blank State Amnesia:** Forgetting to write loading skeletons, Spinners, or empty states. The page displays a completely broken, unstyled layout for a split second while waiting for asynchronous API data to arrive.
* **The Un-paginated Map Loop:** Writing generic queries that pull all database records at once, mapping them directly to the DOM without implementing infinite scroll, limits, or pagination—guaranteeing a browser crash once production data grows.
* **The Optimistic Success Scenario:** Writing network mutation code that completely assumes an HTTP 200 OK response, missing catch blocks to handle timeouts, validation errors, or payment failures.

#### Git & Repo Structure Litter
* **The Missing .gitignore Avalanche:** Committing giant directories of system junk directly into the public repository—stuff like the local `.next/` build output, `.env` files containing raw security keys, and the massive `node_modules/` folder.
* **The Uniform "Initial Commit" History:** Bundling 4,000 lines of highly complex application logic, styling systems, and database schemas into one single, massive initial commit, leaving zero step-by-step developer history.
* **The Ghost Config File Cluster:** Dropping configuration files for four different styling and build tools simultaneously (e.g., mixing up Tailwind config formats, outdated PostCSS variants, and unnecessary Webpack configurations) because it got confused across conflicting framework prompts.

#### Accessibility (a11y) Shortcuts
* **The Clickable `<div>` Without ARIA:** Making layout boxes or custom cards interactive by slapping an `onClick` handler directly onto a plain `<div>`, completely skipping `role="button"`, keyboard navigation support (`onKeyDown`), or `tabIndex={0}`.
* **The Redundant Image Alt Tag:** Outputting trash for image descriptions, frequently outputting literal variable names or structural phrases like `alt="hero image illustration"` or `alt="icon_3_final"`.
* **The Heading Hierarchy Chaos:** Jumping wildly across heading ranks based entirely on font size choices rather than semantic structure (e.g., placing an `<h3>` directly inside a hero section, followed by an `<h1>` lower down the page).
* **The Empty Icon-Only Button:** Creating sleek, minimalist utility buttons containing only an icon component with zero inner text, zero `aria-label`, and zero hidden screen-reader text (`sr-only`), leaving it entirely contextless for assistive technologies.

#### Production Deployment Landmines
* **The Env-Var Breakage Trap:** Referencing arbitrary environment variables inside static site generation steps without providing safe fallbacks, crashing the entire production build if the variable isn't injected on the build server.
* **The Hardcoded Date Copyright Footer:** Outputting a literal static string like `© 2024 Company Name` inside the footer component instead of using a runtime lookup or a reliable date utility, causing the site to instantly look neglected and outdated.
* **The Mixed Content HTTP Protocol Leak:** Hardcoding third-party asset pathways or font CDNs using unsecured `http://` protocols, triggering mixed-content block warnings in production browsers forcing `https://`.

#### Security & Input Vulnerabilities
* **The `dangerouslySetInnerHTML` Open Invitation:** Rendering user-generated input fields or external API text payloads directly using React’s `dangerouslySetInnerHTML` or raw `innerHTML` properties without running it through a sanitization library (like DOMPurify), exposing the application to basic Cross-Site Scripting (XSS) injections.
* **Client-Side Premium Feature Security:** Attempting to lock down premium interfaces, admin dashboards, or gated paywall sections using nothing but client-side routing logic flags (`if (!user.isPremium) router.push('/pricing')`), which is completely bypassable via developer tools.
* **The Raw Console Log Data Leak:** Leaving verbose debugging logs like `console.log("USER DATA FOR DEBUG:", user)` wide open within form submissions or authentication flows, printing sensitive user tokens, emails, or internal state schemas directly to the production browser console.
* **The Over-Indexed Prisma/ORM Query:** Writing database operations that pull down complete, bloated multi-column user or post rows instead of explicitly scoping down the payload size using selective queries, creating massive backend latency.
* **The Missing Uniqueness Constraint Panic:** Setting up registration or database writing routines that completely omit safe upsert logic, transaction batching, or duplicate validation rules, throwing hard unhandled 500 server crashes the moment a user clicks a submit button twice.

#### Text, Copywriting, & SEO/AEO/GEO Slop
* **The Predictive Introduction Blueprint:** Framing articles with predictable macro-statements: "In today's fast-paced digital world...", "In the rapidly evolving landscape of X...", or "Now more than ever, businesses are turning to X."
* **The Incessant "Key Takeaways" TL;DR Box:** Plunking down an identical, 3-bullet "Key Takeaways" card right under the $H1$ heading of every single piece of content, resulting in repetitive, recycled text that says the exact same thing as the intro.
* **The Uniform FAQ Schema Stack:** Ending every single blog post, landing page, or service page with exactly 4 to 5 highly generic questions formatted in perfect accordions purely to inject microdata schemas for Google rich snippets.
* **The Parallel Bullet List Overkill:** Structuring sections with a bulleted list where every single bullet begins with a bolded 2-3 word concept hook (Enhanced Performance: Boosts your...).
* **The Aggressive Synonym Loop:** Stuffing multiple variations of the same keyword phrase into a single paragraph to hit LSI (Latent Semantic Indexing) entities ("automated sales agent", "AI sales bot", "autonomous selling software").
* **The Over-Literal Search Intent Heading:** Writing headings that look like raw Google searches instead of natural, editorial copy (e.g., `## How to fix Solana transaction dropped node error`).
* **The Geometric Internal Link Spam:** Inserting hyper-obvious, automated internal anchor text into every single paragraph to pass an SEO checklist.
* **The Definitive "Is" Paragraph (The Definition Bait):** Starting sections with an unprompted, textbook-style definition paragraph optimized purely for LLM scrapers to extract as a direct answer ([Concept] is a [Category] that allows users to [Action]).
* **The "It's Important to Note" Safe-Guarding Cushion:** Littering paragraphs with passive, defensive transitions to avoid making hard, absolute claims ("While X is highly effective, it's worth noting that individual results may vary").
* **The Fake Consensus Statement:** Inventing fake industry consensus to signal authority: "Experts agree that...", "The industry standard is moving towards...", or "According to recent trends..." without ever citing a single concrete source.
* **The Linguistic "Uncanny Valley" Vocabulary:** Relying on words heavily baked into core LLM reinforcement tuning: repetitive algorithmic keywords (e.g., "elevate", "dynamic", "bespoke").
* **The Hyphenated Buzzword Chain:** Creating artificial compound adjectives by stringing words together with hyphens to sound technical or advanced (e.g., "game-changing", "next-generation", "hyper-scalable", "future-proof").
* **The Grandiose Conclusion Wrap-up:** A final section that always begins with "In conclusion," "To wrap it up," or "Ultimately," followed by an overly dramatic, pseudo-philosophical summary of a highly mundane topic.
