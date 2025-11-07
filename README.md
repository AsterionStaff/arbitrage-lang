# Arbitrage Language Files

A repository containing all **language files** used by the **Arbitrage** framework.

This repository serves as a centralized collection of localization files that provides support for multiple languages in Arbitrage Framework.

---

## Repository Structure

All language files must be located inside the `languages` directory:
```
arbitrage-lang/
└── languages/
├────── sh_english.lua
├────── sh_russian.lua
├────── ...
└── README.md
```

The main completed file in this repository is:

> **`languages/sh_russian.lua`**

It serves as the reference file for other translations.

---

## Adding a New Language

To add support for a new language:

1. Navigate to the `/languages` directory.
2. Duplicate an existing file (for example, `sh_english.lua`).
3. Rename the new file using the following format: `sh_<language>.lua`

Example:  
`sh_french.lua`, `sh_spanish.lua`, etc.

4. Open the new file in a text editor.
5. Update the language code and translated text inside the `Arbitrage.language:Add()` function.

Each file should follow this structure:

```lua
Arbitrage.language:Add("en", {
    name = "English"
}, {
    ["#example_key"] = "Example Text",
})
```

Change "en" to your language code (for example, "fr" for French) and replace "Example Text" with your translated content.
