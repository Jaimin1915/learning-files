# Lesson 4: Keeping Characters Consistent

Sources: [Character Reference](https://flick.art/docs/character-reference) · [Extract Frame](https://flick.art/docs/extractframe)

**Why:** if every shot starts from a text description, faces and costumes drift. A **reference sheet** (the same person from 3 angles on one image) attached to every shot keeps them identical.

## Make a sheet from your own clip (best way)
1. **Extract a frame:** select the video → drag the slider to a clear moment → **Image → Extract Frame → This frame** (First / This / Last frame). Pick a sharp frame, not a motion-blurred one.
2. Select the frame and ask the chat:
   ```
   Using the selected image as the exact reference for [name]'s face, costume and art style,
   create a character reference sheet: front view, side view and three-quarter view, full body,
   standing with a calm neutral expression, plain light background, no text or labels.
   Follow Project memory. Use GPT Image 2.5, medium, 1 image. Show me the cost before running.
   ```
3. Cost: **5 credits** (GPT Image 2.5 medium).

**Tip:** ask for a **neutral expression** on the sheet. Emotion (crying, smiling) is added in each scene. My Arjuna frame was crying, so I asked for "calm, not sad".

## Check the sheet against a list
Write the character's must-keep details and tick each one. Example (Arjuna):
- [ ] Hair in a **top bun** with gold ring, in all 3 views
- [ ] Sun emblem on chest armor
- [ ] Red sash, cream dhoti
- [ ] Gandiva bow, white-feathered arrows

## Store and protect it
- Put all sheets in a section named **Characters**, rename each node (e.g. "Arjuna Sheet"), then **lock** the section.
- For a new angle or costume, ask for a new sheet *from the existing sheet*.

## Using sheets in scenes
- Attach the **sheets**, not the original frames (frames can carry watermarks and emotions).
- **Character Reference** action: up to 5 character images + up to 5 scene images.
- Prompt rule: **describe only the change** (scene, pose, light). The person comes from the reference.
- Characters with only 1–2 scenes (e.g. the farmer) don't need a sheet: make scene A, then use scene A as the reference for scene B.
