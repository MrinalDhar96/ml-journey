# ML Journey

Senior full-stack developer to machine learning foundations: a hands-on learning repo built around weekly notebooks, small experiments, and written reflections.

This repository currently covers Week 1: Python patterns for ML work and NumPy fundamentals. The goal is to rebuild core machine learning intuition from the ground up, with examples that connect familiar software engineering concepts to data pipelines, tensor operations, and model-building workflows.

## Current Focus

**Week 1: Dev Environment + NumPy**

- Refresh Python concepts commonly seen in ML codebases.
- Learn NumPy arrays, dtypes, reshaping, broadcasting, indexing, and vectorized math.
- Implement small matrix and normalization utilities from scratch.
- Use NumPy to treat images as tensors and perform real pixel-level transformations.

## Repository Structure

```text
.
├── README.md
└── Week 1 — Dev Environment + NumPy/
    ├── python_ml_refresher.ipynb
    ├── numpy_part_1_arrays.ipynb
    ├── numpy_part_2_indexing.ipynb
    ├── numpy_part_3_linear_algebra.ipynb
    └── mini_project_image_numpy_array.ipynb
```

## Notebooks

| Notebook | What it covers |
| --- | --- |
| `python_ml_refresher.ipynb` | List comprehensions, generators, decorators, `**kwargs`, and OOP patterns through an ML lens. Includes examples such as batch generators, pipeline configuration, and model-like class structure. |
| `numpy_part_1_arrays.ipynb` | NumPy array anatomy, dtypes, built-in initializers, reshaping, broadcasting rules, manual matrix addition, and scalar multiplication. |
| `numpy_part_2_indexing.ipynb` | Multidimensional slicing, boolean masking, fancy indexing, dataset shuffling, min-max normalization, and z-score standardization. |
| `numpy_part_3_linear_algebra.ipynb` | Dot products, matrix multiplication, transpose, inverse, determinants, eigen-decomposition, and solving linear systems. |
| `mini_project_image_numpy_array.ipynb` | Loads an image from the web and manipulates it as a NumPy tensor: grayscale conversion, flipping, rotation, cropping, brightness changes, clipping, and Matplotlib dashboard visualization. |

## Setup

### 1. Clone the repository

```bash
git clone <repo-url>
cd ml-journey
```

### 2. Create and activate a virtual environment

```bash
python3 -m venv .venv
source .venv/bin/activate
```

On Windows:

```bash
python -m venv .venv
.venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install numpy matplotlib pillow requests jupyter
```

Optional, if you prefer JupyterLab:

```bash
pip install jupyterlab
```

### 4. Start Jupyter

```bash
jupyter notebook
```

Or:

```bash
jupyter lab
```

Then open the notebooks inside `Week 1 — Dev Environment + NumPy/`.

## Suggested Learning Order

1. `python_ml_refresher.ipynb`
2. `numpy_part_1_arrays.ipynb`
3. `numpy_part_2_indexing.ipynb`
4. `numpy_part_3_linear_algebra.ipynb`
5. `mini_project_image_numpy_array.ipynb`

This order moves from language patterns to array fundamentals, then into indexing, linear algebra, and a small visual project.

## Key Concepts Practiced

- Vectorized computation instead of Python loops.
- Memory-aware array representation through `dtype`, shape, and views.
- Broadcasting rules for efficient tensor operations.
- Dataset-style row and feature extraction.
- Boolean masks for filtering and outlier handling.
- Fancy indexing for arbitrary row selection and shuffling.
- Feature scaling with min-max normalization and z-score standardization.
- Linear algebra primitives used in classical ML.
- Image manipulation as tensor manipulation.

## Mini Project: Image as a NumPy Array

The Week 1 mini project demonstrates how a real image can be represented as a 3D tensor with shape:

```text
(height, width, channels)
```

The notebook performs:

- Image loading using `requests` and `Pillow`.
- RGB tensor inspection with NumPy.
- Grayscale conversion using luminosity weights.
- Flip and rotation operations through slicing.
- Cropping through coordinate ranges.
- Brightness scaling with `np.clip`.
- Final visualization with `matplotlib.pyplot.subplots`.

## Progress

| Week | Topic | Status |
| --- | --- | --- |
| Week 1 | Dev Environment + NumPy | In progress |

## Notes

This is a learning repository, so notebooks intentionally include explanations, scratch implementations, and validation cells. The emphasis is not just using ML libraries, but understanding the array operations and mathematical building blocks that those libraries depend on.

