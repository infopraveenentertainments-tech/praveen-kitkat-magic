PRAVEEN KITKAT — DYNAMIC CLOUDFLARE WEBSITE

This package keeps the public website dynamic through Supabase.

Files:
- public/index.html — dynamic public website
- worker.js — Cloudflare Worker that serves the public assets
- wrangler.jsonc — Cloudflare deployment configuration
- README.txt — upload/deployment instructions

The index.html supplied in this package already:
- Reads About text from Supabase
- Reads the hero image from Supabase
- Reads gallery items from Supabase
- Saves booking enquiries to the bookings table
- Makes Book a Show scroll to the booking form without reloading
- Shows booking success/error status

DEPLOYMENT
1. Put the files/folders in the GitHub repository:
   public/index.html
   worker.js
   wrangler.jsonc

2. In Cloudflare, connect the GitHub repository as a Workers deployment.

3. Build command: None

4. Deploy command:
   npx wrangler deploy

5. Root directory:
   /

Do NOT deploy this as a plain static-only Pages site if you are following the
Worker configuration above. The frontend remains dynamic because it connects
to Supabase from the browser.

SUPABASE SECURITY
The browser uses the Supabase publishable key. That is normal for a frontend.
Protect database operations with Supabase Row Level Security (RLS).
Never place a Supabase service_role/secret key in index.html.

BOOKING FLOW
Visitor -> index.html -> Supabase bookings table -> admin dashboard.

The supplied index.html is the user's uploaded dynamic version; its Supabase
URL/key and dynamic content logic are preserved.
