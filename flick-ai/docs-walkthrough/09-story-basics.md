# 09 · Story (Your Script Page)
[Docs page](https://flick.art/docs/script-view-basics)

**Story = your project's notebook.** Script, notes, character rules, all in one page. You and the agent both write here.

## Where it is
![Story page](images/09-story-page.jpg)
**1** **STORY** tab (or the Story button on the canvas toolbar) · **2** document menu · **3** **Project memory** card · **4** outline (hover to jump to a scene) · **5** Agent memory · **6** quick help from the agent

## 1. Write
Type `/` to add a block: heading, list, table, **Script**, **Project memory**.
Shortcuts: `#` heading · `-` list · `1.` numbered list

## 2. Script box (for screenplays)
![Script box](images/09-script-box.jpg)
**1** script box · **2** scene line · **3** action lines
- `Enter` = next line (Flick guesses the type)
- `Tab` = change the line type (Scene, Action, Character, Dialogue…)
- Start a line with `INT.` or `EXT.` = new scene

## 3. Bring in your script
| You have | Do |
|---|---|
| Notes or text (like your Gita script) | **Paste** with `Ctrl+V` |
| A real screenplay file (.fountain, .fdx, .pdf, .docx) | Script box → **Upload** |
| A Markdown file | Document menu → **Import Markdown** |

## 4. Project memory: the most important card
The agent reads it **every message**. Put:
- the style recipe
- each character's look
- rules ("no text in images", "ask before generating")

**Keep it short.** There's a limit (8000 characters).

## 5. Document menu
![Document menu](images/09-doc-menu.jpg)
**1** font · **2** Import Markdown · **3** download as PDF / Markdown · **4** Focus mode (`Esc` to leave)

## Rules
1. **Write the brief and memory before generating anything.**
2. **One character = one spelling.** "Arjuna" and "Arjun" become 2 characters.
3. **Ask the agent to help:** "draft scene 2", "make a table of characters", "rename X to Y everywhere".
4. **The agent keeps forgetting your style?** Put it in Project memory, not in chat.

## AI + You
- **AI:** drafts scenes, tightens lines, makes the character table.
- **You:** decide what happens and what each scene must make the viewer feel.

## Practice (free)
Open **STORY** → paste a short idea → type `/` → add **Project memory** with your style + 1 character → ask the agent: *"Make a table of the characters in this story. Don't generate anything."*

---

## Script line types: when to use which
| Type | Use it for | Example |
|---|---|---|
| **Scene** | Start of a new place or time | `EXT. KURUKSHETRA BATTLEFIELD - DAWN` |
| **Action** | What we **see** happen | `Arjuna drops his bow and sits down.` |
| **Character** | Who speaks (just the name, above their line) | `ARJUNA` |
| **Dialogue** | What they say | `Krishna, I cannot do this.` |
| **Parenthetical** | How they say it (short, in brackets) | `(whispering)` |
| **Transition** | How we move to the next scene | `CUT TO:` · `FADE OUT.` |
| **Shot** | A specific camera shot | `CLOSE ON ARJUNA'S SHAKING HANDS` |
| **Act** | A big part of the story (only for longer films) | `ACT ONE` |

**Order to remember:** Scene → Action → Character → (Parenthetical) → Dialogue → Transition.

**Simple rule:** for short films you mostly need just **Scene, Action, Character, Dialogue**.

Mini example:
```
EXT. KURUKSHETRA - DAWN          ← Scene
Arjuna sits in the chariot.       ← Action
ARJUNA                            ← Character
(softly)                          ← Parenthetical
Krishna, I cannot do this.        ← Dialogue
CLOSE ON KRISHNA'S SMILE          ← Shot
CUT TO:                           ← Transition
```

## What is Markdown?
Plain text with a few symbols that turn into formatting.

| You type | You get |
|---|---|
| `# Title` | big heading |
| `## Part` | smaller heading |
| `- item` | bullet list |
| `1. item` | numbered list |
| `**bold**` | **bold** |

All the `.md` files in this GitHub repo are Markdown. In Flick you can bring one in with **Import Markdown**, or download your Story with **Download as Markdown**. Text from ChatGPT or Claude is usually Markdown already, so it pastes into Story nicely.
