[← Back to Preset Collection](../README.md)

# Preset Name: Medieval Fantasy
*Created by r33Cy*

## Summary
The **Medieval Fantasy** preset is a high-fidelity "Scene Director" for RimWorld, designed to completely overhaul the game's narrative tone. It interprets real-time game data and converts it into a gritty, low-fantasy dialogue system. By stripping away modern language and industrial terminology, it creates an immersive atmosphere where pawns speak as hardy survivors in a world of steel, hearths, and social obligation.

**Best Used With:** High-immersion "Medieval Overhaul" or "Total Conversion" playthroughs.

---

## Key Features

* **The Gritty Lexicon & 1700 Veto:** This preset strictly forbids modern slang (e.g., "okay," "cool," "guys") and industrial or sci-fi terminology. It utilizes a **"1700 Chronological Veto"**—any concept originating after the Industrial Revolution must be described by its physical components (Material, Element, Function) rather than its modern name.
* **British Orthography Lock:** To maintain a consistent "Old World" atmosphere, the system mandates **British English** spelling standards exclusively (e.g., Labour, Honour, Organise, Centre), prohibiting Americanised variants.
* **Character Archetype Enforcement:** Dialogue is filtered through status-specific roles; for example, Slaves must address colonists exclusively as **"Master"** or **"Mistress,"** while colonists address peers as **"kin"** or **"comrade"**.
* **Personality-Driven Syntax (The Personality Lock):** The preset utilizes over 25 distinct personality overrides—such as "Stoic," "Abrasive," "Haughty," or "Simpleton"—formatted with **optimised whitespace** to dictate the specific rhythm, vocabulary, and grammar of a pawn’s speech.
* **Dynamic Social Mode Logic:** The system intelligently switches between "Solo Mode" (a single thought or soliloquy) and "Social Mode," which mandates a dialogue chain of **4 to 8 turns** to ensure a natural back-and-forth between characters.
* **Relational Friction Protocol:** Injects realistic drama by allowing colonists to bypass standard polite behaviour and initiate arguments or slights—even with their spouses or best friends—if their mood drops too low or if they have a volatile personality.
* **Sensory Threat Reconstruction:** Pawns discuss active threats and map conditions using a sensory translation protocol. Instead of naming mechanical events like "Toxic Fallout," they describe the visceral impact (e.g., "the choking yellow haze"), though they maintain the ability to name specific narrative **"Villains"** (e.g., "Idris the Red") found in the data.
* **Anti-"Sage" Mandate:** To keep the setting grounded, the preset prohibits flowery narrator prose and restricts high-medieval grammar (e.g., "thee" and "thou") exclusively to characters with "High Noble" or "Scholar" backgrounds.
* **Gender-Locked Kinship:** The AI cross-references the [Gender] field for every address to ensure appropriate terms like "Sir," "Dame," "Brother," or "Sister" are used correctly during interactions.
* **"Crowded Thought" Trigger:** If a pawn has a "thought" in a social setting, the AI forces them to "mutter aloud" (to self) to allow nearby pawns to hear and react, triggering a social dialogue chain instead of a private monologue.
* **Beast Addressing Logic:** Contains specialised protocols for interacting with animals, forcing the AI to use "Instinctive Reaction" language, such as short-burst exclamations, tactical commands, or visceral, guttural curses.
* **Data Quarantine Protocol:** Strictly forbids the AI from parroting raw text from internal perspectives or chronological events. It uses a **"Component Blueprint"** to force the generation of entirely new dialogue based on those contexts.
* **The "Void Rule":** Automatically cross-checks the `CanTalk` status from pawn profiles; if a pawn is incapacitated or otherwise ineligible, the system locks the AI into a "None" action and excludes them from the dialogue chain.
* **Latin-Only Restriction:** A strict technical guardrail that prevents CJK (Chinese, Japanese, Korean) characters or Unicode symbols from bleeding into the output, ensuring compatibility with English-only interfaces.
* **Double-Translation Engine:** Acts as a bridge for players using multi-language mod setups by interpreting Chinese intent-parsing data and translating it first to English, then to the "Gritty Medieval" dialect.
* **Advanced Profile Engineering:** The preset uses custom Scriban logic to clean raw game data, renaming conflicting tags to "Current Mood Modifiers" and stripping technical formatting for a cleaner, high-integrity AI prompt.

---

For required/recommended mods, AI settings, and provider details, please refer to the [top-level README](../README.md).