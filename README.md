# ef-diagrams

Mermaid sources and rendered PNGs for Everfit solution-design docs. Confluence cannot render
mermaid, so each diagram is committed as a `.mmd` source plus a `.png` embedded from
`raw.githubusercontent.com`.

One folder per design doc. Diagrams are numbered in the order they appear in that doc.

| Folder | Design doc |
| --- | --- |
| `consultation-document/` | [Solution Design: Multi-Consultation Documents (BE)](https://everfit.atlassian.net/wiki/x/4wKv4w) |

## Rendering

```bash
npx @mermaid-js/mermaid-cli -i <name>.mmd -o <name>.png -b white -s 2
```

Embed in Confluence with the raw URL:
`https://raw.githubusercontent.com/thucvo-everfit/ef-diagrams/main/<folder>/<name>.png`

Edit the `.mmd`, re-render, and commit both files together — the PNG is what Confluence shows.
`d1-system-context.png` and `d4-notification-fanout.png` predate this convention and have no
`.mmd` source yet.
