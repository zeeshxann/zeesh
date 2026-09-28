# Eco Sync Client Desk

Source of the Eco Sync Client Desk artifact: one self-contained `index.html` (HTML, CSS and JS inline).

- Views: Home, Clients, Money (invoices and quotations), Team, Activity, How we work.
- Data: client records, team, settings and activity live in the artifact's shared database (`window.claude.use("db")`), not in this file. Opened outside claude.ai, the page loads but shows "Live data isn't available".
- Access: the lock screen checks the team code stored in the desk's `settings/access` record. The fallback `DEFAULT_CODE` in the source is a placeholder (`CHANGE_ME`) and is only used if that record is missing.
