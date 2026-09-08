# Yang Hong's academic homepage

Personal website for Yang Hong, who is currently building a startup and has a research background in AI and cybersecurity. Incoming M.S. student in Security Informatics at Johns Hopkins University. Built with Jekyll for GitHub Pages, with an academic layout inspired by [Rui Yang's homepage](https://yangrui2015.github.io/).

## Local preview

Use Ruby 3.3 and Bundler. On macOS, Homebrew Ruby can be selected for the current terminal with `export PATH="/opt/homebrew/opt/ruby@3.3/bin:$PATH"`.

```sh
bundle config set --local path vendor/bundle
bundle install
bundle exec jekyll serve --host 127.0.0.1
```

Open http://127.0.0.1:4000. To build the production site:

```sh
JEKYLL_ENV=production bundle exec jekyll build
```

GitHub Pages publishes from the root of the default branch, `master-/root`, at https://expiol.github.io/. Pushing to this branch triggers a site build. Generated `_site/` output and local dependencies are not committed.

## Updating content

- `_config.yml`: name, email, photo, location, site URL, and publishing settings.
- `_pages/about.md`: introduction, research interests, and news.
- `_data/academic.yml`: public education, brief research experience, internships, and publication groups. This data is shared by the homepage and CV. Keep private CV details out of this file.
- `_publications/`: one Markdown file per paper. The homepage, publications page, and CV all read this collection. Use an existing file as a template, with `authors`, `topic`, `date`, `venue_short`, `summary`, `paperurl`, and `bibtex`. Optional `arxiv` and `pdfurl` fields enable preprint and PDF links.
- `_pages/cv.md`: a brief HTML CV showing education, institutions and roles, and paper titles. Omit task-level work descriptions, skills inventories, and detailed project contributions. The source CV PDF remains private: do not copy it into the repository or add a download link. Its former public path is also excluded from the build.
- `assets/css/academic.css`: responsive layout and print styles; no JavaScript or Node build is needed.
- `_layouts/academic.html` and `_includes/academic/`: shared page structure and rendering.

Existing `/`, `/publications/`, `/cv/`, and TrustCom publication URLs are retained. `/about/`, `/about.html`, and `/resume` redirect to their current pages. Unused Academic Pages sample content is retained in the repository but excluded from the generated site via `_config.yml`.

## Content sources

Only the owner's selected public background is included. Current status: building a startup and an incoming JHU student. Keep the planned Spring 2027 start in the education section; the introduction only needs the incoming-student status. The JHU work is a research collaboration primarily with Ph.D. student Rui Yang, currently paused with plans to resume after enrollment. Mention Prof. Yinzhi Cao as a paper co-author and link to his official JHU faculty page. Publication author lists remain unchanged. The two added preprints use arXiv's titles, author order, dates, and links:

- [Same Request, Different Boundary](https://arxiv.org/abs/2609.00578)
- [SoK: When Safe Agents Fail Together](https://arxiv.org/abs/2609.00595)
- [PentestLLM, COMPSAC 2026](https://doi.org/10.1109/COMPSAC69091.2026.00095): venue and author order verified against the publisher's [Crossref record](https://api.crossref.org/works/10.1109/COMPSAC69091.2026.00095). The published author order differs from the supplied CV; the website follows the publication record.
- [LLMs for CTF challenge solving, TrustCom 2024](https://doi.org/10.1109/TrustCom63139.2024.00213): existing publication record, with full author names from the CV.

## Credits

Originally based on [Academic Pages](https://github.com/academicpages/academicpages.github.io), which builds on [Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes). See `LICENSE` for the original MIT license.
