PRAVEEN KITKAT — DYNAMIC WEBSITE
================================

This version has:
- Dynamic services
- Dynamic gallery uploads
- Dynamic videos (URL based)
- Editable homepage/about content
- Booking enquiries saved in Supabase
- WhatsApp enquiry handoff
- Mobile-friendly admin dashboard
- Supabase email/password authentication

SETUP
1. Create a free Supabase project at https://supabase.com
2. Open SQL Editor and run schema.sql
3. Create one Auth user under Authentication > Users (your email/password).
4. In Project Settings > API, copy Project URL and anon/public key.
5. Open app.js and admin.js and replace:
   PASTE_YOUR_SUPABASE_URL
   PASTE_YOUR_SUPABASE_ANON_KEY
6. Upload the website to Cloudflare Pages or another static host.
7. Open /admin.html to manage the site.

IMPORTANT SECURITY NOTE
The included SQL gives write access to authenticated users because the first version is intended for a single private admin account. Do not create additional Auth users. For a larger team, tighten the RLS policies to an admin role table.

YOUR WHATSAPP
+91 90355 28821

YOUR INSTAGRAM
https://www.instagram.com/mr_magic_pro/

The supplied photos and two videos are included in assets/.
