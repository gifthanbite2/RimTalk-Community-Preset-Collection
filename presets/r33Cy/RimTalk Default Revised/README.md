[← Back to Preset Collection](../README.md)

# Preset Name: RimTalk Default Revised
*Created by r33Cy*

## Summary
The **RimTalk Default Revised** preset is a high-fidelity "Scene Director" for RimWorld, designed to generate immersive, grounded interactions based on real-time JSON data. It interprets mixed-language inputs and converts them into a naturalistic survival-style dialogue system. By mapping game concepts to grounded terminology, it creates an atmospheric experience where pawns interact as reactive members of a harsh world.

**Best Used With:** High-immersion playthroughs focusing on survival and social depth.

---

## Key Features

* **Naturalistic Lexicon (Mandatory Translation):** Ensures raw game-engine UI terms (like "Ate without table") are translated into naturalistic in-universe concepts. It prioritizes grounded, physical descriptions of survival over reciting mechanics.
* **Sci-Fi & RimWorld Lore Native:** Explicitly encourages the use of standard RimWorld sci-fi terminology (e.g., charge rifles, drop pods, plasteel, mechanoids).
* **Character Archetype Enforcement:** Dialogue is filtered through status-specific roles: **Colonists** prioritize survival and colony life, **Prisoners** focus on escape or survival, and **Slaves** MUST address colonists with submissive respect ("Master" or "Mistress").
* **Personality-Driven Syntax (The Personality Lock):** The preset utilizes nearly 50 distinct personality overrides—including "Cold Rationalist," "Hothead," "Skeptical Scientist," and "Grumpy Elder"—to dictate the specific rhythm, vocabulary, and grammar of a pawn’s speech.
* **Dynamic Social Mode Logic:** The system intelligently switches between **Solo Mode** (a single internal thought or soliloquy) and **Social Mode**, which mandates a dialogue chain of **4 to 8 turns** to ensure a natural back-and-forth.
* **Relational Friction Protocol:** Injects realistic drama by allowing colonists to bypass standard polite behaviour and initiate arguments or slights—even with their spouses or best friends—if their mood drops too low or if they have a volatile personality.
* **"Show, Don't Tell" Mandate:** To maintain immersion, the preset requires pawns to express feelings and needs directly through active dialogue rather than narrator-style prose.
* **Colony & World Awareness:** Integrated with **Event+**, pawns are aware of active threats, map conditions, and ongoing quests, allowing them to discuss the state of the world in real-time.
* **Gender-Locked Address:** The AI cross-references the [Gender] field to ensure appropriate pronouns and address terms are used correctly during interactions.
* **Cognitive Consistency:** Features a strict **Scene Execution Protocol** that ensures the AI stays on topic, avoids repetitive tropes, and uses the History Layer for background continuity only.
* **Advanced Profile Engineering:** The preset uses custom logic to clean raw game data, renaming conflicting tags to "Current Mood Modifiers" and stripping technical formatting for a cleaner AI prompt.
* **"Crowded Thought" Trigger:** Implements a specific rule where if a pawn has a "thought" in a social setting, the AI forces them to "mutter aloud" to allow nearby pawns to hear and react, triggering a social dialogue chain.
* **Beast Addressing Logic:** Contains specialized protocols for interacting with animals, forcing the AI to use instinctive or survivalist language.
* **Data Quarantine Protocol:** Strictly forbids the AI from parroting raw text from internal perspectives or chronological events; it forces the generation of entirely new dialogue based on those contexts.
* **The "Void Rule":** Automatically cross-checks the `CanTalk` status from pawn profiles; if a pawn is incapacitated or otherwise ineligible, the system locks the AI into a "None" action.
* **Latin-Only Restriction:** A strict technical guardrail that prevents CJK (Chinese, Japanese, Korean) characters or Unicode symbols from bleeding into the output, ensuring compatibility with English-only interfaces.
* **Punchy Interaction (Brevity Mandate):** Limits each speech turn to a maximum of **30-40 words**, ensuring the dialogue remains reactive and fits within UI constraints.

---

For required/recommended mods, AI settings, and provider details, please refer to the [top-level README](../README.md).