# 🌷 Moodscape

A personal mood journal built with HTML, CSS, and JavaScript. Capture daily feelings, save meaningful moments, and explore your entries in a clean purple interface.

## Features

- 😊 Five moods: Great, Good, Okay, Low, and Stressed
- 📝 Journal entries with a date, title, and note
- 💾 Automatic browser saving when storage is available
- 🔍 Search entries by title or text
- 🎛️ Filter entries by mood
- 📊 Statistics for total entries, days recorded, and most recorded mood
- 🌙 Light and dark themes
- 📤 Export entries as a JSON backup
- 📥 Import backups without duplicating matching entry IDs
- 🗑️ Delete entries with confirmation
- 📱 Responsive layout

## Technologies

- HTML5
- CSS3
- Vanilla JavaScript
- Browser Local Storage

## Getting Started

1. Download or clone the repository:

   ```bash
   git clone https://github.com/YOUR_USERNAME/moodscape.git
   cd moodscape
   ```

2. Open `index.html` in your browser.

No dependencies, API keys, or build tools are required.

## Project Structure

```text
moodscape/
├── index.html
└── README.md
```

## How to Use

### Add an Entry

1. Select your mood.
2. Choose a date.
3. Enter a title and note.
4. Click **Save this moment**.

Titles support up to **70 characters** and notes up to **2,000 characters**.

### Browse Your Journal

- Search by words in an entry’s title or note.
- Select a mood to filter results.
- Entries appear by date, newest first.
- Click **Delete** to remove an entry after confirmation.

### Back Up and Restore

Click **Export** to download a JSON backup.

Click **Import** to restore a Moodscape backup. Importing merges entries with the current journal and skips matching entry IDs.

Imports support files up to **5 MB** and **10,000 entries per backup**.

### Change the Theme

Click **Dark mode** or **Light mode**. The preference is saved when browser storage is available.

## Privacy and Storage

Entries are stored locally in your browser. The app does not upload them to a server.

- Entries do not automatically sync across browsers or devices.
- Clearing browser data may remove saved entries.
- Local Storage is not encrypted by this app.
- Export backups regularly to keep a separate copy.
- If browser saving is unavailable, entries remain only in the current tab.

## Statistics

| Statistic | Meaning |
|---|---|
| Total entries | Number of saved journal entries |
| Days recorded | Number of distinct entry dates |
| Most recorded mood | Mood selected most often; ties display multiple moods |

These statistics describe your entries and do not provide a health assessment.

## Customization

Edit the CSS variables in `index.html`:

```css
:root {
  --bg: #f7f5fb;
  --panel: #ffffff;
  --text: #302945;
  --accent: #7860dc;
  --soft: #f0ebff;
}
```

Edit the `body.dark` variables to customize dark mode.

## Limitations

- Entries cannot currently be edited after saving.
- Unsaved form drafts are not restored after refreshing.
- Storage capacity depends on the browser.
- The app is a personal journal, not a medical or diagnostic tool.

## Future Ideas

- Edit existing entries
- Calendar view
- Mood trend charts
- Journal prompts
- Optional reminders
