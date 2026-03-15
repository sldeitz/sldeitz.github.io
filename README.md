# shilohdeitz.com — GitHub Pages Site

Built with [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) Jekyll theme.

## Setup Instructions

### 1. Create your GitHub repository
- Go to github.com and create a new repo named `yourusername.github.io`
- Upload all these files to the repo (or clone and push)

### 2. Update `_config.yml`
Open `_config.yml` and replace:
- `url: "https://yourusername.github.io"` → your actual GitHub Pages URL
- `repository: "yourusername/yourusername.github.io"` → your GitHub username/repo
- `url: "mailto:your.email@slu.edu"` → your real SLU email address

### 3. Add your profile photo
- Save your photo as `assets/images/profile.jpg`
- Commit and push to GitHub

### 4. Add your CV PDF
- Save your CV as `assets/Deitz-CV-2025-Dec.pdf`
- Commit and push

### 5. Set up the contact form (free)
- Go to https://formspree.io and sign up (free)
- Create a new form and copy your Form ID
- In `_pages/contact.md`, replace `YOUR_FORM_ID` with your actual ID

### 6. Enable GitHub Pages
- In your repo: Settings → Pages → Source: Deploy from branch → main
- Your site will be live at `https://yourusername.github.io` within a few minutes

### 7. (Optional) Connect your custom domain
- In GitHub repo: Settings → Pages → Custom domain → enter `shilohdeitz.com`
- In your domain registrar (wherever you bought shilohdeitz.com), update DNS:
  - Add 4 A records pointing to GitHub's IPs:
    - 185.199.108.153
    - 185.199.109.153
    - 185.199.110.153
    - 185.199.111.153
  - Add a CNAME record: `www` → `yourusername.github.io`
- Cancel your Squarespace subscription once DNS propagates (24–48 hrs)

## File Structure

```
├── _config.yml          # Main site configuration
├── _data/
│   └── navigation.yml   # Top nav links
├── _pages/
│   ├── about.md
│   ├── research.md
│   ├── publications.md
│   ├── teaching.md
│   └── contact.md
├── assets/
│   └── images/
│       └── profile.jpg  # Add your photo here
├── index.md             # Homepage
├── Gemfile
└── README.md
```

## Local Development (optional)

If you want to preview changes locally before pushing:

```bash
gem install bundler
bundle install
bundle exec jekyll serve
# Visit http://localhost:4000
```

## Updating Content

All content pages are plain Markdown files in `_pages/`. Edit them directly on GitHub (click the pencil icon) or in any text editor. Changes go live within ~1 minute after pushing.
