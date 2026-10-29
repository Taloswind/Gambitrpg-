GambitRPG website and how-to-play video
=======================================

What's in this folder
---------------------
website/        The new GambitRPG website. Open website/index.html in any
                browser to see it on your computer.
  index.html    The whole page: text, layout and styles.
  art/          Logo, character art, photos, review thumbnails and the
                how-to-play video that plays on the page.
  cards/        Every card in the base deck (all 52, both jokers and the
                card back) as images. The page uses 12 of them; the rest are
                there if you want them.
video/          The how-to-play video on its own (3:46, 720p, with
                voiceover and music). Good for YouTube, Instagram or Facebook.
video-script.txt  Every narration line, in order.


Putting the website online
--------------------------
gambitrpg.com currently points to a Google Sites page. Google Sites can't
host a custom page like this one, so it needs a regular web host. The
easiest free option:

  1. Go to https://app.netlify.com/drop
  2. Drag the whole "website" folder onto the page.
  3. Netlify gives you a working link in a few seconds.
  4. Make a free account to keep it, then use "Domain settings" to point
     gambitrpg.com at it. Netlify walks you through it, and you'd change the
     domain's settings wherever you bought the domain.

Other free hosts that work the same way: Cloudflare Pages, GitHub Pages.

Keep the folder structure as it is. The page looks for files in art/ and
cards/ next to index.html.


Changing things later
---------------------
Open index.html in a plain text editor (Notepad works; VS Code is nicer).

- Shop items (free modules, coming-soon products): search for
  "const PRODUCTS". Each line is one product. To start selling a PDF, change
  type:"soon" to type:"paid", add price:9 (or whatever) and a url:"..." link
  to wherever it's sold (itch.io, DriveThruRPG, Gumroad and so on).
- Stores: search for "const RETAILERS". One line per store: name, a short
  note, and a link.
- Any other words on the page: search for them and type over them.

Save the file, then drag the website folder onto Netlify again to update the
live site.


A few things to double-check
----------------------------
- Captions in the "At the table" photo section were written from the
  pictures. Check that they describe Anna and the other photos correctly.
- The "Coming soon" products and expansion names came from the Kickstarter
  page. Remove any that aren't planned anymore.
- The page uses Google Fonts, so it needs an internet connection to show the
  intended typefaces.
