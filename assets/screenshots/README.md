# Screenshots needed

Drop image files into this folder using the exact names below. Each page's `<img>` tag
already points at these paths with an `onerror` fallback, so nothing else needs to change —
the placeholder mockup disappears the moment the real file is present.

| Filename | Used on | Aspect ratio | Capture |
|---|---|---|---|
| `scan-capture-queue.png` | Home hero, Product §1 | Phone (9:18.5) | `scan.tsx` mid-capture or the live grading queue, a few confidence badges visible |
| `teacher-review-grading.png` | Home — For Teachers | Wide chip (~16:7) | `review-queue.tsx` / `review/[scanId].tsx`, a few flagged answers showing |
| `tutor-practice-builder.png` | Home — For Tutors | Wide chip (~16:7) | `textbook/generate.tsx` (practice set) or `gradebook/[classId].tsx` (progress) |
| `student-results-feedback.png` | Home — For Students | Wide chip (~16:7) | `result-detail/[resultId].tsx` with visible AI feedback text |
| `digitize-upload-extract.png` | Product §2 | Browser (16:10.5) | `upload.tsx`, extracted questions pre-save |
| `build-assessment-generated.png` | Product §3 | Phone (9:18.5) | `textbook/generate.tsx`, generated questions ready to assign |
| `lesson-plan-calendar.png` | Product §4 | Phone (9:18.5) | `lesson-plans.tsx` or `lesson-plan/[id].tsx` |
| `flashcards-study-session.png` | Product §5 | Phone (9:18.5) | `study/[assignmentId].tsx`, mid-flip |
| `reach-translated-iep.png` | Product §6 | Phone (9:18.5) | Translated assessment or IEP reading-level variant |
| `analytics-heatmap.png` | Product §7 | Browser (16:10.5) | `analytics/[assignmentId].tsx`, grade distribution + heatmap |
| `classroom-sync.png` | Product §8 | Phone (9:18.5) | `classroom.tsx`, courses/roster with sync status |

Phone screenshots: capture full-screen from the simulator/device, no cropping needed.
Browser screenshots: crop out browser chrome — the mockup already draws its own window frame.
Wide chip images: crop tight on the most legible part of the screen (a card, a stat row).

Always capture with real, populated data — empty states undercut the pitch.

Note: the "For Admin" card (home) and "For Districts" §9 (product) are no longer photo
placeholders — they're a live HTML/CSS/SVG recreation of the actual admin dashboard
(same numbers as the real `(admin)/index.tsx` screen: 6 teachers, 214 students, 76% avg,
grade-distribution donut). No screenshot needed there.
