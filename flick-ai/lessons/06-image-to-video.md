# Lesson 6: Turning Images into Video

Sources: [Generate Video](https://flick.art/docs/video) · [Choosing a model](https://flick.art/docs/choosing-a-model) · [Where is my generation](https://flick.art/docs/where-is-my-generation)

## Start from the image (important)
**Select the still → Video → Generate Video.** The **Start Frame** fills automatically.

If you click **+ → Generate Video** on the toolbar instead, you get an **empty** node ("Connect image to generate video") and Run stays grey. Fix: drag from the image's **+** connection point to the video node, or delete the empty node and start from the image.

## Settings I used (Free plan)
| Setting | Value |
|---|---|
| Model | **Auto** |
| Ratio | 16:9 |
| Resolution | 720p (default) |
| Duration | 5s |
| End Frame | **empty** (usually) |
| Batch | 1x |
| Cost | **20** |

## Start Frame vs End Frame
- **Start Frame** = where the clip begins. **End Frame** = where it must finish; the model invents the motion between.
- **Leave End Frame empty** for small motion (glow, hair, flags, slow push-in). Using the same image as the end frame cancels camera moves and can freeze the clip.
- **Use End Frame** for a **change**: sitting → standing, far → near. Both frames need the same angle and background, or the result morphs and glitches.
- Risky change? **Tell it with a cut instead**: show "before" (Arjuna collapsed) then "after" (Arjuna standing). Viewers fill in the motion.

## Frame to Video vs Omni Reference
| | Frame to Video ✅ | Omni Reference |
|---|---|---|
| What it does | Animates your **exact** picture | Builds a **new** shot from references |
| Use when | You already approved the still | You don't have the exact picture |

## Motion prompt formula
**What stays still + what moves gently + camera move + safety line**
```
Krishna stays calm and still with his right hand raised, mouth closed, gentle smile.
A soft golden glow slowly pulses behind him, his hair and peacock feather sway gently,
flags wave softly. Very slow camera push-in, no cuts.
His face, crown and costume stay exactly the same.
```

## Tricks that worked
- Picture suggests motion you don't want (galloping horses)? Say "stands still" **twice in different words**.
- "Does not shoot an arrow" when a character is holding a drawn bow.
- **One action per shot** ("turns one page", not "turns pages and writes").
- Hands are hardest: check fingers.
- Do risky shots (crowds, horses) **one at a time**; check before the next.

## Check every clip, especially the LAST second
Video drifts toward the end (Arjuna's bun vanished in the final second).
- [ ] Face, costume, hair same to the last frame
- [ ] Correct count (horses, fingers)
- [ ] Mouth closed if nobody speaks
- [ ] Camera move happened
- [ ] Only a bad last second? **Trim it in the editor** (free) instead of regenerating

## Waiting
Video can take minutes. Watch the node status: pending → processing → done. Only **failed** means retry (once). **Never delete a node that's still processing**: you're still charged.
