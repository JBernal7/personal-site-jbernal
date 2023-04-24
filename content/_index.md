---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:

  - block: v1/about  #v1/about #about.avatar
    id: about
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      # Override your bio text from `authors/admin/_index.md`?
    design:
      spacing:
        # Customize the section spacing. Order is top, right, bottom, left.
        padding: ["200px", "0", "180px", "0"]
     
#  - block: experience
#    content:
#      title: Experience
#      # Date format for experience
#      #   Refer to https://wowchemy.com/docs/customization/#date-format
#      date_format: Jan 2006
#      # Experiences.
#      #   Add/remove as many `experience` items below as you like.
#      #   Required fields are `title`, `company`, and `date_start`.
#      #   Leave `date_end` empty if it's your current employer.
#      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
#      items:
#        - title: CEO
#          company: GenCoin
#          company_url: ''
#          company_logo: org-gc
#          location: California
#          date_start: '2021-01-01'
#          date_end: ''
#          description: |2-
#              Responsibilities include:
#
#              * Analysing
#              * Modelling
#              * Deploying
#        - title: Professor of Semiconductor Physics
#          company: University X
#          company_url: ''
#          company_logo: org-x
#          location: California
#          date_start: '2016-01-01'
#          date_end: '2020-12-31'
#          description: Taught electronic engineering and researched semiconductor physics.
#    design:
#      # Choose how many columns the section has. Valid values: '1' or '2'.
#      columns: '2'
#      spacing:
#       # Customize the section spacing. Order is top, right, bottom, left.
#       padding: ["40px", "0", "20px", "0"]
        
  - block: markdown
    id: parallax1
    design:
      background:
        image:
          # Name of image in `assets/media/`.
          filename: jb_catching33.jpg
          # Apply image filters?
          filters:
            # Darken the image? Range 0-1 where 1 is transparent and 0 is opaque.
            brightness: 0.7
          #  Image fit. Options are `cover` (default), `contain`, or `actual` size.
          size: cover
          # Image focal point. Options include `left`, `center` (default), or `right`.
          position: center
          # Use a fun parallax-like fixed background effect on desktop? true/false
          parallax: true
          # Text color (true=light, false=dark, or remove for the dynamic theme color).
          text_color_light: true 
          

  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      buttons:
        - name: All
          tag: '*'
        - name: People & Nature
          tag: people-and-nature
        - name: Environment & Planning
          tag: environment-planning
        - name: Initiatives
          tag: initiatives
        - name: Macroecology
          tag: macroecology
        - name: Habitat Suitability Modeling
          tag: hsm
        - name: Other
          tag: Demo  
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: masonry
      # For Showcase view, flip alternate rows?
      flip_alt_rows: true
      
  - block: markdown
    id: parallax2
    design:
     background:
       image:
         # Name of image in `assets/media/`.
         filename: jb_catching33.jpg
         # Apply image filters?
         filters:
           # Darken the image? Range 0-1 where 1 is transparent and 0 is opaque.
           brightness: 0.7
         #  Image fit. Options are `cover` (default), `contain`, or `actual` size.
         size: cover
         # Image focal point. Options include `left`, `center` (default), or `right`.
         position: center
         # Use a fun parallax-like fixed background effect on desktop? true/false
         parallax: true
         # Text color (true=light, false=dark, or remove for the dynamic theme color).
         text_color_light: true
     spacing:
         # Customize the section spacing. Order is top, right, bottom, left.
         padding: ["200px", "0", "100px", "0"]
        
  - block: collection
    id: publications
    content:
     title: Publications
     filters:
       folders:
         - publication
       exclude_featured: false
    design:
     columns: '2'
     view: citation

  - block: collection
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card      
   

  - block: markdown
    id: parallax3
    design:
      columns: '1'
      background:
        image:
          # Name of image in `assets/media/`.
          filename: jb_catching33.jpg
          # Apply image filters?
          filters:
            # Darken the image? Range 0-1 where 1 is transparent and 0 is opaque.
            brightness: 0.7
          #  Image fit. Options are `cover` (default), `contain`, or `actual` size.
          size: cover
          # Image focal point. Options include `left`, `center` (default), or `right`.
          position: center
          # Use a fun parallax-like fixed background effect on desktop? true/false
          parallax: true
          # Text color (true=light, false=dark, or remove for the dynamic theme color).
          text_color_light: true

 
  - block: collection
    id: talks
    content:
      title: SciComm
      subtitle: 'Events, talks & more' 
      count: 3
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact


  - block: markdown
    id: parallax4
    design:
      background:
        image:
          # Name of image in `assets/media/`.
          filename: jb_catching33.jpg
          # Apply image filters?
          filters:
            # Darken the image? Range 0-1 where 1 is transparent and 0 is opaque.
            brightness: 0.6
          #  Image fit. Options are `cover` (default), `contain`, or `actual` size.
          size: cover
          # Image focal point. Options include `left`, `center` (default), or `right`.
          position: center
          # Use a fun parallax-like fixed background effect on desktop? true/false
          parallax: true
          # Text color (true=light, false=dark, or remove for the dynamic theme color).
          text_color_light: true

  - block: collection
    id: blog
    content:
      title: Recent Posts
      subtitle: 'Code, news, and reflections from a biologist'
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        folders:
          - post
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: compact
      columns: '2'
 
#  - block: markdown
#    content:
#      title: Gallery
#      subtitle: ''
#      text: |-
#        {{< gallery album="demo" >}}
#    design:
#      columns: '1'
 
#  - block: collection
#    content:
#      title: Recent Publications
#      text: |-
#        {{% callout note %}}
#        Quickly discover relevant content by [filtering publications](./publication/).
#        {{% /callout %}}
#      filters:
#        folders:
#          - publication
#       exclude_featured: true
#    design:
#      columns: '2'
#      view: citation
  
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
      # Contact (add or remove contact options as necessary)
      email: jessicabernal@uma.es
      address:
        street: Avenida Cervantes 2
        city: Malaga
        region: Andalusia
        postcode: '29071'
        country: Spain
        country_code: ES
        coordinates:
          latitude: 36.72
          longitude: -4.42
      # Automatically link email and phone or display as text?
      autolink: true
#      # Email form provider
#      form:
#       provider: netlify
#       formspree:
#         id:
#       netlify:
#         # Enable CAPTCHA challenge to reduce spam?
#         captcha: false
#    design:
#      columns: '2'
      
  - block: markdown
    id: parallax1
    design:
     background:
       image:
         # Name of image in `assets/media/`.
         filename: jb_catching33.jpg
         # Apply image filters?
         filters:
           # Darken the image? Range 0-1 where 1 is transparent and 0 is opaque.
           brightness: 0.7
         #  Image fit. Options are `cover` (default), `contain`, or `actual` size.
         size: cover
         # Image focal point. Options include `left`, `center` (default), or `right`.
         position: center
         # Use a fun parallax-like fixed background effect on desktop? true/false
         parallax: true
         # Text color (true=light, false=dark, or remove for the dynamic theme color).
         text_color_light: true 
---
