---
title: "Team"
sections:
  - block: team-showcase
    id: team
    content:
      title: "Team"
      text: "The people currently working on DiNum-GEO."
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
            <div class="partner-item"><img src="/media/partners/ub_logo.png" alt="University of Belgrade"></div>
            <div class="partner-item"><img src="/media/partners/grf_logo.png" alt="Faculty of Civil Engineering, University of Belgrade"></div>
            <div class="partner-item"><img src="/media/partners/bgs_logo.png" alt="British Geological Survey"></div>
            <div class="partner-item"><img src="/media/partners/durham_logo.png" alt="Durham University"></div>
            <div class="partner-item" aria-hidden="true"><img src="/media/partners/ub_logo.png" alt=""></div>
            <div class="partner-item" aria-hidden="true"><img src="/media/partners/grf_logo.png" alt=""></div>
            <div class="partner-item" aria-hidden="true"><img src="/media/partners/bgs_logo.png" alt=""></div>
            <div class="partner-item" aria-hidden="true"><img src="/media/partners/durham_logo.png" alt=""></div>
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
