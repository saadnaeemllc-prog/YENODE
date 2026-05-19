# Beyenode GitHub Pages Setup

This folder is ready for GitHub Pages.

## Files included
- index.html — your website page
- CNAME — custom domain file for beyenode.com
- .nojekyll — prevents GitHub Pages from applying Jekyll processing

## Upload steps
1. Go to GitHub and create a new repository.
   Example name: beyenode-site

2. Upload all files from this folder into the repository root.
   Do not put them inside another folder.

3. Go to:
   Repository → Settings → Pages

4. Under Build and deployment:
   Source: Deploy from a branch
   Branch: main
   Folder: /root

5. Click Save.

6. In Custom domain, enter:
   beyenode.com

7. Wait for GitHub to verify DNS.

8. After verification, enable:
   Enforce HTTPS

## DNS records for beyenode.com

At your domain provider, add these records:

A     @     185.199.108.153
A     @     185.199.109.153
A     @     185.199.110.153
A     @     185.199.111.153

CNAME www   your-github-username.github.io

Replace `your-github-username` with your real GitHub username.

## Important
If you want www.beyenode.com to work, the CNAME record is required.
If you only want beyenode.com, the four A records are enough.
