LISS — LIGHT INTERNATIONAL SCHOOL SYSTEM
Offline-first local prototype for schools in Liberia

START HERE
1. Extract this ZIP into a new folder; keep older copies as backups.
2. Open the folder in VS Code.
3. For PWA/offline testing, run index.html using VS Code Live Server (localhost). Opening directly as file:// will limit service-worker/PWA behavior.
4. Choose Administrator, Teacher, Student, or Parent/Guardian on the welcome screen.
5. Add sample students and teachers in the Administrator workspace before testing other portals.

FEATURES INCLUDED IN THIS PROTOTYPE
- Welcome screen with four role portal entry points.
- Local administrator workspace for student/teacher records, classes, subjects, attendance, notifications, school settings, backups and reports.
- Student and teacher records support male/female avatar defaults, date of birth, and optional profile photo.
- Teacher profile can be assigned multiple classes and multiple subjects.
- Teacher portal shows assigned classes/subjects, supports local mark entry for assigned students/subjects, and creates assignments, homework and quizzes.
- Student portal shows virtual ID card, allows a local photo update, lists assignments/quizzes and can save quiz responses locally.
- Parent/guardian portal calculates semester/yearly performance summaries and attendance analytics for children with matching guardian names.
- Birthday greetings for records whose date of birth matches the current local calendar day.
- Semester 1: First, Second, Third Period + Exam; Semester 2: Fourth, Fifth, Sixth Period + Exam.
- Semester average = (three period marks + exam mark) / 4. Yearly average = (Semester 1 average + Semester 2 average) / 2 when both are complete.
- Marks below 75 are highlighted red. Administrator can lock/reopen grade entry by academic year and semester.
- Report-card preview/printing, student ID preview/printing, JSON export/import, responsive layout and service-worker cache.

IMPORTANT LIMITATIONS — PLEASE READ BEFORE REAL SCHOOL USE
This is still a local front-end prototype, not a production school management system. Portal selection is NOT secure authentication; the PIN fields are not a secure credential system and must not be used for real passwords. Roles do not have server-enforced access control. All records live in the same browser profile on one device; other users/devices will not receive changes or messages. A person using the same browser may access local records. Do not enter sensitive or real student data until secure backend authentication, role-based authorization, encrypted transport, protected storage, proper parent-child account linking, audit logging, backups, and privacy/security review are implemented.

The QR-like image on ID cards is a decorative placeholder and is NOT scannable. Quiz responses and assignments are local only. Notifications are saved locally and are not pushed to other devices. Birthday greetings depend on dates of birth being entered. Report card calculations follow the formula above; each school should confirm its official grading rules before using printed reports. Attendance analytics are only as complete as the local attendance records.

BACKUP SAFETY
Use Export JSON Backup regularly and store copies somewhere safe. Clearing browser data may erase local records. Importing a backup replaces the current local records. Keep the original ZIP untouched.
