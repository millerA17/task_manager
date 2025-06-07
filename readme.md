# Task Manager Web App

A simple, standalone project and task management tool built as a single HTML file. It runs entirely in your browser—no server or database required—and stores all data in `localStorage`. You can export and import your data as JSON to move between origins or share with others.

---

## Features

* **Projects & Tasks**: Create multiple projects and assign tasks to them.
* **Weekly Matrix View**: Organize tasks by day and category in a week grid.
* **Master View**: See all tasks across projects in one list.
* **Persistent Storage**: Data is saved automatically in browser `localStorage`.
* **Export / Import**: Backup your data as a JSON file (`Export Data`) and restore it (`Import Data`).
* **Auto-Load Default Data**: If you include a `backup.json` in the app root, it will automatically load on page load.

---

## Getting Started

### Running Locally

1. **Download or clone the repo**:

   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   cd <repo-name>
   ```
2. **Open `index.html`** in your browser (double-click or right-click → "Open with...").
3. **Use the app**. Your data lives under the `file://` origin and won’t mix with any online version.

---

## Hosting Online

You can host this static app for free. Choose one:

### GitHub Pages

1. Ensure your repo is **public**.
2. Rename your HTML to `index.html` (if not already) and push to `main`.
3. In **Settings → Pages**, set the source to `main` branch (root folder).
4. Visit `https://<your-username>.github.io/<repo-name>/`.

### Netlify Drop

1. Go to [Netlify Drop](https://app.netlify.com/drop).
2. Drag & drop the project folder or just `index.html`.
3. Netlify will provide a live URL immediately.

---

## Data Backup & Restore

* **Export Data**: Click the `Export Data` button to download a JSON backup of all projects, tasks, and matrix entries.
* **Import Data**: Click the `Import Data` button and select a previously exported JSON file to restore.
* **Auto-Load on Page Load**: If you place a `backup.json` file in the same directory as `index.html`, it will be fetched and imported automatically upon site load.

---

## Updating Default Data

To pre-seed the app with your own default projects and tasks:

1. Generate a backup JSON via **Export Data**.
2. Rename it to `backup.json` and place it alongside `index.html`.
3. Commit & push to your hosting repo. On next deploy, visitors will see those defaults.

---

## Forking & Sharing

Anyone can fork your GitHub repo and:

1. Enable GitHub Pages on their fork to get their own live link.
2. Or use Netlify Drop on their clone to spin up a separate URL.

They can also download the ZIP from GitHub, open locally, and use **Export/Import** to transfer their data.

---

## License

This project is open source—feel free to adapt and share!
