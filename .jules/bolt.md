## 2024-11-05 - Notebook Environment Setup Optimization
**Learning:** Google Colab notebook environments benefit significantly from reduced network downloads during initialization.
**Action:** When setting up environments in `.ipynb` files, always look for opportunities to reduce fetched data, such as using `git clone --depth 1` instead of a full clone, and `--profile minimal` for Rust installations.
