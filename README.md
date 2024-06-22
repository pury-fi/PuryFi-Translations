# PuryFi-Translations
Internationalization (i18n) files for the PuryFi browser extension

# PuryFi Translation Framework

Our translation framework, based on the i18n standard, facilitates the localization of our extension. We invite users to contribute by forking our Git repository.

## How It Works:

1. **Automatic Scanning**: 
   - The options page is automatically scanned by our internal tool to detect new, removed, or changed text entries.
   - The repository is updated whenever a new version is released.

2. **Translation Structure**:
   - **message**: Contains the translated text.
   - **description**: Contains the original English text for reference. If this differs from the current English version, the entry will be marked as "changed" and will need a new translation.
   - **status**: Indicates the state of the translation:
     - `new`: Newly added translation entry.
     - `null`: No changes detected.
     - `changed`: Original text has changed and needs revision.
     - `removed`: Entry has been removed and should be deleted.
     - `manual`: Requires manual revision as it is not covered by the scanner.

3. **Manual Revisions**:
   - Entries not starting with "options__" are not automatically scanned and require periodic manual revisions.

## Example Entry:

```json
"options-title": {
  "message": "PuryFi - Optiones",
  "description": "PuryFi - Options",
  "status": "new" | null | "changed" | "removed" | "manual"
}
```

By forking the repository and contributing translations, users help ensure our extension is accessible to a broader audience. Thank you for your support!

---
