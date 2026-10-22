# 🌷 Moodscape

A personal mood journal built with HTML, CSS, and vanilla JavaScript. Record your feelings, revisit meaningful moments, and explore your journal through calendar and chart views.

## Features

### Journaling

- Five moods: Great, Good, Okay, Low, and Stressed
- Entries with a date, title, and note
- Edit existing entries
- Delete entries with confirmation
- Mark meaningful entries as favorites
- Writing prompts for inspiration
- Automatic draft saving and recovery when browser storage is available

### Browsing

- Search entry titles and notes
- Filter by mood or favorites
- Sort by newest or oldest
- Calendar view with mood icons and entry counts
- Select a calendar date to view its entries

### Statistics

- Total entries
- Distinct days recorded
- Favorite entry count
- Most recorded mood, including ties
- Mood distribution chart across all entries

### Other Features

- Light and dark themes
- Responsive layout
- JSON backup export and import
- Compatibility with backups from the earlier Moodscape version

## Technologies

- HTML5
- CSS3
- Vanilla JavaScript
- Browser Local Storage

## Getting Started

1. Clone the repository:

   ```bash
   git clone https://github.com/YOUR_USERNAME/moodscape.git
   cd moodscape
   ```

2. Open `index.html` in your browser.

Replace `YOUR_USERNAME` with your GitHub username.

No dependencies, API keys, installation, or build commands are required.

## Project Structure

```text
moodscape/
├── index.html
└── README.md
```

## How to Use

### Create an Entry

1. Select a mood.
2. Choose a date.
3. Enter a title and note.
4. Click **Save moment**.

Titles support up to **70 characters**. Notes support up to **2,000 characters**.

### Edit an Entry

Click **Edit** on an entry, update the form, and select **Save changes**.

**Cancel edit** discards the current edit and preserves the saved entry.

### Use Writing Prompts

Click **New prompt** to change the suggestion.

Click **Add to note** to append the prompt to your current note.

### Recover a Draft

The current form is saved automatically when browser storage is available. Reopening the app in the same browser restores the draft.

Only one draft is stored at a time. Saving an entry clears its draft.

### Search and Filter

Use the search box, mood selector, and **Favorites only** checkbox to narrow the journal.

Choose **Newest first** or **Oldest first** to change the order.

### Explore the Calendar

Open **Calendar** and navigate between months.

Each recorded day displays mood icons and an entry count. Select a day to view its entries. Use **Clear date** to remove the date filter.

Selecting a calendar day resets the search, mood, and favorites filters.

### View the Mood Chart

Open **Mood chart** to see entry counts for each mood across the whole journal.

The chart describes recorded entries and does not provide a health assessment.

## Backups

### Export

Click **Export** to download a JSON file containing saved entries, including favorite status.

Unsaved drafts and theme preferences are not included.

### Import

Click **Import** and select a Moodscape JSON backup.

- New entry IDs are added.
- Existing matching IDs are preserved.
- Matching entries are not overwritten.
- Older Moodscape backups remain supported.
- Each import supports up to **5 MB** and **10,000 entries**.

## Privacy and Storage

The app stores entries, drafts, and theme preferences locally in your browser. It does not upload journal content to a server.

- Data does not automatically sync across devices or browsers.
- Clearing browser data may delete your journal and draft.
- The app does not encrypt Local Storage.
- Browser saving depends on available storage and permissions.
- Export important entries regularly.

If saving is unavailable, changes remain in the current tab and may be lost when it closes.

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

Edit `body.dark` to customize dark mode.

Update the `prompts` array in the JavaScript to change the writing suggestions.

## Limitations

- No account system or cloud synchronization
- One recoverable draft at a time
- Backup import preserves existing entries with matching IDs
- Statistics reflect journal entries rather than one mood per day
- Local storage capacity varies by browser
- This journal is not a medical or diagnostic tool

## Future Ideas

- Optional reminders
- Encrypted backups
- Custom mood labels
- Tags and categories
- Monthly journal summaries
