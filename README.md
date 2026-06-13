# Quotes Dataset

A clean, minimalist, open-source dataset of high-quality curated quotes organized by category in standardized JSON format.

## Overview

This repository provides a light-weight, dependency-free collection of famous quotations across multiple themes (motivation, life, programming, creativity, success, wisdom). It is designed to be easily consumed in web applications, CLI tools, mobile apps, and educational projects.

## Categories

| Category | File | Description |
| :--- | :--- | :--- |
| **Motivation** | [`quotes/motivation.json`](quotes/motivation.json) | Inspiration for action, resilience, and personal drive |
| **Life** | [`quotes/life.json`](quotes/life.json) | Reflections on human experience and perspective |
| **Programming** | [`quotes/programming.json`](quotes/programming.json) | Insights on software engineering, craft, and code simplicity |
| **Creativity** | [`quotes/creativity.json`](quotes/creativity.json) | Ideas on art, innovation, and original thinking |
| **Success** | [`quotes/success.json`](quotes/success.json) | Wisdom on goals, achievement, and learning from failure |
| **Wisdom** | [`quotes/wisdom.json`](quotes/wisdom.json) | Timeless philosophy and self-knowledge |

All quotes are aggregated into a single master file at [`data/quotes.json`](data/quotes.json).

## Data Schema

Each quote record follows this consistent schema:

```json
{
  "quote": "The only way to do great work is to love what you do.",
  "author": "Steve Jobs",
  "category": "motivation"
}
```

## Example Usage

### JavaScript / Node.js

```javascript
import quotes from './data/quotes.json' assert { type: 'json' };

// Get a random quote
const randomQuote = quotes[Math.floor(Math.random() * quotes.length)];
console.log(`"${randomQuote.quote}" — ${randomQuote.author}`);
```

### Python

```python
import json, random

with open('data/quotes.json', 'r') as f:
    quotes = json.load(f)

selected = random.choice(quotes)
print(f'"{selected["quote"]}" — {selected["author"]}')
```

## Repository Structure

```
activity/
├── README.md
├── CONTRIBUTING.md
├── LICENSE
├── .gitignore
├── data/
│   └── quotes.json
└── quotes/
    ├── creativity.json
    ├── life.json
    ├── motivation.json
    ├── programming.json
    ├── success.json
    └── wisdom.json
```

## Contributing

Contributions are welcome! Please read [`CONTRIBUTING.md`](CONTRIBUTING.md) for details on adding quotes, checking schema validity, and submitting pull requests.

## License

This project is open-source and available under the terms of the [MIT License](LICENSE).
