# German-flashcards

![GitHub Pages Deployment](https://img.shields.io/badge/GitHub%20Pages-Active-brightgreen?logo=github)
![Tech Stack](https://img.shields.io/badge/Tech--Stack-HTML%20%7C%20CSS%20%7C%20JavaScript-blue?logo=javascript)
![API Integration](https://img.shields.io/badge/AI-Gemini%20API-orange?logo=google)
![License](https://img.shields.io/badge/License-MIT-green)

A lightweight, responsive web-based flashcard and vocabulary application designed for German B1 practice. Features gender-based color coding, real-time vocabulary search, and an AI-powered admin dashboard for automated vocabulary entry.

## Features

- **Gender-Based Color Coding:** Cards feature distinct bottom border colors to aid article retention:
  - Blue (`der` - Masculine)
  - Pink (`die` - Feminine)
  - Green (`das` - Neuter)
  - Yellow (`verb` - Verbs)
  - Purple (`other` - Adjectives/Adverbs/Other)
- **Multiple Categories:** Toggle instantly between Nouns (*Nomen*), Verbs (*Verben*), and Other parts of speech (*Andere*).
- **Interactive Flashcards:** Click anywhere on a card to reveal the English translation and example sentence.
- **Vocabulary Search:** Search for words across all datasets in real-time right from the main view.
- **Automated Shuffling:** Words auto-shuffle every time a category is selected.
- **AI-Powered Admin Dashboard (`admin.html`):** Add new vocabulary seamlessly using Google Gemini API for automated translations, B1 example sentences, and gender classifications, then commit changes directly to GitHub via the REST API.

## Project Structure

```text
├── index.html     # Core flashcard UI & live search function
├── admin.html     # Admin dashboard with Gemini AI & GitHub API integrations
├── nouns.json     # Vocabulary dataset for nouns
├── verbs.json     # Vocabulary dataset for verbs
├── others.json    # Vocabulary dataset for adjectives/adverbs
└── README.md      # Project documentation
```

## JSON Data Structure

To extend or update the flashcard datasets manually or via the admin panel, ensure entries follow this structure:

```json
[
  {
    "word": "die Entscheidung",
    "example": "Ich habe eine wichtige Entscheidung getroffen.",
    "translation": "decision",
    "gender": "die"
  }
]
```

Valid values for `gender`: `der`, `die`, `das`, `verb`, `other`.

## Admin Dashboard & AI Workflow

Access `admin.html` in your browser to manage vocabulary:
1. Enter your **Gemini API Key** and **GitHub Personal Access Token** in the API Settings panel (stored safely in your browser's local storage).
2. Type a German word and click **✨ AI Fill** to automatically generate its article, English translation, and a B1-level example sentence.
3. Click **💾 Commit & Save to GitHub** to push the update directly to your repository without leaving the page.

## Getting Started

Open `index.html` in any modern web browser or deploy via GitHub Pages to access the flashcards and live search functionality.
