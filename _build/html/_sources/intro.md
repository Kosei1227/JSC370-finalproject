# NeurIPS Trends (1987 – 2023)

Welcome! This site summarises my JSC 370 final project, where I **scraped,
cleaned and analysed every NeurIPS conference paper published between 1987
and 2023** — over 70000 abstracts in total — to reveal long-term research
trends.


1. **Web scraping**  
   * Parallel requests to *papers.nips.cc* for each year  
   * Saved title + abstract for every submission into a single CSV

2. **Data hygiene**  
   * Removed papers with missing abstracts or fewer than 5 words  
   * Computed helper columns such as `title_length`, `abstract_length`

3. **Exploratory analysis**  
   * Year-by-year publication counts  
   * Evolution of median abstract length, title length, and more

4. **Semantic embedding + clustering**  
   * Sentence embeddings via **SPECTER-2** (HuggingFace + AdapterHub)  
   * 2-D projection with **UMAP**, clustering with **HDBSCAN**  
   * TF–IDF to label each cluster with representative n-grams

5. **Growth-rate modelling**  
   * Linear, Ridge, Random-Forest & Gradient-Boost regressors  
   * Compared R² / RMSE across clusters and time-windows

6. **Interactive visuals**  
   * 2 Plotly dashboards (live on the next page):  
     * **Figure 1** Publication counts vs. GBoost fit for the 5
       fastest-growing clusters  
     * **Figure 2** Top-20 topics ranked by predicted growth slope  

---

## How to navigate this site

| Page | What you’ll find |
|------|------------------|
| **Home (you’re here)** | Methodology overview, links, and references |
| **Embedding Trend Analysis** | The full Jupyter notebook with hidden code and two interactive Plotly figures |
| **Interactive Figures** | The full set of interactive figures generated from trend embedding analysis |

Use the sidebar on the left to jump between pages.  
All code is available on GitHub — click the *“View source”* button in the top-right corner of any page.

> **Tip for readers:** Hover, pan, and zoom freely inside any Plotly figure; click *“Download plot as PNG”* in the toolbar for high-resolution images.
