---
# Početna strana ("O projektu"), srpska verzija content/_index.md.
# Iste sekcije kao na engleskom; menja se samo tekst.
sections:
  - block: about-hero
    id: hero
    content:
      acronym: "DiNum-GEO"
      title: "Integracija digitalnih i numeričkih modela za optimizaciju u geotehnici"
      image: "home/about-illustration.jpg"
      image_alt: >-
        Ilustracija gradske lokacije u preseku: bušotine i slojevi tla čine
        osnovu digitalnog modela terena, mreža konačnih elemenata okružuje
        tunel, a veze podataka ga povezuju sa informacionim modelom objekta.

  - block: about-intro
    id: about
    content:
      title: "O projektu"
      lead: >-
        DiNum-GEO odgovara na izazove geološko-geotehničke neizvesnosti,
        optimizacije projektovanja i upravljanja rizicima u projektima
        podzemne gradnje kroz:
      items:
        - "Integraciju digitalnih modela terena i numeričkih modela"
        - "Uključivanje prostorne varijabilnosti tla u MKE simulacije primenom inovativnih geostatističkih algoritama"
        - "Potpuno interoperabilnu digitalnu računarsku platformu sa ažuriranjem modela"
        - "Pristup koji će služiti kao osnova za bezbednije projektovanje urbane infrastrukture"

  - block: about-objectives
    id: objectives
    content:
      title: "Istraživački ciljevi"
      items:
        - code: "RO1"
          title: "Digitalno informaciono modeliranje terena"
          text: "Geostatističko 3D modeliranje stratigrafije i prostorne varijabilnosti tla"
          icon: "home/objectives/ro1.png"
        - code: "RO2"
          title: "Numeričko modeliranje metodom konačnih elemenata"
          text: "Probabilističko MKE modeliranje podzemnih konstrukcija i interakcije tla i konstrukcije"
          icon: "home/objectives/ro2.png"
        - code: "RO3"
          title: "Razmena podataka"
          text: "Interoperabilan prenos podataka između GIM i MKE alata"
          icon: "home/objectives/ro3.png"
        - code: "RO4"
          title: "Veza sa informacionim modeliranjem objekata (BIM)"
          text: "Upravljanje podzemnim konstrukcijama i GIM-om zasnovano na BIM-u"
          icon: "home/objectives/ro4.png"
        - code: "RO5"
          title: "Validacija"
          text: "Procena uticaja neizvesnosti na odgovor konstrukcije"
          icon: "home/objectives/ro5.png"
    design:
      css_class: "dng-tint"

  - block: about-team
    id: team
    content:
      title: "Tim"
      # data/authors slugovi, redosled prikaza
      members:
        - milos
        - me
        - ksenija
        - jelena-ninic
        - tijana-jovanovic
      link: "team/"
      link_text: "Biografije na stranici Tim"

  - block: about-institutions
    id: institutions
    content:
      title: "Naučnoistraživačke organizacije"
      items:
        - name: "Građevinski fakultet, Univerzitet u Beogradu"
          logo: "media/partners/grf_logo.png"
          website: "https://web1.grf.bg.ac.rs/home"
          mark: "Vodeća NIO"
          highlight: true
          link: "team/#partner-grf"
        - name: "Univerzitet u Daramu"
          logo: "media/partners/durham_logo.png"
          website: "https://www.durham.ac.uk/"
          mark: "Partnerska NIO"
          link: "team/#partner-durham"
        - name: "Britanski geološki zavod"
          logo: "media/partners/bgs_logo.png"
          website: "https://www.bgs.ac.uk/"
          mark: "Partnerska NIO"
          link: "team/#partner-bgs"
    design:
      css_class: "dng-tint"

  - block: about-funding
    id: funding
    content:
      title: "Finansiranje"
      # Logotipi, tekst i podaci o projektu: data/sr/funding.yaml
---
