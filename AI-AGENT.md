# TASK: Add Romantic Gallery & YouTube Video — DO NOT CHANGE EXISTING STRUCTURE

You are working on the existing GitHub project:

`Amrin002/myfuture`

Main target file:

`loveletter.html`

## CRITICAL RULE

**DO NOT CHANGE, REFACTOR, REDESIGN, REORDER, OR REMOVE THE EXISTING STRUCTURE.**

The current `loveletter.html` already has its own romantic design, layout, animations, audio system, letter content, buttons, and JavaScript.

Your job is ONLY to **ADD new content** to the existing page.

Think of this as:

> "Add new sections to the existing love letter."

NOT:

> "Redesign the love letter."

### Absolutely DO NOT:

- Rewrite the existing HTML structure.
- Replace the existing CSS.
- Change the existing color palette.
- Change the existing typography.
- Change the existing background.
- Remove existing animations.
- Remove existing audio/music functionality.
- Change the existing letter content.
- Change existing buttons.
- Change existing JavaScript unless absolutely required for the new feature.
- Change the existing page order except inserting the new sections at the requested location.
- Replace the existing romantic style with a new design.
- Add a navbar.
- Add a sidebar.
- Add frameworks.
- Add React/Vue/etc.
- Add external CSS frameworks.
- Add unnecessary dependencies.

---

# CURRENT CONTENT TO PRESERVE

The existing page contains the romantic letter addressed to:

**Celline Shanela**

The letter should remain exactly as it currently exists.

The existing signature:

**From Christian**

must also remain unchanged.

Do not rewrite or "improve" the existing letter.

---

# FEATURE 1 — ROMANTIC GALLERY

Add a new section AFTER the existing love letter content and BEFORE the existing final signature/ending section, if that location already exists naturally in the current structure.

Do not move existing elements unnecessarily.

Section title:

### 📸 Our Little Memories

Supporting text:

> "Ini aku ada buat kamu sesuatu di bawah di liat yaaa..."

The gallery should feel like an extension of the existing romantic design.

## Gallery requirements

Create a gallery containing 6 images:

```text
asset/gallery/photo-1.jpg
asset/gallery/photo-2.jpg
asset/gallery/photo-3.jpg
asset/gallery/photo-4.jpg
asset/gallery/photo-5.jpg
asset/gallery/photo-6.jpg
```

If the files do not exist, create the directory and use the paths above as placeholders.

Do NOT generate fake images.

The user will replace the images later.

Each image should:

- follow the existing visual style
- have rounded corners consistent with the existing design
- have a subtle shadow
- have a soft hover effect
- use `object-fit: cover`
- use `loading="lazy"`
- remain responsive on mobile
- not break the existing layout

Use a simple responsive grid.

Desktop:

- 3 columns

Tablet:

- 2 columns

Mobile:

- 1 or 2 columns depending on available width

Do not introduce a completely new visual language.

---

# FEATURE 2 — YOUTUBE VIDEO

After the gallery, add a new section.

Title:

### 🎬 Ini Untuk Kamu, Sayang

Supporting text:

> "Salah satu bentuk sayangku sama kamu."

Add a responsive YouTube embed.

Use this placeholder:

```html
https://www.youtube.com/embed/VIDEO_ID
```

The agent MUST NOT invent a YouTube video ID.

Keep `VIDEO_ID` as a placeholder until the user provides the real YouTube link.

Use an iframe with:

```html
loading="lazy" allow="accelerometer; autoplay; clipboard-write; encrypted-media;
gyroscope; picture-in-picture; web-share" allowfullscreen
```

The video must maintain a 16:9 aspect ratio and work properly on mobile.

---

# IMPORTANT — EXISTING AUDIO

The page already has background music/audio.

DO NOT:

- replace the audio
- remove the audio
- change the audio source
- modify autoplay behavior
- modify existing audio controls
- create another competing audio player

The new YouTube video must coexist with the existing music system.

If YouTube autoplay could conflict with the existing audio, DO NOT enable YouTube autoplay.

---

# ROMANTIC TRANSITION

Between the existing letter and the gallery, add only a subtle transition.

Use the existing visual language.

Example concept:

> "Ada sesuatu lagi yang ingin aku kasih buat kamu..."

Then:

> **♡ Lihat di sini ♡**

Do NOT create a complicated modal or new application flow.

Keep it simple.

---

# FINAL CONTENT

The existing ending/signature must remain.

Do not replace:

> From Christian

Do not rewrite the original letter.

Do not insert additional paragraphs into the existing letter.

The gallery and video are ADDITIONS only.

---

# CSS RULES

If CSS is required:

1. Add only the minimum CSS required.
2. Scope new CSS classes specifically to the new sections.
3. Do not modify existing selectors unless absolutely necessary.
4. Avoid generic selectors such as:

```css
.container
.card
.button
img
section
```

because they may affect the existing page.

Prefer unique classes such as:

```css
.memories-section
.memories-gallery
.memory-card
.memory-video-section
.memory-video-wrapper
```

The new CSS must not leak into the existing design.

---

# JAVASCRIPT RULES

Do not modify existing JavaScript unless absolutely necessary.

The gallery should work without JavaScript if possible.

Do NOT introduce:

- React
- Vue
- jQuery
- Bootstrap
- Tailwind
- external UI libraries

Keep the page self-contained.

---

# RESPONSIVENESS

The existing page must continue working on:

- Desktop
- Tablet
- Android phone
- Small mobile screens

Test for:

```text
320px
375px
390px
430px
768px
1024px
1440px
```

The new gallery and video must not cause horizontal scrolling.

---

# VISUAL PRINCIPLE

The most important visual rule:

**The new gallery and video must look like they were always part of the existing `loveletter.html`.**

Do not make them look like a separate website.

Existing design = source of truth.

Use the existing:

- colors
- border radius
- shadows
- typography
- spacing
- romantic atmosphere
- animation style

when appropriate.

---

# FILE STRUCTURE

Only add what is necessary.

Expected:

```text
loveletter.html

asset/
└── gallery/
    ├── photo-1.jpg
    ├── photo-2.jpg
    ├── photo-3.jpg
    ├── photo-4.jpg
    ├── photo-5.jpg
    └── photo-6.jpg
```

Do NOT modify unrelated files.

---

# VALIDATION

Before finishing:

1. Read the original `loveletter.html`.
2. Identify its existing structure.
3. Preserve all existing content.
4. Add the gallery.
5. Add the YouTube section.
6. Verify existing audio still works.
7. Verify existing animations still work.
8. Verify existing buttons still work.
9. Verify no existing section was accidentally removed.
10. Verify there is no horizontal overflow on mobile.
11. Verify all image paths are correct.
12. Verify YouTube uses `/embed/VIDEO_ID`.
13. Verify there are no broken HTML tags.
14. Verify CSS selectors do not unintentionally affect existing components.
15. Review the final diff before committing.

---

# GIT RULE

Before modifying anything:

```bash
git status
```

If the working tree contains user changes:

**DO NOT overwrite them.**

After implementation:

```bash
git diff -- loveletter.html
git status
```

The final diff should contain ONLY the additions required for:

- Gallery
- YouTube video
- Minimal supporting CSS/HTML

Do not include unrelated formatting changes.

Commit message:

```text
feat: add romantic memories gallery and youtube video
```

---

# FINAL REQUIREMENT

The existing website is already considered the "base design".

Your responsibility is:

**ADD, NOT REBUILD.**

If you are unsure whether a change modifies the existing design, DO NOT make that change.

The final result should feel like:

**the same love letter, but with a small personal gallery and a special video gift added to it.**
