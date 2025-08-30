# OSS Campaign Form

A multilingual, accessible web application for generating personalized campaign messages to support open source and digital sovereignty in the EU.

## Features
- **Single-page HTML app** for easy deployment and use
- **Multilingual support**: 24 official EU languages, with translations managed via YAML files in the `lang/` directory
- **Accessibility**: WCAG 2.2 AA compliance, dark/light mode toggle
- **Personalized message generation**: Users enter their details and receive a tailored campaign message for their EU representative
- **No data collection**: All processing is local; no user data is stored or sent
- **Copy to clipboard**: One-click button to copy the generated message
- **Organization/affiliation auto-fill**: Suggests organization based on project or company
- **SVG branding**: OSI logo included

## How It Works
1. User selects their language from the dropdown (all EU languages supported)
2. User fills out the form with their name, city, postal code, company, project, and organization/affiliation
3. The app generates a personalized campaign message using instructions and templates from the selected language's YAML file
4. User can copy the message to their clipboard and send it via email to their EU representative

## Directory Structure
```
oss-campaign.html      # Main HTML app
lang/                  # YAML translation files for each language
  en.yaml
  de.yaml
  ...
```

## Adding/Editing Languages
- To add a new language, create a YAML file in the `lang/` directory using the same structure as the others
- To edit translations, update the relevant YAML file
- The language dropdown in the app should be updated to include any new language codes and names

## Running Locally
Due to browser security restrictions, you must run a local web server to load YAML files:

```
# Python 3
python3 -m http.server
# or
# Node.js
npx serve
```
Then open `http://localhost:8000/oss-campaign.html` in your browser.

## Accessibility & Inclusion
- Fully keyboard accessible
- High contrast and dark/light mode support
- All UI text and instructions are translatable

## License
Open source, MIT License.

## Credits
- Project by Mike Gifford
- Translations provided by GitHub Copilot
- SVG logo from the Open Source Initiative

## Contact
For questions or contributions, open an issue or pull request.
