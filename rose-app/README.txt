HER LITTLE ROSE  -  installable app package (version v2)
==========================================================

WHAT IS IN THIS FOLDER
  index.html            the game
  manifest.webmanifest  makes it installable (name, colors, icons)
  sw.js                 offline copy + update checker
  icon-*.png            app icons

STEP 1 - PUT IT ONLINE (once, free, about 5 minutes)
  Option A (easiest): Netlify Drop
    1. Go to https://app.netlify.com/drop and sign in (free account).
    2. Drag this whole folder onto the page.
    3. You get a link like https://something.netlify.app  (you can rename it in Site settings).
  Option B: GitHub Pages
    1. Create a free GitHub account and a new public repository.
    2. Upload all the files in this folder to it.
    3. Settings > Pages > deploy from the main branch.
       Link: https://YOURNAME.github.io/REPOSITORY/
  (The screens of these websites change now and then, so the wording may differ a little.)

STEP 2 - SEND HER THE LINK
  Android (Chrome): she opens the link and taps "Install" (a small bar appears), or menu > Install app.
  iPhone (Safari):  she opens the link, taps the Share button, then "Add to Home Screen".
  After that the game is an icon on her home screen, opens full screen, and works offline.

HOW UPDATES WORK
  Every time you change the game, ask Claude for a new package (the version number inside sw.js goes up).
  1. Upload the new folder to the same place (Netlify: Deploys > drag the folder again).
  2. When she opens the app with internet, a pink bar says "فيه تحديث جديد للعبة!" - she taps "حدّثي" and she has the new version.
  Her progress (coins, roses, streak, decor...) stays - updates never erase it.

IMPORTANT
  * Her progress is saved on her phone for this exact web address. Keep the SAME address forever;
    if the address changes she starts from zero.
  * Progress from the claude.ai link does NOT move into the app (different storage place).
    Send her only ONE of the two so she does not play in two places.
  * On iPhone, install it to the home screen - then the phone keeps its saved data safely.

IF THE PAGE KEEPS SPINNING / STAYS BLANK
  1. In Netlify open your site > Deploys: the latest deploy must say "Published". Wait 1-2 minutes after a new site is created.
  2. Make sure you dragged the FOLDER (the one that directly contains index.html), not the .zip and not a folder that contains another folder.
     On the live site, https://YOURSITE.netlify.app/manifest.webmanifest should open and show text. If it says "Page not found", the files are in a sub-folder.
  3. Try the link on a phone using mobile data. If it opens there, your Wi-Fi/school network is blocking or slowing the new address.
  4. Try a private/incognito window, or press Ctrl+Shift+R to hard-reload.
