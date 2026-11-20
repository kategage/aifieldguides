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
Colors follow the CIL palette (no CIL name or logo). Deep green #003A40 is the ink, red #F9423A the accent (text-safe #C42A22 on light), on a warm paper #FBF8F3. Secondary accents: purple #7474C1, teal #00968F, yellow #F0B323, peach #FF8D6D. Faction and camp colors in the guides are data colors and stay separate.

Schibsted Grotesk for headings, Figtree for body. Map motif: folded-map logo mark, map grid, dotted trails, scale bars, and the animated hero map in `assets/map-light.svg` / `assets/map-dark.svg` (it respects reduced motion).

## Analytics
Pages still load the existing GTM container (GTM-KJ48VZZ5). Swap the ID in each page if this site gets its own container.
