+++
# -----------------------
# Basic Info
# -----------------------
title = "{{ .Name }}"            # Auto-set from filename
subtitle = ""                    # Optional subtitle per post
date = "{{ .Date }}"             # Auto-set creation date
draft = true                     # Keep true until ready to publish
description = "Short description of the post."  # SEO / social sharing
tags = []                        # Add post-specific tags
categories = ["posts"]           # Keep in 'posts' section
ShowToc = true                   # Table of Contents
showReadingTime = true           # PaperMod reading time
showBreadCrumbs = true           # Show breadcrumbs
showPostNavLinks = true          # Enable previous/next post navigation

# -----------------------
# SEO / Social Sharing
# -----------------------
[seo]
twitter = "pirikli"         # Replace with your Twitter handle
facebook = "https://facebook.com/pirikli"  # Replace with Facebook page
image = "images/seo-share.jpg"       # Path to social sharing image
keywords = []                         # Post-specific SEO keywords
description = ""                      # Optional SEO description override

# -----------------------
# Extra Metadata
# -----------------------
aliases = []                          # Redirects if needed
slug = "{{ .Name | urlize }}"         # URL-friendly slug
+++
