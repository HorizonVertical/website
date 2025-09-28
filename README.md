# Website
HorizonVertical is hosting its website [www.horizonvertical.org](https://horizonvertical.org).
This website is built using [Zola](https://www.getzola.org), GitHub Pages, and GitHub Actions.
Domain: `horizonvertical.org` is managed by imkoga002.

## Notifications
### How to Add New Notifications
To add a new notification, you can create a new file in the `content/notifications` directory of [website repository](https://github.com/horizonvertical/website) that is pushed to our GitHub organization.
Step-by-step instructions:
1. Clone the reposirory. `git@github.com:horizonvertical/website.git`
2. Create a new file in the `content/notifications` directory with the following format:
   ```
   ---
   title: "Your Notification Title"
   date: YYYY-MM-DD
   ---
   Your notification content goes here.
   ```
3. Commit your changes and push them to the repository. That's all!

Our website is set up to automatically build and deploy whenever changes are pushed to the `main` branch. This means that your new notification will be live on the website shortly after you push your changes.

## GihHub Pages
Our website is hosted on GitHub Pages. And it's SSG (Static Site Generator) based on Zola. So some settings are changed to make it work.
1. Source of Pages is `gh-pages` branch.
2. Build directory is `public`.
3. Custom domain is set to `www.horizonvertical.org` with 2 settings:
  - This is set in the `CNAME` file in the `./static/` directory of the repository.
  - This is set in the setting of Pages as Custom domain.
4. GitHub Actions is using workflow file for Zola to build the site and deploy.
