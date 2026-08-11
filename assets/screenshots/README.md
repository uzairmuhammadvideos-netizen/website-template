# Screenshots needed

Drop image files into this folder using the exact names below. Each page's `<img>` tag
already points at these paths with an `onerror` fallback, so nothing else needs to change —
the placeholder mockup disappears the moment the real file is present.

Every tour section (`#tour` on the home page) now has clickable tags above its mockup —
each tag swaps in a different screenshot via `data-shot` on the button. The first tag in
each row is the section's original/default image (already listed below); the rest are new.

| Filename | Used on | Tag | Aspect ratio | Capture |
|---|---|---|---|---|
| `teacher-review-grading.png` | Home — For Teachers | Dashboard (default) | Wide chip (~16:7) | Home dashboard with a pending review alert (e.g. `newteacher@test.com` demo account) |
| `teacher-review-grading-1.png` | Home — For Teachers | Review Queue | Wide chip (~16:7) | `review-queue.tsx`, PENDING REVIEW list with flagged FRQ answers |
| `teacher-review-grading-2.png` | Home — For Teachers | FRQ Review | Wide chip (~16:7) | `frq-review/[submissionId].tsx`, mid-review of a flagged answer |
| `analytics-new.png` | Home — For Admin | — | Browser (matches image, ~1.4:1) | `(admin)/analytics.tsx`, school-wide grade distribution + heat map |
| `scan-capture-queue.png` | Home hero, Tour §1 Scan & Grade | Vision grading (default) | Phone (9:18.5) | `scan.tsx` mid-capture or the live grading queue, a few confidence badges visible |
| `scan-confidence-scoring.png` | Tour §1 Scan & Grade | Confidence scoring | Phone (9:18.5) | Graded question with a confidence badge highlighted |
| `tutor-practice-builder.png` | Home — For Tutors | — | Wide chip (~16:7) | `textbook/generate.tsx` (practice set) or `gradebook/[classId].tsx` (progress) |
| `student-results-feedback.png` | Home — For Students | — | Wide chip (~16:7) | `result-detail/[resultId].tsx` with visible AI feedback text |
| `digitize-upload-extract.png` | Tour §2 Digitize | Document AI (default) | Browser (16:10.5) | `upload.tsx`, extracted questions pre-save |
| `digitize-auto-rubric.png` | Tour §2 Digitize | Auto-rubric writing | Browser (16:10.5) | Auto-generated rubric for an essay question |
| `build-assessment-generated.png` | Tour §3 Build | Textbook-aware generation (default) | Phone (9:18.5) | `textbook/generate.tsx`, generated questions ready to assign |
| `build-abc-variants.png` | Tour §3 Build | A/B/C variants | Phone (9:18.5) | Shuffled A/B/C variant list |
| `build-iep-variants.png` | Tour §3 Build | IEP variants | Phone (9:18.5) | Simplified IEP reading-level variant |
| `lesson-plan-calendar.png` | Tour §4 Lessons | AI chat editing (default) | Phone (9:18.5) | `lesson-plans.tsx` or `lesson-plan/[id].tsx` |
| `lesson-plan-eek.png` | Tour §4 Lessons | Standards-aligned | Phone (9:18.5) | `lesson-plan/[id].tsx`, learning objectives + materials with AI Adjust chips |
| `lesson-plan-chat.png` | Tour §4 Lessons | Chat | Phone (9:18.5) | `lesson-plan/[id].tsx`, "Talk to InnedAI" chat sheet open |
| `flashcards-study-session.png` | Tour §5 Flashcards | Student-facing (default) | Phone (9:18.5) | `study/[assignmentId].tsx`, mid-flip |
| `flashcards-spaced-practice.png` | Tour §5 Flashcards | Spaced practice | Phone (9:18.5) | Spaced-practice review loop / scheduling view |
| `reach-translated-iep.png` | Tour §6 Reach | Reading-level rewrite (default) | Phone (9:18.5) | Simplified IEP reading-level variant, side-by-side with original |
| `reach-multi-language.png` | Tour §6 Reach | Multi-language | Phone (9:18.5) | Fully translated assessment for an ELL student |
| `analytics-heatmap.png` | Tour §7 Analytics | Item analysis (default) | Browser (16:10.5) | `analytics/[assignmentId].tsx`, per-question difficulty breakdown |
| `analytics-heatmaps-detail.png` | Tour §7 Analytics | Heatmaps | Browser (16:10.5) | Student-by-question heatmap view |
| `classroom-sync.png` | Tour §8 Classroom | Two-way sync (default) | Phone (9:18.5) | `classroom.tsx`, courses/roster with sync status |
| `classroom-roster-import.png` | Tour §8 Classroom | Roster import | Phone (9:18.5) | Roster import flow from Google Classroom |
| `admin-dashboard.png` | Tour §9 Admin | School-wide rollups (default) | Browser (16:10.5) | `(admin)/analytics.tsx`, school-wide performance rollups |
| `admin-console-directory.png` | Tour §9 Admin | Admin console | Browser (16:10.5) | `(admin)/teachers.tsx` or `(admin)/classes.tsx`, searchable directory |

Phone screenshots: capture full-screen from the simulator/device, no cropping needed.
Browser screenshots: crop out browser chrome — the mockup already draws its own window frame.
Wide chip images: crop tight on the most legible part of the screen (a card, a stat row).

Always capture with real, populated data — empty states undercut the pitch.

Note: the "For Admin" card on the home page (the platform-grid overview, not the tour) still
uses a live HTML/CSS/SVG recreation of the admin dashboard, not a screenshot — leave that one
alone. Only Tour §9 (inside the expandable "Full Product Tour") now takes photos, so its tags
can swap between two different admin views like every other tour section.
