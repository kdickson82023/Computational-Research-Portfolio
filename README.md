# Computational Research Portfolio

## About this repository

This repository describes selected computational research projects from my doctoral and postdoctoral work in microbial ecology, metagenomics, and metatranscriptomics.

Most of the code associated with these projects is currently unavailable in a public repository because the underlying research is unpublished or under publication embargo. I take reproducibility and open scientific workflows seriously. I also take academic integrity and scientific publishing ethics seriously. The absence of project code from this repository reflects publication and institutional restrictions rather than an absence of computational work. I will not upload project code, intermediate data, or other materials that could disclose unpublished results. Code will be made publicly available as publication and institutional restrictions permit.

My computational work has primarily used Python, R, Bash, Linux/HPC environments, and Jupyter for the analysis of large-scale sequencing and experimental datasets. My work includes reproducible bioinformatics workflows, taxonomic and functional analysis of microbial communities, genome-resolved metagenomics, metatranscriptomics, longitudinal analysis, statistical analysis, and scientific visualization.

## Selected projects (with working pre-publication titles)

### Assessing the impacts of *Asparagopsis taxiformis* and bromoform on rumen eukaryote community composition and metabolism

As a postdoctoral researcher at UC Davis, I worked on a large collaborative research program investigating the rumen microbiome and strategies for reducing enteric methane emissions. I analyzed longitudinal metagenomic and experimental data from approximately 280 bioreactor samples and five rumen samples, as part of a dataset totaling approximately 27 TB. The work included comparing microbial-community responses across experimental conditions and methane-mitigation interventions, including bromoform from Asparagopsis, 3-NOP, ionophores, and defined microbial consortia. My computational work included processing and integrating sequencing and experimental metadata; taxonomic and functional analysis; comparative analysis across treatments and time points; statistical analysis and visualization; and development of reproducible analysis workflows.

This project produced a set of metagenome-assembled genomes for rumen ciliates and required working with complex metagenomic datasets in which eukaryotic organisms represented a challenging minority of the microbial community. I conducted genome-resolved analyses and investigated the functional potential of these organisms, including carbohydrate-active functions relevant to plant biomass degradation.


### Herbivore gut microbial consortia and lignocellulose degradation

My doctoral research examined microbial consortia enriched from herbivore gut communities for their ability to degrade plant biomass.

I analyzed metatranscriptomic and microbial-community data from anaerobic enrichment experiments using substrates including alfalfa, sugarcane bagasse, reed canary grass, xylan, and other plant-derived materials. The project included experimental manipulation of microbial communities using antibiotic selection and comparison of community composition and functional activity across treatments.

The computational work included sequencing-data processing, taxonomic and functional analysis, differential and comparative analyses, statistical analysis, and integration of multi-omic results with experimental observations.

## Computational tools and approaches

My computational work spans shotgun metagenomics, metatranscriptomics, microbial and eukaryotic genomics, genome-resolved analysis, amplicon sequencing, functional annotation, phylogenomics, microbial community ecology, and longitudinal multi-omics analysis. I have built and maintained workflows for datasets ranging from individual genome-resolved analyses to approximately 27 TB of longitudinal metagenomic, metatranscriptomic, metabolomic, and experimental data.

### Sequencing read processing and quality control

I have developed and run preprocessing and quality-control workflows for large metagenomic and metatranscriptomic sequencing datasets, including removal or filtering of low-quality and unwanted sequence data and preparation of reads for downstream assembly, mapping, and community analysis.

Tools I have used for these tasks include:

- **BBMap** for read processing and sequence manipulation;
- **Sickle** for quality trimming; and
- **SortMeRNA** for identification and filtering of ribosomal RNA sequences.

Quality control continues throughout my analytical workflows rather than being treated solely as a preprocessing step. I routinely evaluate intermediate and final outputs for biological and technical anomalies, consistency across samples, and suitability for downstream analysis.

### Metagenomic assembly and genome recovery

I have performed genome-resolved metagenomic analyses of complex microbial communities, including communities containing organisms whose genomes are repetitive, poorly represented in reference databases, and difficult to assemble.

My assembly, genome-recovery, and genome-quality toolkit includes:

- **metaSPAdes** for metagenomic assembly;
- **MetaBAT2** for metagenomic binning;
- **COBRA** for improving genome recovery from metagenomic assemblies;
- **BUSCO** for evaluation of genome completeness using conserved orthologs; and
- **dRep** for comparison and dereplication of recovered genomes.

A major focus of my postdoctoral work was adapting genome-resolved approaches to rumen microbial eukaryotes, particularly anaerobic fungi and ciliates. These organisms present unusual computational challenges because of extreme AT richness and long repeat regions in their genomes, which are consequently difficult to assemble and possess limited reference resources.

