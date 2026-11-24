# Tomoaki Kameda — personal research website

Source of <https://kamecham.github.io/TomoakiKameda.github.io/>, built with Jekyll and the
[Beautiful Jekyll](https://github.com/daattali/beautiful-jekyll) theme (MIT License, see `LICENSE`).

## Pages

| File | Page |
| --- | --- |
| `index.md` | Home (About, Featured Research, News, Methods & Skills) |
| `projects.md` | Research |
| `publications.md` | Publications and presentations |
| `cv.md` | CV |
| `resume.md` | Teaching & Resources |
| `ja/index.md` | 日本語ページ |

## CV (PDF)

The LaTeX source is `_cv/Kameda_CV.tex` (ignored by Jekyll). Rebuild and copy the PDF:

```bash
latexmk -pdf -outdir=/tmp/cvbuild _cv/Kameda_CV.tex && cp /tmp/cvbuild/Kameda_CV.pdf assets/cv/
```

Keep it a public version: no home address, phone number, or date of birth.

## Local preview

```bash
bundle install
bundle exec jekyll serve --baseurl "" --livereload
```

Then open <http://localhost:4000/>.
