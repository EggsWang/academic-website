---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
# Biography
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
# Experience->Education Background
  - block: experience
    content:
      title: Education Background
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Master of Library Science
          company: Peking University
          company_url: 'https://www.pku.edu.cn'
          company_logo: org-gc
          location: Beijing, China
          date_start: '2022-09-01'
          date_end: ''
          description: |2-
              GPA: 3.72/4
              Core Units:
              * Research Methods: Qualitative & Quantitative, Academic Writing
              * Library Science: Library Science Theory, Research on Documentation, Information Resource Management, Seminar on Library Science Trends, Seminar on Public Libraries, Advanced Topic in Unser Research
              * Other Electives: Gender and Development (Sociology)
        - title: Bachelor of Engineering of Cyber Security
          company: Wuhan University
          company_url: 'http://www.whu.edu.cn'
          company_logo: org-x
          location: Wuhan, China
          date_start: '2018-09-01'
          date_end: '2022-06-30'
          description: |2-
              GPA:3.32/4
    
              Core Units:
              * Higher Mathematics, Database System, Programming, The Principle of Operating System, Cryptology
    design:
      columns: '2'
# ->Awards
# Publication
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
      title: Recent Writing
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
# Project
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
        - name: Library History
          tag: Library History
        - name: Other
          tag: Demo
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
# Recent&Upcoming Talks->Conference Attended
  - block: collection
    id: talks
    content:
      title: Conference Attended
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
  - block: collection
    id: posts
    content:
      title: Recent Posts
      subtitle: ''
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
  - block: markdown
    content:
      title: Gallery
      subtitle: ''
      text: |-
        {{< gallery album="demo" >}}
    design:
      columns: '1'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        Ask me anything! No matter it is about academics, daily life or other things!
      # Contact (add or remove contact options as necessary)
      email: ordinaryeggsy@gmail.com
      address:
        street: 5 Yiheyuan Road
        city: Haidian District
        region: Beijing
        postcode: '100060'
        country: China
        country_code: CN
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
