# Jungle. — how to add a project

## One-time setup (do this once)

1. Upload the contents of this folder to the repo `ronijbarahi/jungle`
   (GitHub website → Add file → Upload files → drag → Commit changes).
2. Open the `demo/` folder in the repo and delete every file in it.
   Those images are mockups for brands that were never Jungle clients.
3. Wait ~2 minutes for GitHub Pages to rebuild.
4. Go to https://designbyjungle.com/admin
5. Click "Sign In with Token". Follow the link it gives you to GitHub,
   generate the token, copy it, paste it back into the box.

The token is saved in your browser. You only do this again when it expires.

## Every time after that

1. Go to https://designbyjungle.com/admin
2. Click "Projects".
3. Click "Add Project" (or open an existing one to edit it).
4. Fill the fields. Drag images into the image fields.
5. Click Save / Publish.
6. Wait about 60 seconds, then refresh designbyjungle.com.

## Field notes

- **URL slug** — lowercase, hyphens, no spaces. This becomes the web address
  of the project page. Once you have shared a link, do not change it.
- **Card number** — the small "01", "02" on the homepage grid. If you reorder
  projects, renumber these by hand.
- **Homepage tags** — short. Two items, e.g. `Rebrand · Packaging`
- **Scope** — longer. Three items, e.g. `Rebrand · Packaging · Retail`
- **Results** — optional. Leave empty and that section just disappears.
  Three results looks best.
- **Images** — Homepage thumbnail is the grid image. Hero is the big one at
  the top of the project page. Image 2/3/4 run down the page.
  Leave any blank and you get an empty placeholder box, not a broken image.

## Where the content actually lives

`data/projects.json` — one file, all projects. The CMS writes to it.
The homepage and the project pages both read from it.
Never edit the project list inside index.html or project.html again.
