# Verity Minecraft Mod (JE + BE)

**Verity Minecraft mod** is the ThatMob horror entity: talk, adapt, stalk. Yellow-ball look. Hey it's me, it's Verity. Java 1.21.x and Bedrock 26.40. CurseForge pack name matches.

Java entity: `files/je/VerityEntity.java`. Entry: `VerityMod.java`. Renderer: `VerityRenderer.java`. Spawner: `VeritySpawner.java`. AI clients live in `files/ai/`. Bedrock scripts: `files/be/`.

<img width="739" height="415" alt="images1" src="https://github.com/user-attachments/assets/d945939b-3425-4865-a410-a97b770db569" />

Java: drop the JE jar into mods on 1.21.x. Bedrock: install the BE pack on 26.40. SKLauncher is a different repo. MelonLoader is Unity - not this.

Spoken lines beyond the table: point AI at Ollama or Groq. Without those, dialogue stays on the table + `files/be/dialogue.js`.

<img width="526" height="296" alt="images2" src="https://github.com/user-attachments/assets/4d4a3177-9ade-47f4-a0ef-9a6881d918d5" />

## Editions

| Edition | Folder | Version | Talk / spawn |
|---|---|---|---|
| Java | `files/je/` | 1.21.x | `VerityDialogue` / `VeritySpawner` |
| Bedrock | `files/be/` | 26.40 | `dialogue.js` / `spawner.js` |

Do not mix JE jars into a Bedrock world folder.

<img width="811" height="455" alt="images3" src="https://github.com/user-attachments/assets/2dea8f52-1261-4fd2-92b7-b95e1a5d2e52" />

## What it does

ThatMob horror entity. Talks. Adapts. Stalks. Dialogue table + spawn rules in v6.2. Cruelty / spawn rate / talk chance stay in the config.

`VerityAI` is the adapt layer. Renderer is `VerityRenderer`. If Verity never spawns, cruelty / spawn is at zero. Raise the rate in the spawner files.

<img width="526" height="296" alt="images4" src="https://github.com/user-attachments/assets/161ad0c9-31b1-4c34-8ef8-dbe4e89946b4" />

## Java vs Bedrock

JE has the Java AI clients (Groq / Ollama). BE is script-driven. Same character, two stacks. A JE world will not load the BE scripts.

## Troubleshooting

| Symptom | Cause |
|---|---|
| Never spawns | Spawn / cruelty at 0 |
| Silent | Dialogue table empty / AI clients off |
| Wrong game | SKLauncher vs this mod |
| BE scripts ignored | Loaded as a JE jar |
| Movie / track hits | Wrong Verity |

## v6.2

Dialogue table + spawn rules. Resource pack optional.
