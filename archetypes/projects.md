+++
# ======================================================
# PYTHON PROJECT — REUSABLE ARCHETYPE FRONT MATTER
# ======================================================
# This front matter is optimized for:
# - SEO discoverability
# - Clean URL structure
# - Future automation
# - Filtering & taxonomy expansion
# - Hugo archetype compatibility
# ======================================================


# ------------------------------------------------------
# CORE PROJECT METADATA
# ------------------------------------------------------
# Title auto-generated from filename.
# Example: hugo new projects/tic-tac-toe.md
# → "tic-tac-toe" becomes title.
title = "{{ .Name }}"

# Creation timestamp (auto-generated).
date = "{{ .Date }}"

# Keep as draft until ready to publish.
draft = true

# Clean URL slug.
# Ensures lowercase, URL-safe formatting.
slug = "{{ .Name | urlize }}"


# ------------------------------------------------------
# PROJECT CLASSIFICATION
# ------------------------------------------------------
# These fields allow filtering, sorting,
# automation, and future structured analytics.

difficulty = "Beginner"       # beginner | intermediate | advanced
technology = "Python"         # python | django | flask | etc.
status = "In Progress"         # in-progress | revised | completed
estimated_hours = ""           # Total time invested
project_related = false        # Link to related project (true/false)


# ------------------------------------------------------
# SEO — SEARCH OPTIMIZATION FIELDS
# ------------------------------------------------------
# Flat structure used intentionally.
# Nested tables may break archetype parsing.

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
# - Code snippets & learning documentation
#
# This flat TOML structure ensures:
# ✔ Archetype stability
# ✔ SEO readiness
# ✔ No silent truncation
# ✔ Maximum portability
# ------------------------------------------------------
+++

# {{ .Name | title }}

## 1. Project Overview
Write a brief description in your own words.  
What does this project do? Why did you choose it?

## 2. Project Objective
- Learning goal: What Python concept(s) are you practicing?
- Expected output / functionality.

## 3. Core Python Concepts Learned
List and describe each concept in your own words:
- Variables & Data Types
- Loops & Conditionals
- Functions
- Lists / Dictionaries / Sets
- Modules / Libraries
- OOP (if applicable)

Include small personal examples.

## 4. Practical Implementation
Document key code snippets:

### Example snippet
def example_function():
    print("Hello, world!")
Explain why each piece works and your thought process.

## 5. Errors & Debugging
Problems encountered
Error messages
How you solved them
Lessons learned

## 6. Insights & Reflections
What worked well
What was tricky
How you can improve

## 7. Next Steps / Questions
Extensions or improvements
Things you’re curious to explore next
Open questions

## 8. Resources Used
Books, tutorials, documentation, StackOverflow links

## 9. Quick Notes / Tips (Optional)
Short, reusable tricks or observations

## 10. Version History (Optional)
v1.0: Initial project
v1.1: Added feature X

## 11. Evergreen Reminder
This log is revisitable and updatable.
Keep refining both your code and your notes.
