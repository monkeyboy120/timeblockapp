# timeblockapp

# ⏰ TimeBlocks

**TimeBlocks** is a cross-platform time-blocking app that combines a clean, customizable UI with native Apple Calendar integration. Built with **SvelteKit** and powered by **Capacitor**, it works on iOS, macOS, and the web. A custom Capacitor plugin in Swift connects to Apple Calendar (via EventKit), and Supabase handles real-time sync and user authentication.

---

## ✨ Features

- 📆 Pull in events from **Apple Calendar**
- 🧱 Create custom time blocks via a clean drag-and-drop interface
- 🔄 **Sync** your schedule across all devices using **Supabase**
- 🧑‍💻 Built with **SvelteKit** and styled with **TailwindCSS**
- 📱 Works as a **native app** on iOS/macOS and as a **web app**
- 🔒 Login with **Sign in with Apple**

---

## 📦 Tech Stack

| Layer       | Technology                           |
|-------------|---------------------------------------|
| Frontend    | [SvelteKit](https://kit.svelte.dev/), [TailwindCSS](https://tailwindcss.com/) |
| Native Bridge | [Capacitor](https://capacitorjs.com/), Swift (EventKit) |
| Backend     | [Supabase](https://supabase.com/) (PostgreSQL, Auth, Storage) |
| Auth        | Sign in with Apple (via Supabase) |
| Sync & DB   | Supabase Realtime / Supabase DB |
| Calendar API | Apple EventKit (via Capacitor plugin) |

---

## 🛠️ Project Structure

```plaintext
timeblocks/
├── src/                    # SvelteKit app
│   ├── routes/             # Routes for calendar, auth, etc.
│   ├── lib/                # API and calendar logic
│   └── components/         # Reusable UI components
├── native/                 # Native iOS plugin for Apple Calendar
│   └── CalendarPlugin.swift
├── public/                 # Static assets and app manifest
├── supabase/               # SQL schema, edge functions, etc.
├── capacitor.config.ts     # Capacitor app config
└── README.md
