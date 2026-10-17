# AI Programming Foundations — Data Workflow Project

A complete, reproducible data workflow in a single Jupyter notebook: loading a
tabular dataset from CSV, cleaning it with documented and reusable functions,
exploring it with summary and correlation functions, and visualizing the
results in four labelled figures. The analysis asks how well four flower
measurements distinguish three iris species, and finds that petal measurements
separate them almost completely while sepal measurements do not.

**Dataset:** [Iris](https://archive.ics.uci.edu/dataset/53/iris) — UCI Machine
Learning Repository (150 rows, 5 columns). [`iris.csv`](iris.csv) is the same data with a header row added. Section 2.1 of the notebook provides a `refresh_from_source()`
utility that re-downloads the published file and checks it against a recorded
SHA-256 digest; it is not run as part of the analysis.

## Files

| File | Contents |
|---|---|
| `data_workflow.ipynb` | The full analysis |
| `iris.csv` | The dataset the notebook loads |
| `requirements.txt` | Pinned dependency versions |
| `module_summary.pdf` | Written report with citations |

## How to run

**1. Clone the repository**

```bash
git clone https://github.com/tcolo/ai-programming-foundations-project.git
cd ai-programming-foundations-project
```

**2. Create and activate a virtual environment**

```bash
python3 -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate
```

**3. Install dependencies**

```bash
pip install -r requirements.txt
```

**4. Open and run the notebook**

```bash
jupyter lab data_workflow.ipynb
```

Then choose **Run → Restart Kernel and Run All Cells**. The notebook runs top to
bottom with no manual steps and no network access; it reads only `iris.csv` from
this folder.


## Requirements

Python 3.12 or newer, which is the floor set by the pinned package versions.
Developed and tested on Python 3.14.3.
