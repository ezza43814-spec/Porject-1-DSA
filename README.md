# SortLab — 15,000 Record Sorting GUI

A university Data Structures & Algorithms project using real-world NYC Airbnb listing data loaded from a public GitHub-hosted CSV (48,895 listings, 2019 archive). Sort any first 15,000 records using one of **eight hand-written algorithms**.

## Setup (Windows / Mac / Linux)

1. Install Python 3.10 or newer.
2. Open a terminal inside this folder.
3. Install dependencies: `python -m pip install -r requirements.txt`
4. Run: `python -m streamlit run app.py`
5. Open the local URL displayed in the terminal (typically `http://localhost:8501`).

Internet is needed to load the default dataset on the first run. You can use **Upload CSV** to try your own CSV.

## Algorithms
Bubble, Selection, Insertion, Merge, Hybrid Merge (Insertion cutoff 32), Quick (iterative 3-way), Heap, and Shell Sort. All are implemented from scratch in `sorting_algorithms.py` and do not call built-in sorting for the output. Data is not modified in-place outside each sorting call.

## Demo script for presentation
1. Go to **Original Data** and show 15,000 website records.
2. Select **price**, **Hybrid Merge Sort** and **Ascending**, then press **Run Sorting**.
3. Show the output CSV, execution time, comparisons and writes.
4. Change algorithm to Quick or Merge and compare results.
5. In the **Benchmark** tab compare all eight on a sample of 500 to make slow algorithms practical for classroom use.
6. Explain the complexity table in **Learn Algorithms**.

## Source
https://raw.githubusercontent.com/pjournal/boun01g-data-mine-r-s/gh-pages/Assignment/AB_NYC_2019.csv

This is an archived 2019 dataset, not live Airbnb stock.

## Notes
- The default 15,000 rows are the **first** 15,000 from the source, not a random sample.
- Quadratic algorithms (Bubble, Selection, Insertion) may take a long time on 15,000 rows; reduce record count when demonstrating them.
- Input columns should be numeric or text. Null/missing values are placed last in both ascending and descending sorts.
- Benchmark results depend on machine load, input shape and interpreter; don't treat one timing as a universal ranking.
