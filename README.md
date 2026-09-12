# hubandcircles-data

Source data for **Napa ja piirit / Hub & Circles** – cycling routes around Rovaniemi, Finland.
This repository is edited with [hubandcircles-manager](https://github.com/mtpajula/hubandcircles-manager)
and published as a static site by the same tool; the site itself lives in
[hubandcircles-site](https://github.com/mtpajula/hubandcircles-site).

Layout (ARKKITEHTUURI.md chapters 5–6 of the manager repo):

| Path | What |
|---|---|
| `project.json` | Project settings: name, area, languages, themes default, feedback repo |
| `publish.json` | Frontend version, publish targets, cache header rules |
| `themes/*.json` | Theme cards (winter, mtb, gravel, road, touring) |
| `routes/<id>/` | Route card `route.json`, `track.gpx`, `media/` |
| `services/` | Service points: imported snapshots and manual corrections |
| `sources/` | Snapshots of external registers (Lipas) written by the import commands |

Routes imported from the Finnish sports facility register [Lipas](https://www.lipas.fi/) carry
`lipas_id` and `maintainer: "municipal"`. Route texts are Finnish (`fi`) and English (`en`).

Report a route problem by opening an issue in this repository.

## License

Code and data in this repository: MIT (see `LICENSE`). Route geometries imported from Lipas:
© Jyväskylän yliopisto / Lipas, CC BY 4.0.
