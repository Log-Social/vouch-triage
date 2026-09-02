# vouch-triage

The weekly review tool for Vouch, served at
<https://log-social.github.io/vouch-triage/>.

One static HTML file, no build step. It signs in against Supabase and reads a
review queue; every row it can reach is behind row-level security and a reviewer
flag on the account, so this page grants nothing on its own.

Source of truth is `triage/index.html` in the private `vouch-weekly` repo — edit
it there and run `./tools/deploy_triage.sh`. Do not edit this copy.
