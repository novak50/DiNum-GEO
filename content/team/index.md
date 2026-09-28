---
title: "Team"
sections:
  - block: team-showcase
    id: team
    content:
      title: "Team"
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
      title: "Partner Institutions"
      text: >-
        <div class="partner-details-wrap">
          <div class="partner-details-grid">
            <div class="partner-detail-card" id="partner-grf">
              <div class="partner-detail-logo">{{< relimg "media/partners/grf_logo.png" "Faculty of Civil Engineering, University of Belgrade" >}}</div>
              <p>The Faculty of Civil Engineering, University of Belgrade is one of the leading academic institutions in Serbia, dedicated to education, research, and innovation in civil engineering, geodesy, and geoinformatics. The faculty emphasizes the integration of theoretical knowledge and practical application, fosters international collaboration, and contributes to infrastructure development and sustainable practices through cutting-edge research and consulting services.</p>
            </div>
            <div class="partner-detail-card" id="partner-durham">
              <div class="partner-detail-logo">{{< relimg "media/partners/durham_logo.png" "Durham University" >}}</div>
              <p>Durham University is a leading research university in the United Kingdom and a member of the Russell Group. It is globally recognized for research and education across engineering, science and other disciplines, with a strong emphasis on interdisciplinary collaboration. It features expertise in computational engineering, numerical modelling and geotechnical engineering, supported by advanced computational facilities and strong links with industry and research partners.</p>
            </div>
            <div class="partner-detail-card" id="partner-bgs">
              <div class="partner-detail-logo">{{< relimg "media/partners/bgs_logo.png" "British Geological Survey" >}}</div>
              <p>The British Geological Survey (BGS) is the United Kingdom's national organization focused on delivering geoscience expertise to support sustainable resource management, natural hazard mitigation, and environmental protection. BGS plays a critical role in advancing scientific understanding of the Earth's processes and systems, conducting applied research for sustainable development, and maintaining national geological databases and maps.</p>
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
      title: "Funding"
      # Logos, text and grant facts come from data/funding.yaml (shared with the homepage).
---
