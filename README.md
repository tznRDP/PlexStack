# KomStack

Personal asset repository for my [Kometa](https://kometa.wiki/) setup.

This repo hosts custom posters, backgrounds, overlays, and metadata files.
Movie and show/season/episode artwork, collection overlays, and related
Kometa config.

## Structure

```
Kometa/
├── Metadata/
│   ├── Poster/
│   │   └── <Show>/
│   │       └── <Season>/      # Poster images, referenced by url_poster
│   ├── Background/
│   │   └── <Show>/
│   │       └── <Season>/      # Background images, referenced by url_background
│   └── <Show>.yml              # Kometa metadata file for that show
└── Overlays/
    └── Networks/
        └── <Network>/          # Overlay assets (e.g. BBC Earth, Netflix)
```

Each show gets its own metadata file under `Kometa/Metadata/`, referencing
images from the matching `Poster/<Show>/<Season>/` and
`Background/<Show>/<Season>/` folders via raw GitHub URLs, e.g.:

```
https://raw.githubusercontent.com/tznRDP/KomStack/main/Kometa/Metadata/Poster/<Show>/<Season>/<file>.png
```

Movies use the same `Poster/`/`Background/` structure without the
`<Season>/` layer.

## Notes

- This is a personal collection assembled for my own library — artwork may
  be sourced from various community sites (e.g. MediUX) or custom-made.
- No warranty, no support — use at your own risk if you're browsing for
  ideas.
- Nothing sensitive lives here; it's image assets and Kometa config only.
