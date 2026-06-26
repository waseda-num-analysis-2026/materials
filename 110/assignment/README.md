# Exercise 10–12 — Lecture 11

Numerical Analysis 2026 / **Lecture 11** assignments in your Ex 10–12 GitHub Classroom repository.

You already have **Ex 10.0** (`integration-handout.qmd`) and **Ex 10.1** (`ex10-1.qmd`) in this repository. This README replaces the previous repo README with **Lecture 11** instructions.

---

## Step 1 — Copy Lecture 11 files from `materials`

After `git pull` in your cloned [`materials`](https://github.com/waseda-num-analysis-2026/materials) repository, copy **all three files** below into the **root** of this Ex 10–12 GitHub Classroom repository. **Overwrite** the existing `README.md`.

```bash
# From your cloned materials repo (adjust paths as needed):
cp 110/assignment/README.md /path/to/your-ex10-12-repo/
cp 110/assignment/ex11-1.qmd /path/to/your-ex10-12-repo/
cp 110/assignment/ex11-2.qmd /path/to/your-ex10-12-repo/
```

Or download from GitHub:
[`README.md`](https://github.com/waseda-num-analysis-2026/materials/blob/main/110/assignment/README.md),
[`ex11-1.qmd`](https://github.com/waseda-num-analysis-2026/materials/blob/main/110/assignment/ex11-1.qmd),
[`ex11-2.qmd`](https://github.com/waseda-num-analysis-2026/materials/blob/main/110/assignment/ex11-2.qmd).

---

## What to submit (Lecture 11)

| Exercise | File | What to do |
|---|---|---|
| **Ex 11.0** | `integration-handout.qmd` | Continue editing your copy. Add **≥ 3 Q&A blocks** on handout **§4–5** (Simpson's rule, Lagrange interpolation, Newton-Cotes). **Do not delete** your Ex 10.0 Q&A. |
| **Ex 11.1** | `ex11-1.qmd` | Complete Simpson's rule and convergence comparison. |
| **Ex 11.2** | `ex11-2.qmd` | Complete two-AI comparison and fact-checking on Runge's phenomenon. |

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

## Render (Lecture 11)

```bash
quarto render ex11-1.qmd
quarto render ex11-2.qmd
```

**IMPORTANT:** This creates `ex11-1.html`, `ex11-2.html`, and the corresponding `ex11-*_files/` directories. Commit and push the HTML files together with the source `.qmd` files.

---

## Submit (Lecture 11)

**Deadline (JST): Jul 2 (Thu), 23:59** — Ex 11.0, 11.1, and 11.2.

You may push as many times as you like before the deadline; the **last commit before the deadline** will be graded.

```bash
git add integration-handout.qmd
git add ex11-1.qmd ex11-2.qmd
git add ex11-1.html ex11-2.html ex11-1_files ex11-2_files
git commit -m "Submit Ex 11"
git push
```

**IMPORTANT:** After pushing, open your repository on GitHub and check that the rendered HTML files are visible in the browser.

---

## Need help?

- Mattermost: <https://class.s-top.dev/numerical-analysis-2026/channels/question>
- Materials repo: <https://github.com/waseda-num-analysis-2026/materials>
- Lecture 11 slides: <https://waseda-num-analysis-2026.github.io/materials/110/11th.html>
- Lecture 12 (same repository; deadline Jul 9) will be released in `120/assignment/` in the materials repo.
