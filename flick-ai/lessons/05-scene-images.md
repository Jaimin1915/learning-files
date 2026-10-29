# Lesson 5: Generating Scene Images

Sources: [Generate Image](https://flick.art/docs/generate-image) · [Your first three-shot film](https://flick.art/docs/your-first-three-shot-film)

## Order matters
1. **Establishing shot first** (the location). It decides what the place looks like, then becomes the **location reference** for every other shot there.
2. Then the other shots in that location.
3. Then other locations.

## How to make one image
- **+ → Generate Image**, or select reference nodes and ask the chat.
- Model: **Nano Banana Pro** or **GPT Image 2.5** (I used GPT Image 2.5 medium: 5 credits).
- `@` references another asset; **1x** = how many images.

## My scene prompt template
```
Scene [N] still. Use [Character Sheet(s)] for the exact characters.
Use [location still] ONLY for the [chariot / battlefield / background] and art style,
not for the pose or expression.
[Shot size + angle]: [subject] [action/pose], [setting], [lighting], [mood].
[What to avoid].
Follow Project memory. 16:9. Use GPT Image 2.5, medium, 1 image. Show me the cost before running.
```

## Tricks that worked
| Trick | Why |
|---|---|
| "Use X **ONLY** for the background" | Stops the AI copying a pose or crying face from the reference |
| "Keep empty space on the right for text" | Leaves room for on-screen verse/captions later |
| "Eyes open" when the scene needs eyes to close | The video model needs something left to animate |
| "Facing the viewer" vs "facing Arjuna" | Makes the ending feel different from a similar mid-film shot |
| Distinctive details (orange turban, mustache) | Lets you check a character without a sheet is the same in the next shot |
| "Not a storm: no lightning, not scary" | Keeps the mood your brief asked for |
| Small storytelling props (phone face-down) | Shows change without words |

## Prompt basics (from the docs)
- Subject first, then setting, then framing.
- Style comes from the project's pinned style. Don't add style words in the prompt.
- Compare a small batch from a clear prompt, then make one focused change.

## Review every image
- [ ] Characters match their sheets
- [ ] Correct count of things (e.g. exactly 4 horses)
- [ ] Framing as asked
- [ ] Same style as the other shots
- [ ] No extra limbs, no unwanted text
- [ ] Zoom out (Ctrl+scroll) and judge it **in sequence** with the other shots, not alone

**Failed one check?** Don't regenerate straight away. Name the problem; often a small edit or the editor fixes it for less.
