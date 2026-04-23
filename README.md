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
| `020/` | Errors and Cancellation | [Slides](https://waseda-num-analysis-2026.github.io/materials/020/2nd.html) · [Handout](https://waseda-num-analysis-2026.github.io/materials/020/2nd-handout.html) · [Python Guidelines](https://waseda-num-analysis-2026.github.io/materials/020/python_guidelines/python_guidelines.html) | TBD |
| ...    | ... | ... | ... |

## Exercises

| # | Exercise | Link | Deadline |
|---|----------|------|----------|
| 1.1 | Hello GitHub | [Access](https://classroom.github.com/a/oobb4OWM) | Apr 17, 23:59 |
| 1.2 | Summarize How to Use GitHub | [Access](https://classroom.github.com/a/TeNDgSNv) | Apr 23, 23:59 |
| 2.1, 2.2 | Errors (one repo) | [Access](https://classroom.github.com/a/Xj_QQlK9) | Apr 24, 23:59 |
| 2.3 | Cancellation in Quadratic Equation (same repo as 2.1) | [Access](https://classroom.github.com/a/Xj_QQlK9) | Apr 30, 23:59 |

## Setup (one-time)

To run the Python code in handouts (e.g. `2nd-handout.qmd`), set up a virtual environment and install the required packages:

```bash
cd materials                       # move into the cloned folder
python3 -m venv .venv              # create a virtual environment
source .venv/bin/activate          # macOS / Linux
# .venv\Scripts\activate           # Windows (PowerShell)
pip install -r requirements.txt
```

> When you open this folder in **VS Code**, the Python extension will usually offer to use `.venv` automatically.
> If not, run the command palette → `Python: Select Interpreter` → choose `.venv`.

## Getting Updates

If you have already cloned this repository, run the following commands to get the latest materials:

```bash
cd materials   # move into the cloned folder
git pull
```

If `requirements.txt` has been updated, also run:

```bash
source .venv/bin/activate          # if not already activated
pip install -r requirements.txt
```

> If you haven't cloned yet, go back to **Mission 5** in the [Lecture 1 slides](https://waseda-num-analysis-2026.github.io/materials/010/1st.html).
