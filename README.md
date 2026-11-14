# Goal UI screenshots for PR #323

Captured from commit `fdfb711f24328512c1f9e689fca5ce5e7e0bcf2a` with BrowserOS Neo.

These are original, unmodified application screenshots, not mockups. The app ran with its own temporary data and the local `faux-1` scripted provider. No production conversations, account credentials, or real provider calls appear in this set. The token figures are demo usage, not a performance or cost benchmark.

## Suggested PR captions

### Desktop: active loop

The objective stays visible above the composer. The first evaluation requested more work, and the same run continued automatically. Pause remains available.

![Desktop: active Goal loop](01-desktop-goal-active.png)

### Desktop: verified completion

The Goal reaches Completed after 2 evaluated turns. The latest result names the concrete verification evidence.

![Desktop: completed Goal after 2 evaluated turns](02-desktop-goal-completed.png)

### Mobile: persistent Goal bar

The objective and loop state remain visible above the message box. Resume is available for a blocked goal.

![Mobile: persistent Goal bar](03-mobile-goal-bar.png)

### Mobile: Goal controls

The sheet shows the objective, state, evaluated turns, active time, tokens, and latest result. Resume, Edit, a summary draft in PiP, settings, and Delete are available together.

![Mobile: Goal controls](04-mobile-goal-controls.png)

### Mobile: editing

The objective can be edited without replacing the conversation. This form was filled through the real UI, then saved successfully.

![Mobile: edit the objective](05-mobile-goal-edit.png)

### Desktop: deletion confirmation

Deletion asks for confirmation. The message explains that the conversation and current work stay intact. This capture stops before confirmation.

![Desktop: confirm goal deletion](06-desktop-goal-delete.png)

## Evidence and limits

- Desktop viewports: **1440 × 1000** CSS pixels, device scale 1.
- Mobile viewports: **390 × 844** CSS pixels, device scale 1.
- The loop fixture used real `write` and `read` tools in a temporary folder.
- First evaluation: `continue`; only a draft existed.
- Second evaluation: `met`; the final file contained `GOAL_PR_PROOF_OK` followed by a newline, with a read-tool result.
- The second work turn was held briefly to capture its Active state, then released. The app's UI and continuation policy were not changed for these captures.
- `loop-evidence.json` records both scripted verdicts and the exact verified contents.
- `release-readiness.txt` is the verified demo output.
- The mobile fixture exercised resume, pause, edit/save, and deletion confirmation through the UI.
- BrowserOS reported no console errors or warnings after the capture flow.
- `manifest.json` records image dimensions, byte sizes, timestamps, and SHA-256 hashes.
- `contact-sheet.png` is a scaled overview only; use the 6 original PNGs for review or upload.

The source code was not changed for this screenshot task. Nothing was pushed or uploaded to GitHub. Upload the PNGs to the PR and use the captions above; replace the relative image links with GitHub's attachment links.
