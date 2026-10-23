# No Way Home

A 3D lane runner set in Bengaluru traffic. One static page: `index.html`.

## Deploy to Vercel

### Option A: Vercel CLI (fastest)
1. Install Node.js 18 or newer.
2. In this folder, run:
   ```
   npx vercel
   ```
   Log in when asked, accept the defaults (no build command, output directory `.`).
3. For the production URL, run:
   ```
   npx vercel --prod
   ```

### Option B: GitHub
1. Push this folder to a new GitHub repository.
2. In Vercel, choose **Add New → Project**, import the repository.
3. Framework preset: **Other**. Leave build command and output directory empty. Click **Deploy**.

Every push to the main branch then redeploys automatically.

## Test locally
```
npx serve .
```
Then open the address it prints.

## Notes
- Progress is saved in the browser (localStorage), per device.
- Preview a time of day by adding `#tHHMM` to the URL, for example `/#t2130` for 9:30 pm IST.
- three.js and fonts load from cdnjs and Google Fonts, so the page needs internet access.
