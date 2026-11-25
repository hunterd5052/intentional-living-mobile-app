# Intentional Living App: Roadmap Checklist

Each box is one session and one GitHub issue. Sessions are kept small on purpose, so each one teaches **one** idea and leaves time to reflect.

## How a session works

A session is about 1 to 2 hours:

1. **Recap** (5 min): what happened last time and where it sits on this roadmap.
2. **Goal and forecast** (10 min): what we are doing, why, and what "done" looks like.
3. **Build together** (45 to 75 min): the work itself.
4. **Reflect** (15 min): open the pull request and fill in the template, which GitHub adds to every new PR automatically ([.github/pull_request_template.md](../.github/pull_request_template.md)). It asks:
   - What does this do, and why?
   - Where does it sit in the architecture map?
   - What did I learn, what was harder than expected, and what is still confusing?
   - What guesses did I make that should be checked later?

   The issue says what needs doing and why. The pull request is where you reflect, because it sits next to the exact changes you made.

If a session finishes early, stop and reflect anyway. Starting the next box is optional, not expected.

Rough size: about 100 sessions to a public launch, and about 85 until testers have the app in hand (6.3). At one session a week, that is around a year and a half to the test. That is fine: the goal is learning, not speed. Sessions marked *(can merge)* are good candidates to combine on a long day.

Milestones are marked with ★. They are the moments to stop and celebrate.

---

## Phase 0: Foundations (7 sessions)

The goal of this phase is to understand how an app is put together, and to see it working, before the long non-coding phases.

