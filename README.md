# 🌿 Quencher Mixer — Website

Premium wild-crafted Honduras sea moss brand. This is the source code for the Quencher Mixer website, deployable on GitHub Pages, Netlify, or any static hosting.

---

## 📁 File Structure

```
quencher-mixer/
├── index.html          ← Main website page
├── css/
│   └── style.css       ← All styles
├── js/
│   └── main.js         ← Interactivity (navbar, FAQ, animations)
├── images/             ← Add your product photos here
│   └── (add your images here)
└── README.md
```

---

## 🚀 How to Deploy on GitHub Pages (Free Hosting)

### Step 1 — Create a GitHub Repository
1. Go to [github.com](https://github.com) and sign in (or create a free account)
2. Click the **+** in the top right → **New repository**
3. Name it: `quencher-mixer` (or `quenchermixer.com` if you have a custom domain)
4. Set to **Public**
5. Click **Create repository**

### Step 2 — Upload Files
**Option A (Easy — No coding required):**
1. On your new repo page, click **uploading an existing file**
2. Drag and drop ALL files and folders from this project
3. Click **Commit changes**

**Option B (Using Git):**
```bash
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/YOUR_USERNAME/quencher-mixer.git
git push -u origin main
```

### Step 3 — Enable GitHub Pages
1. Go to your repo → **Settings** → **Pages**
2. Under "Source", select **Deploy from a branch**
3. Choose **main** branch → **/ (root)**
4. Click **Save**
5. Your site will be live at: `https://YOUR_USERNAME.github.io/quencher-mixer/`

---

## 🌐 Custom Domain Setup (e.g. quenchermixer.com)

1. Buy your domain from Namecheap, GoDaddy, or Google Domains
2. In GitHub Pages settings, enter your custom domain name
3. At your domain registrar, add these DNS records:
   ```
   A     @    185.199.108.153
   A     @    185.199.109.153
   A     @    185.199.110.153
   A     @    185.199.111.153
   CNAME www  YOUR_USERNAME.github.io
   ```
4. Check "Enforce HTTPS" in GitHub Pages settings

---

## 📸 Adding Your Product Images

1. Add your sea moss photos to the `/images/` folder
2. In `index.html`, replace the emoji placeholders (🌿) with actual `<img>` tags:
   ```html
   <img src="images/sea-moss-dried.jpg" alt="Quencher Mixer Dried Honduras Sea Moss" />
   ```
3. **SEO tip:** Always use descriptive alt text on images!

---

## 📧 Connecting Email Signup

The signup form is ready — just connect it to an email marketing platform:

**Recommended: Mailchimp (Free up to 500 contacts)**
1. Sign up at mailchimp.com
2. Create an Audience
3. Get your Mailchimp form action URL
4. In `js/main.js`, replace the `handleSignup` function with a fetch POST to Mailchimp

**Alternative: ConvertKit, Klaviyo, or EmailJS**

---

## 🔍 SEO Checklist

- [x] Title tag optimized
- [x] Meta description with keywords
- [x] Open Graph tags for social sharing
- [x] Schema.org structured data (Organization + Product)
- [x] Semantic HTML structure (h1, h2, h3 hierarchy)
- [x] Alt text placeholders on images
- [x] Canonical URL tag
- [x] Sitemap (create at sitemap.xml — see below)

### Create sitemap.xml
Create a file called `sitemap.xml` in your root folder:
```xml
<?xml version="1.0" encoding="UTF-8"?>
<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
  <url>
    <loc>https://quenchermixer.com/</loc>
    <changefreq>weekly</changefreq>
    <priority>1.0</priority>
  </url>
</urlset>
```

Then submit it to [Google Search Console](https://search.google.com/search-console).

---

## 📊 Adding Google Analytics

Add this just before `</head>` in index.html (replace `G-XXXXXXXXXX` with your ID):
```html
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

---

## 🛒 Shop Links

- **Walmart:** https://www.walmart.com/ip/Sea-Moss-Dried-Honduras-Quencher-Mixer/1096704300?classType=REGULAR&selectedSellerId=101342418
- **TikTok Shop:** https://shop.tiktok.com/us/pdp/quencher-mixer-sea-moss-gel-kit-92-minerals-organic-powerhouse/1729489189265117468

---

## 📬 Contact

- Phone: 919-438-1403
- Email: customersupport@quenchermixer.com
- TikTok: @quenchermixer

---

*© 2025 Quencher Mixer. All rights reserved.*
