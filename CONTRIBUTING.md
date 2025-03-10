# Contributing to Articles in Waypedia

[Português](./CONTRIBUTING.pt.md) · English

Thank you for your interest in contributing to Waypedia! To ensure consistency across all articles, please follow these guidelines.

## Creating an Article

Articles should be `.mdx` files and must be placed in the `src` folder. The file name must follow these rules:

- Use only lowercase letters
- Do not use accents, diacritics or special characters
- Avoid using more than one consecutive space, unless really necessary
- No spaces at the beginning or end of the name

## Organizing by Language

Place the article in the appropriate subfolder inside `src`:

- For articles in Portuguese: `src/pt/`
- For articles in English: `src/en/`

## File Structure

Each article must start with a _frontmatter_ formatted as follows:

```yml
---
id: "Unique article identifier (must be the same across translations)" # REQUIRED
title: "Article title" # REQUIRES
banner: "URL for a banner image" # optional
---
```

🔹 The `id` field must be identical for all translated versions of the articles.

## Updating `mappings.json`

After creating the article or adding a translation to it, add the following entry to `mappings.json`:

```json
"article-id": {
    "en": "english-article-file-name",
    "pt": "portuguese-article-file-name"
}
```

**⚠ Do not include .mdx at the end of the article name in this definition.**
If your article doesn't have a certain translation yet, you may put `null` (without quotation marks) in the place where the file name would be.

## Review and Pull Requests

> [!CAUTION]
> Before submitting your contribution, make sure all the rules have been followed.
> Otherwise, your pull request may be rejected.

If you have any questions, feel free to ask. Thank you for contributing to Waypedia!
