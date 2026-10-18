## End to End Data Science Project


## ⚙️ Project Components & Architecture (Short Points)

* **`template.py` (Structure Initializer):** Pure project ke files aur folders (components, pipelines, config files) ko bina manually banaye ek single click mein automatic setup aur initialize karta hai.
* **`setup.py` (Package Installer):** Project ko ek local Python package (`mlproject`) mein convert karta hai, jisse source files ko pure system mein aasan internal importing mil sake.
* **`requirements.txt` (Dependencies Manifest):** Data science standard tools (`numpy`, `pandas`, `scikit-learn`), database operations, advanced algorithms (`xgboost`, `catboost`) aur tracking parameters ki libraries manage karta hai.
* **`data_ingestion.py` (Data Router):** Local paths ya SQL database connection se data collect karta hai aur use validation ke liye **80% Training Set** aur **20% Testing Set** mein split karta hai.
* **`data_transformation.py` (Preprocessing Pipeline):** Numerical columns ko median value se fill karke scale karta hai aur categorical strings ko numbers (`OneHotEncoder`) mein convert karke preprocessing pickle file (`preprocessor.pkl`) generate karta hai.
* **`model_trainer.py` (Model Engine & MLOps):** Multiple algorithms par automated loops run karke hyperparameter tuning karta hai aur best tuned model ko save karne ke sath **MLflow & DagsHub** cloud servers par metric tracking variables push karta hai.
* **`utils.py` (Shared Infrastructure):** PyMySQL secure database query routines, standard matrix execution functions aur pickle serialization algorithms ke reusable static operations hold karta hai.
* **`logger.py` (Telemetry Tracking):** System execution shuru hote hi timestamp based logs (`MM_DD_YYYY_HH_MM_SS.log`) record karta hai taaki runtime tracking perfect bani rahe.
* **`exception.py` (Fault-Tolerance Tracer):** Poore application code flow ke crashes line-by-line check karta hai aur script path aur exact line numbers ke sath diagnostics formats standard reports generate karta hai.
* **`.gitignore` & `.dvcignore` (Noise Control Filters):** Caching memory clusters (`__pycache__`), local server libraries (`venv/`), raw tracking overhead datasets aur private credential blocks (`.env`) ko repositories operations se dynamic filter-out karte hain.
