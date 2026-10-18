# GitHub upload aur deployment guide

## 1. ZIP extract karein

`careplus-glass-healthcare.zip` ko Extract All karein. `index.html` open karke local website dekh sakte hain.

## 2. GitHub repository banayein

GitHub par sign in karke New repository open karein.

- Repository name: `careplus-glass-healthcare`
- Description: `A modern, responsive healthcare website with glassmorphism UI, doctor discovery, interactive profiles, and appointment previews. Built with HTML, CSS & JavaScript.`
- Portfolio/demo share karne ke liye Public choose karein. Public repo ka source sab dekh sakte hain.
- README archive mein included hai; duplicate README initialize karna zaroori nahi.
- Create repository click karein.

## 3. Files upload karein

Empty repository mein uploading an existing file link use karein; existing repository mein Add file > Upload files use karein.

Extracted folder ke andar ki files upload karein. ZIP ya outer folder upload na karein. `index.html`, `style.css`, `script.js` aur baqi pages repository ke top level par hone chahiye.

Commit message: `Add CarePlus glassmorphism healthcare website`

Commit changes click karein. Repository mein `index.html` aur README nazar aane chahiye.

## 4. GitHub Pages enable karein

Repository Settings > Pages mein jayein. Build and deployment ke Source mein Deploy from a branch choose karein. Branch `main` aur folder `/(root)` select karke Save karein. Agar branch ka naam different hai to files wali branch select karein.

Deployment complete hone par isi page par Visit site link milega. Project URL ka pattern `https://YOUR-USERNAME.github.io/careplus-glass-healthcare/` hoga; ye template hai, abhi live URL nahi.

Official reference: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## 5. Live website check karein

- Home aur baqi navigation links open karein.
- Doctors page par search, filter aur profile dialog check karein.
- Appointment page par sample data se preview check karein.
- Mobile par menu aur forms dekhein.
- Contact/appointment previews real submissions nahi hain.

## Agar issue aaye

- 404: `index.html` root mein aur Pages source sahi branch/folder par check karein.
- Design missing: `style.css` aur `script.js` same folder mein hon; filenames ki capitalization same rahe.
- Purana design: hard refresh karein aur latest deployment ka status check karein.
- Photos/fonts missing: external Unsplash/Google Fonts access aur internet connection check karein.
- Deployment failed: repository Actions tab mein failed Pages run ki details dekhein.

## Future updates

Changed files same names ke saath upload aur commit karein. Configured publishing branch par updates Pages deployment trigger karte hain.

Real patient bookings start karne se pehle verified clinic details aur secure booking backend connect karna zaroori hai.
