Synk Landing (single-file) — Netlify Drop ready

HOW TO DEPLOY (no coding):
1) Go to https://app.netlify.com/drop
2) Drag-and-drop the *folder* containing this index.html, or zip and drop it.
3) Netlify gives you a live URL instantly.

HOW TO TURN THE DUMMY FORM INTO A REAL NETLIFY FORM (later):
- Replace the <form> tag with the version below and REMOVE the JS submit handler.

Current (demo):
<form id="waitlistForm" class="..."> ... </form>

Netlify Forms (real submissions):
<form name="waitlist" method="POST" data-netlify="true" class="...">
  <input type="email" name="email" required class="...">
  <input type="hidden" name="form-name" value="waitlist">
  <button>Join Waitlist</button>
</form>

Notes:
- After deploying with data-netlify="true", form submissions will appear in your Netlify dashboard under Forms.
- You can also add a thank-you page by adding: action="/thanks.html" (create that file).

CUSTOMIZE:
- Edit text directly in index.html.
- Update team names in the TEAM section.
- Change pricing numbers or plan names as needed.
- Colors: gradient uses Tailwind; adjust in CSS vars at top (grad1/grad2).

Made to cover: hero, story, social proof, visual (AI advantage), pricing, conversion path, team.
