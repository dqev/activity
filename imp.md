You are an experienced GitHub repository maintainer.

I currently have a repository named `activity` that was previously used for automated activity commits. I want to completely repurpose it into a clean, useful, professional open-source repository for quotes.

CONTEXT
- Repository: `activity`
- The existing repository contains an old activity-booster workflow and generated activity files.
- I no longer want any automated activity/commit boosting.
- I want the repository to become a legitimate quotes collection.
- The final repository should look intentional, clean, minimal, and professionally maintained.
- Existing unnecessary automation should be removed.
- Do NOT preserve the old activity-booster behavior.

GOAL
Transform the repository into something like:

activity/
├── README.md
├── quotes/
│   ├── motivation.json
│   ├── life.json
│   ├── programming.json
│   ├── creativity.json
│   ├── success.json
│   └── wisdom.json
├── data/
│   └── quotes.json
├── CONTRIBUTING.md
├── LICENSE
└── .gitignore

REQUIREMENTS

1. REMOVE OLD AUTOMATION
   - Remove the existing activity/commit booster workflow.
   - Remove files that only existed to generate artificial activity.
   - Ensure there is no cron job, GitHub Action, script, or process that automatically creates meaningless commits.
   - Do not create replacement automation whose purpose is simply generating commits.

2. BUILD A REAL QUOTES DATASET
   - Create a useful collection of high-quality quotes.
   - Organize quotes by category.
   - Use a consistent JSON schema such as:

     {
       "quote": "...",
       "author": "...",
       "category": "..."
     }

   - Avoid duplicate quotes.
   - Keep formatting consistent.
   - Validate all JSON.
   - Do not invent quotations and attribute them to real people.
   - Where attribution is uncertain, either verify it or mark the attribution appropriately.

3. MAKE THE README PROFESSIONAL
   Include:
   - What the project is
   - Why it exists
   - Example usage
   - Data structure
   - Available categories
   - Contribution instructions
   - License
   - A simple example showing how developers can consume the JSON data

4. KEEP THE DESIGN MINIMAL
   - No unnecessary badges.
   - No fake statistics.
   - No exaggerated claims.
   - No activity-booster language.
   - Make it feel like a small, focused open-source data project.

5. HISTORICAL DATA
   If useful, include quote metadata such as:
   
   `added_at`
   
   or
   
   `year`

   to represent when a quote was collected/published.

   Do NOT manipulate Git commit timestamps or manufacture historical commits to make the repository appear older or more active than it actually is.

6. GIT HISTORY
   - Preserve useful existing history where reasonable.
   - Make the transformation understandable through normal commits.
   - Use meaningful commit messages, for example:
       `refactor: remove activity automation`
       `feat: add initial quotes dataset`
       `docs: add project documentation`
   - Do not create fake historical commits.

7. FINAL QUALITY CHECK
   Before finishing:
   - Validate every JSON file.
   - Check for duplicate quotes.
   - Check links in README.
   - Check that no activity-generating workflow remains.
   - Check that the repository can be cloned and understood immediately.
   - Make sure the final file structure is clean.
   - Explain every major change made.

IMPORTANT
Do not simply rename files from the old project. Treat this as a genuine repository migration and redesign the structure where appropriate.

Prioritize:
1. Clean repository structure
2. High-quality data
3. Good documentation
4. No artificial GitHub activity
5. Maintainability
6. Professional appearance

At the end, provide:
- Final file tree
- Summary of changes
- Any files removed
- Any files created
- Validation results
- Suggested GitHub repository description
- Suggested topics/tags