# Obsidian Formatting Reference

## Editing This Document

Always use str_replace to make targeted edits to this file. Never rewrite the whole file at once. Only the specific section being changed should be touched -- everything else must remain exactly as it is. If adding a new section, append it cleanly without disturbing existing content.

## Revisiting Existing Articles

When revising an article that was written earlier in the conversation, ask the user to paste the current version from Obsidian rather than relying on memory. The Obsidian version is always the authoritative source. Memory of earlier article content becomes less reliable as the conversation grows.

---

## Writing Style

Plain prose under clean headers. No callout boxes. No bullet points unless listing something genuinely list-like. Write like a Wikipedia article — clear, grounded, and matter of fact, but with enough warmth to fit a living world. Start the article body by referencing the article's name directly, as Wikipedia does. Weave links to related articles into the prose where natural. Leave gaps on purpose. Not everything needs to be explained.

Do not use em dashes anywhere in articles. This includes double hyphens (--) used as em dash replacements. Both are forbidden.

When a character's name carries a meaningful etymology relevant to their identity or role, include the meaning in parentheses directly after the name on first reference. Keep it brief and natural. Example: "Lucien (meaning light)" or "Edric (from an old word meaning prosperous ruler)".

---

## Article Template

Every article type uses the same base template. Headers are added or removed depending on what the article actually needs. Never leave an empty header in a finished article.

```markdown
---
type: 
region: 
status: draft
created: YYYY-MM-DD
last_updated: YYYY-MM-DD
tags: []
---
The [Name] is a...

## Description
---
## History
---
```

**type** — place / person / group / event / concept / item / resource

**region** — the primary region this belongs to

**status** — draft / active / archived

**tags** — apply from the Tag Registry only. Do not include `draft` as a tag — status handles that in the frontmatter.

No blank line between the frontmatter closing `---` and the start of the article body. Each header is followed immediately by a `---` dividing line, then the body text beneath it. Paragraphs are written as continuous blocks, not one sentence per line.

**Connections** is not a standard section. Only include it when there are important relationships that did not come up naturally in the article body and would otherwise be missing from the graph. Most articles will not need it. Obsidian builds the graph from any link anywhere in the document, so prose links are sufficient in the majority of cases.

---

## Linking Rules

Links use Obsidian's alias syntax when the article title does not fit naturally into the sentence. `[[Article Name|display text]]` — the left side is the exact article title, the right side is how it appears in the prose. For example, `[[Apiarianism|Apiarian]]` or `[[The Great Swamp|the Great Swamp]]`.

The first mention of any term in an article is linked. Subsequent mentions of the same term within the same article are plain text.

Alternative names and nicknames for a thing are also linked on their first use, even if the primary name has already been linked earlier in the same article. Example: if Mireblood is linked early in an article, the first use of Witchsap later in the same article still links back to the Mireblood article via `[[Mireblood|Witchsap]]`.

---

## Capitalization

Proper nouns are capitalized — named places, named groups, named events, named items with established identities. Examples: Mireblood, Witchsap, Verdant Veins, Cauldron Tap, Swampfolk.

Generic descriptors stay lowercase — "the swamp," "a witch hut," "the peat," "a village."

Cultural identity terms are capitalized the same way nationalities are — Swampfolk, Apiarian, Brackfolk.

---

## Tags and Frontmatter Redundancy

Type and region appear in both the frontmatter fields and the tags. This is intentional. Frontmatter fields enable filtering and search, while tags enable visual graph organization and color coding by group. Always ensure the two are consistent -- if the region field says Great Swamp, the tag should be `great-swamp`. Never let them contradict each other.

---

## Additional Headers by Type

Optional headers to add when an article genuinely needs them.

**Places** — `## Culture` `## Function`

**People** — `## Background` `## Role` `## Relationships`

**Groups** — `## Structure` `## Goals`

**Events** — `## Causes` `## Outcome` `## Aftermath`

**Concepts** — `## Origins` `## Significance`

---

## Tag Registry

Apply tags from this list only. To add a new tag, update this registry first.

### Type
`place` `person` `group` `event` `concept` `item` `resource`

### Region
`flower-forest` `great-swamp` `trading-town` `central-sea` `jungle` `southern-islands`

### Theme
`apiarianism` `verdant-veins` `maritime` `colonial` `magic` `trade` `piracy`

### Status
`stub` `active` `archived`
