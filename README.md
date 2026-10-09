# German-flashcards

A lightweight, responsive web-based flashcard application designed to aid German B1 vocabulary practice. Features article-based color coding for noun gender retention and dataset switching.

## Features

- **Gender-Based Color Coding:** Nouns are color-coded at the bottom border for visual memory cues:
  - Blue (`der` - Masculine)
  - Pink (`die` - Feminine)
  - Green (`das` - Neuter)
- **Multiple Categories:** Practice Nouns (*Nomen*), Verbs (*Verben*), and Other parts of speech (*Andere*).
- **Interactive Reveal:** Click anywhere on the card to display the translation.
- **Automated Shuffling:** Words auto-shuffle upon switching categories.

## Project Structure

```text
├── index.html     # Core application UI and logic
├── nouns.json     # Vocabulary dataset for nouns
├── verbs.json     # Vocabulary dataset for verbs
├── others.json    # Vocabulary dataset for adjectives/adverbs
└── README.md      # Documentation
```
## JSON Data Structure
To extend or update the flashcard datasets, ensure your JSON files strictly follow this structure:

```text
[
  {
    "word": "die Entscheidung",
    "example": "Ich habe eine wichtige Entscheidung getroffen.",
    "translation": "decision",
    "gender": "die"
  }
]
```
