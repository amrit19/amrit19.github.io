---
layout: about
title: about
permalink: /

profile:
  align: right
  image: prof_pic.jpg
  image_circular: true # crops the image to make it circular

selected_papers: true # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page

announcements:
  enabled: true # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
---

I am a Software Development Engineer II in the Applied AI Solutions org at Amazon Web Services, where I build AI systems over petabyte-scale automotive and industrial data. For autonomous driving (ADAS/AV) teams, I work on a multi-modal video search system that helps developers surface rare edge cases across video, sensor and annotation data using plain-English queries. In the industrial space, I work on time series anomaly detection for predictive maintenance of equipment.

<div class="journey">
  <style>
    .journey ol { list-style: none; margin: 1.25rem 0 1.5rem; padding: 0; position: relative; }
    .journey ol::before { content: ""; position: absolute; left: 0.45rem; top: 0.4rem; bottom: 0.4rem; width: 2px; background: var(--global-divider-color); }
    .journey li { position: relative; padding: 0 0 1rem 1.75rem; }
    .journey li:last-child { padding-bottom: 0; }
    .journey li::before { content: ""; position: absolute; left: 0; top: 0.35rem; width: 0.95rem; height: 0.95rem; border-radius: 50%; background: var(--global-bg-color); border: 2px solid var(--global-theme-color); }
    .journey li.now::before { background: var(--global-theme-color); }
    .journey .when { font-size: 0.8rem; font-weight: 600; letter-spacing: 0.03em; text-transform: uppercase; color: var(--global-text-color-light); }
    .journey .what { font-weight: 600; }
    .journey .areas strong {
      font-weight: 700;
    }
    .journey .areas { font-size: 0.92rem; }
    .journey .tags { margin-top: 0.2rem; }
    .journey .tags a { font-size: 0.78rem; display: inline-block; margin: 0.15rem 0.3rem 0 0; padding: 0.05rem 0.55rem; border: 1px solid var(--global-theme-color); border-radius: 1rem; text-decoration: none; }
    .journey .tags a:hover { background: var(--global-theme-color); color: var(--global-bg-color); }
  </style>
  <ol>
    <li class="now">
      <div class="when">Now</div>
      <div class="what">Independent research: multi-agent LLMs</div>
      <div class="areas"><strong>Multi-Agent LLMs</strong> for inference-time preference elicitation and multi-agent fine-tuning</div>
      <div class="tags"><a href="{{ '/projects/' | relative_url }}">current research</a></div>
    </li>
    <li class="now">
      <div class="when">2024 – present</div>
      <div class="what">Amazon Web Services, Applied AI Solutions</div>
      <div class="areas"><strong>Deep Learning &amp; Information Retrieval</strong> for video search in ADAS/autonomous driving · <strong>Deep Learning &amp; Statistical Learning</strong> for anomaly detection in industrial predictive maintenance</div>
      <div class="tags"><a href="{{ '/cv/' | relative_url }}">experience</a></div>
    </li>
    <li>
      <div class="when">2022 – 2024</div>
      <div class="what">MS Informatics, Penn State, FAIR Lab</div>
      <div class="areas"><strong>Bayesian Statistics, Algorithm Design &amp; Multi-Agent AI</strong> for voting systems of humans and LLMs · Best MS Thesis Award in AI; NeurIPS 2024, WWW 2025, KDD 2026</div>
      <div class="tags"><a href="{{ '/publications/' | relative_url }}">publications</a><a href="{{ '/projects/' | relative_url }}">projects</a><a href="{{ '/teaching/' | relative_url }}">teaching</a></div>
    </li>
    <li>
      <div class="when">2020 – 2022</div>
      <div class="what">SAP Labs India</div>
      <div class="areas"><strong>Web Development</strong> for a next-generation payroll application in SAP SuccessFactors</div>
      <div class="tags"><a href="{{ '/cv/' | relative_url }}">experience</a></div>
    </li>
    <li>
      <div class="when">2019</div>
      <div class="what">Schneider Electric India, Summer Intern</div>
      <div class="areas"><strong>IoT, Mobile App &amp; Web Development</strong> for a door-entry system</div>
      <div class="tags"><a href="{{ '/cv/' | relative_url }}">experience</a></div>
    </li>
    <li>
      <div class="when">2016 – 2020</div>
      <div class="what">B.Tech Computer Science, NIT Rourkela</div>
      <div class="areas"><strong>Computer Vision &amp; Machine Learning</strong> for emotion recognition from human gait · CVIP 2021, ICCIS 2019</div>
      <div class="tags"><a href="{{ '/projects/' | relative_url }}">projects</a><a href="{{ '/publications/' | relative_url }}">publications</a></div>
    </li>
  </ol>
</div>

I completed my MS in Informatics (Data Science concentration) at [Penn State](https://ist.psu.edu/) in the [FAIR Lab](https://sites.google.com/view/fairailab), advised by [Dr. Hadi Hosseini](https://faculty.ist.psu.edu/hadi/). I was also mentored by and collaborated with [Dr. Debmalya Mandal](https://debmandal.github.io/). My thesis, [_Recovering Ground Truth Rankings When the Majority Is Misinformed_](https://etda.libraries.psu.edu/catalog/29018avp6267), won Best Master's Thesis on an AI-related topic at the Penn State AI Awards. This work on _surprisingly popular_ voting led to publications at [NeurIPS 2024](https://proceedings.neurips.cc/paper_files/paper/2024/hash/054e9f9a286671ababa3213d6e59c1c2-Abstract-Conference.html), [WWW 2025](https://doi.org/10.1145/3696410.3714707) and [KDD 2026](https://doi.org/10.1145/3770855.3817549). Before that, I earned my B.Tech in Computer Science and Engineering from [NIT Rourkela](https://www.nitrkl.ac.in/), where I did my undergraduate thesis in the Intelligent Computing and Computer Vision group with [Dr. Anup Nandy](https://www.nitrkl.ac.in/CS/~nandya/).

More broadly, I am interested in:

- Computational social choice: recovering ground truth from noisy, disagreeing preferences through rank aggregation and _surprisingly popular_ voting
- Aligning AI with human preferences: preference elicitation and learning from human feedback for large language models
- Multi-agent LLM systems, including inference-time preference elicitation and multi-agent fine-tuning
- Probabilistic and Bayesian models of human behavior, such as Mallows and Plackett-Luce ranking models
- Multi-modal search and retrieval over large-scale video and sensor data

## academic service

- Reviewer, KDD 2026, Datasets and Benchmarks Track
- Reviewer, The ACM Web Conference (WWW) 2025, Main Track
