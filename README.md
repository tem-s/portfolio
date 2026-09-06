# Temilola Eniola-Jegede — Portfolio

This is a single-page personal portfolio built to showcase my technical projects, business ventures, and skills as a final-year Computer Systems Engineering student.

http://temi-portfolio-site.s3-website.eu-west-2.amazonaws.com/

---

## About

This site brings together three sides of my work:

- **Technical projects** — coursework and independent builds in Java, C#, and web development
- **Business ventures** — three e-commerce brands I've built and run alongside my degree (Replēn, The Làfíà Edit, Jumper-Junction)
- **Certifications & skills** — AWS Cloud Practitioner, Azure Fundamentals, and hands-on placement experience

---

## Tech stack

- HTML5, CSS3, vanilla JavaScript — no framework or build step required
- Google Fonts (Space Grotesk + Newsreader)
- Hosted on AWS (S3 + CloudFront)

## Project structure

```
portfolio/
├── index.html          # Page structure and content
├── style.css           # All styling, layout, and responsive rules
├── script.js           # Mobile nav toggle
├── .vscode/
│   └── launch.json      # VS Code debug config (opens index.html in Chrome)
└── README.md
```

## Running locally

No installation or build step needed — it's a static site.

**Option 1 — open directly:**
Double-click `index.html`, or open it in a browser via `File > Open`.

**Option 2 — Live Server (recommended for editing):**
1. Install the "Live Server" extension in VS Code
2. Right-click `index.html` → "Open with Live Server"
3. The page auto-refreshes on save

**Option 3 — VS Code debugger:**
Press `F5` (uses the config in `.vscode/launch.json`) to open the site in Chrome with debugging attached.

## Deployment

Hosted on AWS using:

1. **S3** — stores the static files (`index.html`, `style.css`, `script.js`)
2. **CloudFront** — serves the site over HTTPS with edge caching, using Origin Access Control so the S3 bucket itself stays private

To redeploy after making changes: upload the updated files to the S3 bucket, then create a CloudFront invalidation (`/*`) so the CDN cache picks up the new version.

## Sections

| Section | Content |
|---|---|
| Hero | Name and tagline |
| About | Education, background, and aspirations |
| Business ventures | Replēn, The Làfíà Edit, Jumper-Junction |
| Projects | EECS Support System, Horse Race Simulator, Pedestrian & Cyclist GPS, Weather App, this portfolio |
| Skills | Technical and business/professional skills |
| Certifications | AWS Cloud Practitioner, Azure Fundamentals |
| Contact | Email and LinkedIn |

## Contact

- Email: temiajenifuja@gmail.com
- LinkedIn: [linkedin.com/in/temilola-jegede](https://www.linkedin.com/in/temilola-jegede)
