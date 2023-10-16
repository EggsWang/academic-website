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
          company_url: ''
          company_logo: org-gc
          location: Beijing, China
          date_start: '2022-09-01'
          date_end: ''
          description: |2-
              GPA: 3.72/4

              Core Units:

              * Library Theory
              * Seminar on Library Science Trend
              * Other
        - title: Bachelor of Engineering of Cyber Security
          company: Wuhan University
          company_url: ''
          company_logo: org-x
          location: Wuhan, China
          date_start: '2018-09-01'
          date_end: '2022-06-30'
          description: |2-
              GPA:3.32/4
              Core Units:
    design:
      columns: '2'
# Accomplishment->Research Interests
  - block: accomplishments
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      # e.g. title: 'Accomplish&shy;ments'
      title: Research Interests
      subtitle:
      # Date format: https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: https://www.coursera.org
          date_end: ''
          date_start: '2021-01-25'
          description: ''
          organization: Coursera
          organization_url: https://www.coursera.org
          title: Library History
          url: ''
        - certificate_url: https://www.edx.org
          date_end: ''
          date_start: '2021-01-01'
          description: Formulated informed blockchain models, hypotheses, and use cases.
          organization: edX
          organization_url: https://www.edx.org
          title: Sociology of Library
          url: https://www.edx.org/professional-certificate/uc-berkeleyx-blockchain-fundamentals
        - certificate_url: https://www.datacamp.com
          date_end: '2020-12-21'
          date_start: '2020-07-01'
          description: ''
          organization: DataCamp
          organization_url: https://www.datacamp.com
          title: Comparative Library Science
          url: ''
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
# Skill->Additional Information
  - block: features
    content:
      title: Additional Information
      items:
        - name: Language
          description: Chinese(native, traditional and simplified characters), English(efficient)
          icon: r-project
          icon_pack: fab
        - name: Hobby
          description: Accordian, Kendo
          icon: chart-line
          icon_pack: fas
        - name: Crazy
          description: 100%
          icon: camera-retro
          icon_pack: fas
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
      email: wangdanjun@stu.pku.edu.cn
      phone: 
      appointment_url: 'https://calendly.com'
      address:
        street: 5 Yiheyuan Road
        city: Haidian District
        region: Beijing
        postcode: '100060'
        country: China
        country_code: CN
      directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
      contact_links:
        - icon: twitter
          icon_pack: fab
          name: DM Me
          link: 'https://twitter.com/Twitter'
        - icon: skype
          icon_pack: fab
          name: Skype Me
          link: 'skype:echo123?call'
        - icon: video
          icon_pack: fas
          name: Zoom Me
          link: 'https://zoom.com'
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
