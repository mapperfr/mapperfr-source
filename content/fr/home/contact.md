---
# An instance of the Contact widget.
widget: contact

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 130

title: Contact
subtitle: Pour me joindre par email

content:
  # Automatically link email and phone or display as text?
  autolink: false
  
  # Email form provider
  form:
    provider: formspree
    formspree: 
      id: mnqwzevw
    netlify:
      # Enable CAPTCHA challenge to reduce spam?
      captcha: false

  # Contact details (edit or remove options as required)
  # email: 
  # phone: 
  address:
    # street: 
    # city: Marseille
    # region: 
    # postcode:
    # country: France
    # country_code: FR
  # coordinates:
  #   latitude: ''
  #   longitude: ''
  directions: 
  # office_hours:
  # appointment_url: 'https://calendly.com'
  contact_links:
    - icon: mastodon
      icon_pack: fab
      name: Me contacter sur Mastodon
      link: 'https://mapstodon.space/@jeremy'
    # - icon: video
    #   icon_pack: fas
    #   name: Zoom Me
    #   link: 'https://zoom.com'

design:
  columns: '2'
---
