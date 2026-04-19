# tesfagrid-web

The research home of the **Tesfa Grid** programme — a geometric framework
for prime numbers, maintained by Tesfaye Dereje from Addis Ababa, Ethiopia.
Deployed at [tesfagrid.io](https://tesfagrid.io).

This site publishes mathematical findings from the programme: proved
theorems, algorithms derived from them, and empirical observations under
investigation. It is the academic face of the work. The commercial
application — cryptographic software for hospitals and HSM vendors —
lives separately at [ethoryx.io](https://ethoryx.io).

## Structure

| File                     | Volume | Purpose                                                     |
|--------------------------|--------|-------------------------------------------------------------|
| `index.html`             | —      | Programme introduction and table of volumes                 |
| `theorem-7.html`         | I      | The mod-6 gap constraint, proved                            |
| `column-class-sieve.html`| II     | Prime-generation algorithm, 75% candidate reduction         |
| `oscillation-law.html`   | III    | Empirical sign-alternation finding (Z = 211)                |
| `publications.html`      | —      | Papers, preprints, BibTeX for each volume                   |
| `team.html`              | —      | Principal investigator bio, future Institute vision         |
| `style.css`              | —      | Shared academic journal stylesheet                          |
| `tesfagrid-icon.svg`     | —      | Favicon — 6-column grid with prime markers                  |
| `vercel.json`            | —      | Routing config for clean URLs                               |

## Design philosophy

This site is built to feel like a well-made mathematical monograph, not
a tech startup landing page. Cream paper, oxblood accent, EB Garamond
body type, drop caps, typographic ornaments, theorem boxes, and the
Tufte-inspired sidenote convention. The intention is that a serious
reader should feel at home — and a casual visitor should understand
immediately that this is a place for mathematics, not marketing.

## Deployment

This repository is deployed on Vercel. Every push to `main` triggers
an automatic rebuild.

```bash
# One-time local setup
npm install -g vercel
vercel login

# Manual deploy (not normally needed — CI handles it)
vercel --prod
```

The custom domain `tesfagrid.io` is attached via Vercel project settings.
DNS is managed in Cloudflare, with the root and `www` records pointed at
Vercel's infrastructure.

## Contributing

Corrections, clarifications, and collaboration proposals are welcomed.
The preferred channel is email to **research@ethoryx.io**. For typo-level
fixes, pull requests are also accepted.

## License

All content on this site — text, code, and mathematics — is published
under the [MIT License](LICENSE). You may copy, adapt, or build upon it
with attribution.

## Citation

To cite the programme as a whole:

```bibtex
@misc{tesfagrid2026,
  author       = {Tesfaye Dereje},
  title        = {The Tesfa Grid: a geometric framework for prime numbers},
  year         = {2026},
  howpublished = {\url{https://tesfagrid.io}},
  note         = {Independent research programme, Addis Ababa, Ethiopia}
}
```

Individual volumes have their own BibTeX entries listed on each page.

---

© 2026 Tesfaye Dereje · Addis Ababa, Ethiopia
