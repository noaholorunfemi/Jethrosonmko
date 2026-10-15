D PSALMIST MUSIC MINISTRY WEBSITE — SUPABASE CONNECTED VERSION

FILES
- index.html: updated website and secure Supabase sign-in
- styles.css: website design stylesheet

IMPORTANT
This version connects to the Supabase project you created. The website uses the public publishable key in the browser, which is intended for public website use. Admin changes are restricted by the Supabase Row Level Security policies and the admin user UUID you configured.

BEFORE UPLOADING
1. Keep a backup of the current website files in GitHub.
2. Upload BOTH index.html and styles.css to the same folder in the GitHub repository, replacing the old versions.
3. Keep any other existing assets/files that the website currently uses.
4. Wait for Netlify to finish deploying, then open the live website.

ADMIN LOGIN
1. Open https://jethrosonmko.netlify.app/?admin=1
2. Enter the email address and password of the Supabase Auth user you created.
3. Save content from the admin panel to publish it online.
4. New images/audio uploaded through the admin panel go to the public site-media Storage bucket.

CHECKLIST
- Supabase project URL is configured.
- Supabase publishable key is configured.
- Public read + admin update policy for public.site_content should exist.
- The site-media bucket should be public.
- Storage INSERT/UPDATE/DELETE policies should restrict writing to your admin user UUID.

NOTE ABOUT OLD LOCAL UPLOADS
Files uploaded before this connection was added may still exist only in the old browser's IndexedDB. They do not automatically move to Supabase. Re-upload any old photos or MP3s through the new admin panel. Existing local text edits on the browser that had them should be reviewed and saved to publish them.
