# Physical Fitness and Developer Productivity

A notebook-based research project examining physical-fitness and software-developer productivity data. The repository combines survey-data preparation, categorical encoding, visual exploration, and a written research report.

## Research workflow

```text
MetricsDataset → Preprocessing → MetricsCleanedData → Encoding → EncodedData
                                                                  |
                                                       Charts and heatmaps
```

| Artifact | Role |
| --- | --- |
| [preProcessing.ipynb](preProcessing.ipynb) | Load survey records and prepare the analytical dataset, including removal of timestamp and email fields |
| [encoding.ipynb](encoding.ipynb) | Transform survey responses into encoded values |
| [barCharts.ipynb](barCharts.ipynb) | Produce bar-chart views of the encoded dataset |
| [heatmap.ipynb](heatmap.ipynb) | Explore relationships through a correlation heatmap |
| `Dataset/` | Original, cleaned, and encoded data artifacts |
| [Report.pdf](Report.pdf) | Research narrative and interpretation |

## Explore the analysis

Use Python with Jupyter, pandas, NumPy, Matplotlib, seaborn, and an Excel-reading engine such as openpyxl:

```bash
python -m pip install jupyter pandas numpy matplotlib seaborn openpyxl
jupyter notebook
```

Open the notebooks in workflow order. Their file-loading cells reference dataset basenames such as `MetricsDataset.xlsx` and `EncodedData.xlsx`; use the matching artifacts from `Dataset/` in the notebook's working location. Select the reader according to the artifact's actual encoding: the preparation and encoding notebooks write CSV-formatted output using `.xlsx` filenames, and subsequent cells show their intended reader calls.

## Technical contributions

The project shows a complete exploratory research workflow, from removing identifying survey fields to encoding responses and presenting multivariate relationships. Separate notebooks preserve the distinction between data preparation and visualization, while the report connects the computational artifacts to the study's research questions.
