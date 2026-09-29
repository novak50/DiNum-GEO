---
title: "Tim"
sections:
  - block: team-showcase
    id: team
    content:
      title: "Tim"
      user_groups:
        - Team
      # Order set by `weight:` in data/authors/*.yaml
      sort_by: weight
    design:
      show_role: true
      show_organizations: false
      show_interests: false
      show_social: true
      max_columns: 3
      align: center

  - block: markdown
    id: partners
    content:
      title: "Naučnoistraživačke organizacije"
      text: >-
        <div class="partner-details-wrap">
          <div class="partner-details-grid">
            <div class="partner-detail-card" id="partner-grf">
              <div class="partner-detail-logo">{{< relimg "media/partners/grf_logo.png" "Građevinski fakultet, Univerzitet u Beogradu" >}}</div>
              <p>Građevinski fakultet Univerziteta u Beogradu jedna je od vodećih akademskih institucija u Srbiji, posvećena obrazovanju, istraživanju i inovacijama u oblasti građevinarstva, geodezije i geoinformatike. Fakultet neguje povezivanje teorijskog znanja i praktične primene, podstiče međunarodnu saradnju i doprinosi razvoju infrastrukture i održivim praksama kroz vrhunska istraživanja i konsultantske usluge.</p>
            </div>
            <div class="partner-detail-card" id="partner-durham">
              <div class="partner-detail-logo">{{< relimg "media/partners/durham_logo.png" "Univerzitet u Daramu" >}}</div>
              <p>Univerzitet u Daramu je vodeći istraživački univerzitet u Velikoj Britaniji i član grupe Rasel (Russell Group). Globalno je prepoznat po istraživanju i obrazovanju u oblasti inženjerstva, prirodnih nauka i drugih disciplina, sa snažnim naglaskom na interdisciplinarnu saradnju. Raspolaže ekspertizom u računarskom inženjerstvu, numeričkom modeliranju i geotehničkom inženjerstvu, uz podršku naprednih računarskih resursa i snažne veze sa privredom i istraživačkim partnerima.</p>
            </div>
            <div class="partner-detail-card" id="partner-bgs">
              <div class="partner-detail-logo">{{< relimg "media/partners/bgs_logo.png" "Britanski geološki zavod" >}}</div>
              <p>Britanski geološki zavod (BGS) je nacionalna organizacija Velike Britanije posvećena pružanju geonaučne ekspertize kao podrške održivom upravljanju resursima, ublažavanju prirodnih hazarda i zaštiti životne sredine. BGS ima ključnu ulogu u unapređenju naučnog razumevanja procesa i sistema Zemlje, sprovodi primenjena istraživanja za održivi razvoj i održava nacionalne geološke baze podataka i karte.</p>
            </div>
          </div>
        </div>
        <style>
          .partner-details-wrap {
            width: 100vw;
            margin-left: calc(50% - 50vw);
            margin-right: calc(50% - 50vw);
            padding: 2rem 1.5rem 0;
            box-sizing: border-box;
          }
          .partner-details-grid {
            max-width: 80rem;
            margin: 0 auto;
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 2rem;
          }
          @media (max-width: 768px) {
            .partner-details-grid { grid-template-columns: 1fr; }
          }
          .partner-detail-card {
            scroll-margin-top: 6rem;
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
            gap: 1rem;
            padding: 1.75rem 1.5rem;
            border-radius: 0.75rem;
            background: rgba(0, 0, 0, 0.03);
          }
          .partner-detail-logo {
            height: 64px;
            display: flex;
            align-items: center;
            justify-content: center;
          }
          .partner-detail-logo img {
            max-height: 100%;
            max-width: 220px;
            width: auto;
            height: auto;
            object-fit: contain;
          }
          .partner-detail-card p {
            width: 100%;
            text-align: justify;
            hyphens: auto;
            -webkit-hyphens: auto;
            font-size: 0.9rem;
            line-height: 1.6;
            color: rgba(0, 0, 0, 0.7);
            margin: 0;
          }
          .dark .partner-detail-card { background: rgba(255, 255, 255, 0.06); }
          .dark .partner-detail-card p { color: rgba(255, 255, 255, 0.75); }
        </style>

  - block: about-funding
    id: funding
    content:
      title: "Finansiranje"
      # Logotipi, tekst i podaci o projektu: data/sr/funding.yaml
---
