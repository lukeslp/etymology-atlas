---
license: cc-by-sa-3.0
task_categories:
  - feature-extraction
tags:
  - linguistics
  - etymology
  - historical-linguistics
  - cognates
  - language-families
  - phonology
  - typology
  - nlp
  - glottolog
  - wiktionary
size_categories:
  - 1M<n<10M
---

# Etymology Atlas: Global Language Relationships

How did the word 'mother' travel from Proto-Indo-European *méh₂tēr to modern languages across four continents? This dataset maps 4.17 million etymological relationships connecting words across 19,401 languages.

The Etymology Atlas integrates five authoritative linguistic sources into a unified graph structure:

• **etymology-db**: 3.75 million word relationships extracted from Wiktionary, capturing borrowings, cognates, derivations, and semantic shifts
• **Glottolog**: Complete catalog of the world's languages with geographic coordinates, family trees, and endangerment status
• **Lexibank IE-CoR**: 4,981 expert-annotated cognate sets for Indo-European languages—the gold standard for computational historical linguistics
• **PHOIBLE**: Phoneme inventories for 2,177 languages with articulatory features (manner, place, voicing)
• **WALS**: 76,475 typological feature values covering word order, tone systems, case marking, and 189 other structural properties

Researchers can trace how words evolved, map language contact zones, analyze sound change patterns, or build phylogenetic models of language families. The Parquet format enables efficient querying of the full graph on a laptop.

Data sources are linked by ISO 639-3 codes and Glottocodes, enabling cross-table joins between etymology, phonology, and typology.

## Files

| File | Records | Description |
|------|---------|-------------|
| `etymologies.parquet` | 4.17M | Core etymology graph |
| `languages.parquet` | 19,401 | Language metadata from Glottolog |
| `cognate_sets.parquet` | 4,981 | Expert cognate groups (IE-CoR) |
| `phonemes.parquet` | 105,484 | PHOIBLE phoneme data |
| `linguistic_features.parquet` | 76,475 | WALS typological features |

## Citation

```bibtex
@dataset{etymology_atlas_2026,
  title = {Etymology Atlas: Global Language Relationships},
  author = {Steuber, Luke},
  year = {2026},
  doi = {10.5281/zenodo.18321479},
  url = {https://huggingface.co/datasets/lukeslp/etymology-atlas}
}
```

## Distribution

- **GitHub**: [lukeslp/etymology-atlas](https://github.com/lukeslp/etymology-atlas)
- **Kaggle**: [lucassteuber/etymology-atlas](https://www.kaggle.com/datasets/lucassteuber/etymology-atlas)
- **HuggingFace**: [lukeslp/etymology-atlas](https://huggingface.co/datasets/lukeslp/etymology-atlas)

## License

CC BY-SA 3.0
