# Personal site

Plain HTML, CSS and one font from Google Fonts. No build step.

## Files
- `index.html` home: work for hire, links to Projects and Professional
- `projects.html` personal projects (one row per subdomain)
- `professional.html` services and client work
- `photography.html`, `lifeguarding.html` job pages
- `retail.html` resume page (add a `resume.pdf` next to it for the download button)
- `404.html` not found page, `style.css` all styling, `images/` your photos

## Edit
Search every file for "Your Name", "yourdomain.com", "yourusername" and placeholder text and replace it.
Put photos in `images/` (see the comment in `photography.html`).

## Put it on GitHub
1. Create a new repository on github.com (name it anything, public or private).
2. Click "uploading an existing file", drag in everything from inside this folder (not the folder itself), and commit.
   Or with git: `git init`, `git add .`, `git commit -m "site"`, then add the remote and `git push`.

## Connect to Cloudflare
1. Cloudflare dashboard > Workers & Pages > Create > Pages > Connect to Git, pick the repository.
2. Framework preset: None. Build command: leave empty. Build output directory: `/` (or leave blank). Deploy.
3. Open the project > Custom domains > Set up a custom domain and enter your domain (e.g. `yourdomain.com`).
   The domain needs to be on Cloudflare DNS. Cloudflare adds the record for you.
4. Your project subdomains keep working. They are separate DNS records, so this doesn't affect them.

Every push to GitHub redeploys the site automatically.
