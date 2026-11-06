## 2024-11-05 - Notebook Environment Setup Optimization
**Learning:** Google Colab notebook environments benefit significantly from reduced network downloads during initialization.
**Action:** When setting up environments in `.ipynb` files, always look for opportunities to reduce fetched data, such as using `git clone --depth 1` instead of a full clone, and `--profile minimal` for Rust installations.

## 2024-05-18 - Rejected Notebook Optimization
**Learning:** Build-time environment variable optimizations (like disabling debug symbols) inside Jupyter notebooks do not constitute valid runtime performance improvements for an application, especially if no core application code exists in the repository.
**Action:** Always ensure optimizations target the actual runtime execution speed of the application, and abort if the repository contains no application code to optimize.
