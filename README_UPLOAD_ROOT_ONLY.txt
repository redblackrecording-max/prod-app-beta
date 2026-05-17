TCG Machines Production Dashboard — GitHub/Azure Upload Package v15

Temporary dashboard passcode: TCG9000

IMPORTANT UPLOAD RULE:
Upload the CONTENTS of this folder to the ROOT of your GitHub repo.
Do not upload the ZIP itself.
Do not put everything inside an extra nested folder.

Your GitHub repo root should show:
- index.html
- config.js
- manifest.json
- service-worker.js
- inventory_value_stream.html
- pretesting_clickable_sop_dashboard.html
- testing_dashboard.html
- shipping_receiving_dashboard.html
- scanner_main_assembly_clickable_sop_dashboard.html
- chassis_clickable_sop_dashboard.html
- SBX_Pre_Testing_SOP_R01.docx
- Shipping_and_Receiving_SOP_R01.pdf

What changed in v15:
- Rebuilt and rechecked the index page from scratch.
- Removed audio from every dashboard button.
- Removed all top-page wording about audio.
- Embedded the logo, cogs, and wizard directly inside index.html so those images cannot disappear if asset folders fail.
- Made the wizard more vibrant and prominent.
- Kept the passcode screen, but the actual dashboard is inside the same index.html and opens after login.
- Included a cache-kill service worker to remove old stale Azure/iPhone caches.

After Azure redeploys, open your site like this:
https://YOUR-AZURE-LINK/?v=15

If your iPhone still shows an old version:
Settings > Safari > Advanced > Website Data > search your azurestaticapps.net site > Delete.
Then reopen the ?v=15 link.

Security note:
The passcode is for preview convenience only. For real sensitive SOP/company data, have IT enable Microsoft/Entra authentication. The optional config example is included as OPTIONAL_staticwebapp.config.example.json, but it is intentionally not active.


Update in this beta:
- Wizard background is now centered as the full background and should no longer appear cut off on mobile.
- All audio has been removed from buttons.
