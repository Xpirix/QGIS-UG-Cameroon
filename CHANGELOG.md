# Changelog

All notable changes to this site are recorded here.

The format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project uses [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.1.0] - 2026-09-23

Ports the content work from
[michaekong/QGIS-CAMEROUN](https://github.com/michaekong/QGIS-CAMEROUN) into
this repository, keeping the original commit history and authorship.

### Added

- Cameroon branding artwork: the association ecusson, the site icon, the tile
  icon and the `topo.png` blog hero.
- An about us page introducing the executive bureau and the community.
- An internal regulations page setting out the association rules, served at
  `/rules/`.
- A team photograph on the about us page.
- Events listings with dates and times.

### Changed

- Homepage title, subtitle, hero logo and mission copy now speak for the
  Cameroon user group.
- Brand palette moves to the Cameroon flag colours, keeping the official QGIS
  green as the secondary colour.
- The navigation bar uses the Cameroon location prefix and logo, and reads the
  local `static/config/navigation.json`.
- The footer logo is the Cameroon ecusson.
- The "edit this page" and issue links point at this repository on `main`.

### Removed

- `content/about.md` and `content/rules.md`, which duplicated the pages above
  and collided with them on their Hugo `url` values.

### Notes

Four changes from the source repository were deliberately left behind. Its
`flake.lock` was older than ours, its `README.md` edit pointed readers inside
the theme submodule, its Playwright config replaced the staging URL with a
placeholder, and its SVG edits repainted the official QGIS wordmark. The
committed build output (`public/`, `public_dev/`, `resources/`) was also
dropped, and the theme stays a submodule rather than vendored files.

## [1.0.0] - 2026-09-23

### Added

- Initial site from the QGIS user group website template.
