# ChatWave Admin

Private admin dashboard for managing ChatWave invite codes.

## Site
https://carl7202.github.io/chatwave-admin/

## Deployment
A GitHub Actions workflow at `.github/workflows/pages.yml` deploys the static page whenever `main` is updated. In the repository, open **Settings → Pages** and set **Build and deployment → Source** to **GitHub Actions** if needed.

## Security
- The page contains only the Supabase project URL and publishable key; never put a service-role key in browser code.
- Privileged operations are handled by the `chatwave-admin-invites` Edge Function, which checks the signed-in account ID server-side.
- ChatWave numbers are fictional identifiers and do not support SMS or calls.
