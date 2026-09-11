<h1 align="center">🗺️ PhyloGeoPlot</h1>

<table align="center">
  <tr>
    <td valign="top" width="45%">

<details open>
<summary><strong>Table of Contents</strong></summary>

1. [📝 About the project](#-about-the-project)
2. [⚙️ Installation](#%EF%B8%8F-installation)
3. [📦 Dependencies](#-dependencies)
4. [💻 Basic usage](#-basic-usage)
5. [📖 Documentation](#-documentation)
6. [📚 Examples](#-examples)
7. [✅ Tests](#-tests)
8. [📋 License](#-license)
9. [✏️ Citation](#-citation)

</details>

    </td>
    <td valign="top" align="center" width="55%">
      <img src="https://raw.githubusercontent.com/tahiri-lab/PhyloGeoPlot/main/images/logo_phylogeoplot.jpg" alt="PhyloGeoPlot Logo" width="500">
    </td>
  </tr>
</table>

<p align="center">
  <img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="License: MIT">
  <img src="https://img.shields.io/badge/contributions-welcome-blue.svg" alt="Contributions">
  <img src="https://img.shields.io/badge/python-3.10+-blue.svg" alt="Python">
  <img src="https://img.shields.io/pypi/v/phylogeoplot.svg" alt="PyPI version">
  <img src="https://img.shields.io/badge/Documentation%20-%20GitHub%20Wiki-green.svg" alt="Documentation - GitHub Wiki">
</p>

<h2 align="center">A Python toolkit for phylogeographic visualization linking phylogenetic and geographic data</h2>

---

## 📝 About the project

**PhyloGeoPlot** is a powerful Python package for linked visualization of phylogenetic trees and geographic occurrence data. It connects taxa represented in a phylogenetic tree to their geographic coordinates and can optionally integrate environmental raster layers.

Key goals:
- simplify phylogeographic figure production;
- support publication-quality visual outputs;
- provide reproducible pipelines for biogeographic analyses.

## ⚙️ Installation

Install from PyPI:

```bash
pip install phylogeoplot
```

PhyloGeoPlot requires **Python >= 3.10**.

## 📦 Dependencies

Main dependencies are installed automatically with `pip`:

- Biopython
- Cartopy
- Rasterio
- Matplotlib
- Pandas
- NumPy
- scikit-image

## 💻 Basic usage

```python
from phylogeoplot.visualisation.tree_to_map_raster import PhyloGeoPlotter

plotter = PhyloGeoPlotter(
    nwk_file="sequences_tree.nwk",
    gps_file="coordinates.csv",
    offset_file="offsets.csv",
    raster_file="environment.tif",
    raster_band=1,
)

plotter.plot()
plotter.save(output_dir="output")
```

Raster input is optional.

## 📖 Documentation

Detailed documentation is available in the [PhyloGeoPlot Wiki](https://github.com/tahiri-lab/PhyloGeoPlot/wiki).

Useful pages:

- [Installation](https://github.com/tahiri-lab/PhyloGeoPlot/wiki/Installation)
- [Input Data](https://github.com/tahiri-lab/PhyloGeoPlot/wiki/Input-Data)
- [Preprocessing](https://github.com/tahiri-lab/PhyloGeoPlot/wiki/Preprocessing)
- [Visualization](https://github.com/tahiri-lab/PhyloGeoPlot/wiki/Visualization)
- [Examples](https://github.com/tahiri-lab/PhyloGeoPlot/wiki/Examples)
- [Testing and Development](https://github.com/tahiri-lab/PhyloGeoPlot/wiki/Testing-and-Development)
- [Troubleshooting](https://github.com/tahiri-lab/PhyloGeoPlot/wiki/Troubleshooting)
- [Citation](https://github.com/tahiri-lab/PhyloGeoPlot/wiki/Citation)

## 📚 Examples

The repository contains sample datasets and walkthrough notebooks for:

- Malagasy *Coffea*
- North Atlantic Cumacea

See the [Examples](https://github.com/tahiri-lab/PhyloGeoPlot/wiki/Examples) page for details.

## ✅ Tests

Run the test suite with:

```bash
python -m pytest -v
```

## 📋 License

PhyloGeoPlot is distributed under the [MIT License](https://github.com/tahiri-lab/PhyloGeoPlot/blob/main/LICENSE).

## ✏️ Citation

Citation information will be added here following publication.
