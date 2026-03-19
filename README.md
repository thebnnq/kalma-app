# Kalma — GitHub Pages Site

This repository hosts the public web presence for the **Kalma** wellness app.

## Pages

| Page | File | URL |
|------|------|-----|
| Homepage | `index.html` | `https://yourusername.github.io/kalma/` |
| Privacy Policy | `privacy-policy.html` | `https://yourusername.github.io/kalma/privacy-policy.html` |
| Terms of Service | `terms-of-service.html` | `https://yourusername.github.io/kalma/terms-of-service.html` |
| Delete Account | `delete-account.html` | `https://yourusername.github.io/kalma/delete-account.html` |

## Deploying to GitHub Pages

1. Create a new GitHub repository (e.g. `kalma` or `kalma-site`)
2. Upload all `.html` files to the root of the repository
3. Go to **Settings → Pages**
4. Under **Source**, select **Deploy from a branch**
5. Choose **main** branch, **/ (root)** folder → Save
6. Your site will be live at `https://yourusername.github.io/kalma/` within ~60 seconds

## Using a Custom Domain (e.g. kalma.app)

1. Add a file named `CNAME` to the repo root containing just your domain:
   ```
   kalma.app
   ```
2. In your domain registrar (Namecheap, Cloudflare, etc.), add these DNS records:

   | Type | Name | Value |
   |------|------|-------|
   | A | @ | 185.199.108.153 |
   | A | @ | 185.199.109.153 |
   | A | @ | 185.199.110.153 |
   | A | @ | 185.199.111.153 |
   | CNAME | www | yourusername.github.io |

3. Back in GitHub Pages settings, enter your custom domain and enable **Enforce HTTPS**

## Updating App Links

In `index.html`, update the Google Play badge href with your actual Play Store URL:
```html
<a href="https://play.google.com/store/apps/details?id=YOUR_APP_ID" class="badge-store">
```

## Files

```
kalma-site/
├── index.html           ← Homepage
├── privacy-policy.html  ← Privacy Policy
├── terms-of-service.html← Terms of Service
├── delete-account.html  ← Account Deletion
└── README.md            ← This file
```
