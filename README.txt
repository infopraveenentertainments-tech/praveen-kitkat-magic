PRAVEEN KITKAT DYNAMIC WEBSITE

Files:
- public/index.html  = public website
- public/admin.html  = Supabase admin dashboard
- wrangler.jsonc     = Cloudflare Workers Static Assets configuration

IMPORTANT:
1. Upload the CONTENTS of this folder to the root of your GitHub repository (public folder included).
2. In Cloudflare Workers Builds, keep Root directory as /.
3. Build command: None
4. Deploy command: npx wrangler deploy
5. Redeploy.

The website uses the Supabase URL and publishable key already supplied for this project.
Do not put a Supabase service_role/secret key into HTML.

Admin URL after deployment:
https://YOUR-WORKERS-DOMAIN/admin.html
