# latex-titlepage-wwu
Titlepage for Latex following the WWU Corporate Design

## Installation

Copy `wwutitlepage.sty` and `wwucd` in `/path/to/texmf/tex/latex/wwutitlepage`. Note: on macOS `texmf` folder needs to be created at `~/Library/texmf`.

Install dependencies using `tlmgr` (background, everypage).

[Download](https://sso.uni-muenster.de/imperia/md/content/wwu/cd/download/print/wwu-brief-2017_fuer_latex.zip) the `Meta` font ([source](https://sso.uni-muenster.de/intern/post/schreibvorlagen.html)).

Install the Meta Font into texmf-local (read the `liesmich.txt` provided with the font and get the correct path via `kpsewhich --var-value TEXMFLOCAL`) and update tex filename database (`sudo -H mktexlsr`) and enable map (`sudo -H updmap-sys --enable Map=meta.map`).

## Usage

```
\wwutitlepage[color]{logo_of_institute.pdf}{title}{subtitle}
```
