# r33Cy's Preset Collection

This folder contains a collection of custom presets for the **RimTalk** mod created by **r33Cy**.

## Presets Included

* **[Medieval Fantasy](./Medieval%20Fantasy/README.md)**: A high-fidelity "Scene Director" designed to overhaul RimWorld's narrative tone into a gritty, low-fantasy dialogue system.
* **[RimTalk Default Revised](./RimTalk%20Default%20Revised/README.md)**: An atmospheric, grounded survival-style preset that interprets mixed-language inputs and converts them into naturalistic dialogue.

---

## Required Add-On Mods
* [RimTalk](https://steamcommunity.com/sharedfiles/filedetails/?id=3551203752) (Main Framework)
* [RimTalk Event+](https://steamcommunity.com/sharedfiles/filedetails/?id=3612632140) (For quest, threat and map condition awareness)
* [RimTalk - Expand Memory](https://steamcommunity.com/sharedfiles/filedetails/?id=3608181242) (For conversational continuity)
* [RimTalk - Expand Thoughts](https://steamcommunity.com/sharedfiles/filedetails/?id=3661175034) (For psychological depth)

## Recommended Add-On Mods
*These mods aren't required, but they greatly enhance the experience of this preset.*
* [RimTalk: Expand Literature](https://steamcommunity.com/sharedfiles/filedetails/?id=3633249209)  (Converts the subjective thoughts recorded by *Expand Thoughts* into tangible opinion changes in the social panel)
* [RimTalk: Expand Relation](https://steamcommunity.com/sharedfiles/filedetails/?id=3661493651) (To track opinion changes; Trust, affection, and respect automatically influence social standings with gradual, smooth changes that track thought decay)
* [RimTalk DynamicColors](https://steamcommunity.com/sharedfiles/filedetails/?id=3628773219) (For visual highlighting for names and keywords, making dialogue easier to follow)

---

## Preset Notes
*These settings are recommended to get the best experience with the presets in this collection.*

### AI Model & Provider
* **Model:** Gemma-4-31B (or similar high-capability models)
* **Provider/API:** TabbyAPI (Local)

The listed Gemma model is highly recommended and works very well with this preset, but it comes with a hardware caveat. 

**Hardware Caveat:** This preset requires a large context window. Currently, I am running a **20k context window**. To run a model of this size with such a large context window requires a significant amount of VRAM. For reference, simply loading the model alone consumes around 16 GB of VRAM. Users should select a model size that matches their available hardware to ensure smooth performance.

### AI Settings Tips
* **TabbyAPI & ExllamaV3 Configuration:** Below are the essential `config.yml` settings I use to run the Gemma model efficiently with a 20k context window:
  * **Backend:** `exllamav3` — Ensures the most efficient memory management.
  * **Cache Mode:** `4,4` — Uses 4-bit KV cache. This is absolutely critical for fitting a 20k context window into VRAM without running out of memory.
  * **Max Seq Len / Cache Size:** `20480` (20k) — Essential for handling the heavy data overhead from the **Expand** mod series and the robust prompt logic.
  * **Chunk Size:** `4096` — Set to the maximum ideal bound to vastly accelerate prompt ingestion speed (Time to First Token) for the massive 20k context.
* **Reasoning Tokens (Critical):** If you are using the reasoning version of this Gemma model, note that it uses non-standard reasoning tokens. You MUST configure TabbyAPI to catch these so the thoughts don't bleed into the game:
  * **reasoning:** `true`
  * **force_enable_thinking:** `true`
  * **reasoning_start_token:** `"<|channel>"`
  * **reasoning_end_token:** `"<channel|>"`
* **Tuning (Sampler Overrides):** I highly recommend creating a `rimtalk.yml` file in your `TabbyAPI\sampler_overrides\` folder and activating it by setting `override_preset: rimtalk` in your config. An optimal preset prevents repetitive loops over a 20k context window:
  * **temperature:** `0.85` & **min_p:** `0.05`
  * **repetition_penalty:** `1.05` (with a penalty_range of 8192)
  * **DRY Multiplier:** `0.4` (Base 1.75, Allowed Length 10, dry_range 8192)

### Other Details
Due to the complexity of the rulesets (such as the "Personality Lock" and specific lexicons), these presets are best paired with **highly capable models** (like Gemma-4-31B, DeepSeek-R1, or similar) that can handle the complex "Scene Execution Protocol" without breaking character.
