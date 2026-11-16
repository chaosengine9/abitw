ANOTHER BRICK IN THE WALL - website files
=========================================

FILES (upload all of them to the same folder on your host)
  index.html            the game
  questions.json        the questions; the game loads this by itself every time it opens
  manifest.webmanifest, sw.js, icon-192.png, icon-512.png, apple-touch-icon.png
                        make it installable on a phone or tablet and let it work offline after a first visit

PUTTING IT ON GITHUB PAGES (free; the repository and the site are both public)
  1. github.com > New repository. Name it, for example, brick-wall. Choose Public. Create.
  2. "uploading an existing file": drag in ALL the files from this folder (not the folder itself). Commit.
  3. Settings > Pages > Build and deployment: Source = "Deploy from a branch", Branch = main, folder = / (root). Save.
  4. After a minute or two the address appears at the top of that page:
     https://YOUR-USERNAME.github.io/brick-wall/
  Any other static web host works too; just keep the files together in one folder.

ON YOUR PHONE OR TABLET
  Open the address. iPhone/iPad (Safari): Share > Add to Home Screen.
  Android (Chrome): menu > Install app (or Add to Home screen).

UPDATING LATER
  Replace questions.json (or index.html) in the repository: Add file > Upload files, drop the new copy in,
  commit. The site republishes in a minute or two. The game fetches the newest questions.json whenever it
  opens with a connection; if you are offline it uses the last copy it saved.

NOTES
  - questions.json here is your earlier file. Replace it with the newly merged one when you have it.
  - The "Load questions" button still lets you test a different file for one session; it does not change
    what the website loads next time.
  - The list of questions is publicly readable on a public site. It is only music facts.
