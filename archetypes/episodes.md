+++
# -----------------------
# Basic Info
# -----------------------
title = "{{ .Name }}"            # Auto-set from filename
subtitle = ""                    # Optional subtitle per episode
date = "{{ .Date }}"             # Auto-set creation date
draft = true                     # Keep true until ready to publish
description = "Short description of the episode."  # SEO / social sharing
tags = []                        # Add episode-specific tags
categories = ["episodes"]        # Keep in 'episodes' section
ShowToc = true                   # Table of Contents
showReadingTime = true           # PaperMod reading time
showBreadCrumbs = true           # Show breadcrumbs
showPostNavLinks = true          # Enable previous/next post navigation

# -----------------------
# SEO / Social Sharing
# -----------------------
[seo]
twitter = "YourTwitterHandle"       # Replace with your Twitter handle
facebook = "https://facebook.com/yourpage"  # Replace with Facebook page
image = "images/seo-share.jpg"     # Path to social sharing image
keywords = []                       # Episode-specific SEO keywords
description = ""                    # Optional SEO description override

# -----------------------
# Extra Metadata
# -----------------------
aliases = []                        # Redirects if needed
slug = "{{ .Name | urlize }}"       # URL-friendly slug
+++
