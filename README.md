# oop_python

Object-oriented programming in Python, studied from the data model up:
notes, runnable experiments and tested katas, written as part of a deliberate
effort to deepen my fundamentals alongside my work as a Python backend
developer (Django, DRF, FastAPI).

## What this repo is
- Study notebooks: concepts worked through with small, runnable examples
- Katas (in progress): small backend-flavored tasks with pytest tests that
  check behavior *and* design constraints
- Every decision is tied back to the four pillars (encapsulation, abstraction,
  inheritance, polymorphism) and to composition, SOLID and DI
- Target: Python 3.12+, typed, checked with Ruff and Mypy

## What's inside
| Notebook | Topics |
|----------|--------|
| `10_single_inheritance.ipynb` | Inheritance, `isinstance()` / `issubclass()`, inheriting from `object`, `@classmethod` / `@staticmethod` with inheritance |
| `11_multiple_inheritance.ipynb` | Multi-level and multiple inheritance, MRO, operator overloading |
| `12_encapsulation_polymorphism_abstraction.ipynb` | Public / protected / private and name mangling, polymorphism, ABC and `@abstractmethod` |

Progress and the full roadmap live in [PROGRESS.md](PROGRESS.md).

## Running locally
    python -m venv .venv
    source .venv/bin/activate        # Windows: .venv\Scripts\activate
    pip install -r requirements.txt
    jupyter lab                      # open the notebooks
    pytest -q                        # run katas (once added)

## Why it exists
Real backend work rewards knowing what happens under the hood: why a Django
model field is a descriptor, how `super()` walks the MRO in a CBV with
mixins, what FastAPI's `Depends` is actually injecting. This repo is where I
build that intuition, one tested example at a time.
