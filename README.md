# Рекомендуемый порядок ознакомления
1. `locations.ipynb` генерирует локации `locations.csv`.
1. `proximity_model.ipynb` делает бинарную классификацию `[dist(merch, tx) < 0.005]`. Для фичей используется `locations.csv`. Генерируется `proximity_model.cbm`.
1. `solution.ipynb` используется классификатор близости и DBSCAN, чтобы находить терминал. Основная функция - `find_merchant`.
