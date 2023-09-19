---
widget: portfolio
headless: true # This file represents a page section.

weight: 30

# ... Put Your Section Options Here (title etc.) ...
title: Réalisations
subtitle: ''

content:
  # Choose which content to display in the widget
  filters:
    # Folders to display content from
    folders:
      - realisations
    # Uncomment below to only show content with specific tags:
#    tags:
#      - Machine Learning
    # Uncomment below to exclude content with specific tags:
#    exclude_tags:
#      - preface    
    # Uncomment below to show specific Hugo Page kinds
    kinds:
      - page
#      - section

  # Field to sort by, such as Date or Title
  sort_by: 'Date'
  sort_ascending: false

  # Filter toolbar (optional).
  # Add or remove as many filters (`filter_button` instances) as you like.
  # To show all items, set `tag` to "*".
  # To filter by a specific tag, set `tag` to an existing tag name.
  # To remove toolbar, delete/comment all instances of `filter_button` below.
  filter_button:
    - name: Tous
      tag: '*'
    - name: web
      tag: web
    - name: espace public
      tag: espace-public
    - name: print
      tag: print

  # Default filter toolbar button (e.g. 0 corresponds to the first `filter_button` instance above)
  filter_default: 0

design:
  # Choose how many columns the section has. Valid values: '1' or '2'.
  columns: '1'
  # Choose a listing view
  view: masonry
  # For Showcase view, flip alternate rows?
  flip_alt_rows: false
---