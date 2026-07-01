# ✍️ How to write a new post (no code, all in the browser)

Your blog lives at **https://nandita-roy.github.io/**. You never need to install
anything or open a terminal — you write posts right on the GitHub website.
When you save (“commit”), the site rebuilds itself and your post goes live in
about a minute.

---

## Step by step

1. **Open the repo:** go to
   👉 https://github.com/Nandita-Roy/Nandita-Roy.github.io
   (sign in as **Nandita-Roy**).

2. **Open the posts folder:** click into **`content`**, then **`posts`**.

3. **Create the file:** click the **`Add file`** button (top right) →
   **`Create new file`**.

4. **Name it:** in the filename box type your post name ending in `.md`, e.g.
   `my-first-trip.md`
   - Use lowercase and dashes instead of spaces — this becomes the web address:
     `nandita-roy.github.io/posts/my-first-trip/`.
   - (The `content/posts/` part is already filled in for you because you're
     inside that folder.)

5. **Paste the template** (copy the block in the next section) into the big
   text box, then edit it:
   - `title` → your post's title
   - `date` → today's date
   - `draft: false` → **this is what publishes it.** Leave it `true` while
     you're still writing and it stays hidden.
   - `tags` and `summary` are optional.
   - Write your post below the second `---` line.

6. **Check how it looks:** click the **`Preview`** tab (top of the edit box) to
   see your formatting before saving.
   - Want a bigger side-by-side preview? Paste your text into
     **https://dillinger.io** — it renders Markdown live as you type.

7. **Publish:** scroll down to **“Commit changes”**, leave *“Commit directly to
   the `main` branch”* selected, and click the green **`Commit changes`**
   button.

8. **That's it.** Wait ~1 minute, then refresh **https://nandita-roy.github.io/**
   — your new post is there. 🎉

> To edit a post later: open its `.md` file on GitHub, click the ✏️ **pencil**
> icon (top right of the file), make changes, and **Commit changes** again.

---

## The template to paste

```markdown
---
title: "My Post Title"
date: 2026-07-01T00:00:00Z
draft: false
tags: ["life", "travel"]
summary: "A one-line teaser shown in the post list."
---

Write your post here using Markdown.
```

There's also a copy of this saved as **`content/posts/_template.md`** in the
repo if you'd rather grab it from there (open it and click the **Copy raw
file** button).

---

## Markdown cheat sheet

```markdown
# Big heading
## Smaller heading

Normal paragraph. Leave a blank line between paragraphs.

**bold**   *italic*   `inline code`

- bullet list
- second item

1. numbered list
2. second item

> a quote / callout

[link text](https://example.com)

![photo caption](/images/photo.jpg)
```

**Adding images (also in the browser):** go to the **`static/images/`** folder
on GitHub → **`Add file`** → **`Upload files`** → drag your photo in →
**Commit changes**. Then in your post reference it as `/images/yourfile.jpg`.

---

### The whole thing in one line
**Create new file → paste the template → set `draft: false` → Commit changes.**
No terminal, no git commands — just the GitHub website.
