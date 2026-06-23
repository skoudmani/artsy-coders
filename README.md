# Artsy Coders 🌌

An interactive Python workshop where you turn real astronomy data into pictures of the Universe. You'll learn `matplotlib` by **painting galaxies**, mapping supermassive black holes, and watching planets orbit. Perfect for curious coders and space enthusiasts.

## The workshop: three notebooks

The workshop is split into **three separate notebooks**. Run them in order, but each stands alone.

1. **`1_Plotting_Foundations.ipynb`**: a gentle warm-up in `matplotlib`: line plots, scatter plots, colour and style, and comparing multiple lines.
2. **`2_Painting_the_Galaxy.ipynb`**: *the core of the workshop.* Load a real supercomputer galaxy simulation and visualise it: 2D maps, stars, gas-density images (`imshow`), an edge-on view, a 3D rotation animation, and a "your turn" supermassive-black-hole-binary challenge.
3. **`3_Run_Your_Own_Simulation.ipynb`**: a hands-on bonus: run your own N-body gravity simulation of a mini solar system and experiment with it (add planets, change speeds and masses), plus optional 3D and "tiny-changes-wild-results" demos. No physics background needed — just run and play.

## Built for any classroom 🛟

These notebooks are designed to be extremely robust and can deal with kernel restarts, network interruptions etc:

- **Every code cell is self-contained.** Each one imports its own libraries and (re)loads its own data, so any cell can be run on its own, in any order, any number of times.
- **No data, no problem.** The galaxy notebook loads the provided data files if present, but falls back to a built-in synthetic galaxy if they're missing: so the visualisations always work, even if the environment loses the `data/` folder.
- If anything looks stuck: **Kernel → Restart**, then re-run just the cell you care about. No need to start from the top.

## Data

The galaxy notebook looks for data under:

```
data/galaxies/gas.csv      # columns: x, y, z, mass
data/galaxies/stars.csv    # columns: x, y, z, mass
data/smbhs/smbhs.csv       # columns: x, y, z, mass
data/smbhs/gas.csv         # columns: x, y, z, mass
```

If these files aren't available, the notebook automatically generates a stand-in galaxy so the workshop can run anyway.

## Requirements

See `requirements.txt` (`matplotlib`, `numpy`, `pandas`, `ipython`).

## Licence & credits

**Author: Dr Sophie Koudmani.** Licensed under the GNU General Public License v3.0 (GPLv3). Collaboration is encouraged. These notebooks were prepared with the assistance of large language models; the core workshop ideas and educational concepts are the original work of the author.
