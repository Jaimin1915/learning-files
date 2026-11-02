# My Flick Prompt Library

Fill-in-the-blank templates. Replace `[...]`. Each one comes from Flick's docs or a tested workflow. Add your own tested prompts under each section.

---

## 1. Images

### Scene (7 parts)
```
[Subject, one clear subject] [action/pose], [setting].
[Shot size], [angle], [lens]mm lens.
[Light source] from [direction]; [bright areas]; [dark areas].
Focus on [subject part]; [foreground/background] softly out of focus.
[1–2 texture details if the style needs them].
```

### Character turnaround sheet (from "The Duel" workflow)
```
Use the provided character reference as the direct reference.
Create a [live-action studio photograph / 2D character sheet] of [character], shown as a three-view character turnaround on a pure white seamless background.

Layout: three full-body views in one horizontal image: front view, side view, back view. Same scale, same head height, same ground line, even spacing.

Locks:
facial identity 100% match the provided character reference
hairstyle and beard 100% match the provided character reference
outfit design, colors and overall styling 100% match the provided character reference
[key props] 100% match the provided character reference

Lighting and camera: large soft key light from the front, slightly above head height; soft fill from the opposite side. Eye-level camera at chest height, long lens, identical camera distance for all three views.
The image contains only the three figures and their contact shadows on pure white.
```

### Character in a new scene (Character Reference)
```
Keep the facial identity, structure, features and expression from the provided character reference.
Keep the hairstyle, outfit design and colors from the provided character reference.
[Only the change: new pose, new place, new light]. [Framing]. [Light that matches the scene].
```

### Edit an image
```
Edit the provided base image.
Keep the composition, camera position and framing unchanged.
Only change [one thing].
```

### Sketch → finished image
```
Use the provided sketch as the composition reference. composition 100% exactly match the provided sketch. camera position 100% unchanged. framing 100% unchanged. character pose 100% match the provided sketch.
Use the provided face reference for the character identity. facial identity 100% match the provided face reference.
[Light, materials, focus].
```

### Live-action realism add-ons (use 2–4, not all)
`subtle film grain` · `slight sensor noise` · `mild lens softness` · `soft white bloom` · `realistic skin texture, visible pores` · `realistic fabric texture` · `material wear, aged surface, use marks`

### My tested prompts
| Date | Model | Prompt (short) | What worked |
|---|---|---|---|
| | | | |

---

## 2. Video

### Frame to Video: the 3-sentence prompt
```
[Subject] [one action], [pace word: slowly/gently/steadily].
[Camera: "Static camera, locked framing." OR one move: "Slow push in toward her face."]
[What must not change: face, costume, lighting and framing stay the same.]
```

### Continue a clip (Extend Video)
```
[Only what happens next, e.g. "she sets the cup down and looks out of the window"]
```
Do not describe the scene again.

### My tested prompts
| Date | Model | Prompt (short) | What worked |
|---|---|---|---|
| | | | |

---

## 3. Camera moves (one per shot)
| Move | Write it like this |
|---|---|
| Static | `Static camera, locked framing. The camera does not move.` |
| Push in | `Slow push in toward [subject]'s face.` |
| Pull out | `Slow pull out, revealing [what appears].` |
| Pan | `Slow pan from [A] to [B]; the camera stays in place and rotates.` |
| Tilt | `Slow tilt up from [his feet] to [his face].` |
| Track | `The camera moves beside [him] at his walking speed, same distance and eye-level framing throughout.` |
| Lead | `The camera stays in front of them and moves backward at their walking speed.` |
| Orbit | `The camera slowly orbits around [subject], keeping [him] centered.` |
| Crane | `The camera rises slowly from ground level to a high angle above [subject].` |
| Handheld | `Subtle handheld camera, slight natural shake, following [him].` |

---

## 4. Performance (Seedance)
```
Character:
[First visible action]. Then [next action]. Only after [trigger], [reaction].
Camera:
[One camera instruction].
Voice:
He says, "[line]". [Volume], [pace], [pause before "word"], [emphasis]. He does not raise his voice.
```
Write behavior, not emotions: `her eyes stop moving for one beat` instead of `she is sad`.

---

## 5. Omni Reference
```
[Character A]'s appearance matches @Image1 100%. [Character B]'s appearance matches @Image2 100%.
Use @Image3 for the location, layout and lighting.
Use @Video1 only for [camera language and blocking / choreography and timing].
[What happens in this shot, in order].
```
Mention **every** attached reference in the prompt, or it may be ignored.

---

## 6. Action (Seedance Action Guide)
```
[A]'s appearance matches @Image1 100%. [B]'s appearance matches @Image2 100%.
Real-time speed, no slow motion.

[0–2s] Preparation: [weight shift / foot plants / weapon draws back].
[2–4s] Attack: [A closes distance with (exact movement)].
[4–5s] Contact: [where it lands or where the block meets it].
[5–7s] Reaction: [B recoils / slides back / loses balance].
[7–8s] Recovery: [both reset stance].

Camera: [one job, e.g. locked medium-wide shot keeping both bodies and the weapon path visible].
Sound: [breath before exertion], [cloth movement], [impact at contact], [footsteps after].
```

---

## 7. 3D Stage → clip
```
Use @Image1 for the characters' appearance, materials and lighting.
Follow the character action and camera movement in @Video1.
```
(@Image1 = AI-rendered first frame of the 3D recording, @Video1 = the 3D recording)
