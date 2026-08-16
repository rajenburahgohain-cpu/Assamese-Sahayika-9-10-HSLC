ASSAMESE SAHAYIKA - COMPLETE ARCHITECTURE

Flow:
GitHub Pages -> Supabase -> Your Content + Online Search + AI + Translation

1. Create Supabase project.
2. Run supabase/schema.sql.
3. Create your private owner account in Supabase Auth.
4. Configure owner-only RLS INSERT/UPDATE/DELETE policies.
5. Deploy Edge Functions:
   ai-answer, translate, online-search
6. Put AI/search/translation secrets ONLY in Supabase Edge Function Secrets.
7. In index.html replace:
   YOUR_SUPABASE_PROJECT_URL
   YOUR_SUPABASE_PUBLISHABLE_OR_ANON_KEY
8. Upload index.html to GitHub Pages.

Important:
- Google result pages should not be scraped directly. Use an approved search API/provider in the Edge Function.
- AI and translation keys must never be put in public HTML.
- UPI intent is included, but automatic payment verification requires a payment gateway + server webhook.
- Add/Edit/Delete must remain owner-only.
