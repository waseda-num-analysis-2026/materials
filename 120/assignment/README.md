# Exercise 10–12 — Lecture 12

Numerical Analysis 2026 / **Lecture 12** assignments in your Ex 10–12 GitHub Classroom repository.

**Ex 10** and **Ex 11** are already in this repository (handout Q&A, `ex10-1.qmd`, `ex11-1.qmd`, `ex11-2.qmd`, etc.). This README replaces the previous repo README with **Lecture 12** instructions.

---

## Step 1 — Copy Lecture 12 files from `materials`

After `git pull` in your cloned [`materials`](https://github.com/waseda-num-analysis-2026/materials) repository, copy **all three files** below into the **root** of this Ex 10–12 GitHub Classroom repository. **Overwrite** the existing `README.md`.

```bash
# From your cloned materials repo (adjust paths as needed):
cp 120/assignment/README.md /path/to/your-ex10-12-repo/
cp 120/assignment/ex12-1.qmd /path/to/your-ex10-12-repo/
cp 120/assignment/ex12-2.qmd /path/to/your-ex10-12-repo/
```

Or download from GitHub:
[`README.md`](https://github.com/waseda-num-analysis-2026/materials/blob/main/120/assignment/README.md),
[`ex12-1.qmd`](https://github.com/waseda-num-analysis-2026/materials/blob/main/120/assignment/ex12-1.qmd),
[`ex12-2.qmd`](https://github.com/waseda-num-analysis-2026/materials/blob/main/120/assignment/ex12-2.qmd).

---

## What to submit (Lecture 12)

| Exercise | File | What to do |
|---|---|---|
| **Ex 12.0** | `integration-handout.qmd` | Continue editing your copy. Add **≥ 3 Q&A blocks** on handout **§6–7** (Hermite interpolation, Gauss quadrature). **Do not delete** prior Q&A from Ex 10.0 / Ex 11.0. |
| **Ex 12.1** | `ex12-1.qmd` | Complete Gauss-Chebyshev quadrature. |
| **Ex 12.2** | `ex12-2.qmd` | Complete comparison of trapezoidal, Simpson, and Gauss-Legendre methods. |

Handout reference:
[`100/integration-handout.qmd`](https://github.com/waseda-num-analysis-2026/materials/blob/main/100/integration-handout.qmd)
· Q&A protocol:
[`AI_TUTOR.md`](https://github.com/waseda-num-analysis-2026/materials/blob/main/AI_TUTOR.md)

---

## Setup

If you have not already set up the Python environment for this repository:

```bash
python3 -m venv .venv
source .venv/bin/activate          # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

Then select the `.venv` interpreter in VS Code / Cursor.

---

## Render (Lecture 12)

```bash
quarto render ex12-1.qmd
quarto render ex12-2.qmd
```

**IMPORTANT:** This creates `ex12-1.html`, `ex12-2.html`, and the corresponding `ex12-*_files/` directories. Commit and push the HTML files together with the source `.qmd` files.

---

## Submit (Lecture 12)

**Deadline (JST): Jul 9 (Thu), 23:59** — Ex 12.0, 12.1, and 12.2.

You may push as many times as you like before the deadline; the **last commit before the deadline** will be graded.

```bash
git add integration-handout.qmd
git add ex12-1.qmd ex12-2.qmd
git add ex12-1.html ex12-2.html ex12-1_files ex12-2_files
git commit -m "Submit Ex 12"
git push
```

**IMPORTANT:** After pushing, open your repository on GitHub and check that the rendered HTML files are visible in the browser.

---

## Need help?

- Mattermost: <https://class.s-top.dev/numerical-analysis-2026/channels/question>
- Materials repo: <https://github.com/waseda-num-analysis-2026/materials>
- Lecture 12 slides: <https://waseda-num-analysis-2026.github.io/materials/120/12th.html>
