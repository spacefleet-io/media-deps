# media-deps

Prebuilt media libraries (ffmpeg, mpv and their dependencies) that SpaceFleet's client apps bundle.

Each release `media-deps-<target>-<version>` holds:

- `media-deps-<target>.tar.gz`: the bundle the apps ship;
- `media-deps-<target>-source.tar.gz`: the complete corresponding source of everything in that bundle,
  with the build recipe and scripts that produced it;
- a `.sha256` file next to each.

The bundles are built from the `sf/*` branches of our forks in this organisation (one repository per library,
upstream history included) by `packages/media-deps` in https://github.com/spacefleet-io/clients, which also
documents how to rebuild them.

## Licence

The bundles contain code under the GPL, LGPL and other licences; each library's own licence files are inside the
bundle and its source archive. Our build tooling is GPL-3.0-only. A bundle built with x264/x265 is GPL as a whole.
