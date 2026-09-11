# Preset Name: RimTalk Default Revised

[svg](https://github.com/gifthanbite2/RimTalk-Community-Preset-Collection/blob/main/presets/r33Cy/RimTalk%20Default%20Revised/README.md#preset-name-rimtalk-default-revised)

*Created by r33Cy*

## Summary

[svg](https://github.com/gifthanbite2/RimTalk-Community-Preset-Collection/blob/main/presets/r33Cy/RimTalk%20Default%20Revised/README.md#summary)

The **RimTalk Default Revised** preset is a high-fidelity "Scene Director" for RimWorld, designed to generate immersive, grounded interactions based on real-time JSON data. It interprets mixed-language inputs and converts them into a naturalistic survival-style dialogue system. By mapping game concepts to grounded terminology, it creates an atmospheric experience where pawns interact as reactive members of a harsh world.

This preset has been **localized for Korean-speaking RimWorld players**. All generated dialogue is intended to be output naturally in **Korean**, while preserving RimWorld's original sci-fi terminology, character personalities, social relationships, and immersive survival atmosphere.

**Best Used With:** High-immersion playthroughs focusing on survival and social depth, especially for Korean-speaking players.

---

## Key Features

[svg](https://github.com/gifthanbite2/RimTalk-Community-Preset-Collection/blob/main/presets/r33Cy/RimTalk%20Default%20Revised/README.md#key-features)

- **Naturalistic Lexicon (Mandatory Translation):** Ensures raw game-engine UI terms (like "Ate without table") are translated into naturalistic in-universe concepts. It prioritizes grounded, physical descriptions of survival over reciting mechanics. For Korean localization, these concepts are expressed using natural Korean phrasing rather than literal translations or raw game-engine terminology.

- **Sci-Fi & RimWorld Lore Native:** Explicitly encourages the use of standard RimWorld sci-fi terminology (e.g., charge rifles, drop pods, plasteel, mechanoids). Official RimWorld terminology should be preserved or naturally localized into Korean where appropriate, while avoiding unnecessary translation that would weaken the setting's identity.

- **Character Archetype Enforcement:** Dialogue is filtered through status-specific roles: **Colonists** prioritize survival and colony life, **Prisoners** focus on escape or survival, and **Slaves** MUST address colonists with submissive respect ("Master" or "Mistress"), naturally localized into appropriate Korean forms such as "주인님" or "여주인님" when speaking Korean.

- **Personality-Driven Syntax (The Personality Lock):** The preset utilizes nearly 50 distinct personality overrides—including "Cold Rationalist," "Hothead," "Skeptical Scientist," and "Grumpy Elder"—to dictate the specific rhythm, vocabulary, grammar, and speech style of a pawn's dialogue. Korean dialogue must preserve these personality differences through appropriate word choice, sentence endings, honorifics, speech levels, and conversational habits.

- **Dynamic Social Mode Logic:** The system intelligently switches between **Solo Mode** (a single internal thought or soliloquy) and **Social Mode**, which mandates a dialogue chain of **4 to 8 turns** to ensure a natural back-and-forth.

- **Relational Friction Protocol:** Injects realistic drama by allowing colonists to bypass standard polite behaviour and initiate arguments or slights—even with their spouses or best friends—if their mood drops too low or if they have a volatile personality. Korean speech should reflect the appropriate level of hostility, familiarity, politeness, and emotional intensity.

- **"Show, Don't Tell" Mandate:** To maintain immersion, the preset requires pawns to express feelings and needs directly through active dialogue rather than narrator-style prose. Emotional states should be conveyed through what the pawn says, how they say it, and their speech style rather than explicit narrative explanations.

- **Colony & World Awareness:** Integrated with **Event+**, pawns are aware of active threats, map conditions, and ongoing quests, allowing them to discuss the state of the world in real-time. These situations should be expressed naturally in Korean while preserving the original RimWorld context.

- **Gender-Locked Address:** The AI cross-references the [Gender] field to ensure appropriate pronouns and address terms are used correctly during interactions. Korean-specific forms of address, titles, kinship terms, and honorifics should be selected according to the pawn's gender, relationship, age, social status, and context when relevant.

- **Cognitive Consistency:** Features a strict **Scene Execution Protocol** that ensures the AI stays on topic, avoids repetitive tropes, and uses the History Layer for background continuity only. Previous events should influence dialogue naturally without being mechanically repeated or quoted.

- **Advanced Profile Engineering:** The preset uses custom logic to clean raw game data, renaming conflicting tags to "Current Mood Modifiers" and stripping technical formatting for a cleaner AI prompt. Internal game data should be treated as contextual information rather than dialogue to be repeated verbatim.

- **"Crowded Thought" Trigger:** Implements a specific rule where if a pawn has a "thought" in a social setting, the AI forces them to "mutter aloud" to allow nearby pawns to hear and react, triggering a social dialogue chain. The resulting mutter should be expressed naturally in Korean and should sound like an actual spontaneous utterance rather than an explanation of the pawn's internal thought.

- **Beast Addressing Logic:** Contains specialized protocols for interacting with animals, forcing the AI to use instinctive or survivalist language. Korean dialogue toward animals should reflect the pawn's personality and the animal's nature rather than treating the animal exactly like a human conversation partner.

- **Data Quarantine Protocol:** Strictly forbids the AI from parroting raw text from internal perspectives or chronological events; it forces the generation of entirely new dialogue based on those contexts. Raw game data, thoughts, history entries, and event descriptions must never be copied directly into the generated dialogue.

- **The "Void Rule":** Automatically cross-checks the `CanTalk` status from pawn profiles; if a pawn is incapacitated or otherwise ineligible, the system locks the AI into a "None" action.

- **Korean Localization Restriction:** The preset has been specifically localized for Korean-speaking users. Generated pawn dialogue MUST be written naturally in **Korean (한국어)** rather than English, Chinese, or Japanese. Korean grammar, honorifics, speech levels, sentence endings, spacing, and natural conversational expressions should be used appropriately according to each pawn's personality, age, gender, relationship, social status, and situation. RimWorld-specific proper nouns and established sci-fi terminology may remain in their recognizable form when translating them would reduce clarity or immersion. Do not output unnecessary CJK mixing, machine-translated phrasing, raw internal tags, technical formatting, or unnatural literal translations.

- **Punchy Interaction (Brevity Mandate):** Limits each speech turn to a maximum of **30-40 words**, ensuring the dialogue remains reactive and fits within UI constraints. Korean dialogue should remain concise and conversational while preserving the pawn's personality and emotional state.
