# Kinerix Legal Documents

Public hosting for Kinerix legal documents (NextRep Athletics Technologies LLC).

**These pages are a rendered mirror.** The source of truth is the `cfg_legal_surface_copy`
table in the Kinerix backend (published surfaces only, `is_active = true`), rendered by the
`legal-docs` edge function. This mirror exists because the shared `supabase.co` domain
rewrites HTML responses to `text/plain`; store listings need a URL that renders.

| Page | Source surface |
|---|---|
| `privacy.html` | `LEGAL-PRIVACY-BODY` |
| `terms.html` | `LEGAL-TERMS-BODY` |
| `delete.html` | `LEGAL-DELETE-BODY` |

**Do not edit the HTML here by hand.** When counsel copy changes in `cfg_legal_surface_copy`,
regenerate by re-fetching the edge-function routes and commit the refreshed files.
