PRAVEEN KITKAT — DYNAMIC WEBSITE

WHAT THIS VERSION DOES
1. Premium responsive website layout.
2. Booking form writes enquiries directly into Supabase.
3. Booking form DOES NOT reload the page.
4. Admin dashboard at /admin.html.
5. Admin can log in, view bookings, update site content and add/delete gallery URLs.
6. Gallery and site content load dynamically from Supabase.
7. Designed for Cloudflare Workers Static Assets.

FILES
- index.html = public website
- admin.html = admin dashboard
- supabase_setup.sql = database setup
- wrangler.jsonc = Cloudflare deployment configuration
- assets/ = put your photos/videos here if you want local files

SUPABASE
Project URL is already configured in the HTML files.
The publishable browser key is also configured. A Supabase publishable/anon key is intended to be used in browser code; never put a service_role/secret key in these files.

ONE-TIME SUPABASE SETUP
1. Supabase Dashboard -> SQL Editor.
2. Create a new query.
3. Open supabase_setup.sql.
4. Copy ALL of it.
5. Paste it into SQL Editor.
6. Run it.
7. Confirm Success.

ADMIN LOGIN
Supabase Dashboard -> Authentication -> Users -> Add user.
Create your own admin email/password.
Then open:
YOUR-SITE-URL/admin.html

CLOUDFLARE
Repository root:
index.html
admin.html
wrangler.jsonc
supabase_setup.sql
assets/

Cloudflare Workers Build settings:
Build command: None
Deploy command: npx wrangler deploy
Root directory: /

IMPORTANT
If you use GitHub Pages, it will not run the wrangler deployment command. Use Cloudflare Workers with the wrangler.jsonc file, or configure your existing Cloudflare project to deploy this repository.

BOOKING FLOW
Visitor fills the form -> Supabase bookings table -> success message on same page.
Nothing redirects/reloads.

GALLERY
For now the admin accepts public image/video URLs. This keeps the first dynamic version reliable. You can later add Supabase Storage uploads.
