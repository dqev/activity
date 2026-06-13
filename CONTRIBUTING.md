# Contributing Guidelines

Thank you for considering contributing to the Quotes dataset!

## Guidelines for Adding Quotes

1. **Accuracy & Attribution**: Ensure quotes are attributed to their actual authors.
2. **Category Selection**: Choose from existing categories (`motivation`, `life`, `programming`, `creativity`, `success`, `wisdom`).
3. **No Duplicates**: Check both the target category JSON file and `data/quotes.json` to ensure the quote isn't already listed.
4. **Schema Compliance**: Every entry must strictly follow:
   ```json
   {
     "quote": "Quote string.",
     "author": "Author Name",
     "category": "category-name"
   }
   ```
