# Wisebase Flutter App

Flutter Android app for **Wisebase**, a multi-role workforce management platform (owner, HR, manager, employee). I built Wisebase at DataC and keep improving it.

**Product page:** https://conntinuity.datac.com/

## Screenshots

<img width="32%" alt="Owner home" src="https://raw.githubusercontent.com/mnashat18/WiseBase-app/b5eb275a5b9ea57cba296eb795b79ce064fbd9f3/.claude/owner_today.png" />
<img width="32%" alt="Readiness requests" src="https://raw.githubusercontent.com/mnashat18/WiseBase-app/b5eb275a5b9ea57cba296eb795b79ce064fbd9f3/.claude/owner_requests.png" />
<img width="32%" alt="Start a readiness check" src="https://raw.githubusercontent.com/mnashat18/WiseBase-app/b5eb275a5b9ea57cba296eb795b79ce064fbd9f3/.claude/employee_scan_start_final.png" />

## What the app does

- Login with email and Google sign-in
- Role-based screens for owner, HR, manager and employee
- Readiness requests and check history
- Guided check with camera and voice steps
- Alerts, notifications and push notifications (Firebase Cloud Messaging)
- Workforce, compliance and reports views for managers

## Tech stack

Flutter, Dart, Material Design, REST APIs, Firebase Cloud Messaging.

## How it fits together

The app calls the Wisebase REST APIs. The backend is Directus on PostgreSQL, and the Wisebase AI service analyses the scan data. The repo includes the Directus extensions the mobile app uses in `backend/`.

```text
Flutter app  ->  REST APIs  ->  Directus / PostgreSQL  ->  AI service
```

## Repository layout

| Path | Contents |
| --- | --- |
| `lib/` | App source (screens, services, state, widgets) |
| `test/` | Unit and widget tests |
| `android/` | Android project |
| `backend/` | Directus extensions used by the app |
| `docs/` | Project documentation |
| `assets/` | Branding assets |

The `*.md` reports in the root (audits, plans and acceptance notes) are internal review notes.

## Run locally

```bash
flutter pub get
flutter run
```

Build a release APK:

```bash
flutter build apk --release
```

## Related repositories

- [WiseBase-frontend](https://github.com/mnashat18/WiseBase-frontend): Angular web app
- [WiseBase-ai-server](https://github.com/mnashat18/WiseBase-ai-server) and [WiseBase_ai_v2](https://github.com/mnashat18/WiseBase_ai_v2): AI services

## Author

Mohamed Nashat Ghonim, Full-Stack Developer
[LinkedIn](https://www.linkedin.com/in/mohamed-nashat-ghonim/) · [GitHub](https://github.com/mnashat18) · mnashat2508@gmail.com
