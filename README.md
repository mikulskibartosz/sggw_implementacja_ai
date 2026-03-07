## UV + Linux/MacOs

uv venv
source .venv/bin/activate
uv pip install -r requirements.txt

## Venv + Windows

python.exe -m venv .venv
.venv/Scripts/activate
pip install -r requirements.txt

python.exe -m pip install -r requirements.txt

## Lista komend

### MLFLOw

| Komenda | Opis |
|---------|------|
| `mlflow ui` | Uruchamia interfejs webowy MLflow |
| `mlflow run .` | Uruchamia projekt MLflow z bieżącego katalogu |
| `mlflow run . -P alpha=0.5` | Uruchamia projekt z parametrem |


### DVC

| Komenda | Opis |
|---------|------|
| `dvc init` | Inicjalizuje DVC w projekcie |
| `dvc add data/dataset.csv` | Dodaje plik do śledzenia przez DVC |
| `dvc remote add -d myremote s3://bucket/path` | Dodaje zdalne repozytorium |
| `dvc remote add -d myremote /Users/...` | Dodaje zdalne repozytorium (lokalny katalog) |
| `dvc remote add -d myremote gdrive://folder_id` | Dodaje Google Drive jako zdalne repozytorium |
| `dvc push` | Wysyła dane do zdalnego repozytorium |
| `dvc pull` | Pobiera dane ze zdalnego repozytorium |
| `dvc checkout` | Przywraca dane z zdalnego repozytorium |
| `dvc du . ` | Pokazuje rozmiar danych w projekcie |
| `dvc gc --workspace` | Usuwa niepotrzebne dane z cache |