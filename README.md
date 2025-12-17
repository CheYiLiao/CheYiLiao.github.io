# Academic Portfolio - Jekyll Template

A modular, maintainable academic portfolio website for GitHub Pages.

## 📁 Folder Structure

```
academic-site/
├── _config.yml          # Site settings & personal info
├── _data/               # Your content (YAML files)
│   ├── about.yml        # Bio/introduction
│   ├── talks.yml        # Invited talks
│   ├── publications.yml # Papers
│   ├── services.yml     # Academic service
│   ├── awards.yml       # Honors & awards
│   └── teaching.yml     # Courses taught
├── _includes/           # Section templates (HTML)
│   ├── nav.html
│   ├── about.html
│   ├── talks.html
│   ├── publications.html
│   ├── services.html
│   ├── awards.html
│   └── teaching.html
├── _layouts/
│   └── default.html     # Main page template
├── assets/
│   ├── css/style.css    # Stylesheet
│   ├── js/main.js       # JavaScript
│   └── images/          # Your images (create this)
└── index.html           # Main page
```

## 🚀 Quick Start

### 1. Create GitHub Repository
Create a new repo named `yourusername.github.io`

### 2. Upload Files
Upload all files from this folder to your repository

### 3. Edit Your Info

**Step 1: `_config.yml`** - Basic info
```yaml
author:
  name: Your Name
  title: Assistant Professor
  email: you@university.edu
  ...
```

**Step 2: `_data/*.yml`** - Your content
- `about.yml` - Your bio (supports Markdown)
- `publications.yml` - Your papers
- `talks.yml` - Your presentations
- etc.

### 4. Add Your Photo
1. Create `assets/images/` folder
2. Add your photo as `profile.jpg`
3. Update `_config.yml`: `photo: /assets/images/profile.jpg`

### 5. Deploy
Push to GitHub. Your site will be live at `https://yourusername.github.io` in ~1 minute.

## ✏️ How to Edit Content

### Adding a Publication
Edit `_data/publications.yml`:
```yaml
- title: "Your Paper Title"
  authors:
    - "Your Name"
    - "Coauthor"
  venue: "Conference 2025"
  links:
    - name: "PDF"
      url: "https://arxiv.org/..."
    - name: "Code"
      url: "https://github.com/..."
```

### Adding a Talk
Edit `_data/talks.yml`:
```yaml
- date: "2025/06"
  type: "Keynote"
  venue: "Conference Name"
  venue_url: "https://..."
  title: "Your Talk Title"
  slides: "/assets/slides/talk.pdf"
```

### Modifying Section Layout
Edit files in `_includes/`. For example, to change how publications display, edit `_includes/publications.html`.

### Changing Colors
Edit CSS variables in `assets/css/style.css`:
```css
:root {
    --primary-color: #1565c0;  /* Change this */
    --text-dark: #2c3e50;
    ...
}
```

## 🔧 Local Development (Optional)

To preview changes locally before pushing:

```bash
# Install Jekyll (one time)
gem install bundler jekyll

# Run local server
bundle init
bundle add jekyll
bundle exec jekyll serve
# View at http://localhost:4000
```

## 📝 Adding New Sections

1. Create data file: `_data/newsection.yml`
2. Create template: `_includes/newsection.html`
3. Add to `index.html`: `{% include newsection.html %}`
4. Add nav link in `_includes/nav.html`

## 🎨 Customization Tips

- **Fonts**: Change in `_layouts/default.html` (Google Fonts link) and `assets/css/style.css`
- **Colors**: All in CSS `:root` variables
- **Layout**: Modify grid/flexbox in CSS
- **Sections**: Reorder `{% include %}` statements in `index.html`

## 📄 License

Feel free to use this template for your personal academic website.
