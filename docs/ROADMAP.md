# Intentional Living App: Roadmap Checklist

Each box is one session of about 1 to 2 hours, and each one becomes a GitHub issue. Every session follows the same shape: recap, then goal and why, then building it together, then a wrap-up on where it fits in the architecture.

Rough size: about 40 sessions. At one per week, that's under a year to a version you can test with family and friends.

## Phase 0: Foundations (3 sessions)
- [ ] 0.1 Architecture map: how the UI, app logic, local database, cloud backend and APIs talk to each other, drawn around the daily plan
- [ ] 0.2 GitHub basics: repo structure, README, issues, labels, milestones, and your first commit
- [ ] 0.3 Turn this checklist into GitHub issues and a project board

## Phase 1: Research (8 sessions)
- [ ] 1.1 Research plan: goals, questions, who to recruit (5 organizers, 5 aspiring organizers)
- [ ] 1.2 Interview guide and consent script, plus a practice run on yourself
- [ ] 1.3 Psychology review, part 1: uncertainty and stress, expressive writing, the planning fallacy
- [ ] 1.4 Psychology review, part 2: habit formation, identity-based habits, motivation and rewards
- [ ] 1.5 Competitor teardown: what Todoist, Structured, Habitica and Day One get right and wrong
- [ ] 1.6 Run interviews (spread across a few weeks, with notes tagged as you go)
- [ ] 1.7 Affinity mapping: barriers, struggles, wants and needs
- [ ] 1.8 Findings summary: organizers vs aspiring organizers, 2 personas, 1 journey map

## Phase 2: Requirements (4 sessions)
- [ ] 2.1 Functional requirements: what the app must do
- [ ] 2.2 Non-functional requirements: speed, privacy, offline use, accessibility
- [ ] 2.3 Prioritize the first version (MoSCoW) and write down what's out of scope
- [ ] 2.4 Data model: tasks, events, habits, journal entries, and how they relate

## Phase 3: Design (8 sessions)
- [ ] 3.1 Figma basics, learned by building one simple screen
- [ ] 3.2 Information architecture: tabs, navigation, and user flows
- [ ] 3.3 Wireframes: dashboard and daily plan
- [ ] 3.4 Wireframes: calendar, fuzzy due dates, quick-add
- [ ] 3.5 Wireframes: habits, journal, and promise capture
- [ ] 3.6 Wireframes: morning brief, Sunday week report, energy check-in
- [ ] 3.7 Clickable prototype
- [ ] 3.8 Usability test with 3 interviewees, then revise

## Phase 4: Build setup (4 sessions)
- [ ] 4.1 Tech decisions: Expo, local database, whether a backend is needed yet (with the architecture map updated)
- [ ] 4.2 Project setup: Expo, TypeScript, linting, folder structure, first app running on your phone
- [ ] 4.3 Backlog: requirements turned into user stories with acceptance criteria
- [ ] 4.4 Sprint planning: how sprints work at your pace, and planning sprint 1

## Phase 5: Build the core (about 12 sessions, as sprints)
- [ ] 5.1 Data layer: saving and loading tasks, events and habits
- [ ] 5.2 Quick-add with fuzzy due dates (today, tomorrow, this week, next 2 weeks, this month)
- [ ] 5.3 Daily plan screen: chronological checklist
- [ ] 5.4 Calendar views: month, week, day
- [ ] 5.5 Habits tab: weekly targets, consistency score, character traits
- [ ] 5.6 Scheduling engine, part 1: fit flexible items into free time by priority
- [ ] 5.7 Scheduling engine, part 2: the reserve, rollovers, overbooking warnings
- [ ] 5.8 Energy check-in that changes which tasks are proposed
- [ ] 5.9 Journal with guided prompts, and turning entries into tasks
- [ ] 5.10 One-tap promise capture plus the evening reflection reminder
- [ ] 5.11 Morning brief and Sunday week report
- [ ] 5.12 Notifications

## Phase 6: Friends and family test (3 sessions)
- [ ] 6.1 Build and share a test version (TestFlight and Android internal testing)
- [ ] 6.2 Collect feedback and log it as issues
- [ ] 6.3 Retrospective: what you learned, and what comes next

## Later (after the first version)
- Screen-time rewards and blocking chosen apps, like screen-time apps do (needs a feasibility check: iOS Screen Time API entitlement, Android usage access)
- Shared habits in groups of 2 to 5 people
- Community tab for households and group projects
- App store launch
