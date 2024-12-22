# Importing rust functions/modules in Python

- [install Pixi](https://pixi.sh/dev/)
- create a new project: 
```
pixi init rustlib
```
- install dependencies:
```
pixi add rust python jupyter ipykernel maturin pip
```
- init cargo project (choose pyo3):
```
pixi run maturin init
```
- build rustlib module:
```
pixi run maturin build
```
- pip install rustlib from wheel file:
```
pixi run pip install target/wheels/rustlib-(...).whl
```
- import rustlib module into Python and execute underlying functions 