# Assignment 3: Programming for AI

## How to run
1. Install Python 3 with `numpy`, `pandas` and `matplotlib`.
2. Put `Assignment3_Programming_for_AI.ipynb` and the `data/` folder (`sensor_cube.npy`, `sensor_meta.npz`, `weather_stations.csv`, `student_performance.csv`) in the same directory.
3. Open the notebook and choose **Kernel > Restart and Run All**.

Running the notebook creates `dashboard.png`, `dashboard.pdf` and `wave.gif` in the same folder.

## One thing that was hard
Cleaning the weather dates in Q4 was the hardest part. The file mixes `YYYY-MM-DD` and `DD/MM/YYYY`, and a plain `pd.to_datetime` misread 23 rows by treating the day as the month. I parsed each format separately and checked that every date falls between 1 March and 28 June 2026.
