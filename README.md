# Master-Thesis-HRP
Inhalte des Repositorys sind Daten und Code, die zur Erstellung und Validierung der Ergebnisse für die Masterarbeit verwendet wurden.

## Voraussetzungen & Umgebung

Die Notebooks wurden unter folgender Umgebung entwickelt und getestet:

### Systemumgebung
- Betriebssystem: Windows 10 (Build 10.0.26200)
- Python-Version: 3.8.16 (64-bit, MSC v.1916)
- Anaconda3 (64-bit)
- Jupyter Notebook (6.5.4)
  
### Benötigte Python-Pakete

Das Projekt verwendet u.a. folgende externe Bibliotheken:

- numpy
- pandas
- scipy
- matplotlib
- seaborn
- plotly
- scikit-learn
- pyportfolioopt (pypfopt)
- riskfolio-lib
- yfinance
- requests
- beautifulsoup4 (bs4)
- IPython

Standardbibliotheken wie `os`, `sys`, `math`, `time`, `csv`, `typing` usw. sind Teil von Python und müssen nicht separat installiert werden.
Die Importe sind in jedem Notebook angegeben.

### Requirements

numpy==1.24.3
pandas==2.0.3
scipy==1.10.1
matplotlib==3.7.1
seaborn==0.12.2
plotly==5.9.0
scikit-learn==1.3.2
pyportfolioopt==1.5.5
Riskfolio-Lib==6.1.1
yfinance==0.2.63
requests==2.32.4
beautifulsoup4==4.12.2
IPython==8.12.0

## Handhabung

### Schritt 1: Aufbereitung der Daten

Im Ordner Daten-Bearbeitung liegen die Notebooks, die zur Bearbeitung der Daten verwendet wurden.
Innerhalb des Ordners liegen auch die CSV-Dateien mit den abgerufenen Rohdaten. Diese werden von den Notebooks eingelesen.
Die CSV-Dateien müssen im selben Ordner/Verzeichnis liegen, damit diese eingelesen werden können.
Auszuführen sind die kompletten Notebooks (Run All)
Ergebnis sind aufbereitete Daten, die als CSV exportiert werden. Zudem werden die Daten innerhalb der Notebooks visualisiert.
Zwischenergebnisse werden als CSV exportiert und wurden verwendet, die Implementierung in Excel manuell nachzuvollziehen und zu validieren.

### Schritt 2: Erzeugung der Ergebnisse

Im Ordner ErzeugungErgebnisse liegen die Notebooks, in denen die Optimierungsmethoden auf den Datensätzen angewandt wurden.
Die Bezeichnung der Notebooks gibt Aufschluss darüber, um welche Ergebnisse es sich handelt, z.B. Noteboks mit dem Zusatz "3jahre" bilden Ergebnisse auf 3-jährigen Testzeitfenstern
Innerhalb des Ordners liegen auch die CSV-Dateien mit den bereinigten Daten. Diese werden von den Notebooks eingelesen.
Die CSV-Dateien müssen im selben Ordner/Verzeichnis liegen, damit diese eingelesen werden können.
Auszuführen sind die kompletten Notebooks (Run All)
Ergebnisse sind CSV-Dateien mit Renditen für jede Optimierungsmethode (HRP, Minimum-Variance,...)

### Schritt 3: Auswertung der Ergebnisse

Im Ordner Auswertungen liegen die Notebooks, mit denen die unter Schritt 2 erzeugten Ergebnisse anhand von Performance-Metriken und Visualisierungen ausgewertet werden.
Die Bezeichnung der Notebooks gibt Aufschluss darüber, um welche Auswertung es sich handelt, z.B. Noteboks mit dem Zusatz "3jahre" bilden Ergebnisse auf 3-jährigen Testzeitfenstern
Innerhalb des Ordners liegen auch die CSV-Dateien mit den erzeugten Ergebnissen. Diese werden von den Notebooks eingelesen.
Die CSV-Dateien müssen im selben Ordner/Verzeichnis liegen, damit diese eingelesen werden können.
Auszuführen sind die kompletten Notebooks (Run All)
Ergebnisse sind Diagramme und Performance-Metriken

### Schritt 0: Validierung

Im Ordner Validierung-Tests liegen Notebooks und Excel-Dateien (xlsx, xlsm), die verwendet wurden um Implementierungen manuell zu überprüfen
CSV-Dateien müssen im selben Ordner/Verzeichnis liegen, damit diese eingelesen werden können.


# Master-Thesis-HRP

This repository contains data and code that were used to generate and validate the results presented in the master’s thesis.

## Requirements & Environment

The notebooks were developed and tested under the following environment:

### System Environment
- Operating System: Windows 10 (Build 10.0.26200)
- Python Version: 3.8.16 (64-bit, MSC v.1916)
- Anaconda3 (64-bit)
- Jupyter Notebook (6.5.4)

### Required Python Packages

The project uses, among others, the following external Python libraries:

- numpy
- pandas
- scipy
- matplotlib
- seaborn
- plotly
- scikit-learn
- pyportfolioopt (pypfopt)
- riskfolio-lib
- yfinance
- requests
- beautifulsoup4 (bs4)
- IPython

Standard libraries such as `os`, `sys`, `math`, `time`, `csv`, `typing`, etc. are part of Python and do not need to be installed separately.  
All imports are listed within the respective notebooks.

### Requirements

numpy==1.24.3
pandas==2.0.3
scipy==1.10.1
matplotlib==3.7.1
seaborn==0.12.2
plotly==5.9.0
scikit-learn==1.3.2
pyportfolioopt==1.5.5
Riskfolio-Lib==6.1.1
yfinance==0.2.63
requests==2.32.4
beautifulsoup4==4.12.2
IPython==8.12.0

## Usage

### Step 1: Data Preprocessing

The folder Daten-Bearbeitung contains notebooks used for data preparation.
The folder also contains the CSV files with the retrieved raw data, which are read by the notebooks.

The CSV files must be located in the same directory to be read correctly.
All notebooks should be executed completely ("Run All").

The outputs are cleaned and processed datasets, which are exported as CSV files.
In addition, the data are visualized within the notebooks.

Intermediate results are saved as CSV files and were used to manually verify and validate the implementation in Excel.

### Step 2: Generation of Results

The folder ErzeugungErgebnisse contains notebooks where the optimization methods are applied to the datasets.

The filenames indicate which results are produced, e.g., notebooks containing "3jahre" correspond to rolling 3-year test windows.

The folder also contains the cleaned CSV datasets used as inputs for the notebooks.
The CSV files must be located in the same directory to be read correctly.

All notebooks should be executed completely ("Run All").

The outputs are CSV files containing returns for each optimization method (e.g., HRP, Minimum Variance, etc.).

### Step 3: Evaluation of Results

The folder Auswertungen contains notebooks used to analyze the results created in Step 2 using performance metrics and visualizations.

The filenames indicate the respective evaluation window, e.g., notebooks containing "3jahre" correspond to 3-year test windows.

The folder also contains the CSV files with the generated results, which are read by the notebooks.
The CSV files must be located in the same directory to be read correctly.

All notebooks should be executed completely ("Run All").

The outputs are visualizations and performance metrics.

### Step 0: Validation

The folder Validierung-Tests contains notebooks and Excel files (.xlsx, .xlsm) that were used to manually verify the implementations.

CSV files must be located in the same directory in order to be read correctly.
