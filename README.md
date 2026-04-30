# Baby Shower Invitation

This is a one-page GitHub Pages baby shower invitation for `invite.gabevazquez.com`.

## Files

- `index.html` = the invitation page
- `styles.css` = the design
- `CNAME` = custom domain setting for GitHub Pages
- `assets/og-baby-shower.png` = social preview image for text messages, Facebook, etc.
- `assets/photo-1.svg`, `photo-2.svg`, `photo-3.svg` = placeholder images you can replace

## Edit this in VS Code

1. Open this folder in VS Code.
2. Open `index.html`.
3. Replace the filler info:
   - Names
   - Date and time
   - Party location
   - Google Maps link
   - Registry link
   - RSVP phone number
4. Replace the placeholder pictures in `/assets/` with your real photos.
5. Keep the social preview image named `og-baby-shower.png` unless you also update the meta tags in `index.html`.

## Put it on GitHub

1. Go to github.com.
2. Create a new repository, for example: `baby-shower-invite`.
3. Upload all files in this folder to the repository.
4. Go to repository `Settings` → `Pages`.
5. Under `Build and deployment`, choose:
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/root`
6. Under `Custom domain`, enter:

```text
invite.gabevazquez.com
```

7. Save.
8. Check `Enforce HTTPS` after GitHub finishes issuing the certificate.

## DNS setup

At the DNS provider for `gabevazquez.com`, create this record:

```text
Type: CNAME
Host/Name: invite
Value/Target: YOUR-GITHUB-USERNAME.github.io
TTL: Auto or default
```

Replace `YOUR-GITHUB-USERNAME` with your actual GitHub username.

GitHub says custom subdomains for GitHub Pages should use a CNAME record pointing to your GitHub Pages default domain, and the custom domain should also be added in the repository Pages settings.

## Test the social preview

After the site is live, send yourself this link by text:

```text
https://invite.gabevazquez.com/
```

If the preview image does not update right away, wait a bit. Text apps and social apps cache previews.
