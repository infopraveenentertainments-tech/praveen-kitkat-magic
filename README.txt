PRAVEEN KITKAT DYNAMIC WEBSITE — BOOK BUTTON FIX V4

This version keeps Supabase dynamic functionality.

The two booking CTAs are now real buttons with an independent click handler:
- Book a Show
- Book a Magic Show

They do NOT depend on Supabase JavaScript or normal anchor navigation.
A tap scrolls directly to the booking section and updates the URL hash to #book.

Deploy:
Build command: None
Deploy command: npx wrangler deploy
Root directory: /

IMPORTANT:
Replace the previous public/index.html with this version and redeploy.
After deployment, open the live URL in a private/incognito tab or clear the
site cache before testing, so the old JavaScript is not being served.
