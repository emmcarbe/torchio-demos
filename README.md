# Torchio: demonstration editions

The editions pressed with [Torchio](https://github.com/emmcarbe/torchio),
kept apart from the engine so that materials with limited rights can be
added and removed without touching it.

Demonstration editions generated with Torchio from the sources in
`sources/`. To regenerate, for example:

```sh
node ../torchio/tools/press.js --site sources/odissea odissea
node ../torchio/tools/press.js --site sources/vangogh vangogh
node ../torchio/tools/press.js --site sources/odd-contract odd-contract
```

Run the commands from this repository with the `torchio` repository checked
out beside it. Directory input is intentional: it includes the manifest and
only the source files and sidecars actually consumed by the press.

## Materials and rights

- **ODD contract** (`sources/odd-contract/`): a synthetic CC0 document and
  customization that make the processing cascade inspectable. Custom elements
  receive exact processing from the edition ODD; ordinary TEI elements use the
  conservative TEI All fallback contracts. It is a test, not an edition of a
  historical source.

- **Odyssey** (`sources/odissea/`): Homer, *Odyssey*, Greek text from the
  [Perseus Digital Library](https://github.com/PerseusDL/canonical-greekLit)
  (`tlg0012.tlg002.perseus-grc2`), CC BY-SA 4.0. The derived demo is
  distributed under the same licence.
- **Van Gogh letters** (`sources/vangogh/`): 30 letters from
  [Vincent van Gogh, The Letters](https://vangoghletters.org/) (Van Gogh
  Museum and Huygens ING, ed. Leo Jansen, Hans Luijten and Nienke Bakker),
  TEI files from the [eeditiones/vangogh](https://github.com/eeditiones/vangogh)
  repository, CC BY-NC-SA 4.0. The derived demo is distributed under the
  same licence, for non-commercial use only.
- **Bellum Alexandrinum** (`sources/bellum/`): critical edition by Cynthia
  Damon et al., [Digital Latin Library](https://github.com/digitallatin/caesar-balex),
  CC BY-SA 4.0; the files are declared by their authors a beta version
  pending peer review by the Society for Classical Studies. Temporary test
  sample. The derived demo is distributed under the same licence (CC BY-SA
  4.0).
- **Romualdus Salernitanus, Chronicon** (`sources/romualdo/`): digital
  scholarly edition by Paolo Monella, ALIM Project, from the
  [paolomonella/romualdus](https://github.com/paolomonella/romualdus)
  repository, GPL 3.0. Offered by the editor as a test case. The derived
  demo is distributed under the same licence.
- **Ursus Beneventanus, Adbreviatio artis grammaticae** (`sources/orso/`):
  digital scholarly edition (section *De nomine*, Codex Casanatensis 1086)
  by Paolo Monella, ALIM Project, from the
  [paolomonella/ursus](https://github.com/paolomonella/ursus) repository,
  GPL 2.0. Offered by the editor as a test case. The derived demo is
  distributed under the same licence.
- **The Book of the Tales of Canterbury: the General Prologue** (`sources/canterbury/`):
  transcripts of all 54 witnesses and the full collation from the
  [Canterbury Tales Project](https://talesofcanterbury.org/GP/), ed. Barbara Bordalejo and Peter
  Robinson. Materials under copyright; pressed and republished here by
  invitation of the editor as a test case. This is a temporary demo and it
  will be removed.
- **Frankenstein, Volume III** (`sources/frankenstein/`): the
  [Shelley-Godwin Archive](https://shelleygodwinarchive.org/) transcription of
  Bodleian MS. Abinger c.56, CC0. A genetic edition: Mary Shelley's hand and
  her campaigns of correction, followed through the `handShift` declarations.
- **Specimen** (`sources/specimen/`): a micro-edition constructed for
  demonstration purposes (imaginary witnesses, didactic variants, declared
  as such on the title page); base text: the opening of the Odyssey in
  Ippolito Pindemonte's translation (public domain); CC0 encoding.
- Geographic lookups use data derived from
  [GeoNames](https://www.geonames.org/) (CC BY 4.0); map coastlines from
  [Natural Earth](https://www.naturalearthdata.com/) (public domain). The
  map page uses [Leaflet](https://leafletjs.com/) (BSD-2, bundled) and tiles
  © OpenStreetMap contributors (ODbL), loaded from the OSM servers when the
  page is viewed.

Torchio's code remains MIT; the licences above concern the contents of the
demos.
