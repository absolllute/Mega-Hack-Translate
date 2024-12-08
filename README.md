# Mega Hack Translation Project

This project aims to provide accurate translations for Mega Hack in languages other than British English. The first translations will be available in Mega Hack v8.1.0 which is in active development.

## Contributing

To contribute to existing languages, please edit the existing language's JSON and create a pull request with your changes.

To contribute a new language, you will need to copy the [base.json](/langs/base.json) and rename it such that the filename is in the format "aa-AA.json" where:
- "aa" is the two-letter language code defined in [ISO 639](https://en.wikipedia.org/wiki/List_of_ISO_639_language_codes)
- "AA" is the two-letter regional code defined in [ISO 3166](https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes)

Regional dialects of languages are allowed too, such as en-US alongside en-GB.

## Translation Guide

Please remember that proper nouns, such as "Mega Hack" and "Geometry Dash", should not be translated.

Translations should not always be literal and instead should match common terms used by the community already. For example, do not translate "wave" if "wave" is the commonly spoken term in your language.

Titles for hacks and options should be kept as short as possible so that they fit in the interface. For Latin-based languages, 20 characters is a good estimate. However, this depends on character sizes so it isn't a strict guideline.

Any tags ending in `/PRE` or `/SUF` are prefixes or suffixes to input boxes respectively. Prefixes should include spaces after their colons, for where user input begins. Parent tags do not need this space as this is the placeholder text, shown when the input box is empty.

```
{
  "EXAMPLE_INPUT": "Time (s):",
  "EXAMPLE_INPUT/PRE": "Time: ",
  "EXAMPLE_INPUT/SUF": "s"
}
```

Tags ending in `/TIP` are tooltips for UI elements.

Please do NOT change any of the tags, they are used to identify the translations.