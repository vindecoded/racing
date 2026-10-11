# Third-party components

VINDecoded Rush uses these open-source components. License texts are included
beside this file and copied into the static build.

| Component | Usage | License |
|---|---|---|
| [Three.js](https://github.com/mrdoob/three.js) 0.180.0 | Renderer/loaders, Reflector ocean reflection, geometry batching; vehicle example informs the adapted Rapier lab setup | [MIT](three-MIT.txt) |
| [Rapier](https://github.com/dimforge/rapier) / `@dimforge/rapier3d-compat` 0.21.0 | Shared race vehicle contacts; Free drive rigid-body and raycast vehicle simulation | [Apache 2.0](rapier-Apache-2.0.txt) |
| [Meshoptimizer](https://github.com/zeux/meshoptimizer) | Three.js bundled 0.22 decoder; 1.3.0 build-time encoder | [MIT](meshoptimizer-MIT.txt) |
| [glTF Transform](https://github.com/donmccurdy/glTF-Transform) 4.5.1 | Offline car asset optimization | [MIT](gltf-transform-MIT.txt) |

The adapted vehicle implementation is `src/rapier-handling.js`, using our own
controls, tuning, practice geometry, telemetry and car rig. Upstream reference:
https://threejs.org/examples/physics_rapier_vehicle_controller.html

The coastal Poly Haven and Kenney assets are CC0. Their individual sources,
authors, transformations and file hashes are documented in the source checkout
at `pacific-overdrive/docs/coast-assets.md` and accompanying asset manifests.
Additional Kenney villas, shops, cars and Blender-posed cheering spectators are
documented in `pacific-overdrive/docs/district-assets.md`; their original CC0
license files and provenance manifest accompany `assets/districts/`.
The beach umbrellas and folding chairs are CC0 derivatives of 3D Assets'
[Beach Surf and Paddle Kit](https://3dassets.dev/packs/beach-surf-and-paddle-kit),
which discloses AI-assisted source geometry. Source URLs, hashes and the CC0
legal text accompany `assets/beach/`; the reproduction workflow is documented
in `pacific-overdrive/docs/beach-assets.md`.
The Kestrel GT is an original fictional vehicle; it is not a licensed car model.
The five rival cars (Haze, Apex, Reef, Cinder, Ghost), their liveries and race
numbers are original procedural designs in the Kestrel house style.

## Traffic cars and wreck debris (CC0 1.0)

Civilian traffic (sedan, SUV, van, taxi, delivery van, pickup, luxury SUV) and
the wreck debris pieces are CC0 1.0 derivatives of Kenney's
[Car Kit 3.1](https://kenney.nl/assets/car-kit) (www.kenney.nl), the same pinned
archive recorded in `assets/districts/manifest.json`. Wheels are kept separate,
the palette is baked to vertex colours and the body paint is retinted at
runtime. `assets/traffic/manifest.json` and `assets/traffic/PROVENANCE.md`
record the archive URL and SHA-256, each source file's SHA-256 and each
derivative's SHA-256; the original licence is `assets/traffic/LICENSE-car.txt`.

## Sound and music (CC0 1.0)

All recorded sound and music is CC0 1.0 (public domain dedication; attribution
not required, given here with thanks). Files are re-encoded MP3 derivatives in
`assets/audio/`; `assets/audio/manifest.json` records each source URL, author,
SHA-256 of the original and of the derivative, and the exact excerpt used. The
CC0 legal text is `assets/audio/CC0-1.0.txt`. The engine, wind, tyre hiss,
scrape and UI tones are synthesized at runtime.

| Sound | Source | Author | License |
|---|---|---|---|
| Surf bed (seamless loop) | [Sea: Waves S0266](https://bigsoundbank.com/sea-waves-s0266.html) | Joseph SARDIN, BigSoundBank.com | CC0 1.0 |
| Gull calls | [Gulls on the Harbor S2573](https://bigsoundbank.com/gulls-on-the-harbor-s2573.html) | Joseph SARDIN, BigSoundBank.com | CC0 1.0 |
| Tyre squeal loop | [Tire squeal S0500](https://bigsoundbank.com/tire-squeal-s0500.html) | Joseph SARDIN, BigSoundBank.com | CC0 1.0 |
| Crowd cheer | [Applause: 600 People S0021](https://bigsoundbank.com/applause-600-people-s0021.html) + [Shouts and Applauses of Teens #1 S0236](https://bigsoundbank.com/shouts-and-applauses-of-teens-1-s0236.html) | Joseph SARDIN, BigSoundBank.com | CC0 1.0 |
| Impacts, crunches, landings | [Impact Sounds](https://kenney.nl/assets/impact-sounds) | Kenney (www.kenney.nl) | CC0 1.0 |
| Menu and HUD clicks/chimes | [Interface Sounds](https://kenney.nl/assets/interface-sounds) | Kenney (www.kenney.nl) | CC0 1.0 |
| Race music | [Virtual Rush](https://opengameart.org/content/virtual-rush) (loop version; not the CC-BY "remixed" derivative) | vitalezzz | CC0 1.0 |
| Menu and results music | [Synth Wave](https://opengameart.org/content/synth-wave) | Pro Sensory | CC0 1.0 |

## Fonts (SIL Open Font License 1.1)

| Font | Usage | License |
|---|---|---|
| [Barlow and Barlow Condensed](https://github.com/jpt/barlow) by The Barlow Project Authors, latin subset via [Fontsource](https://fontsource.org/fonts/barlow-condensed) 5.3.0 | All interface type; self-hosted woff2 in `fonts/` (no runtime font CDN) | [OFL 1.1](../fonts/OFL.txt) |

`fonts/PROVENANCE.json` records each file's source URL and SHA-256;
`scripts/import-fonts.mjs` in the source checkout re-downloads and verifies them.

## Sunset Run course additions (CC0)

| Asset | Usage | License |
|---|---|---|
| [Watercraft Kit 2.1](https://kenney.nl/assets/watercraft-kit) by Kenney | Five offshore boats (sailboats, speedboat, fishing boat, liner) in `assets/watercraft/`; source archive URL, SHA-256 and per-file hashes in its `manifest.json` and `PROVENANCE.md` | CC0 1.0 (`assets/watercraft/License.txt`) |
| [City Kit Suburban 2.0](https://kenney.nl/assets/city-kit-suburban) / [City Kit Commercial 2.1](https://kenney.nl/assets/city-kit-commercial) by Kenney | Two more villas, a shop, a street planter and two cafe parasols (canopies recoloured) in `assets/districts/` | CC0 1.0 (`assets/districts/LICENSE-*.txt`) |
