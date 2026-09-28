---
# Homepage ("About"). Each block below is one section; the layouts live in
# layouts/_partials/hbx/blocks/about-*/block.html and the styles in
# assets/css/hbx/blocks/about/style.css.
sections:
  - block: about-hero
    id: hero
    content:
      acronym: "DiNum-GEO"
      title: "Digital and Numerical Model Integration for Optimization in Geotechnics"
      image: "home/about-illustration.jpg"
      image_alt: >-
        Illustration of an urban site in cross-section: boreholes and soil
        layers feed a digital ground model, a finite element mesh surrounds a
        tunnel, and data links connect it to a building information model.

  - block: about-intro
    id: about
    content:
      title: "About the Project"
      lead: >-
        DiNum-GEO addresses challenges in geological-geotechnical uncertainty,
        design optimization and risk management in underground construction
        projects by:
      items:
        - "Integrating digital ground models and numerical models"
        - "Incorporating soil spatial variability into FEM simulations using innovative geostatistical algorithms"
        - "Featuring a fully interoperable digital computing platform with model updating"
        - "Proposing an approach that will serve as a basis for safer design of urban infrastructure"

  - block: about-objectives
    id: objectives
    content:
      title: "Research Objectives"
      items:
        - code: "RO1"
          title: "Digital Ground Information Modelling"
          text: "Geostatistical 3D modelling of stratigraphy and soil spatial variability"
          icon: "home/objectives/ro1.png"
        - code: "RO2"
          title: "Finite Element Numerical Modelling"
          text: "Probabilistic FEM modelling of underground structures and soil-structure interaction (SSI)"
          icon: "home/objectives/ro2.png"
        - code: "RO3"
          title: "Data Exchange"
          text: "Interoperable transfer between GIM and FEM tools"
          icon: "home/objectives/ro3.png"
        - code: "RO4"
          title: "Building Information Modelling Link"
          text: "BIM-based management of underground structures and GIM"
          icon: "home/objectives/ro4.png"
        - code: "RO5"
          title: "Validation"
          text: "Assessing the influence of uncertainty on structural response"
          icon: "home/objectives/ro5.png"
    design:
      css_class: "dng-tint"

  - block: about-team
    id: team
    content:
      title: "Team"
      # data/authors slugs, in display order
      members:
        - milos
        - me
        - ksenija
        - jelena-ninic
        - tijana-jovanovic
      link: "team/"
      link_text: "Full bios on the Team page"

  - block: about-institutions
    id: institutions
    content:
      title: "Scientific Research Organisations"
      items:
        - name: "Faculty of Civil Engineering, University of Belgrade"
          logo: "media/partners/grf_logo.png"
          website: "https://web1.grf.bg.ac.rs/home"
          mark: "Leading SRO"
          highlight: true
          link: "team/#partner-grf"
        - name: "Durham University"
          logo: "media/partners/durham_logo.png"
          website: "https://www.durham.ac.uk/"
          mark: "Partner SRO"
          link: "team/#partner-durham"
        - name: "British Geological Survey"
          logo: "media/partners/bgs_logo.png"
          website: "https://www.bgs.ac.uk/"
          mark: "Partner SRO"
          link: "team/#partner-bgs"
    design:
      css_class: "dng-tint"

  - block: about-funding
    id: funding
    content:
      title: "Funding"
      # Logos, text and grant facts come from data/funding.yaml (shared with the Team page).
---
