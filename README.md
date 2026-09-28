# Cristina D. M. Miller, PhD — Personal Website

A simple static website designed for GitHub Pages.

## Publish on GitHub Pages
1. Create or open your GitHub repository.
2. Upload the contents of this folder so `index.html` is at the repository root.
3. Commit the files to the `main` branch.
4. Go to **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Choose **main** and **/(root)**, then save if needed.

## Update your name, title, affiliation, bio, or profile links
Edit `data/site.json`.

Example:
```json
{
  "name": "Cristina D. M. Miller, PhD",
  "title": "Research Economist",
  "affiliation": "USDA Rural Development Innovation Center",
  "bio": "[ADD PROFESSIONAL BIOGRAPHY]"
}
```

Shared information is loaded from this file so you do not need to edit every HTML page.

## Replace your photo
Replace `assets/images/profile-placeholder.svg` with your own image, for example `headshot.jpg`, then update the `photo` value in `data/site.json` to:

```json
"photo": "/assets/images/headshot.jpg"
```

## Upload a new CV
Put your current CV at:

`assets/cv/cv.pdf`

Keep the filename `cv.pdf` so the CV buttons continue to work.

## Add research papers
Edit `data/research.json`.

Example:
```json
{
  "publications": [
    {
      "title": "Paper title",
      "coauthors": "Coauthor names",
      "publication": "Journal or publication information",
      "year": "2026",
      "description": "Optional short description.",
      "links": {
        "paper": "https://...",
        "doi": "https://...",
        "data": "",
        "code": ""
      }
    }
  ]
}
```

You can also use the sections `working_papers`, `research_in_progress`, and `reports_other_research`.

## Add teaching affiliations and courses
Edit `data/teaching.json`.

Example:
```json
{
  "institutions": [
    {
      "name": "[INSTITUTION NAME]",
      "courses": [
        {
          "title": "[COURSE TITLE]",
          "term": "[SEMESTER / YEAR]",
          "description": "",
          "links": {
            "syllabus": "",
            "course_materials": ""
          }
        }
      ]
    }
  ]
}
```

## Add professional links
In `data/site.json`, add only the links you want to show. Leave others blank.

```json
"profiles": {
  "google_scholar": "",
  "linkedin": "",
  "orcid": "",
  "github": "",
  "email": ""
}
```

## Notes
- No analytics or tracking are included.
- The site uses only HTML, CSS, JavaScript, and JSON.
- The layout is responsive for desktop, tablet, and mobile.
- Unknown personal or professional information has not been invented.
