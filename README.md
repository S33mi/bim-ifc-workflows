# BIM IFC Workflows with IfcOpenShell

A practical Google Colab notebook that shows how to **read a BIM model as data** — not just geometry.

This matches a common openBIM / digital construction data analysis requirement:

> *Read a BIM model through its objects, parameters, classifications, and relationships.*

---

## What this project demonstrates

| Skill | How it is shown |
|-------|------------------|
| **Objects** | Count and inspect walls, doors, windows, spaces, storeys |
| **Parameters** | Extract property sets (`Pset_WallCommon`, quantities, etc.) |
| **Classifications** | Pattern for reading Uniclass / OmniClass-style references |
| **Relationships** | Spatial structure, storey containment, openings (voids) |
| **Analysis** | Simple quantity-style summaries and pandas tables |
| **Visualization** | Charts for object counts, walls per storey, external/internal, openings, space areas |

---

## Quick start (Google Colab)

1. Open the notebook in [Google Colab](https://colab.research.google.com/)  
   (File → Upload notebook → select `BIM_IFC_Workflow_Colab.ipynb`)
2. Runtime → **Run all**
3. The notebook automatically:
   - Installs `ifcopenshell`, `pandas`, `matplotlib`, `seaborn`
   - Downloads the free **FZK House** sample model
   - Builds tables and charts
   - Exports CSV files you can download from the left sidebar

No local BIM software required.

---

## Files

| File | Description |
|------|-------------|
| `BIM_IFC_Workflow_Colab.ipynb` | Main notebook (run in Colab) |
| `walls_parameters.csv` | Generated — walls + key properties |
| `spaces_summary.csv` | Generated — spaces / rooms |
| `object_counts.csv` | Generated — element counts by IFC class |

*(CSV files appear after you run the notebook.)*

---

## Sample model

Uses the classic **AC20-FZK-Haus** (Karlsruhe Institute of Technology) — a small, well-known IFC4 model that is free to use for learning and testing.

---

## Why BIM matters

BIM more than “I can model in Revit.”  

It helps with the following:

- Treat IFC as a structured dataset
- Query objects and their properties programmatically
- Understand spatial relationships and classifications
- Turn model data into tables, charts, and reports

This notebook is a concrete starting point for that skill set.

---

## Next steps (learning path)

1. Run the notebook and explore the charts/tables
2. Try a different IFC model (export from Revit/Archicad or use other public samples)
3. Filter elements by property (e.g. external load-bearing walls only)
4. Build a simple area or quantity report
5. Learn the `ifcopenshell.api` for writing/editing IFC data
6. Official docs: [https://docs.ifcopenshell.org/](https://docs.ifcopenshell.org/)

---

## Tools used

- [IfcOpenShell](https://ifcopenshell.org/) — open-source IFC library
- pandas — tables and analysis
- matplotlib + seaborn — charts
- Google Colab — zero-install environment

---

## License (MIT)

This educational notebook is free to use and adapt.  
The sample model is provided by the Institute for Automation and Applied Informatics (IAI) / Karlsruhe Institute of Technology (KIT).

---

