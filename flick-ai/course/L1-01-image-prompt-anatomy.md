# Lesson 1.1: Image Prompt Anatomy

Source: [Image Generation Prompts Guide](https://flick.art/docs/Image-Generation-prompts) · [Generate Image](https://flick.art/docs/generate-image)

## The idea
An image model can only draw what you **describe in visible terms**. "Cinematic, epic, beautiful" tells it nothing it can draw. "One window lights the left side of his face, the rest of the room is dark" does.

## The 7-part prompt (in this order)
| # | Part | Ask yourself | Example |
|---|---|---|---|
| 1 | **Subject** | Who or what, and how many? (one clear subject) | an old sage with a long white beard, saffron robe |
| 2 | **Action / pose** | What is he doing, visibly? | sits cross-legged, eyes closed, palms resting on his knees |
| 3 | **Setting** | Where? Only what matters | on a flat rock beside a Himalayan river at dawn |
| 4 | **Framing** | Shot size + angle + lens | medium-wide shot, eye level, 35mm lens |
| 5 | **Light** | Source, direction, bright vs dark areas | low golden sunlight from behind the mountains rims his shoulders; his face in soft shade |
| 6 | **Focus / depth** | What's sharp, what's blurred? | focus on his face; the river and mountains softly out of focus |
| 7 | **Texture** (optional) | Only what the style needs | realistic skin texture, subtle film grain |

**Style** is NOT in the prompt when a project style is pinned. The style button sets the look; the prompt sets the content.

## The rules that change results most
| ❌ Weak | ✅ Strong | Why |
|---|---|---|
| "cinematic, moody" | "a dim room lit only by one window" | Visible light, not a mood label |
| "on his left side" | "on the side facing the window" | Models confuse left and right |
| "no glass in the window" | "an open window, mist drifting through the opening" | Describe the final state, not negatives |
| "maybe a sword or a spear" | "a long spear with a red tassel" | Choose one result, never alternatives |
| Re-describing the face from a reference | "Keep the facial identity, structure and features from the provided character reference" | Reference carries the face; prompt carries the change |
| 10 subjects and actions | One clear subject, one action | Each extra idea weakens the others |

## When you use references
Give every reference **one job**, and name it with a short label:
```
Use the provided sketch for composition, framing, camera position and pose.
Use the provided character reference for facial identity.
Use the provided outfit reference for clothing design and colors.
```
Strong "lock" wording (from the docs and pro workflows):
```
composition 100% match the provided sketch. camera position 100% unchanged.
facial identity 100% match the provided character reference.
```

## Exercise: "Three prompts, one subject" (practice account)
**Model:** GPT Image 2.5 **low** (2 credits each) · **Total: ~12 credits**

Generate the same subject three ways and compare:

**A. Vague**
```
A cinematic epic image of an Indian sage meditating, beautiful and spiritual.
```
**B. Structured (7 parts)**
```
An old sage with a long white beard and a saffron robe sits cross-legged on a flat rock beside a Himalayan river at dawn, eyes closed, palms resting on his knees. Medium-wide shot, eye level, 35mm lens. Low golden sunlight from behind the mountains rims his shoulders and beard; his face is in soft shade. Focus on his face; the river and mountains are softly out of focus. Thin mist over the water.
```
**C. One change from B:** keep everything, change only the framing to `Close-up of his face, eye level, 85mm lens.`

Then make 3 more of B with **1x → 3x** (batch). Notice how results vary even with the same prompt.

## Check your results
- [ ] B matches the picture in your head much better than A
- [ ] In C, only the framing changed (same sage, same light)
- [ ] Light comes from where you said, and the focus is where you said
- [ ] One clear subject, correct count of hands and fingers
- [ ] You can name which part of the prompt caused each difference

## Save to your Prompt Library
Copy prompt B into [prompt-library.md](prompt-library.md) under **Image → My tested prompts**, with the model and what worked.

## Next: Lesson 1.2 Shot sizes, angles and lenses
