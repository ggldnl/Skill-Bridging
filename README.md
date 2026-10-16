# Learning to Bridge Humanoid Robot Skills

Project page for the master's thesis "Learning to Bridge Humanoid Robot Skills", Sapienza University of Rome, 2026.

A single learned policy, the bridge, takes control between two frozen humanoid skills and brings the robot within a deadline to a state from which the next skill can continue. It is learned from retargeted human motion, without access to the skills it connects.

Related: [Skill Composition for Legged Robot Reinforcement Learning](https://ggldnl.github.io/Skill-Composition/), AIRO 2026 @ AIxIA 2026.

## Media

Videos go in `static/videos`, with these names:

| File | Section |
| --- | --- |
| `soccer.mp4` | Teaser and soccer demo, with the bridge |
| `soccer_direct.mp4` | Soccer demo, with direct switches |
| `walk2jump.mp4` | Walk to jump transition |
| `walk2kick.mp4` | Walk to kick transition |
| `jump2walk.mp4` | Jump to walk transition |
| `sokoban.mp4` | Sokoban demo on the Booster T1 |

A missing video is replaced by the matching thesis figure, with a "Video coming soon" badge. The thesis PDF goes in `static/pdfs/thesis.pdf`.

Encode videos as H.264 MP4 so they play in every browser, for example:

```sh
ffmpeg -i input.mp4 -c:v libx264 -crf 26 -preset slow -pix_fmt yuv420p -movflags +faststart -an output.mp4
```

## Local preview

```sh
python -m http.server 8124
```
