# ✍️ How to write a new post

Your blog lives at **https://nandita-roy.github.io/**. Every post is just a
plain text file written in **Markdown** (`.md`). To publish, you add a file and
push it — the site rebuilds and goes live on its own in about a minute.

---

## The quick version

1. Go to the **`content/posts/`** folder.
2. Make a copy of **`_template.md`** and rename it, e.g. `my-first-trip.md`.
   - Use lowercase, and dashes instead of spaces (this becomes the web address:
     `nandita-roy.github.io/posts/my-first-trip/`).
3. Open your new file and edit the top block (the **front matter**):
   - `title` → your post's title
   - `date` → today's date
   - `draft: false` → **this is what actually publishes it** (leave it `true`
     while you're still writing)
   - `tags` and `summary` are optional
4. Write your post below the second `---` line, in Markdown.
5. Save, then **commit and push** (see below). Done — it's live shortly after.

---

## Preview how your Markdown looks

Before publishing, paste your text into **https://dillinger.io** — it shows a
live side-by-side preview of your Markdown so you can check headings, links,
lists, and formatting look right. When it looks good, copy it back into your
`.md` file.

(Prefer a local preview? Run `hugo server -D` in the project folder and open
http://localhost:1313 — it live-reloads as you type.)

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

Images: put files in the **`static/images/`** folder, then reference them as
`/images/yourfile.jpg`.

---

## Publishing (commit & push)

After saving your file, from the project folder run:

```bash
git add .
git commit -m "New post: my first trip"
git push
```

That's the whole workflow: **copy the template → write → set `draft: false` →
push.** The GitHub Actions workflow rebuilds and deploys automatically, and
your post appears at **https://nandita-roy.github.io/** within a minute.
