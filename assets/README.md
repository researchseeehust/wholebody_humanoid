# Project page assets

`docs/index.html` expects these files. Until they exist, the page shows placeholders.
Replace each placeholder `<div class="ph">...</div>` in `index.html` with the commented
`<video>` line (see the teaser block for the pattern).

| File | Content |
|---|---|
| `paper.pdf` | Paper |
| `teaser.mp4`, `teaser.jpg` | Teaser video and poster frame (16:9) |
| `walk_forward.mp4` | Forward walking |
| `walk_lateral.mp4` | Lateral walking |
| `walk_turn.mp4` | Turning in place |
| `push_srb.mp4` | Push, SRB-MPC + WBC baseline |
| `push_ours.mp4` | Same push, WB-MPC + WBC |

Encode with H.264 for browser support, e.g.
`ffmpeg -i in.mp4 -c:v libx264 -crf 23 -pix_fmt yuv420p -an -movflags +faststart out.mp4`.

Also replace every element with `class="tbd"`, the `OWNER` placeholder in GitHub links,
the arXiv link, authors, and affiliations.
