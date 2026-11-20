# aifieldguides.org

Plain-language field guides to the politics of AI, by Kate Gage. Static site on GitHub Pages.

## Pages
- `/` landing page
- `/factions/` The AI Factions: A Political Field Guide
- `/philanthropy/` AI Philanthropy Field Guide
- `/aipoliticalfieldguide/`, `/PhilanthropyFieldGuide/`, `/fieldguide/` redirect old paths to the new ones

## Going live
1. Settings > Pages: deploy from branch `main`, folder `/ (root)`. The `CNAME` file sets the custom domain to aifieldguides.org.
2. At the domain registrar, add DNS:
   - A records for `@`: 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
   - CNAME for `www`: kategage.github.io
3. Once the certificate is issued, tick "Enforce HTTPS" in Settings > Pages.
4. Only after aifieldguides.org loads: copy the files in `_hgi-redirects/` over the matching folders in the Higher-Ground-Institute.github.io repo so the old higherground.institute URLs forward here. Point the aipoliticalfieldguide.org / .com forwards at https://aifieldguides.org/factions/.

`_hgi-redirects/` starts with an underscore, so GitHub Pages does not publish it.

## Brand
Ink #0F1F1A, signal orange #F26B3A (text-safe #B8401A on white), sage #EEF2EC. Archivo for headings, IBM Plex Sans for body, IBM Plex Mono for small labels.

## Analytics
Pages still load the existing GTM container (GTM-KJ48VZZ5). Swap the ID in each page if this site gets its own container.
