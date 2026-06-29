# Movie Recommendation System

A Django MovieLens recommender that demonstrates:

- Content based filtering with TF-IDF and cosine similarity over genres and tags.
- Collaborative filtering with matrix factorization using `TruncatedSVD`.
- A hybrid model that blends content similarity, collaborative scores, and popularity.
- A frontend in HTML, CSS, and JavaScript.

## Run

```powershell
python manage.py runserver
```

Open `http://127.0.0.1:8000/`.

The app reads MovieLens CSV files from:

```text
C:\Users\Kaila\Downloads\archive (40)
```

To use another folder:

```powershell
$env:MOVIELENS_DATA_DIR="C:\path\to\movielens"
python manage.py runserver
```

## Files Used

- `movie.csv`
- `rating.csv`
- `tag.csv`

`genome_scores.csv`, `genome_tags.csv`, and `link.csv` can be added later for richer semantic profiles and poster links.

## Notes

`Surprise` and `implicit` are optional alternatives for collaborative filtering. This version uses packages already available locally: Django, pandas, NumPy, SciPy, and scikit-learn.
