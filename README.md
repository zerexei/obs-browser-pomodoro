# OBS Pomodoro Timer

A lightweight Pomodoro-style productivity timer designed for OBS overlays and stream workflows.

## Features

* ⏱️ Circular countdown timer with animated progress ring
* 💼 90-minute work sessions
* ☕ Automatic short (15 min) and long (30 min) breaks
* 🔄 Repeating work/break cycle
* 🔊 Custom notification sounds for each mode
* ✅ Built-in task tracker
* 📊 Session statistics

  * Completed work sessions
  * Completed breaks
  * Finished tasks
* 💾 Auto-save using localStorage
* 🎨 Clean glassmorphism UI with transparent background
* 🧹 Hard reset button to clear all progress

## Cycle

The timer follows this sequence:

Work (90m)
→ Short Break (15m)
→ Work (90m)
→ Short Break (15m)
→ Work (90m)
→ Long Break (30m)

Then repeats.

## Controls

| Button | Action                |
| ------ | --------------------- |
| Start  | Start the timer       |
| Pause  | Pause the timer       |
| Reset  | Reset current session |
| ⟲      | Hard reset all data   |

## Tasks

* Add tasks using the input field.
* Press **Enter** or click **+** to create a task.
* Mark tasks complete with **✔**.
* Remove tasks with **🗑**.
* Completed tasks automatically move to the bottom.

## Persistence

All timer state, statistics, and tasks are stored in your browser's localStorage, allowing progress to persist between OBS sessions and page reloads.

## Notifications

Place audio files in:

```text
notifications/
├── stomps.mp3
├── clap.mp3
└── crowd-cheers.mp3
```

Used for:

* `stomps.mp3` → Work session start
* `clap.mp3` → Short break start
* `crowd-cheers.mp3` → Long break start

## Usage in OBS

1. Add a **Browser Source** in OBS.
2. Point it to the HTML file or local web server.
3. Set a transparent background.
4. Resize the source to fit your stream layout.

## License

Free to use and modify.
