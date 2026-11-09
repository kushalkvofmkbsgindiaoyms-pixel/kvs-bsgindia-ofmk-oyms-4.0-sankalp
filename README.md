# KV Medak BSG Portal — OYMS 4.0 SANKALP

Official digital portal for the Bharat Scouts and Guides unit at PM SHRI Kendriya Vidyalaya, Ordnance Factory Medak, Eddumailaram, Telangana.

## Project status
The repository is being initialized with the application foundation, database schema, and deployment workflow. Configure Supabase before enabling multi-user production use.

## Stack
- React + Vite
- Supabase Auth and PostgreSQL (optional until configured)
- GitHub Pages deployment

## Development
```bash
npm install
npm run dev
```

## Supabase setup
1. Create a Supabase project.
2. Run `supabase/schema.sql` in the SQL editor.
3. Copy `.env.example` to `.env` and set `VITE_SUPABASE_URL` and `VITE_SUPABASE_ANON_KEY`.
4. Invite the first administrator through Supabase Auth, then assign their role in the `profiles` table.

Without Supabase configuration, the app opens in clearly-labelled local preview mode. Local preview data is stored in this browser only and is not shared or suitable for official records.

## Important
Do not enter real student personal information into preview mode. Enable Supabase, review access policies, and test with authorized staff accounts before official deployment.
