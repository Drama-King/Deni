DENI APP (installable web app / PWA)

Files: index.html, manifest.webmanifest, sw.js, icons/

1. Host the whole folder over HTTPS (required for install + offline).
   Free options: Netlify Drop (drag the folder), GitHub Pages, Cloudflare Pages.
2. Open the link on an Android phone in Chrome -> menu -> "Install app".
   iPhone: Safari -> Share -> "Add to Home Screen".
3. After the first load it works fully offline.

To put it on Google Play: paste your hosted link into pwabuilder.com and
generate the Android package.

Note: data is saved on each device only. Bump CACHE ("deni-v1") in sw.js
whenever you change index.html so users get the update.
