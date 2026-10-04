# Amrit Puhan's personal website: [amrit19.github.io](https://amrit19.github.io)

This is the source for my personal academic website. It covers my research on preference aggregation and _surprisingly popular_ voting, my publications (NeurIPS 2024, WWW 2025, KDD 2026), projects, CV, teaching and academic service.

I am a Software Development Engineer II in the Applied AI Solutions org at Amazon Web Services. I completed my MS in Informatics (Data Science concentration) at Penn State in the [FAIR Lab](https://sites.google.com/view/fairailab), and my B.Tech in Computer Science and Engineering at NIT Rourkela.

- Email: [amrit.puhan@outlook.com](mailto:amrit.puhan@outlook.com)
- [Google Scholar](https://scholar.google.com/citations?user=G1U8jiIAAAAJ) · [OpenReview](https://openreview.net/profile?id=~Amrit_Puhan1) · [LinkedIn](https://www.linkedin.com/in/amrit-puhan-2623a5154) · [GitHub](https://github.com/amrit19)
- [CV (PDF)](https://amrit19.github.io/assets/pdf/Amrit_Puhan_CV.pdf)

## Where the content lives

| What                            | File                                                                                       |
| ------------------------------- | ------------------------------------------------------------------------------------------ |
| About page and academic service | [`_pages/about.md`](_pages/about.md)                                                       |
| Publications                    | [`_bibliography/papers.bib`](_bibliography/papers.bib)                                     |
| News                            | [`_news/`](_news)                                                                          |
| Projects                        | [`_projects/`](_projects)                                                                  |
| CV page                         | [`_data/cv.yml`](_data/cv.yml)                                                             |
| CV PDF                          | [`assets/pdf/Amrit_Puhan_CV.pdf`](assets/pdf/Amrit_Puhan_CV.pdf)                           |
| Teaching & service, coursework  | [`_pages/teaching.md`](_pages/teaching.md), [`_pages/coursework.md`](_pages/coursework.md) |
| Social links                    | [`_data/socials.yml`](_data/socials.yml)                                                   |
| Site settings                   | [`_config.yml`](_config.yml)                                                               |

## Building and deploying

The site is built with [Jekyll](https://jekyllrb.com/) on the [al-folio](https://github.com/alshedivat/al-folio) v1 starter. Every push to `main` runs the deploy workflow, which builds the site into the `gh-pages` branch that GitHub Pages serves.

To preview locally:

```bash
bundle install
bundle exec jekyll serve   # then open http://localhost:4000
```

Template documentation from al-folio is kept in [`docs/`](docs/README.md).

## License

The site's code comes from al-folio and is under the [MIT License](LICENSE). The personal content (text, photos, CV and publications) is © Amrit Puhan, all rights reserved. See [NOTICE.md](NOTICE.md).