- [ ] 0.1 Architecture map, part 1: the layers (screens, app logic, local database, cloud backend, outside APIs like the phone's calendar) and what each one is responsible for
- [ ] 0.2 Architecture map, part 2: trace three journeys through the map: quick-adding a task, importing a calendar event, and backing up to the cloud
- [ ] 0.3 GitHub basics: issues, labels, milestones, branches, and pull requests, practised on a small real doc change
- [ ] 0.4 Turn this roadmap into GitHub issues and a project board
- [ ] 0.5 Architecture spike, part 1: a blank Expo app running on your phone, and what each generated file does
- [ ] 0.6 Architecture spike, part 2: one screen to add and list tasks, with screens, logic, and data in separate folders so the map is visible in the code
- [ ] 0.7 Architecture spike, part 3: save tasks on the phone so they survive a restart, write your first unit test, and update the architecture map with what surprised you

> The spike is a **throwaway** learning app. It lives in its own folder (`spike/`) and is not the real app. It exists so the architecture map stops being abstract, and so there is something to code during research and design.

★ **Milestone: you have an app on your phone that you built and understand end to end.**

## Phase 1: Research (15 sessions)

- [ ] 1.1 Research plan: goals and the questions research must answer
- [ ] 1.2 Recruiting: a short screener and who to ask (5 organizers, 5 aspiring organizers)
- [ ] 1.3 Interview guide and consent script
- [ ] 1.4 Practice interview on yourself, then revise the guide
- [ ] 1.5 Psychology, part 1: uncertainty, stress, and expressive writing
- [ ] 1.6 Psychology, part 2: the planning fallacy and how people estimate time (feeds the task duration estimate)
- [ ] 1.7 Psychology, part 3: habit formation and identity-based habits
- [ ] 1.8 Psychology, part 4: motivation, rewards, and why streaks can backfire
- [ ] 1.9 Competitor teardown, part 1: planners and auto-schedulers (for example Todoist, Structured, and apps that fit tasks into calendar gaps)
- [ ] 1.10 Competitor teardown, part 2: habit and journal apps (for example Habitica, Day One), plus how free, donation-funded apps sustain themselves
- [ ] 1.11 Run interviews 1 to 5 (spread across a few weeks, with notes tagged as you go)
- [ ] 1.12 Run interviews 6 to 10
- [ ] 1.13 Affinity mapping: barriers, struggles, wants, and needs
- [ ] 1.14 Findings summary: organizers vs aspiring organizers, 2 personas, 1 journey map
- [ ] 1.15 Revise the docs from the findings: update the problem statement, values, and this roadmap, and note in each what changed and why

★ **Milestone: the plan is backed by real people, not just your own routine.**

## Phase 2: Requirements (8 sessions)

- [ ] 2.1 Functional requirements, part 1: daily plan, tasks, fuzzy due dates, duration estimates, and the reserve (including the check-in after 3 rollovers)
- [ ] 2.2 Functional requirements, part 2: calendar import and export, the prompts that fill in required fields for imported events, habits, journal, promise capture, morning brief, and Sunday report
- [ ] 2.3 Non-functional requirements: speed, offline use, accessibility
- [ ] 2.4 Privacy and security requirements: sign-in, encrypted backup, and exactly what data ever leaves the device
- [ ] 2.5 Prioritize the first version (MoSCoW) and define the **smallest useful core** you could use yourself every day
- [ ] 2.6 Data model, part 1: tasks, events, habits, journal entries, and how they relate
- [ ] 2.7 Data model, part 2: scheduling inputs (duration estimate, usual awake hours, busy vs flexible events, rollover count) and the fields sync needs (IDs, last-updated time, deleted flag)
- [ ] 2.8 Success measures: write the before-and-after survey (stress, sense of control, having a plan) and decide what else to track during testing

## Phase 3: Design (16 sessions)

- [ ] 3.1 Figma basics, part 1: frames, text, shapes, and auto layout, learned by building one simple screen
- [ ] 3.2 Figma basics, part 2: components, colors, and type styles (a tiny design system)
- [ ] 3.3 Prototype review: screenshot the old prototype's calendar and decide what to keep in the new layout
- [ ] 3.4 Information architecture: tabs and navigation
- [ ] 3.5 User flows: quick-add, importing a calendar event, and the rollover check-in
- [ ] 3.6 Wireframes: dashboard and daily plan
- [ ] 3.7 Wireframes: calendar month, week, and day views (building on the prototype's layout)
- [ ] 3.8 Wireframes: quick-add with fuzzy due dates and duration estimate
- [ ] 3.9 Wireframes: calendar import and the prompts for missing fields
- [ ] 3.10 Wireframes: habits, weekly targets, and character traits
- [ ] 3.11 Wireframes: journal and promise capture
- [ ] 3.12 Wireframes: morning brief, Sunday week report, energy check-in, rollover check-in
- [ ] 3.13 Wireframes: sign-in, backup, and settings (usual awake hours)
- [ ] 3.14 Clickable prototype
- [ ] 3.15 Usability test with 3 interviewees
- [ ] 3.16 Revise the designs from the test

★ **Milestone: a clickable app people have tried, before a line of real code.**

## Phase 4: Build setup (8 sessions)

- [ ] 4.1 Tech decision: the local database on the phone
- [ ] 4.2 Tech decision: backend, sign-in, and encrypted backup and sync (options, trade-offs, and yearly cost)
- [ ] 4.3 Update the architecture map with the decisions from 4.1 and 4.2
- [ ] 4.4 Project setup: Expo, strict TypeScript, linting, folder structure, running on your phone
- [ ] 4.5 Testing setup: install Jest, write a first real test, and learn what is worth testing and what is not
- [ ] 4.6 Continuous integration: a GitHub Action that runs linting, type checks, and tests on every pull request
- [ ] 4.7 Backlog: requirements turned into user stories, with acceptance criteria written so they can become tests
- [ ] 4.8 Sprint planning: how sprints work at your pace, and planning sprint 1

### How testing is learned

Testing is added in layers, so each kind is learned when it is most useful:

1. **Unit tests for pure logic** (first test in 0.7, set up properly in 4.5). Pure functions such as "find the free gaps in a day" take inputs and return outputs, so they are the easiest place to learn.
2. **Test-first for the scheduling engine** (5.11 to 5.15). Write the test from the acceptance criteria, watch it fail, then make it pass. The engine is the heart of the app, so this is where tests protect you most.
3. **Data layer tests** (5.1, 5.2). Check that saving and loading gives back what went in.
4. **One or two screen tests** (5.4) with React Native Testing Library, to learn how to test what the user sees.
5. **A manual test checklist** (5.31) for things that only work on a real phone, like calendar access and notifications.
6. **Continuous integration** (4.6) runs everything on every pull request, so tests become a habit instead of a chore.

## Phase 5: Build the core (31 sessions, as sprints)

**Data**
- [ ] 5.1 Data layer, part 1: saving and loading tasks, with tests
- [ ] 5.2 Data layer, part 2: events, habits, and journal entries, with tests

**Capture and the daily plan**
- [ ] 5.3 Quick-add with fuzzy due dates (today, tomorrow, this week, next 2 weeks, this month) and a rough duration estimate
- [ ] 5.4 Daily plan screen: chronological checklist, with your first screen test
- [ ] 5.5 Checking off, editing, and moving items

**Calendar**
- [ ] 5.6 Calendar views, part 1: month view, based on the prototype's layout
- [ ] 5.7 Calendar views, part 2: week and day views
- [ ] 5.8 Phone calendar, part 1: asking permission and importing events
- [ ] 5.9 Phone calendar, part 2: prompts that fill in required fields for imported events
- [ ] 5.10 Phone calendar, part 3: adding tasks and events made in the app to the phone's calendar

**Scheduling engine (test-first)**
- [ ] 5.11 Scheduling, part 1: find the free gaps between events, within the user's usual awake hours
- [ ] 5.12 Scheduling, part 2: fit tasks into the gaps by due date, priority, and duration
- [ ] 5.13 Scheduling, part 3: explain why each item was placed where it is
- [ ] 5.14 The reserve: rollovers, and the kind check-in after 3 rollovers (shrink it, schedule it, or let it go)
- [ ] 5.15 Overbooking warnings and suggestions for what to push back

★ **Milestone: start using the app yourself every day.** From here on, your own use is a constant source of bugs and ideas. Log them as issues.

**Habits**
- [ ] 5.16 Habits, part 1: weekly targets and the consistency score (test-first for the score)
- [ ] 5.17 Habits, part 2: character traits and identity statements

**Notifications** (before the features that need them)
- [ ] 5.18 Notifications, part 1: permissions and simple local reminders
- [ ] 5.19 Notifications, part 2: timing rules, quiet hours, and calm wording

**Energy, journal, and capture**
- [ ] 5.20 Energy check-in that changes which tasks are proposed
- [ ] 5.21 Journal, part 1: guided prompts
- [ ] 5.22 Journal, part 2: turning entries into tasks, habits, and events
- [ ] 5.23 One-tap promise capture plus the evening reflection reminder
- [ ] 5.24 Morning brief
- [ ] 5.25 Sunday week report

**Accounts and encrypted backup**
- [ ] 5.26 Sign-in
- [ ] 5.27 Encrypting data before it leaves the phone
- [ ] 5.28 Backing up to the cloud
- [ ] 5.29 Signing in on a second device and restoring
- [ ] 5.30 Sync conflicts: what happens when two devices change the same item

**Quality**
- [ ] 5.31 Manual test checklist for real-phone features, and a full pass through it

## Phase 6: Friends and family test (8 sessions)

- [ ] 6.1 EAS setup: build profiles and how builds work
- [ ] 6.2 Internal distribution: getting the app onto testers' phones (check iOS requirements here, see note below)
- [ ] 6.3 Tester onboarding and the "before" survey
- [ ] 6.4 Mid-test check-in: collect feedback and log it as issues
- [ ] 6.5 The "after" survey and comparing results to the success measures from 2.8
- [ ] 6.6 Bug-fix sprint, part 1
- [ ] 6.7 Bug-fix sprint, part 2
- [ ] 6.8 Retrospective: what you learned, and whether the app is ready to go public

> **iOS note:** EAS builds are free (within the free plan's monthly build limits), and Android testers can install them at no cost. Installing a build on **iPhones outside the simulator** generally requires an Apple Developer Program membership ($99 a year). Confirm this in 6.2. If it holds, either start with Android testers or pay for the membership at this point, since launch will need it anyway.

★ **Milestone: real people are using something you built.**

## Phase 7: Public launch (6 sessions)

- [ ] 7.1 Store requirements: Apple Developer Program, Google Play account, privacy policy, privacy labels, and data safety forms
- [ ] 7.2 Transparent funding, part 1: check what Apple and Google allow for in-app donations or tips (see [FUNDING.md](FUNDING.md))
- [ ] 7.3 Transparent funding, part 2: the funding page with the yearly goal, progress bar, and cost breakdown
- [ ] 7.4 Store listings: screenshots and descriptions
- [ ] 7.5 Submit to the App Store and Google Play, and handle review feedback
- [ ] 7.6 Launch retrospective and planning what comes next

★ **Milestone: the app is public, free, and ad-free.**

## Later (after launch)

- Screen-time rewards and blocking chosen apps, like screen-time apps do (needs a feasibility check: iOS Screen Time API entitlement, Android usage access)
- Shared habits in groups of 2 to 5 people
- Community tab for households and group projects
- End-to-end tests that drive the app automatically on a phone or simulator
