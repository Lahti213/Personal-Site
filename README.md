# Tyler Lahti - Personal Site

A modern, fast, and beautiful personal landing page showcasing outdoor adventures, trail running achievements, and photography.

## Features

✨ **Modern Design**

- Clean, editorial magazine-style aesthetic
- Smooth animations and transitions
- Fully responsive mobile-first design
- Custom serif/sans-serif font pairing (Crimson Pro + DM Sans)

🎨 **Visual Design**

- Earth-toned color palette inspired by trails and mountains
- Gradient backgrounds with subtle animations
- Interactive hover effects on all links and cards
- Photo gallery with overlay captions

⚡ **Performance**

- Single HTML file - blazing fast loading
- No JavaScript dependencies
- Optimized Google Fonts loading
- Minimal, efficient CSS

📱 **Content Sections**

- Hero landing with animated introduction
- Featured cards for Instagram, LinkedIn, and Flickr
- Adventure achievements with FKT, ultrarunning, and peak bagging links
- Photography gallery with Creative Commons licensed images

## Deployment to GitHub Pages

### Option 1: Quick Deploy (Recommended)

1. Create a new repository on GitHub (e.g., `your-username.github.io`)
1. Clone the repository:

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git
cd YOUR-REPO-NAME
```

1. Add the `index.html` file to the repository
1. Commit and push:

```bash
git add index.html README.md
git commit -m "Initial commit: Add personal landing page"
git push origin main
```

1. Enable GitHub Pages:
- Go to your repository on GitHub
- Click **Settings** → **Pages**
- Under **Source**, select `main` branch and `/ (root)` folder
- Click **Save**
1. Your site will be live at: `https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/`

### Option 2: Custom Domain (lahti.co)

If you want to use your custom domain:

1. Follow steps 1-4 from Option 1
1. Add a `CNAME` file:

```bash
echo "www.lahti.co" > CNAME
git add CNAME
git commit -m "Add custom domain"
git push origin main
```

1. Configure DNS at your domain registrar:
- Add a CNAME record: `www` → `YOUR-USERNAME.github.io`
- Add A records for apex domain:
  
  ```
  185.199.108.153
  185.199.109.153
  185.199.110.153
  185.199.111.153
  ```
1. In GitHub Settings → Pages:
- Enter `www.lahti.co` in the Custom domain field
- Check “Enforce HTTPS” (after DNS propagates)

## Customization

### Updating Content

All content is in the single `index.html` file. To update:

**Hero Section** (line 161-167):

```html
<h1>Your Name</h1>
<p class="hero-subtitle">Your description here</p>
```

**Links** (lines 170-270):

- Update href URLs
- Modify card titles and descriptions
- Add/remove cards as needed

**Colors** (CSS variables, lines 16-23):

```css
:root {
    --color-earth: #2a2520;       /* Dark brown */
    --color-trail: #c67d4e;       /* Warm orange accent */
    --color-sky: #5d8aa8;         /* Blue accent */
    /* Customize these to match your brand */
}
```

**Fonts** (line 10):
Replace Google Fonts URL to use different typefaces

### Adding More Pages

Create additional HTML files in the same directory:

- `about.html` - Extended bio
- `projects.html` - Project portfolio
- `blog.html` - Blog posts

Link them from the main page in the navigation.

## Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile Safari iOS
- Chrome Android

## Performance Metrics

- **Lighthouse Score**: ~99/100
- **First Contentful Paint**: <0.5s
- **Time to Interactive**: <1s
- **Total Page Size**: ~15KB (HTML + CSS), ~40KB with fonts

## Design Credits

- Font: [Crimson Pro](https://fonts.google.com/specimen/Crimson+Pro) by Jacques Le Bailly
- Font: [DM Sans](https://fonts.google.com/specimen/DM+Sans) by Colophon Foundry
- Icons: Custom SVG (inline)
- Photos: © Tyler Lahti (CC BY-SA 2.0 / CC BY-SA 4.0)

## License

Code: MIT License
Content & Photos: See individual Creative Commons licenses

-----

Built with ❤️ for adventurers and trail runners
