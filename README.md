# IMDb Movie Genre Dataset (1970–2018)

This repository contains a curated **multi-label movie genre dataset** collected from the [IMDb](https://www.imdb.com/) platform.  
The dataset contains **textual** information for use in **deep learning**, **genre prediction**, and **text representation learning** tasks.

---

## Dataset Overview

| Property | Description |
|-----------|--------------|
| **Source** | IMDb (movies released between 1970–2018) |
| **Data Type** | Text |
| **Languages** | English (cleaned summaries), English genre labels |
| **Samples** | Movies from 1970 to 2018 |
| **Files** | `train.csv`, `test.csv`, `full_dataset.csv` |

---

## Dataset Structure

Each `.csv` file includes the following columns:

| Column | Description |
|--------|--------------|
| **imdb_id** | IMDb unique identifier |
| **image_path** | Relative path to poster image (e.g. `Posters/imdb_id.jpg`) |
| **cleaned_summary** | Preprocessed and combined synopsis and plot text |
| **genres_binary** | 0/1 encoded values for each genre (multi-label) |
| **genres_text** | Genre names as text (e.g. `Action | Comedy`) |

---

## Genres

- Action  
- Adventure  
- Animation  
- Biography  
- Comedy  
- Crime  
- Drama  
- Documentary  
- Fantasy  
- Family  
- History  
- Horror  
- Music  
- Mystery  
- Romance  
- Science Fiction  
- Short  
- Sport  
- Thriller  
- War  

---

## File Description

| File | Description |
|------|--------------|
| `train.csv` | Training subset for machine learning models |
| `test.csv` | Test subset (disjoint from training) |
| `full_dataset.csv` | Complete dataset containing all movies |

---

## Preprocessing Notes

- Synopses and plot summaries were **merged and cleaned** (HTML tags, special characters, and duplicates removed).  
- Genres were **standardized** to 20 English labels.  
- Poster filenames are based on their **IMDb IDs**.  
- The dataset **was divided to preserve the data distribution ratio across genres** where possible.
---

---


## Citation

If you use this dataset in your research or project, please cite it as:


---

## License

This dataset is released for **research and educational use only**.  
Movie metadata and poster images are property of **IMDb** and their respective owners.

---

### If you find this dataset useful, please star the repository!
