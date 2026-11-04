# B.Tech AI & ML Mini Project LaTeX Template
## Academic Year: 2025 – 2026
## Department of Artificial Intelligence and Machine Learning
## Chaitanya Bharathi Institute of Technology, Hyderabad

---

## Folder Structure

```
BTech_AIML_MiniProject_2025_26/
├── main.tex               ← Entry point; compile this file
├── titlepage.tex          ← Title page
├── vision.tex             ← Institute & Department Vision/Mission
├── Declaration.tex        ← Student declaration certificate
├── bonafide.tex           ← Bonafide certificate (signed by guide & HOD)
├── abstract.tex           ← Abstract and keywords
├── acknowledgements.tex   ← Acknowledgements
├── Chapters.tex           ← All 6 chapters + Appendix
├── code_attachments.tex   ← Source code appendix
├── reference.bib          ← BibTeX references
├── cbit.png               ← CBIT logo (do not rename)
├── images/                ← Place all project images/figures here
│   └── berlin.jpg         ← Sample image (replace with your figures)
└── README.md              ← This file
```

---

## How to Get Started

### Step 1 – Fill in your details in `main.tex`

Open `main.tex` and update the following commands near the top:

```latex
\newcommand{\projecttitle}{ Title of the Mini Project }
\newcommand{\studentone}{Student Name 1 (Roll No: 160-1-XX-XXX-XXX)}
\newcommand{\studenttwo}{Student Name 2 (Roll No: 160-1-XX-XXX-XXX)}
\newcommand{\studentthree}{Student Name 3 (Roll No: 160-1-XX-XXX-XXX)}
\newcommand{\studentfour}{Student Name 4 (Roll No: 160-1-XX-XXX-XXX)}
\newcommand{\projectguide}{Name of the Guide}
\newcommand{\guidetitle}{Assistant Professor}
\newcommand{\depthod}{Dr. Name of HOD}
```

> If your team has fewer than 4 members, comment out unused `\studentX` lines
> and update `titlepage.tex`, `bonafide.tex`, and `Declaration.tex` accordingly.

---

### Step 2 – Write your content

Edit `Chapters.tex` to replace placeholder text with your actual content.  
The chapters are pre-structured as:

| Chapter | Title |
|---------|-------|
| 1 | Introduction |
| 2 | Literature Survey |
| 3 | System Design and Methodology |
| 4 | Implementation |
| 5 | Results and Discussion |
| 6 | Conclusion and Future Scope |
| Appendix | Code Attachments |

---

### Step 3 – Add your images

Place all figure files (`.png`, `.jpg`, `.pdf`) inside the `images/` folder and
reference them in your `.tex` files using:

```latex
\begin{figure}[H]
    \centering
    \includegraphics[width=0.8\textwidth]{your_figure_name.png}
    \caption{Your caption here}
    \label{fig:yourlabel}
\end{figure}
```

---

### Step 4 – Add references

Edit `reference.bib` to add your references in BibTeX format.  
Tip: Use **Google Scholar → Cite → BibTeX** to get formatted entries.

Cite in text using: `\cite{ref_key}`

---

### Step 5 – Compile

Compile using **pdfLaTeX + BibTeX**:

```
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

Or use **Overleaf** (recommended for beginners):
1. Zip the entire folder.
2. Upload to [overleaf.com](https://www.overleaf.com) → New Project → Upload.
3. Set compiler to `pdfLaTeX` and main document to `main.tex`.

---

## Notes

- Do **not** rename `cbit.png` — it is referenced directly in multiple `.tex` files.
- Use `\label{}` and `\ref{}` for cross-referencing figures, tables, and sections.
- Keep all changes in the designated `.tex` files; do not restructure the template.
