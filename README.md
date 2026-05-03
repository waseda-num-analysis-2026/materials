# Numerical Analysis 2026 — Course Materials

**Instructor:** TANAKA, Kazuaki (田中 一成)  
**Institute for Mathematical Science, Waseda University**

## About

This repository contains course materials for Numerical Analysis 2026 (Foundations and Exercises).

## Structure

Materials are organized by lecture number:

| Folder | Topic | Materials | Video |
|--------|-------|-----------|-------|
| `010/` | Orientation and Guidance | [Slides](https://waseda-num-analysis-2026.github.io/materials/010/1st.html) | [Watch](https://youtu.be/AS3yAQUdcLc) |
| `020/` | Errors and Cancellation | [Slides](https://waseda-num-analysis-2026.github.io/materials/020/2nd.html) · [Handout](https://waseda-num-analysis-2026.github.io/materials/020/2nd-handout.html) · [Python Guidelines](https://waseda-num-analysis-2026.github.io/materials/020/python_guidelines/python_guidelines.html) | [Watch](https://youtu.be/SKz0dKh1vtI) |
| `030/` | Floating-Point Numbers | [Slides](https://waseda-num-analysis-2026.github.io/materials/030/3rd.html) · [Handout](https://waseda-num-analysis-2026.github.io/materials/030/3rd-handout.html) | [Watch](https://youtu.be/9_d11bJozUY) |
| ...    | ... | ... | ... |

## Tutorial Videos

Short how-to videos to help you get started:

| Title | Link |
|-------|------|
| How to Use AI Chat? — Using Python Guidelines as an Example | [Watch](https://youtu.be/9gljhM3yI7Q) |

## Exercises

| # | Exercise | Link | Deadline |
|---|----------|------|----------|
| 1.1 | Hello GitHub | [Access](https://classroom.github.com/a/oobb4OWM) | Apr 17, 23:59 |
| 1.2 | Summarize How to Use GitHub | [Access](https://classroom.github.com/a/TeNDgSNv) | Apr 23, 23:59 |
| 2.0 | Evolve the Handout with AI (≥ 3 Q&A in `2nd-handout.qmd`, see [`AI_TUTOR.md`](AI_TUTOR.md)) | same repo as 2.1 | Apr 30, 23:59 |
| 2.1, 2.2 | Errors (one repo) | [Access](https://classroom.github.com/a/Xj_QQlK9) | Apr 24, 23:59 |
| 2.3 | Cancellation in Quadratic Equation | same repo as 2.1 | Apr 30, 23:59 |
| 3.0 | Evolve the Handout with AI (≥ 3 Q&A in `3rd-handout.qmd`, see [`AI_TUTOR.md`](AI_TUTOR.md)) | same repo as 3.1 | May 7, 23:59 |
| 3.1 | Normalized Floating-Point Numbers | [Access](https://classroom.github.com/a/tIfL0rKn) | May 7, 23:59 |
| 3.2 | $1+\eta-1$ in `float64` (+ video) | same repo as 3.1 | May 7, 23:59 |
| 3.3 | Where the Integer Grid Breaks | same repo as 3.1 | May 7, 23:59 |

## Setup (one-time)

To run the Python code in handouts (e.g. `2nd-handout.qmd`), you need
the packages listed in [`requirements.txt`](requirements.txt). Pick
**one** of the two options below.

### Option A — Virtual environment (recommended, safer)

Best if you also use Python for other classes/projects, because it
keeps each project's packages separate and avoids version conflicts.

```bash
cd materials                       # move into the cloned folder
python3 -m venv .venv              # create a virtual environment
source .venv/bin/activate          # macOS / Linux
# .venv\Scripts\activate           # Windows (PowerShell)
pip install -r requirements.txt
```

> ⚠️ **Don't forget to *use* the venv every time.** Creating `.venv`
> is not enough — Quarto and your code cells must actually run *inside*
> it, otherwise they silently fall back to your system Python.
>
> - **Terminal:** `source .venv/bin/activate` *before* `quarto render`
>   (every new shell).
> - **VS Code / Cursor:** Command Palette → `Python: Select Interpreter`
>   → pick `.venv`. New terminals will then auto-activate, and "Run
>   Cell" will use the venv.

### Option B — System Python (simpler, if you have no other Python projects)

If this is your only Python project and you don't worry about version
conflicts with other work, you can install packages directly into the
Python you already have:

```bash
cd materials
pip install -r requirements.txt
```

> ℹ️ With this option there's nothing to "activate" — Quarto and VS
> Code use your system Python automatically. The trade-off is that any
> future project sharing the same Python may clash with these
> versions.

## Getting Updates

If you have already cloned this repository, run the following commands to get the latest materials:

```bash
cd materials   # move into the cloned folder
git pull
```

If `requirements.txt` has been updated, also re-install:

```bash
# Option A users — activate the venv first if not already:
source .venv/bin/activate
# Both options:
pip install -r requirements.txt
```

> If you haven't cloned yet, go back to **Mission 5** in the [Lecture 1 slides](https://waseda-num-analysis-2026.github.io/materials/010/1st.html).
