# 4slab — public pages

Served by GitHub Pages at https://4slabsapps-ship-it.github.io/. One folder per app, holding
the pages the stores and the apps link to.

- `landfold/privacy.html` — Landfold privacy policy and support page. The source is
  `docs/privacy.html` in the private Landfold repository; edit it there and copy it here. The app
  opens this exact URL (`PRIVACY_POLICY_URL` in `AboutSheet.kt`), so the path must not change.
- `tagprice/privacy.html` — TagPrice privacy policy and support page. The source is
  `docs/privacy.html` in the private TagPrice repository; edit it there and copy it here. The app
  opens this exact URL (`PRIVACY_POLICY_URL` in `DataScreen.kt`), so the path must not change.
- `tagprice/taxpack.manifest.json` — what the app's daily tax-data check reads
  (`TaxPackUpdater.DEFAULT_BASE_URL`). It names the pack the app already bundles, so the check
  answers "up to date" and downloads nothing; new rates ship with new app versions. It never needs
  editing: an app with a newer bundled pack ignores an older manifest. Only when a server publishes
  packs does this file (or the app's address) change.
