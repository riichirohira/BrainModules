# BrainModules

BrainModules is an interactive browser-based viewer for exploring anatomical
seed-correlation maps in the mouse brain. Move the pointer over the cortical
map to select a seed position; the viewer displays regions with similar
corticocortical or thalamocortical input patterns.

The tool accompanies the anatomical seed-correlation analysis described in:

> Hira R, Townsend LB, Smith IT, Yu C-H, Stirman JN, Yu Y, and Smith SL.
> *Mesoscale functional architecture in medial posterior parietal cortex*.
> eLife Reviewed Preprint, 2025, 14:RP105213.
> [https://doi.org/10.7554/eLife.105213.2](https://doi.org/10.7554/eLife.105213.2)

## Download

Download `BrainModules.zip` from the
[GitHub Releases](../../releases) page. The archive is provided as a Release
asset because its size exceeds GitHub's 100 MB limit for ordinary repository
files.

- Archive size: 170,350,854 bytes (approximately 162.5 MiB)
- SHA-256: `6f459d8510def1ad534d5bd8add31e6d53a1d9aa515fe9096beaa56f73832cc9`

## Included maps

The archive contains four sets of precomputed correlation maps. Each map is
shown from five cortical surface views.

| Directory | Projection source | Approximate cortical depth |
| --- | --- | --- |
| `cc300_5V/` | Corticocortical (CC) | 300 um |
| `cc700_5V/` | Corticocortical (CC) | 700 um |
| `tc300_5V/` | Thalamocortical (TC) | 300 um |
| `tc700_5V/` | Thalamocortical (TC) | 700 um |

The anatomical connectivity data are derived from the
[Allen Mouse Brain Connectivity Atlas](https://connectivity.brain-map.org/projection).
The maps visualize non-negative correlations between the binary anatomical
input pattern at a selected seed and the corresponding patterns at other
locations.

## Run locally

1. Extract `BrainModules.zip`.
2. Open `BrainModules/html/index.html` in a desktop web browser.

Google Chrome on a desktop computer is recommended. Loading can take a moment
because the viewer retrieves a precomputed image for every selected seed.

## Controls

- Move the pointer over the brain map to choose a seed position.
- Select `cc300`, `cc700`, `tc300`, or `tc700` to change the map type.
- Select `Overlay` to make the correlation map partly transparent.
- Select `Correlation` to restore the opaque correlation view.
- Select `brain area` to reset the viewer.

## Interpretation and limitations

- Tracer injection sites in the source atlas are not distributed uniformly.
- Experiments include different cell-type-specific projections.
- Large tracer spreads or injection backflow can distort estimated
  correlations.
- Negative correlations are not visualized.
- Findings should be checked against the corresponding source experiments in
  the Allen atlas.
- The viewer is optimized for desktop use and is not designed for smartphones
  or tablets.

## Original implementation

The original viewer was created by Riichiro Hira and Anji Hira, with
supervision by Spencer L. Smith at the University of California, Santa Barbara.

## License

No software or data license was included in the supplied archive. No permission
beyond the rights granted by the relevant copyright holders and source-data
terms should be assumed. The eLife article is separately distributed under its
own Creative Commons license.

