# Nyanza Driving School — website starter

A mobile-friendly bilingual (English/Kiswahili) website starter inspired by the general structure and student-portal concept of https://ors.nyotadriving.ac.tz/. It uses original Nyanza branding and does not copy Nyota's logo or private code.

## Included
- Responsive homepage and mobile navigation
- English/Kiswahili text toggle
- Course information, school contact details, WhatsApp/call links
- Student login/registration preview modal
- Starter Supabase schema in `supabase/schema.sql`
- Setup notes for publishing

## Important status
This is a **front-end starter**, not yet a production student portal. The login/registration form is intentionally a preview and does not create accounts or send data anywhere. The admin dashboard, real authentication, database policies, fee/payment management, attendance, examination records, and SMS/WhatsApp notifications must be implemented and tested before real students use the system.

## Run it on a phone
You can preview the site through a static hosting service after uploading these files to GitHub. Open `index.html` locally if your phone/browser supports it, or publish with GitHub Pages/Netlify after reviewing the files.

## Create the GitHub repository on Android
1. Sign in at https://github.com.
2. Open https://github.com/new.
3. Name the repository `nyanza-driving-school`.
4. Choose **Public** only if you are comfortable with the website source being public. Never put secrets or real student records in a public repository.
5. Add a README, then create the repository.
6. Upload the contents of this folder (not the ZIP itself) using the repository's **Add file → Upload files** option, if available in your mobile browser.

## Supabase setup (later step)
1. Open the Supabase project you intend to use.
2. Inspect the existing tables first; do not delete or recreate tables blindly.
3. Review `supabase/schema.sql` before running it. The script creates new tables only if they do not already exist, but it does not migrate existing table structures.
4. Enable Row Level Security (RLS) and review policies before storing real student data.
5. Use only the Supabase **publishable/anon key** in browser code when required. Never expose the `service_role` key or database password in client-side files or a public repository.

## Business details currently used
- Nyanza Driving School
- Mlango Mmoja, Mwanza, Tanzania
- 0784669618 / 0754692618
- English and Kiswahili

The current generated logo mark is a simple letter N placeholder. Replace it with the school's official logo asset when it is available in the project files.
