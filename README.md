# RNAseq-obesity-simpsons
RNA-seq pipeline sobre el análisis de expresión diferencial de genes relacionados con la obesidad mediante RNA-seq. Incluye control de calidad, alineación, análisis de DEG, gráficos volcano plots y heatmaps. Máster en Bioinformática. Grupo 4.

# 🧬 RNA-seq Differential Expression Analysis - Obesity
**Master en Bioinformática | Secuenciación y Ómicas de Próxima Generación**

## 👥 Grupo 4
- Caren Moreno
- Analia Pastrana  
- Angel Emanuel Guerrero

## 📋 Descripción
Análisis de expresión diferencial de genes relacionados con la obesidad
utilizando datos simulados de RNA-seq basados en personajes de Los Simpson.
Se comparan perfiles metabólicos: Obeso1, Obeso2 y Normopeso.

## 🔧 Pipeline
FastQC → STAR/HISAT2 → featureCounts/Salmon → DESeq2 → Visualización

## 📊 Resultados principales
![Volcano Plot](results/figures/volcano_plot.png)
![Heatmap](results/figures/heatmap.png)

## 🗂️ Estructura del repositorio
```text
RNAseq-obesity-simpsons/
│
├── README.md
├── LICENSE
├── .gitignore
│
├── data/
│   ├── raw/
│   │   └── README_raw_data.md
│   │
│   ├── processed/
│   │   ├── counts_matrix.csv
│   │   ├── metadata.csv
│   │   └── normalized_counts.csv
│   │
│   └── reference/
│       ├── tx2gene.csv
│       └── README_reference.md
│
├── results/
│   ├── figures/
│   │   ├── volcano_plot.png
│   │   ├── MA_plot.png
│   │   ├── PCA_plot.png
│   │   ├── heatmap_all_genes.png
│   │   ├── heatmap_pipelineB_comparison.png
│   │   └── reactome_ORA.png
│   │
│   ├── tables/
│   │   ├── DESeq2_resultados_completos.csv
│   │   ├── DEGs_significativos.csv
│   │   └── enrichment_results.csv
│   │
│   └── qc/
│       ├── fastqc_reports/
│       ├── multiqc_report.html
│       └── QC_summary.md
│
├── scripts/
│   ├── 00_quality_control.sh
│   ├── 01_salmon_quant.sh
│   ├── 02_deseq2_analysis.R
│   ├── 03_visualization.R
│   └── 04_enrichment_analysis.R
│
├── notebooks/
│   ├── PipelineA_analysis.Rmd
│   └── PipelineA_analysis.html
│
├── poster/
│   ├── poster_grupo4.pdf
│   └── poster_grupo4.pptx
│
├── docs/
│   ├── methodology.md
│   ├── session_info.txt
│   └── repositories_justification.md
│
└── environment/
    ├── sessionInfo.txt
    └── packages_versions.txt
```

## Cómo reproducir el análisis
[Agregar descripción de pasos ordenados]

## 🔗 Poster
![Poster](poster/Poster.jpg)
