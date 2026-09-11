<h1 align="center">🗺️ PhyloGeoPlot</h1>

<table>
<tr>
<th align="left">
<img width="441" height="1">
<p> 
<small>
<details open>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#-about-the-project">About the project</a></li>
    <li><a href="#%EF%B8%8F-installation">Installation</a></li>
    <li><a href="#-dependencies">Dependencies</a></li>
    <li><a href="#-basic-usage">Basic usage</a></li>
    <li><a href="#-documentation">Documentation</a></li>
    <li><a href="#-examples">Examples</a></li>
    <li><a href="#-tests">Tests</a></li>
    <li><a href="#-license">License</a></li>
    <li><a href="#-citation">Citation</a></li>
  </ol>
</details>
</small>
</p>
</th>
<th align="center">
<p> 
<small>
<img src="https://raw.githubusercontent.com/tahiri-lab/PhyloGeoPlot/main/images/logo_phylogeoplot.jpg" alt="PhyloGeoPlot Logo" width="220">
</small>
</p>
</th>
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

**PhyloGeoPlot** is a powerful Python package for linked visualization of phylogenetic trees and geographic occurrence data. It connects taxa represented in a phylogenetic tree to their geographic coo[...]

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

## 📧 Contact
Please email us at: <Nadia.Tahiri@USherbrooke.ca> for any questions or feedback.
