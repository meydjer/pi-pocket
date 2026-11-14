# Goal UI screenshots for PR #323

These images are embedded in [TannerMidd/pi-pocket#323](https://github.com/TannerMidd/pi-pocket/pull/323).
They are kept on a separate assets branch so that binaries do not enter the PR's code diff.

The original, unmodified PNGs were captured with BrowserOS Neo from UI commit
`fdfb711f24328512c1f9e689fca5ce5e7e0bcf2a`. The demo used temporary data, a scripted
`faux-1` model, and real file write/read tools. No production conversations or account
credentials appear. Usage figures are demo values, not a real-provider benchmark.

| Image | Viewport | Caption |
| --- | --- | --- |
| `01-desktop-goal-active.png` | 1440 × 1000 | The evaluator requests more work and the same run continues automatically. |
| `02-desktop-goal-completed.png` | 1440 × 1000 | The Goal reaches Completed after 2 evaluated turns and real file verification. |
| `03-mobile-goal-bar.png` | 390 × 844 | The objective and state stay above the message box. |
| `04-mobile-goal-controls.png` | 390 × 844 | Pause/resume, edit, usage, summary draft, settings, and delete controls. |
| `05-mobile-goal-edit.png` | 390 × 844 | The objective is edited in the normal sheet. |
| `06-desktop-goal-delete.png` | 1440 × 1000 | Deletion requires confirmation and preserves the conversation and current work. |

`manifest.json` records the original dimensions, capture timestamps, byte sizes, and SHA-256 hashes.
