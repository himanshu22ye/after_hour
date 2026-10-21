# AFTER HOURS --- Midnight Journal

A personal, atmospheric journaling website for capturing late-night
thoughts, moods, photos, and the music connected to a moment.

## About the Project

**AFTER HOURS** is a small, browser-based journal designed to feel calm
and personal rather than like a productivity dashboard. It uses a dark
charcoal theme, warm amber accents, and elegant typography.

The first version is built as a single-page website using HTML, CSS, and
vanilla JavaScript. It can be opened directly in a browser without
installing a framework or running a backend server.

## Features Implemented

-   **Journal entries:** Add a title and write down your thoughts.
-   **Mood selector:** Choose a mood such as Calm, Happy, Nostalgic,
    Hopeful, Melancholic, Energized, Overwhelmed, or Unsure.
-   **Soundtrack details:** Record the song title and artist associated
    with a moment.
-   **Photo attachment:** Select one image for a moment, preview it, and
    resize it in the browser before saving.
-   **Memory archive:** Display saved entries, including their text,
    mood, soundtrack, and attached photo when present.
-   **Search:** Search entries by title, thoughts, mood, song, or
    artist.
-   **Edit and delete:** Update or remove saved entries.
-   **Writing prompts:** Show a reflective prompt and cycle through
    additional prompts.
-   **Word count and entry statistics:** See the number of saved moments
    and words written.
-   **Export:** Download journal entries as a JSON backup.
-   **Responsive styling:** Layout adapts for smaller screens.
-   **Browser storage:** Entries are saved using `localStorage` and can
    remain available after refreshing or reopening the page in the same
    browser profile.

## Tech Stack

-   **HTML5** --- page structure and form controls
-   **CSS3** --- layout, responsive styling, colors, typography, and
    transitions
-   **Vanilla JavaScript** --- journal logic, photo processing, search,
    editing, deletion, and export
-   **Browser `localStorage`** --- stores journal entries locally
-   **Canvas API** --- resizes uploaded photos before they are stored
-   **Google Fonts** --- DM Sans and Playfair Display (when an internet
    connection is available)

## Project Structure

The current prototype is intentionally kept in one file:

``` text
after_hour/
└── index.html
```

A backup file such as `index.html.bak` may also exist if one was created
during development.

## Run the Project

### Option 1: Open it from Windows

1.  Locate the project folder on your E: drive.
2.  Open `index.html` in a browser such as Brave or Chrome.

For the current setup, the file is located at:

``` text
E:\after_hour\index.html
```

### Option 2: Open it from Ubuntu on WSL

If the project is on the Windows E: drive, open Ubuntu and run:

``` bash
cd /mnt/e/after_hour
explorer.exe "$(wslpath -w "$PWD/index.html")"
```

This opens the HTML file using Windows' default application for HTML
files.

## How to Use

1.  Enter a title (optional) and write your thoughts.
2.  Select a mood.
3.  Add a song title and artist if you want to remember the soundtrack.
4.  Choose a photo to attach to the moment, if desired.
5.  Click **Save this moment**.
6.  Find the entry in the midnight archive.
7.  Use search to find saved entries, or edit and delete entries as
    needed.
8.  Use **Export memories** to download a JSON backup.

## Data Storage and Privacy

This version uses browser `localStorage`. Journal entries are stored in
the browser profile on the device where the website is opened.

-   No account or backend is currently required.
-   Entries do not automatically sync to another browser, computer, or
    phone.
-   Clearing browser site data or losing the browser profile can delete
    entries.
-   Browser storage is not encrypted or password-protected by this
    project.
-   Photos are stored as image data within the saved journal entries, so
    they can use significantly more storage than text alone.
-   Browser storage has limits. If saving fails because storage is full,
    reduce the number or size of photos and export a backup.
-   Export your memories regularly and keep the backup somewhere
    separate from the browser.

**Do not use this prototype to store highly sensitive information.**
Local browser storage should not be treated as permanent or secure
archival storage.

## Current Scope and Future Ideas

The current project is a personal local prototype. Potential next
improvements include:

-   Verify and refine photo restoration when editing an entry.
-   Add date-based browsing and mood filters.
-   Add a "revisit a memory" feature.
-   Add clickable links for saved songs.
-   Improve photo storage management and backup workflows.
-   Split the single HTML file into separate HTML, CSS, and JavaScript
    files.
-   Consider a local database or secure cloud sync only if needed later.

## Project Status

**Current stage:** Working prototype under active development.

The project currently focuses on capturing a moment with written
thoughts, a mood, a song, and an optional photo. Storage is
browser-based; a separate database and cloud synchronization have not
been implemented.

## License

No license has been specified yet. Add a license before distributing or
reusing the project publicly.
