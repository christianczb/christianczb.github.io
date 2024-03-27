---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: skills
    content:
      title: Skills
      text: ''
      # Choose a user to display skills from (a folder name within `content/authors/`)
      username: admin
    design:
      columns: '1'
  - block: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Research Officer
          company: School of Chemical Engineering, The University of Queensland
          company_url: 'https://chemeng.uq.edu.au/'
          company_logo: org-gc
          location: St Lucia, Queensland, Australia
          date_start: '2023-10-01'
          date_end: ''
          description: |2-
              Understanding gas diffusion within agglomerated carbon nanoparticles for electrochemical and supercapacitors applications.

              Responsibilities include:
              * Analysing carbon nanoparticle structures
              * Describing adsorption of diverse gases into the nanoparticle assembly
              * Computing diffusion coefficients of such gases through the nanoparticle assembly
        - title: Teaching Assistant/Tutor 
          company: School of Chemical Engineering, The University of Queensland
          company_url: 'https://chemeng.uq.edu.au/'
          company_logo: org-gc
          location: St Lucia, Queensland, Australia
          date_start: '2021-02-26'
          date_end: '2023-11-15'
          description: |2-
              Tutoring core Chemical Engineering courses
              
              Courses:
              * CHEE3002/2040: Heat and Mass Transfer
              * CHEE7113: Whole of Process Optimisation and Control
              * CHEE3005: Reaction Engineering
              * CHEE3007: Process Modelling and Control
    design:
      columns: '2'
  - block: accomplishments
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Accomplish&shy;ments'
      subtitle:
      # Date format: https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: https://www.coursera.org
          date_end: ''
          date_start: '2015-01-15'
          description: ''
          icon: coursera
          organization: Coursera
          organization_url: https://www.coursera.org
          title: Programming for Everybody (Python)
          url: 'https://www.coursera.org/learn/python'
        - certificate_url: https://www.coursera.org
          date_end: ''
          date_start: '2015-01-25'
          description: ''
          icon: coursera
          organization: Coursera
          organization_url: https://www.coursera.org
          title: An Intuitive Introduction to Probability
          url: ''
    design:
      columns: '2'
  - block: collection
    id: posts
    content:
      title: Recent Posts
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 1
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
  - block: markdown
    content:
      title: Gallery
      subtitle: ''
      text: |-
        {{< gallery album="zeolites" >}}
    design:
      columns: '1'
  - block: collection
    id: featured
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
  - block: collection
    content:
      title: Recent Publications
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: tag_cloud
    content:
      title: Popular Topics
    design:
      columns: '2'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        Get in touch with me:
      # Contact (add or remove contact options as necessary)
      email: zuluagabedoya@gmail.com
      address:
        street: Andrew Liveris Building
        city: St Lucia 
        region: QLD
        postcode: '4072'
        country: Australia
        country_code: AU
      # Choose a map provider in `params.yaml` to show a map from these coordinates
      coordinates:
        latitude: '-27.4991584'
        longitude: '153.0138975'  
      contact_links:
        - icon: twitter
          icon_pack: fab
          name: DM Me
          link: 'https://twitter.com/christianczb'
        - icon: skype
          icon_pack: fab
          name: Skype Me
          link: 'skype:cristian.camilo.zuluaga'
        - icon: video
          icon_pack: fas
          name: Zoom Me
          link: 'https://uqz.zoom.us/my/christianczb'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '2'
---
