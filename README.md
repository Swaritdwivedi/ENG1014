# Interactive Linear Regression Tutorial

This notebook provides an interactive, hands-on introduction to linear regression with visualizations and interactive widgets.

## Prerequisites

Before running this notebook, make sure you have the required packages installed. The notebook requires:

- Python 3.10+
- NumPy
- Matplotlib
- JupyterLab
- ipywidgets (for interactive sliders)

## Installation

### Option 1: Using Conda (Recommended)

If you're using the conda environment from `unit_info/installation/eng1014.yaml`, you'll need to install `ipywidgets`:

```bash
conda activate eng1014
conda install -c conda-forge ipywidgets
```

Or add it to your environment:

```bash
conda install ipywidgets
```

### Option 2: Using pip

```bash
pip install numpy matplotlib jupyterlab ipywidgets
```

## Running the Notebook

1. Start JupyterLab:
   ```bash
   jupyter lab
   ```

2. Open `linear_regression_interactive.ipynb`

3. Run all cells (Cell → Run All) or run them one by one

4. **Important**: Make sure to run the first cell (imports) before using any interactive widgets!

## Features

The notebook includes:

1. **Interactive Regression Line Explorer**: Adjust slope and intercept with sliders to see how they affect the line
2. **Cost Landscape Visualization**: See how Mean Squared Error changes with different parameters
3. **Noise and Outliers Impact**: Experiment with different noise levels and outliers
4. **Gradient Descent Visualization**: Watch how gradient descent finds optimal parameters
5. **Real-World Example**: Predict house prices based on size
6. **Hands-On Practice**: Try building your own regression model

## Troubleshooting

### Widgets not showing?

If the interactive widgets don't appear:

1. Make sure `ipywidgets` is installed:
   ```bash
   pip install ipywidgets
   ```

2. Enable the JupyterLab extension:
   ```bash
   jupyter labextension install @jupyter-widgets/jupyterlab-manager
   ```

3. Restart JupyterLab after installation

### Matplotlib style warnings?

The notebook uses `seaborn-v0_8-darkgrid` style. If you get a warning, you can:
- Install seaborn: `pip install seaborn`
- Or change the style in the first code cell to a built-in matplotlib style like `'default'` or `'ggplot'`

## Learning Path

1. Start with Part 1 to understand the basic concepts
2. Experiment with the sliders to see how parameters affect the line
3. Move through each section sequentially
4. Try modifying the code in Part 6 to experiment on your own

## Standalone HTML Page for GitHub

A standalone interactive HTML page (`regression_line_explorer.html`) is available for Part 1 of the tutorial. This page:
- Works directly in any web browser (no server needed)
- Can be hosted on GitHub Pages for easy student access
- Features interactive sliders for slope and intercept
- Shows real-time MSE and R² calculations
- Includes beautiful error visualization

**To set up on GitHub Pages**, see **[GITHUB_SETUP.md](GITHUB_SETUP.md)** for step-by-step instructions!

## Using in PowerPoint Presentations

Want to use these interactive graphs in your PowerPoint slides? See **[POWERPOINT_INTEGRATION.md](POWERPOINT_INTEGRATION.md)** for detailed instructions!

**⚠️ Important:** For **fully interactive widgets** (sliders that update graphs), use Voilà:
```bash
pip install voila
python export_with_voila.py
```

For static HTML (widgets won't update):
```bash
python export_for_powerpoint.py
```

## Additional Resources

- [Scikit-learn Linear Regression Documentation](https://scikit-learn.org/stable/modules/linear_model.html)
- [NumPy Documentation](https://numpy.org/doc/)
- [Matplotlib Gallery](https://matplotlib.org/stable/gallery/index.html)

Happy learning! 🎓

