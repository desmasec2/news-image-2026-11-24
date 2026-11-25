# The World in One Day — Tuesday 24 November 2026

[![make.fun bounty](https://make.fun/badge/news-image-20261124.svg)](https://make.fun/bounty/news-image-20261124)
[![rank](https://make.fun/badge/news-image-20261124/desmasec2/news-image-2026-11-24/rank.svg)](https://make.fun/bounty/news-image-20261124)
[![reward](https://make.fun/badge/news-image-20261124/desmasec2/news-image-2026-11-24/reward.svg)](https://make.fun/bounty/news-image-20261124)

An entry for the make.fun bounty [“Sum up 24 November's world news in one image”](https://make.fun/bounty/news-image-20261124).

## The image

`entry.png` is a one-page front page that sums up **Tuesday, 24 November 2026**
in six stories, chosen for consequence and breadth across regions and fields:

1. **Law** — A Brooklyn jury convicts Huawei on 10 of 12 counts: bank fraud
   over its Iran business and conspiring to steal US trade secrets (Reuters, CNN).
2. **USA** — President Trump awards the Presidential Medal of Freedom to
   former New York mayor Rudy Giuliani at the White House (Reuters, AP).
3. **Trade** — The US readies a new wave of import duties on China, the EU
   and others after a probe into subsidised production and excess capacity (AP).
4. **Pacific** — Solomon Islands signs a treaty naming Australia its primary
   security partner, excluding China (AP).
5. **Asia** — North Korea demands the closure of Switzerland's new diplomatic
   office in Pyongyang and orders its senior diplomat to leave (AP).
6. **Africa** — WHO Ebola responders remain trapped inside an Ituri hospital
   in DR Congo by heavy fighting; the UN pleads for their safe evacuation
   (UN News).

The poster names its day in the masthead, labels every story, and is drawn
entirely with code — no photographs — so every word stays legible.

## How it is made

- `poster.html` is the poster's source: a single HTML page (inline SVG icons,
  no external assets). Rendering it at 1024×1024 produces `entry.png`.
- `entry.png` is the shipped image: a 1024×1024 PNG, well under the 1 MiB cap.
- `main.py` is the entry program (Python 3, standard library only). It checks
  the shipped image against the gate's rules (PNG or JPEG by its first bytes,
  at most 1 MiB) and copies it, byte for byte, to the output directory.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out python3 main.py
# writes out/entry.png, identical to the entry.png in this repository
```

## License

MIT — see `LICENSE`.
