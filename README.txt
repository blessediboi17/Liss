LISS — LIGHT INTERNATIONAL SCHOOL SYSTEM (OFFLINE DEMO)

FILES
- index.html: app layout and screens
- styles.css: responsive design, SVG icon styling, animation and print layout
- app.js: local demo data, student/teacher forms, attendance, marks, report card, backup tools
- manifest.json: installable PWA metadata
- sw.js: offline app-shell caching

RUN IT
1. Open the LISS_Offline_School_System folder in VS Code.
2. Open index.html using the Live Server extension, or run a local HTTP server.
   PWA service workers generally require localhost or HTTPS; opening the file directly as file:// does not enable service-worker offline caching.
3. Start with Settings to confirm the school name, classes, subjects and grading labels.
4. Add a student and teacher; test attendance and report cards.
5. Use Export backup often.

IMPORTANT LIMITATIONS
- This is a front-end prototype for local testing, not a secure production school system.
- It has no real authentication or server-enforced admin permissions. The Admin dashboard is a navigation screen only.
- Records are stored in localStorage in the current browser profile. Browser storage may be cleared; export backups.
- Offline data is local to one browser/device. There is no cross-device synchronization yet.
- The report card formula is a demo average of available period/test/exam marks. Confirm and configure the school's approved grading policy before official use.
- Default avatars use emoji placeholders for speed. Replace with locally stored optimized 3D-style avatar images when ready.
- Google Fonts are optional and require internet; local fallback fonts are defined.


LATEST PROTOTYPE UPDATES
- Student ID card studio: preview and print stylized student cards with school name, learner name, class, student ID, avatar/photo, and a signature-style first name. The QR pattern is a placeholder only; verification and scanning are not active yet.
- Notification center: save local demo messages addressed to all teachers/students or an individual teacher/student. This does not deliver messages to other devices; secure real-time delivery requires backend accounts.
- PWA install control: appears when the browser signals that the app can be installed. Otherwise use the browser menu > Install app / Add to Home screen when available.
- Offline behavior requires serving the app through localhost or HTTPS for service-worker caching. Opening index.html directly does not activate PWA offline caching.
