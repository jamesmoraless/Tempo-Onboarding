# Agent+ Developer Onboarding Task

## The Brief

A client wants a simple appointment booking tool. A provider sets their availability, and other people can book time with them.

Here's what the client said:

> "We need a way for our team members to share their availability and let external people book meetings with them. It should feel clean and professional. People booking shouldn't need to create an account — just pick a time and confirm. The team member should be able to see what's booked and manage their schedule."

There are no designs. There is no feature list. You need to figure out what to build, how to structure it, and what the UX should look like.

### Expected Core Flows

Your interpretation should cover these areas (how you implement them is up to you):

- **Authentication** — Providers can sign up and log in
- **Availability management** — A provider can set when they're available
- **Public booking page** — Someone without an account can view a provider's availability and book a time slot
- **Booking confirmation & management** — Both sides should know what's booked
- **Provider dashboard** — A logged-in provider sees their upcoming bookings and can manage their availability

Edge cases (double bookings, past dates, empty states, time zones) are your responsibility to think through.

---

## Tech Stack (Non-Negotiable)

You **must** use all of the following:

| Technology | Purpose |
|---|---|
| [Vite](https://vitejs.dev/) | Build tool |
| [React](https://react.dev/) | UI framework |
| [React Router](https://reactrouter.com/) | Routing |
| [TailwindCSS](https://tailwindcss.com/) | Styling |
| [ShadCN/ui](https://ui.shadcn.com/) | Component library |
| [Supabase](https://supabase.com/) | Auth, database, edge functions |
| [TypeScript](https://www.typescriptlang.org/) | Language |
| [Playwright](https://playwright.dev/) | e2e testing |
| [Claude Code](https://docs.anthropic.com/en/docs/claude-code) | Primary development tool |
| [Vercel](https://vercel.com/) | Deployment |

Additional libraries (Zustand, date-fns, etc.) are fine as long as they don't replace anything above.

---

## AI-First Development

Claude Code is your primary development tool. This is not optional.

### Day 1 Setup
1. Install Claude Code CLI
2. Configure MCP servers: **GitHub** + **Supabase** at minimum
3. Review the [Claude Code PR check guide](https://docs.google.com/document/d/1xDPhvIWytfQgdde5eNtbamIrw3ngMkELygkA_vfva4A/edit?usp=sharing)

### Every PR Must Include an "AI Usage" Section

```
## AI Usage
- **Used Claude Code for:** [what you used it for]
- **Wrote/modified manually:** [what you did yourself and why]
- **Rejected AI output:** [anything you didn't use and why]
```

Run `claude` for PR review locally before every submission.

---

## PR Standards

- **Size:** 200–800 LoC ideal, 1,500 LoC max
- **Description:** What it addresses, how to test it, dependencies
- **Media:** Screenshots and/or Loom video of the feature
- **Deployment:** Vercel preview link
- **Tests:** Playwright e2e tests for the feature
- **Commits:** Clean, descriptive messages

---

## Timeline

| Phase | Duration | Focus |
|---|---|---|
| **Week 1** | Days 1–5 | Setup, architecture, core feature build |
| **Week 2** | Days 6–10 | Remaining features, full e2e tests, polish, graduation |
| **Buffer** | Week 3 | Only if needed — EM sets specific targets |

### Day 1 Deliverables (Post in Slack)

1. Claude Code setup confirmation (screenshot)
2. Daily plan for Week 1
3. **Your interpretation of the brief** — What are you building? What product decisions did you make and why?
4. Architecture decisions + high-level system design diagram
5. Clarifying questions or scope notes
6. Link to this repo (forked)

### Weekly Checkpoints

Every Friday: 15-minute call with Engineering Manager. You demo what you shipped, review your scorecard, and set targets for the next week.

---

## Scorecard

You are scored each Friday on a 1–5 scale:

| Category | Weight | What We Measure |
|---|---|---|
| Feature Delivery | 25% | Planned vs. delivered. Quality, not just completion. |
| AI Tool Mastery | 20% | Claude Code usage quality. Critical review of AI output. |
| Code Quality & Testing | 20% | e2e coverage, PR standards, clean code, patterns. |
| Communication | 20% | Standup quality, blocker flagging, Slack clarity. |
| Problem Solving | 15% | Self-sufficiency, initiative, right questions at right time. |

**Graduation:** 3.5+ average, no category below 3.0 in final week.

Full grading criteria: [Developer Onboarding Grading Sheet](https://docs.google.com/document/d/1gw_WiY2pkc3_8yBcKuj9xj7T45kSdFye/edit?usp=sharing&ouid=105346785631447609152&rtpof=true&sd=true)

---

## Full Onboarding Documentation

For complete details on daily requirements, communication guidelines, delivery expectations, and what happens after graduation, see the [Developer Onboarding Page](https://www.notion.so/287994f4c04680dc9fd4ca0bade8d519) on Notion.
