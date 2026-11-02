# AI Co-pilot Toolkit: AI + Flick, Done Like a Director

**Normal AI user:** types a short idea into Flick, hopes for magic, regenerates until bored.
**You:** make the creative **decisions**, let an AI assistant (Claude, ChatGPT…) turn them into **perfect model language**, and judge every result against a plan.

> AI is great at **writing**: long prompts, shot lists, timings, formatting, checklists.
> AI is bad at **taste**: what's true, what's beautiful, what's the story, which take is the one.
> Give AI the typing. **Keep the decisions.**

---

## Who does what
| AI does (don't waste your time) | YOU do (this is what makes you different) |
|---|---|
| Expand your 5-line brief into full prompts | Decide the story, the change, the feeling |
| Rewrite prompts into each model's grammar (Nano Banana locks, Seedance timecodes, 3-sentence motion) | Collect **real references**: film stills, photos, your own sketches |
| Break a scene into a shot list with sizes, angles, lenses | Choose which shots the story actually needs |
| Write 4,000-word action choreography from your description | Watch real fights, gestures, places, and describe what you saw |
| Describe a reference image in camera/light language | Pick the reference that feels right |
| Score a result against your checklist | Make the final call: keep, fix, or cut |
| Track costs, write captions, titles, descriptions | Cultural truth: correct costumes, verses, rituals, respect |
| Draft voice lines and narration | Timing and rhythm in the edit (listen, feel, cut) |

---

## The 8 habits that make you different
1. **Reference-first, not prompt-first.** Before writing anything, collect 3–5 real references (Flickpedia → Classic Film Scenes, your photos). AI can't invent good taste; references carry it.
2. **One project bible.** Style recipe, character locks, location rules in **Project memory**, kept up to date by AI. Every prompt follows it.
3. **Speak each model's language.** Every model has its own grammar. Let AI translate your idea using that model's rules (templates below).
4. **Test one variable.** A/B test one change per run, cheap model first. Log what worked.
5. **Design for the cut, not the single image.** Plan shots as a sequence: wide → medium → close, reverse angles, a clear geography.
6. **Steal like a director.** Find a shot you love in a real film, have AI describe its lens/angle/light, then rebuild it with your characters.
7. **Judge with a checklist, not a feeling.** Write 3 checks before generating; let AI score; you decide.
8. **Be the culture expert.** AI often gets Indian costumes, weapons, verses and rituals wrong. Your knowledge is your edge. Always verify.

---

## Master prompts (copy into Claude/ChatGPT)

### 1. Director's Brief → Project Bible
```
You are my film pre-production assistant for Flick.art.
Here is my idea in my own words:
[your idea in 3–5 lines]
Audience: [who]. Length: [seconds]. Aspect ratio: [16:9/9:16]. Style: [2D cartoon / photoreal / …].

Write a project bible with:
1. One-line goal (who + where + what happens)
2. 4-line brief: what happens / what changes / what the viewer feels / what to avoid
3. Character locks for each character (age, build, face, hair, costume, props, one distinctive detail)
4. Location handbook (layout, light direction, recurring objects, time of day)
5. Style recipe in visible terms (line, color, light, texture)
6. 3 success checks
Keep it short enough to paste into Flick Project memory (under 900 characters for sections 3–5).
```

### 2. Shot list designer
```
Using this project bible: [paste]
Write a shot list for [scene]. For each shot give:
shot number · story job (establish / notice / react / reveal…) · shot size with body framing ("from head to waist") · angle · lens mm · subject action (one) · camera move (one or static) · duration · what must stay the same.
Make the shots cut together: vary size and angle between neighbors, keep screen direction consistent.
```

### 3. Image prompt writer (Nano Banana Pro / GPT Image)
```
Write a Flick image prompt for shot [N] following these rules:
- Order: subject → action/pose → setting → framing (size, angle, lens) → light (source, direction, bright/dark areas) → focus → 1–3 texture details
- Give each attached reference one job with short labels ("the provided character reference") and lock wording ("facial identity 100% match the provided character reference")
- Do not re-describe what the reference already shows; describe only the change
- No left/right (use "the side facing the window"), no "maybe", no vague words like "cinematic", no long negative lists
- Do not mention style (the project style is pinned)
Attached references: [list them and what each is for]
Shot: [paste from shot list]
```

### 4. Motion prompt writer (Frame to Video)
```
Write a 3-sentence motion prompt for this still: [describe the still or attach it]
Sentence 1: the subject's ONE action with a pace word, in order (first… then…).
Sentence 2: ONE camera instruction, or "Static camera, locked framing."
Sentence 3: what must not change (face, costume, lighting, framing).
Also give me: recommended duration, and whether an End Frame would help.
```

### 5. Seedance performance / action writer
```
Write a Seedance 2.5 Reference-to-Video prompt.
References: @Image1 = [character A sheet], @Image2 = [character B sheet], @Image3 = [location], @Video1 = [optional motion/camera reference]
Rules: assign each reference one job ("A's appearance matches @Image1 100%"); write behavior not emotions; separate Character and Camera sections; use time windows (0–2s, 2–4s…); for action use preparation → attack → contact → reaction → recovery; real-time speed, no slow motion; give the camera one job; add a SOUND section with each sound placed where it happens.
What happens: [describe the beat in your own words, including what you observed in real reference footage]
Duration: [s]
```

### 6. Reference analyzer ("steal like a director")
```
[Attach a film still or photo]
Describe this image the way a cinematographer would, for an AI image prompt:
shot size (with body framing), camera height and angle, likely lens mm, composition (where the subject sits, foreground/midground/background), light source + direction + quality, color palette, focus/depth of field, texture.
Then rewrite it as a Flick prompt for: [my character / my scene], keeping the camera and light, changing only the content.
```

### 7. Result critic
```
[Attach the generated image or a frame from the clip]
My goal for this shot: [shot job]. My checks: [3 checks]. Character locks: [paste].
Score each check pass/fail with the exact visual reason.
Then name the ONE main problem and give me ONE changed prompt line to fix it (keep everything else identical).
```

---

## Golden rule
Never paste an AI-written prompt without reading it. Add **one specific detail only you would know**: a real gesture you observed, a correct costume detail, a sound you heard. That detail is what makes the result yours.
