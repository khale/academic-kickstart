+++
widget = "portfolio"  # Use the Portfolio widget
headless = true  # This file represents a page section.
weight = 5

# ... Put Your Section Options Here (title etc.) ...
title = "Teaching"

[content]
  # Page type to display. E.g. project.
  page_type = "teaching"
  
  # Filter toolbar (optional).
  # Add or remove as many filters (`[[content.filter_button]]` instances) as you like.
  # To show all items, set `tag` to "*".
  # To filter by a specific tag, set `tag` to an existing tag name.
  # To remove toolbar, delete/comment all instances of `[[content.filter_button]]` below.
  
  # Default filter index (e.g. 0 corresponds to the first `[[filter_button]]` instance below).
  filter_default = 0
  
  [[content.filter_button]]
    name = "All"
    tag = "*"
  
  [[content.filter_button]]
    name = "Systems"
    tag = "systems"

  [[content.filter_button]]
    name = "Architecture"
    tag = "architecture"

  [[content.filter_button]]
    name = "HPC"
    tag = "hpc"

  [[content.filter_button]]
    name = "Virtualization"
    tag = "virt"

  [[content.filter_button]]
    name = "Security"
    tag = "security"

  [[content.filter_button]]
    name = "Seminars"
    tag = "seminar"


[design]
  # Choose how many columns the section has. Valid values: 1 or 2.
  columns = "2"

  # Toggle between the various page layout types.
  #   1 = List
  #   2 = Compact  
  #   3 = Card
  #   5 = Showcase
  view = 2

  # For Showcase view, flip alternate rows?
  flip_alt_rows = false
+++
