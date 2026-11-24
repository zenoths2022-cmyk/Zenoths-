# ZENOTHS — Since 2022

Mobile-first independent batch website. It is not the official college website.

## Website files
- `index.html` — page design and layout
- `data.js` — event announcements, photo gallery and Instagram links
- `zenoths-dragon-reference.png` — supplied dragon reference artwork

## Phone-only publishing (free)
1. Download and extract `ZENOTHS-website-starter.zip` on your Android phone.
2. Open https://github.com/ and sign in or create an account.
3. Create a **public** repository named `zenoths-batch-website`. Do not add a README or license if you are uploading these files directly.
4. In the repository, use **Add file → Upload files**. Upload `index.html`, `data.js`, `zenoths-dragon-reference.png`, and `README.md` from the extracted folder. Commit the upload to the `main` branch. Keep `index.html` at the repository root.
5. Open repository **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, select branch `main` and folder `/(root)`, then Save.
6. Wait for the deployment to finish. In Settings → Pages, open **Visit site**. The address will look like `https://YOUR-GITHUB-USERNAME.github.io/zenoths-batch-website/`. It can take several minutes to appear.

GitHub Pages on GitHub Free requires a public repository. The website and repository contents are therefore publicly viewable. Do not upload private student details, phone numbers, marks, medical records, or photos without permission.

## Give multiple batch members permission to update
1. Open the repository → **Settings → Collaborators** (sometimes shown under **Collaborators and teams**).
2. Choose **Add people**, enter each member's GitHub username or email, and send the invitation.
3. Give trusted editors **Write** access only. They must accept the invitation using their own GitHub accounts. Avoid giving Admin access unless necessary.
4. Editors can open `data.js` on GitHub mobile/web, tap the pencil/Edit control, make the change, and commit it. GitHub Pages will publish the update automatically after the commit.

## Add or update events
Edit `data.js`. Add objects inside the appropriate array. Keep commas between objects.

Example ongoing or upcoming event:
```js
{ title: "Sports Week", date: "Dec 10–12", description: "Live updates and highlights.", link: "https://example.com" }
```

To move an event from upcoming to ongoing, cut its object from `upcoming` and paste it inside `ongoing`. Remove it from both arrays when it is over, or keep a separate archive later.

## Add photos
1. In the repository, choose **Add file → Create new file** and name it `photos/.keep` (or upload a photo into a `photos` folder if the upload interface supports folders). Commit.
2. Upload photos into the `photos` folder.
3. Add an item to the `gallery` array in `data.js`, for example:
```js
{ src: "photos/sports-day.jpg", alt: "Sports day" }
```
Use the exact filename and letter case. Compress large photos before uploading so the site loads quickly on mobile data.

## Instagram links
Both supplied Instagram profile URLs are already configured in `data.js`.

## Important
The repository is public because GitHub Pages on the Free plan requires public repositories. Anyone can view the source files, but only invited collaborators can edit them. Only trusted members should receive Write access. Keep the college-official disclaimer in the website footer.
