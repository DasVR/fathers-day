# Our Days — Photo Setup Guide

This folder holds all the photos for your memory journey. The app works immediately with placeholders until you add your real images.

## Quick start

1. Copy your photos into this `images/` folder.
2. Open `index.html` in a text editor (or Cursor).
3. Find the `PHOTOS` array near the top of the `<script>` section.
4. Update each entry's `src` to match your filename, and edit the `caption`, `year`, and `note` to match your memories.
5. Double-click `index.html` to open it in Safari or Chrome.

## Hero photo

Add a photo of you and Dad as:

```
images/hero-photo.jpg
```

This is the big polaroid on the cover — pick one you both love.

## Photo entry format

Each photo in the `PHOTOS` array looks like this:

```javascript
{
  src: 'images/early-years-beach-2015.jpg',   // path relative to index.html
  caption: 'That beach day when I was 5...',    // shown on the card and in lightbox
  year: '2015',                                 // shown on hover and in lightbox
  category: 'early-years',                      // early-years | adventures | everyday-love
  note: 'Optional extra line of text',          // optional — delete the line if unused
  tall: true                                    // optional — makes the card taller in the masonry grid
}
```

## Categories

| Category ID     | Label              | Use for                          |
|-----------------|--------------------|----------------------------------|
| `early-years`   | Early Years        | Childhood photos, old memories   |
| `adventures`    | Adventures         | Trips, outings, milestones       |
| `everyday-love` | Everyday Love      | Quiet moments, everyday life     |

## File tips

- **Formats:** `.jpg`, `.jpeg`, `.png`, or `.webp` all work.
- **Naming:** Use descriptive names like `dad-arriq-fishing-2018.jpg` so they're easy to find later.
- **Size:** Resize large photos to around 1200–2000px wide before adding them. This keeps the page fast.
- **Missing photos:** If a file isn't found, the app shows a soft gradient placeholder — captions still appear.

## Pin to MacBook Dock

**Safari (macOS Sonoma+):**
1. Open `index.html` in Safari.
2. File → **Add to Dock** (or Share → Add to Dock).

**Chrome:**
1. Open the page.
2. Menu (⋮) → **Save and Share** → **Install page as app**.

Your dad can open it like any other app when he needs a calm moment.

## Optional background music

Add a peaceful audio file at:

```
audio/calm-ambient.mp3
```

A soft instrumental or nature sound works best. The music toggle appears in the top-right corner only when this file exists. It starts muted — Dad chooses when to turn it on.
