# Account Security Lab

A classroom lesson for Mr. Makedon's class about protecting accounts, recognizing phishing, and getting help after a mistake.

- `index.html`: a clearly labeled message simulation with a decision activity, a warning-sign discussion, and an animated arrow pointing to the lesson link. The arrow animates for 4.8 seconds when it first enters view, then stays still; it respects reduced-motion preferences.
- `lesson.html`: account security guidance and a six-question quiz with explanations and a retry option. The quiz stays hidden and disabled for 10 minutes after the lesson first opens in a browser tab. A popup explains the wait, a countdown shows the remaining time, and the quiz unlocks automatically.

Suggested lesson: spend 5 minutes discussing the simulation, 10 minutes on the account security habits, and 5 minutes on the quiz and exit ticket. Students should use only the fictional examples here, never real passwords, recovery codes, or account details. Follow school guidance when setting up security features on school-managed accounts.

Both pages are self-contained static HTML with inline CSS and JavaScript. They use no external fonts, scripts, analytics, or cookies. Only the quiz unlock deadline is stored in this tab's session storage so refreshing the page or returning from the demo preserves the timer. If storage is blocked, the timer works until reload, which restarts it. A fresh tab session starts a fresh timer. Activity responses and quiz scores stay in page memory and disappear on reload; nothing is submitted or collected. Reading content and the warning-sign reveal work without JavaScript; the quiz stays locked without JavaScript.

The timer is a browser-based classroom pacing aid, not tamper-proof exam enforcement. It counts elapsed time, including time spent on the external classroom tools, and does not track active reading. Retrying an unlocked quiz does not restart the timer.

The existing `index.html` and `lesson.html` paths and link destinations are preserved for the classroom whitelist. GitHub Pages continues to publish from the root of `main`; no hosting or domain change is required.

Content references: CISA's Secure Our World guidance on strong passwords, MFA, and recognizing phishing; FIDO Alliance's passkey guidance. The lesson also includes optional external links to Have I Been Pwned and PasswordMonster for teacher-led exploration. They open in new tabs; use fictional passwords only and keep personal email addresses and breach results private. These external sites load only when their links are followed. The core lesson and quiz still work without visiting them.
