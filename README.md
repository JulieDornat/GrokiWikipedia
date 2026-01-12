# ACL Survey – Collaborative Project

## Project — Short description (state of the art)

This project performs a state-of-the-art comparative analysis of political-domain content in Grokipedia and Wikipedia. The study examines how political actors and events are represented, how sentiment and relations are expressed, and how reference choices differ across the two platforms.

### Motivation

Encyclopedias inform the public about a wide range of topics in a neutral manner and constitute central resources used in large language model (LLM) training. Grokipedia recently emerged as an AI-driven competitor, motivated in part by claims of Wikipedia's left-leaning bias. Grokipedia was created by a private entity owned by a public figure with strong partisan positions, raising questions about its neutrality and the potential downstream effects on LLMs trained using its content.

### Objectives

The project aims to examine political domain representations in Grokipedia and Wikipedia through a combination of quantitative and qualitative analyses. Specific objectives include:

- Examing the references on the subject
- Constructing a state of the art (SoTA)

## Project Structure
```
GrokiWikipedia/
├── acl_latex.tex       ← Main LaTeX file
├── acl.sty             ← ACL style file
├── acl_natbib.bst      ← ACL bibliography style
├── custom.bib          ← Project bibliography
├── figures/            ← Figures used in the paper
├── sections/           ← Sections of the paper
│   ├── intro.tex
│   ├── method.tex
│   └── results.tex
└── README.md
```

- acl_latex.tex : main file that includes sections and bibliography.
- sections/ : each section is in a separate file to make collaboration easier.
- figures/ : stores all images and graphics.
- custom.bib : BibTeX file for all references.

## Installation and Setup

### Option 1: VS Code (recommended)
1. Install VS Code
2. Install LaTeX
    - Windows: [MikTeX](https://miktex.org/download) or [TeX Live](https://www.tug.org/texlive/)
    - Mac: [MacTeX](http://www.tug.org/mactex/)
    - Linux: sudo apt install texlive-full
3. Install the LaTeX Workshop extension in VS Code.
4. Clone the repository in the local directory:

```bash
git clone https://github.com/JulieDornat/GrokiWikipedia.git
```
5. Compile the paper in VS Code:
    - Open acl_latex.tex
    - Click the Build LaTeX project button in LaTeX Workshop
    - The PDF will be generated automatically in the root folder

### Option 2: Overleaf
1. Create a new project on Overleaf → Upload Project
2. Upload all repository files, or link your GitHub repo directly to Overleaf (advanced)
3. Compilation is automatic, and you can edit files directly in Overleaf

## Contributing
To ensure smooth collaboration on GitHub.
Contributing

To ensure smooth collaboration on GitHub, follow these guidelines.

### Using GitHub and VS Code

1. Create a branch before working on a section or making changes:
```bash
git checkout -b my-branch
```

2. Add your changes:

```bash
git add .
git commit -m "Added method section (message you edited to explain on what you have worked)"
```
git status allows to visualize the state of the updated files.

3. Push your branch:
```bash
git push origin my-branch
```
origin can be GrokiWikipedia here. It correspond to the name of the remote directory.

4. Create a Pull Request (PR):

- Go to GitHub. It will suggest you to make a pull request.
- Team members can review, comment, and approve the PR before merging

⚠️Note: Pull request is typically done when we finish a task, including many commits. For example, writing an introduction necessitates several commits ("add problematic", "add catchphrase", etc ).

5. Keep your branch up to date (to do regularly)

```bash
git pull
```

### Using Overleaf

If you prefer to edit the paper on Overleaf:

1. Create a dedicated branch on GitHub for your changes, e.g., overleaf-intro.

2. Edit files on Overleaf as usual.

3. Download the updated files from Overleaf (usually the .tex files you changed).

4. Replace the corresponding files in your GitHub branch and commit.

5. Open a Pull Request to merge your Overleaf changes into main.

⚠️ Note: This method works but requires discipline: always make sure you are on the correct branch and overwrite only the files you modified. **Direct GitHub sync with Overleaf is cleaner**.

## References

- Template used: [Overleaf ACL Conference Template](https://www.overleaf.com/latex/templates/association-for-computational-linguistics-acl-conference/jvxskxpnznfj)

- LaTeX documentation: https://www.latex-project.org/help/documentation/

- Greenstein, Shane, and Feng Zhu. "Is Wikipedia Biased?." American Economic Review 102.3 (2012): 343-348.
- Yasseri, Taha, and Saeedeh Mohammadi. "How Similar Are Grokipedia and Wikipedia? A Multi-Dimensional Textual and Structural Comparison." arXiv preprint arXiv:2510.26899 (2025).
- Leung, Tin Cheuk, and Koleman S. Strumpf. "How AI Reshapes Human Content Creation: The Case of Grokipedia vs Wikipedia." Available at SSRN 5853062 (2025).

## Contributors

- Julie Dornat — Paris Saclay University