### Sequence identification, gene prediction, and functional annotation

I use sequence-search and annotation approaches to connect genomic and transcriptomic data to biological function and to identify genes, proteins, domains, and organisms of interest in complex datasets.

Tools and resources I have used include:

- **MMseqs2** for large-scale sequence searching and comparison;
- **INFERNAL** for covariance-model-based sequence analysis;
- **MetaEuk** for identification and prediction of eukaryotic genes in metagenomic sequence;
- **dbCAN** for annotation and analysis of carbohydrate-active enzymes;
- **Pfam** for protein-family and domain annotation; and
- **HydDB** for functional classification of hydrogenases.

Much of this work has focused on microbial functions involved in plant-biomass degradation, fermentation, interspecies metabolic relationships, and other processes relevant to rumen and anaerobic microbial ecology.

### Read mapping, coverage analysis, and sequence manipulation

I have used read mapping and coverage information both as analytical outputs and as inputs to genome-resolved and transcriptomic analyses.

My toolkit includes:

- **Bowtie2** for sequence alignment and read mapping;
- **CoverM** for calculating coverage and abundance from metagenomic datasets;
- **BEDtools** for manipulating and comparing genomic intervals and sequence-associated data; and
- **seqtk** for sequence-file manipulation and filtering.

I have integrated mapping and coverage outputs with genome annotations, sample metadata, experimental conditions, and other analytical results to examine organismal abundance and activity across treatments and time points.

### Genome-centric metatranscriptomics

My research includes genome-centric analysis of transcriptional activity in complex microbial communities. Linking transcriptional information to recovered genomes is necessary to investigate how particular organisms and functional groups respond to experimental conditions.

In my doctoral research, I used these approaches to study lignocellulose-degrading bacterial consortia. In my postdoctoral work, I used them to characterize taxon-specific transcriptional responses of rumen fungi and ciliates to methane-mitigation interventions including bromoform and *Asparagopsis taxiformis*.

This work requires integrating metagenomic assemblies and genomes, functional annotations, read-mapping results, transcript abundance, experimental metadata, and statistical analyses into a coherent biological interpretation.

### Statistical analysis and microbial community ecology

I have analyzed microbial community and experimental datasets using both community-ecological and differential-abundance/expression approaches.

Tools I have used include:

- **limma** for statistical analysis of high-dimensional biological data;
- **LinDA / MicrobiomeStat** for differential-abundance analysis of microbiome data;
- **vegan** for ecological and multivariate community analysis; and
- **QIIME 2** for amplicon sequence variant analysis.

I use **R** extensively for statistical analysis, integration of experimental and sequencing data, exploratory analysis, visualization, and preparation of publication-quality results.

### Phylogenomics

I have used phylogenomic approaches to establish evolutionary relationships among recovered or reference genomes and to place poorly characterized organisms in a broader taxonomic and evolutionary context.

My phylogenomic toolkit includes:

- **trimAl** for alignment filtering;
- **AMAS** for processing and summarizing sequence alignments; and
- **IQ-TREE** for phylogenetic inference.

This has been particularly useful when working with understudied microbial eukaryotes for which existing reference genomes and annotations are limited.

### Programming, automation, and large-scale data analysis

I use **Python, R, Bash/Unix, Jupyter, Git/GitHub, and high-performance computing environments** to move between specialized bioinformatics software and higher-level biological analysis. My Python work includes **pandas, NumPy, and Biopython** for data manipulation, numerical analysis, parsing and transforming biological sequence data, integrating outputs from multiple bioinformatics tools, and automating repetitive analytical tasks. I use **Bash/Unix** extensively for filesystem and sequence-data manipulation, pipeline execution, automation, HPC job management, and coordinating analyses involving large numbers of samples, genomes, and intermediate files.

My research has required working with datasets as large as approximately **27 TB**, including longitudinal metagenomic, metatranscriptomic, metabolomic, and experimental data. This requires not only executing individual bioinformatics tools but designing analyses in which outputs from many computational stages remain traceable to the appropriate samples, experimental treatments, time points, genomes, and biological questions.

### Reproducible computational workflows

Reproducibility has been an important part of both my doctoral and postdoctoral computational work. I have developed workflows in which sequencing-data processing, genome-resolved analyses, statistical analyses, and downstream interpretation can be repeated systematically rather than reconstructed manually. I am currently incorporating **Snakemake** into the publication workflow for my current research to formalize dependencies among analytical steps and facilitate reproducible execution. The associated research code cannot yet be made public because the underlying manuscripts are in preparation. It will be released as publication and institutional restrictions permit.
