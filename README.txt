PERMISSIONGUARD - PROJECT FOLDER (MITSAI)
=========================================

WHAT IS IN THIS FOLDER
  index.html           The working demo. This is the whole website (one file).
  scenarios.csv        The 6 study scenarios + 1 extra demo. Opens in Excel.
  docs/                The proposal as PDF (3 pages = the one to submit,
                       and the long 13-page version for your own notes).
  extras/              A small script that builds the 3-page PDF (optional).

HOW TO OPEN THE DEMO (2 steps)
  1. Double-click index.html.
  2. It opens in your browser. Pick a scenario on the left. The phone shows the card.
  No install. No internet is needed (the nice font needs internet,
  but without it the page still works with a plain font).

HOW TO PRESENT THE DEMO (suggested order, about 3 minutes)
  1. Click "Regular Android pop-up". Pick S1. Say: "Two lines, two buttons, no reason."
  2. Click "PermissionGuard". Same scenario S1. Say: "It senses the request, decides
     how strongly to interrupt, and shows one reason."
  3. Click Why? to show the three checks.
  4. Pick S2 (maps): small green bar. Say: "Normal requests stay quiet."
  5. Pick the extra Puzzle Quest scenario: orange. Say: "Three levels."
  6. Tick "Study mode" and pick S5. Say: "This rating is wrong on purpose.
     We test if people follow it without thinking."

HOW TO CHANGE THINGS (open index.html in a free editor like VS Code or Notepad)
  Colors ........ top of the file, the list after ":root{"
  Scenarios ..... search for "var SC=" (one block per scenario)
  Rating rules .. search for "function concerns" (adds up the 3 checks)
  Card words .... search for "function screenHtml"
  After each change: save the file, then press refresh in the browser.

HOW TO PUT IT ON THE INTERNET (free, optional)
  Netlify Drop: go to app.netlify.com/drop and drag this folder in.
  You get a link you can open on any phone.

ABOUT NEXT.JS
  You do NOT need Next.js. This project has no server, no accounts, no database.
  One HTML file is easier and safer for a demo. Use Next.js only if your
  instructor asks for it.

HOW THE RATING WORKS (simple)
  Three checks, one concern point each:
    1. Is this permission NOT normal for this type of app?
    2. Does the app's own Data safety label NOT list this data?
    3. Does the app get access ALL THE TIME (background)?
  0 points = Quiet (green). 1 point = Gentle pause (orange). 2 or 3 = Full stop (red).
  The user always decides. The card never changes a permission by itself.

NOTE
  The ratings are prepared by us with simple rules. The prototype is not
  connected to a real phone. Say this clearly in your presentation.
