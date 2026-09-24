---
title: "Team"
sections:
  - block: team-showcase
    id: team
    content:
      title: "Team"
      user_groups:
        - Team
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
        <div class="partner-marquee" aria-label="Partner institutions">
          <div class="partner-track">
            <div class="partner-item">{{< relimg "media/partners/ub_logo.png" "University of Belgrade" >}}</div>
            <div class="partner-item">{{< relimg "media/partners/grf_logo.png" "Faculty of Civil Engineering, University of Belgrade" >}}</div>
            <div class="partner-item">{{< relimg "media/partners/bgs_logo.png" "British Geological Survey" >}}</div>
            <div class="partner-item">{{< relimg "media/partners/durham_logo.png" "Durham University" >}}</div>
            <div class="partner-item" aria-hidden="true">{{< relimg "media/partners/ub_logo.png" "" >}}</div>
            <div class="partner-item" aria-hidden="true">{{< relimg "media/partners/grf_logo.png" "" >}}</div>
            <div class="partner-item" aria-hidden="true">{{< relimg "media/partners/bgs_logo.png" "" >}}</div>
            <div class="partner-item" aria-hidden="true">{{< relimg "media/partners/durham_logo.png" "" >}}</div>
          </div>
        </div>
        <style>
          .partner-marquee {
            overflow: hidden;
            position: relative;
            width: 100%;
            padding: 1.5rem 0;
            -webkit-mask-image: linear-gradient(90deg, transparent, #000 8%, #000 92%, transparent);
            mask-image: linear-gradient(90deg, transparent, #000 8%, #000 92%, transparent);
          }
          .partner-track {
            display: flex;
            align-items: center;
            gap: 3rem;
            width: max-content;
            animation: partner-scroll 28s linear infinite;
          }
          .partner-marquee:hover .partner-track {
            animation-play-state: paused;
          }
          .partner-item {
            flex: 0 0 auto;
            display: flex;
            align-items: center;
            justify-content: center;
            height: 84px;
            padding: 0.75rem 2rem;
            border-radius: 0.75rem;
            background: rgba(0, 0, 0, 0.04);
            white-space: nowrap;
          }
          .partner-item img {
            max-height: 52px;
            max-width: 220px;
            width: auto;
            height: auto;
            filter: grayscale(1);
            opacity: 0.75;
            transition: filter 0.2s, opacity 0.2s;
          }
          .partner-item:hover img {
            filter: none;
            opacity: 1;
          }
          @media (prefers-color-scheme: dark) {
            .partner-item { background: rgba(255, 255, 255, 0.08); color: #e5e7eb; }
          }
          @keyframes partner-scroll {
            from { transform: translateX(0); }
            to { transform: translateX(-50%); }
          }
        </style>

        <div class="partner-details-wrap">
          <div class="partner-details-grid">
            <div class="partner-detail-card">
              <div class="partner-detail-logo">{{< relimg "media/partners/grf_logo.png" "Faculty of Civil Engineering, University of Belgrade" >}}</div>
              <p>The Faculty of Civil Engineering, University of Belgrade is one of the leading academic institutions in Serbia, dedicated to education, research, and innovation in civil engineering, geodesy, and geoinformatics. The faculty emphasizes the integration of theoretical knowledge and practical application, fosters international collaboration, and contributes to infrastructure development and sustainable practices through cutting-edge research and consulting services.</p>
            </div>
            <div class="partner-detail-card">
              <div class="partner-detail-logo">{{< relimg "media/partners/durham_logo.png" "Durham University" >}}</div>
              <p>Durham University is a leading research university in the United Kingdom and a member of the Russell Group. It is globally recognized for research and education across engineering, science and other disciplines, with a strong emphasis on interdisciplinary collaboration. It features expertise in computational engineering, numerical modelling and geotechnical engineering, supported by advanced computational facilities and strong links with industry and research partners.</p>
            </div>
            <div class="partner-detail-card">
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
            font-size: 0.9rem;
            line-height: 1.6;
            color: rgba(0, 0, 0, 0.7);
            margin: 0;
          }
          @media (prefers-color-scheme: dark) {
            .partner-detail-card { background: rgba(255, 255, 255, 0.06); }
            .partner-detail-card p { color: rgba(255, 255, 255, 0.75); }
          }
        </style>

  - block: markdown
    id: funding
    content:
      title: "Funding"
      text: >-
        DiNum-GEO is funded by the **Science Fund of the Republic of
        Serbia**, under the *Dijaspora* 2024 programme (Support for
        Research Visits of Scientists from the Diaspora).


        [Visit the Science Fund of the Republic of Serbia →](https://fondzanauku.gov.rs/?lang=en)
---
