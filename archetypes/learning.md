+++
# ======================================================
# LEARNING LOG — REUSABLE ARCHETYPE FRONT MATTER
# ======================================================
# This front matter is optimized for:
# - SEO discoverability
# - Clean URL structure
# - Future automation
# - Filtering & taxonomy expansion
# - Hugo archetype compatibility
# ======================================================


# ------------------------------------------------------
# CORE POST METADATA
# ------------------------------------------------------
# Title auto-generated from filename.
# Example: hugo new learning/git-rebase.md
# → "git-rebase" becomes title.
title = "{{ .Name }}"

# Creation timestamp (auto-generated).
date = "{{ .Date }}"

# Keep as draft until ready to publish.
draft = true

# Clean URL slug.
# Ensures lowercase, URL-safe formatting.
slug = "{{ .Name | urlize }}"


# ------------------------------------------------------
# CONTENT CLASSIFICATION
# ------------------------------------------------------
# These fields allow filtering, sorting,
# automation, and future structured analytics.

difficulty = ""        # beginner | intermediate | advanced
technology = ""        # python | git | hugo | linux | etc.
status = ""            # in-progress | revised | completed
estimated_hours = ""   # Total time invested
project_related = false


# ------------------------------------------------------
# SEO — SEARCH OPTIMIZATION FIELDS
# ------------------------------------------------------
# Flat structure used intentionally.
# Nested tables (e.g. [seo]) may break archetype parsing.

seo_title = ""         
# Override title for search engines (optional)

seo_description = ""   
# 150–160 character summary for SERP snippets

seo_keywords = ""      
# Comma-separated keywords for indexing

seo_image = ""         
# Path to social preview image (e.g., images/share.jpg)

seo_twitter = ""       
# Twitter handle (without @)

seo_canonical_url = "" 
# Optional canonical URL if republishing


# ------------------------------------------------------
# FUTURE ROUTING / MAINTENANCE
# ------------------------------------------------------
aliases = ""           
# Old URLs for redirect (comma-separated if needed)


# ------------------------------------------------------
# INTERNAL NOTES
# ------------------------------------------------------
# Use the body of the template for:
# - Categories
# - Tags
# - Series grouping
# - Structured reflection
# - Learning documentation
#
# This flat TOML structure ensures:
# ✔ Archetype stability
# ✔ SEO readiness
# ✔ No silent truncation
# ✔ Maximum portability
# ------------------------------------------------------

+++


## Context

I encountered this topic while working on ________.
Initially, I was confused about ________.
This note documents what I currently understand and how I am using it.


---

## Core Concepts Covered

- 
- 
- 


---

## 🔹 Concept 1: __________

### What I Understood

Write the concept in your own words.
Keep it short and clear.
Avoid textbook definitions.


### Minimal Example

```python
# Clean example only
````

### Why This Matters in My Workflow

Explain where or why you would use this.
Mention one practical benefit or realization.

---

## 🔹 Concept 2: __________

### What I Understood

Short explanation in your own words.

### Minimal Example

```python
# Clean example only
```

### Why This Matters in My Workflow

How this improved your understanding or workflow.

---

## 🔹 Concept 3: __________

### What I Understood

Short explanation.

### Minimal Example

```python
# Clean example only
```

### Why This Matters in My Workflow

Where this fits into your learning journey.

---

## Mistakes or Misconceptions (Optional)

* I initially thought ________.
* I misunderstood ________.
* I was overcomplicating ________.

---

## Final Working Version (If Applicable)

```python
# Final clean script or configuration
```

---

## What Changed in My Understanding

* I now see that ________.
* I stopped doing ________.
* I prefer using ________ because ________.
* I still need to explore ________.

---

## Next Step

Next, I want to explore ________.

```

---

# How to Use This Efficiently

- Remove unused sections.
- Do not force 3 concepts if you only learned 1.
- If there’s no script, delete that section.
- Keep total writing time under 90 minutes.
- Publish without over-editing.

---

This template will:

- Keep your posts medium-sized (B-style).
- Show evolution.
- Build presence.
- Protect your learning time.

If you want next, I can design a **micro-version template** for very small learning logs (15–20 minute posts).
```

