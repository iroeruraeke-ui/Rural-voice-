# Rural Voice website starter

Responsive HTML website package for Rural Voice — Giving Rural Communities a Voice.

## Files
- `index.html`: homepage
- `about.html`, `latest.html`, `article.html`, `category.html`
- `contact.html`, `submit-story.html`, `privacy.html`
- `admin.html`: starter administrator sign-in page
- `assets/style.css`: responsive design
- `js/config.js`: Supabase connection placeholders
- `js/site.js`: starter Supabase integration

## Before deployment
1. Extract this ZIP on your phone.
2. Upload the **contents** (not just the ZIP) into the root of your GitHub `rural-voice` repository.
3. In `js/config.js`, replace the placeholder values with your Supabase Project URL and **public anon/publishable key**.
4. Never put a Supabase `service_role` or secret key in browser files.
5. Deploy the repository root on Vercel as a static site; no build command is required.

## Important limitations
The public article listing expects `public.articles` to have `title`, `slug`, `content`, `category`, `status`, and `created_at` columns. It also optionally reads `excerpt`. Confirm the real column names in Supabase.
The admin page checks `profiles.role = 'admin'` after sign-in, but publishing, editing, moderation, spam protection and full security policies still need implementation and testing. The story submission form is not enabled yet. Do not treat this starter as a production-ready CMS until these are completed.
