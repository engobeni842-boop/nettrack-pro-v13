NetTrack Pro V13.8 Owner Portal + Supabase Live Data Patch

What changed:
- Owner Portal now includes live Supabase-backed dashboard cards.
- Owner email remains protected: engobeni842@gmail.com.
- Login/sign-up now attempts to upsert a row into public.profiles.
- Signal A/B generation now attempts to save generated signals into public.signals and public.signal_history.
- Owner dashboard reads profiles, signals, signal_history, subscriptions and payments counts when RLS allows it.
- If Supabase RLS blocks a write/read, the app keeps working and stores a local fallback event for the owner dashboard.
- Google login button is now guarded so users are told to use email login until Google Provider is enabled in Supabase.

Important:
Supabase Auth users cannot be counted from the public browser client without an admin/service role. Do not put a service role key in frontend code. The Owner Portal therefore shows visible/authenticated user state plus database profile counts.

Recommended Supabase check after deploying:
1. Log in as engobeni842@gmail.com.
2. Open Owner Portal.
3. Click Sync My Profile + Last Signals.
4. Generate Signal A/B.
5. Check Supabase Table Editor: profiles, signals, signal_history.

If tables still stay empty, check RLS policies for insert/select permissions.
