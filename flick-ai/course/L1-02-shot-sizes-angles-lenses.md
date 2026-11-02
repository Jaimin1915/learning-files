# Lesson 1.2: Shot Sizes, Angles and Lenses

Sources: [Image Generation Prompts Guide](https://flick.art/docs/Image-Generation-prompts) · [Camera Control](https://flick.art/docs/camera-control) · [3D Stage cameras](https://flick.art/docs/3D-stage-camera) · [04. Plan shots that cut together](https://flick.art/docs/academy-plan-shots-that-cut-together)

## The idea
Every shot answers three camera questions:
1. **How much do we see?** → shot size
2. **From where do we look?** → angle and camera height
3. **What lens?** → how wide, how deep, how "squashed" the space feels

Each choice **means something** to the viewer. Pick it on purpose, then write it in plain visible words.

---

## 1. Shot sizes (from far to close)
| Shot | Abbrev. | What's in frame | Use it to… | Write it like this |
|---|---|---|---|---|
| Extreme wide | EWS | Tiny figure in a huge place | Show scale, loneliness, "where are we" | `extreme wide shot, the figure is small in the lower third of the frame, the valley fills the image` |
| Wide | WS | Whole body + lots of surroundings | Establish the location and who is where | `wide shot, full body visible with space above the head and below the feet` |
| Full | FS | Head to feet, filling the height | Show costume, stance, body language | `full shot, framed from the top of his head to his feet` |
| Medium-wide (cowboy) | MWS | Head to knees | Standoffs, two people talking, action with room | `medium-wide shot, framed from head to knees` |
| Medium | MS | Head to waist | Normal conversation, gestures | `medium shot, framed from the top of the head to the waist` |
| Medium close-up | MCU | Head to chest | Emotion + some body language | `medium close-up, framed from the top of the head to mid-chest` |
| Close-up | CU | Face fills the frame | Strong emotion, the moment of decision | `close-up, his face fills most of the frame, from chin to forehead` |
| Extreme close-up | ECU | One detail: eyes, lips, hand | Tension, a key detail | `extreme close-up of his eyes only` |
| Insert / detail | INS | An object | Show what matters: a letter, a bow, a clock | `close detail shot of the bow string under his fingers` |

💡 **The trick that makes models obey:** name the shot **and** where the frame cuts the body ("from the top of the head to the waist"). Shot names alone are often ignored.

---

## 2. Angles and camera height
| Angle | Effect on the viewer | Write it like this |
|---|---|---|
| Eye level | Neutral, honest, "with them" | `eye-level camera at his eye height` |
| Low angle | Power, heroism, threat | `low-angle shot, camera near the ground looking up at him` |
| High angle | Weakness, smallness, being watched | `high-angle shot, camera above him looking down` |
| Overhead / top-down | Pattern, fate, a "god's view" | `top-down shot directly overhead` |
| Ground level | Speed, footsteps, drama | `camera at ground level, just above the sand` |
| Dutch tilt | Unease, something is wrong | `the camera is tilted about 15 degrees` |
| Over-the-shoulder | Conversation, confrontation | `over-the-shoulder shot from behind Arjuna's shoulder, looking at Krishna` |
| Point of view | We see through their eyes | `point-of-view shot from Arjuna's eyes, looking at the opposing army` |
| Profile / three-quarter / back | Distance, mystery, introspection | `side profile` · `three-quarter view` · `seen from behind` |

⚠️ **Don't use left/right.** Models mix them up. Say "the side facing the camera" or "the edge near the river".

---

## 3. Lenses (focal length)
| Lens | Look | Use it for | Write it like this |
|---|---|---|---|
| 14–24mm (ultra wide) | Huge space, stretched edges, faces distort up close | Epic locations, action from close | `24mm wide-angle lens` |
| 35mm | Natural wide, "documentary" | Walking, scenes with surroundings | `35mm lens` |
| 50mm | Close to the human eye | Neutral medium shots | `50mm lens` |
| 85mm | Flattering portrait, soft background | Close-ups, emotion | `85mm portrait lens, shallow depth of field` |
| 135–200mm (telephoto) | Squashes distance, very blurry background | Spying, heat haze, armies stacked behind | `200mm telephoto lens, compressed background` |

💡 **Lens + distance work together.** A close-up on a 24mm feels intense and distorted; on an 85mm it feels calm and beautiful. Same shot size, different feeling.

In the 3D Stage, the same numbers appear on the camera's **Lens** slider (14mm to 200mm), so what you learn here carries over.

---

## 4. Getting more angles of the SAME shot
Need a reverse shot or reaction shot that matches your image? Don't regenerate from scratch:
1. Select the image → **Image → Change Angle**.
2. Move **Rotation** (around the subject), **Tilt** (up/down), **Forward** (closer/farther).
3. Start with a **small change**. Big moves make the model invent things it can't see.
4. If you expect a medium shot after moving closer, **say so in the prompt**. Moving closer is not a crop.

---

## 5. Shots that cut together
- **Wide → medium → close** is the classic way to lead a viewer into a scene.
- Keep everyone on the **same side** of the action between cuts. If Arjuna faces the camera's right in one shot, keep him facing right in the next, so the geography stays clear.
- Change **both** size and angle between two neighboring shots. A tiny change looks like a jump.

---

## Exercise: the shot ladder (practice account)
**Model:** GPT Image 2.5 **low** (2 credits each) · **Total: ~30 credits**

Use one character for every image, so only the camera changes. If you have **Arjuna Sheet** from your Gita project, attach it as a reference. Otherwise use the base prompt alone.

**Base prompt** (fill in `[SHOT]`):
```
Keep the facial identity, hairstyle and costume from the provided character reference.
Arjuna stands on a dusty battlefield at dawn, holding his bow lowered at his side, calm and focused.
[SHOT]
Low golden sunlight from behind him; soft fill on his face.
```

**Part A: 6 shot sizes** (replace `[SHOT]`, one image each)
1. `Extreme wide shot, he is small in the lower third of the frame, the empty plain and distant armies fill the image. 24mm lens.`
2. `Full shot, framed from the top of his head to his feet. 35mm lens.`
3. `Medium-wide shot, framed from head to knees. 35mm lens.`
4. `Medium shot, framed from the top of the head to the waist. 50mm lens.`
5. `Close-up, his face fills most of the frame, from chin to forehead. 85mm lens, background softly out of focus.`
6. `Extreme close-up of his eyes only. 100mm lens.`

**Part B: 4 angles** (keep `Medium shot, framed from head to waist. 50mm lens.` and add one)
7. `Low-angle shot, camera near the ground looking up at him.`
8. `High-angle shot, camera above him looking down.`
9. `Over-the-shoulder shot from behind his shoulder, looking toward the distant army.`
10. `Seen from behind, he faces the distant army.`

**Part C: the same close-up, 2 lenses**
11. `Close-up of his face, 24mm wide-angle lens, camera very close.`
12. `Close-up of his face, 200mm telephoto lens, the distant army compressed and blurred behind him.`

**Part D (optional): Change Angle**
Take image 4 → **Image → Change Angle** → Rotation a little, Run. Compare it with the original.

## Check your results
- [ ] Each shot size cut the body where you asked
- [ ] The low angle feels powerful; the high angle makes him smaller
- [ ] Image 11 (24mm) looks stretched and intense; image 12 (200mm) flat, calm, with a very blurred background
- [ ] The same Arjuna in all 12 (face, top bun, armor)
- [ ] Write down which shot sizes the model got wrong. Those are the ones to add body landmarks to next time.

## Save to your Prompt Library
Add the shot lines that worked best to [prompt-library.md](prompt-library.md) under **Images → My tested prompts**.

## Next: Lesson 1.3 Lighting and focus
