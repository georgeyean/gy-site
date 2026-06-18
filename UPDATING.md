# Updating Your Website

All editing can be done directly in GitHub — no local installation needed.

## Add or edit a paper

1. Open `data/papers.yaml` in GitHub
2. Copy an existing entry and paste it at the top of the file
3. Fill in the fields: `title`, `authors`, `year`, `status`, `abstract`
4. Status options: `working paper` · `under review` · `revise and resubmit` · `work in progress` · `published`
5. For the job market paper, add `jmp: true`
6. To attach a PDF, upload the file to `static/files/` and set `pdf: "/files/your-paper.pdf"`
7. Commit — the site redeploys automatically in ~2 minutes

## Update your bio

Edit `content/_index.md`. The text below the `---` block is your bio in Markdown.

## Add a teaching entry

Open `data/teaching.yaml` and add:
```yaml
- course: "Course Name and Number"
  role: "Teaching Fellow"
  institution: "Harvard University"
  term: "Fall 2025"
```

## Add an award or fellowship

Open `content/_index.md` and add a line to the `awards:` list in the front matter:
```yaml
awards:
  - "Award Name, Year"
```

## Add a news item

In `content/_index.md`, add to the `news:` list:
```yaml
news:
  - date: "Month Year"
    item: "Description of the news item"
```

## Replace your photo

1. Rename your headshot to `photo.jpg` (square crop, at least 400×400 px)
2. Upload it to `static/images/`
3. Open `hugo.yaml` and uncomment the photo line:
   ```yaml
   photo: "/images/photo.jpg"
   ```

## Upload your CV

1. Upload your PDF to `static/files/` named `cv.pdf`
2. Open `hugo.yaml` and uncomment the cv line:
   ```yaml
   cv: "/files/cv.pdf"
   ```
   The CV button will appear automatically in the hero.

## Add a social link

Open `hugo.yaml` and uncomment (or add) the relevant line under `params:`:
```yaml
scholar: "https://scholar.google.com/citations?user=YOUR_ID"
twitter: "https://twitter.com/YOURHANDLE"
```

## Write a blog post

Create a new file at `content/blog/YYYY-MM-DD-title.md`:
```markdown
---
title: "Your Post Title"
date: 2026-01-15
---

Post content here.
```
