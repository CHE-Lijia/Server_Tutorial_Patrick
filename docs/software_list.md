# Software & Versions

This document serves as the inventory for all software and databases installed on the server. Please check this list before installing new tools to avoid duplication.

## 1. Installed Software
Use the ["Env Alias"](#3-shell-configuration-recommended) command to activate the environment. Click the alias to jump to the [**Environment Mapping**](#2-environment-mapping) table for details.  
Due to the dependency of software and compatibility, some softwares are installed in multiple environments and in different versions.  

| Software | Purpose | Version | DB | Env Alias |
| :--- | :--- | :--- | :--- | :--- |
| abricate | Resistance Screening | 1.2.0 | - | [`env_ann`](#env-mapping) |
| antismash | Secondary Metabolites | 7.1.0 | YES | [`env_ann`](#env-mapping) |
| bacphlip | Phage Prediction | ? | - | [`env_bacphlip`](#env-mapping) |
| bakta | Genome Annotation | 1.8.2 | YES | [`env_ann`](#env-mapping) |
| bcftools | Variant Calling | 1.23.2 | - | [`env_var`](#env-mapping) |
| beast | Evolutionary Analysis | 2.6.3 | - | [`env_evo`](#env-mapping) |
| bedtools | Interval Tools | 2.31.1 | - | [`env_ann`](#env-mapping) |
| bedtools | Interval Tools | 2.31.1 | - | [`env_var`](#env-mapping) |
| blast | Sequence Alignment | 2.16.0 | - | [`env_ann`](#env-mapping) |
| blast | Sequence Alignment | 2.12.0+ | - | [`env_phage`](#env-mapping) |
| bowtie2 | Read Alignment | 2.5.4 | - | [`env_metawrap`](#env-mapping) |
| bwa | Read Alignment | 0.7.18 | - | [`env_metawrap`](#env-mapping) |
| cd-hit | Remove Repeated Genome | 4.6.1 | - | [`env_qc`](#env-mapping) |
| checkm | Quality Assessment | 1.0.18 | YES | [`env_metawrap`](#env-mapping) |
| checkM2 | Quality Assessment | 1.1.0 | YES | [`env_checkm2`](#env-mapping) |
| checkv | Viral Quality | 1.0.3 | - | [`env_phage`](#env-mapping) |
| chopper | Read Filtering | 0.11.0 | - | [`env_qc`](#env-mapping) |
| clair3 | Variant Calling | 2.0.0 | - | [`env_var`](#env-mapping) |
| diamond | Sequence Alignment | 2.0.15 | - | [`env_ann`](#env-mapping) |
| Dorado | Basecalling | 1.4.0 | - | [`act_dorado`](#env-mapping) |
| dRep | Genome Dereplication | 3.4.5 | - | [`env_ann`](#env-mapping) |
| EggNOG-mapper | Functional Annotation | 2.1.13 | YES | [`env_ann`](#env-mapping) |
| fastANI | ANI Calculation | 1.34 | - | [`env_evo`](#env-mapping) |
| fastp | Quality Control | 1.1.0 | - | [`env_qc`](#env-mapping) |
| FastQC | Quality Control | 0.12.1 | - | [`env_qc`](#env-mapping) |
| Filtlong | Read Filtering | 0.3.1 | - | [`env_qc`](#env-mapping) |
| Flye | Genome Assembly | 2.9.6 | - | [`env_asm`](#env-mapping) |
| GTDB-TK | Taxonomy Classification | 2.6.1 | YES | [`env_gtdbtk`](#env-mapping) |
| hmmer | HMM Analysis | 3.4 | - | [`env_ann`](#env-mapping) |
| hmmer | HMM Analysis | 3.4 | - | [`env_metawrap`](#env-mapping) |
| hmmer | HMM Analysis | 3.3.2 | - | [`env_phage`](#env-mapping) |
| ICEScreen | ICE Detection | 1.3.1 | - | [`env_evo`](#env-mapping) |
| INFERNAL | RNA Analysis | 1.1.5 | - | [`env_ann`](#env-mapping) |
| iPHop | Host Prediction | 1.4.2 | YES | [`env_phage`](#env-mapping) |
| iqtree | Phylogenetic Analysis | 3.0.1 | - | [`env_evo`](#env-mapping) |
| ISEScan | IS Identification | 1.7.3 | - | [`env_evo`](#env-mapping) |
| Kraken2 | Taxonomic Classification | 2.1.3 | YES | [`env_ann`](#env-mapping) |
| LEfSe | Biomarker Discovery | 1.1.01 | - | [`env_ann`](#env-mapping) |
| mafft | Multiple Alignment | 7.526 | - | [`env_evo`](#env-mapping) |
| MASH | Distance Estimation | 2.3 | - | [`env_phage`](#env-mapping) |
| MASH | Distance Estimation | 2.3 | - | [`env_plasmid1`](#env-mapping) |
| MAUVE | Genome Alignment | 2018 | - | [`env_plasmid1`](#env-mapping) |
| Medaka | Sequence Correction | 2.2.0 | - | [`env_asm`](#env-mapping) |
| metabat2 | Genome Binning | 2.15 | - | [`env_metawrap`](#env-mapping) |
| metaquast | Assembly Assessment | 5.3.0 | - | [`env_ann`](#env-mapping) |
| metaWRAP | Metagenomics Pipeline | 1.3.0 | - | [`env_metawrap`](#env-mapping) |
| minimap2 | Read Alignment | .28 | - | [`env_ann`](#env-mapping) |
| minimap2 | Read Alignment | 2.30 | - | [`env_var`](#env-mapping) |
| MLST | Sequence Typing | 2.32.2 | - | [`env_ann`](#env-mapping) |
| MobileElementFinder | MGE Identification | 1.1.2 | - | [`env_ann`](#env-mapping) |
| MOB-suite | Plasmid Analysis | 3.1.9 | YES | [`env_plasmid1`](#env-mapping) |
| MultiQC | Report Aggregation | 1.33 | - | [`env_qc`](#env-mapping) |
| mummer4 | Sequence Alignment | 4.0.1 | - | [`env_plasmid1`](#env-mapping) |
| nanofilt | Read Filtering | 2.8.0 | - | [`env_qc`](#env-mapping) |
| NanoPlot | Visualization | 1.46.2 | - | [`env_qc`](#env-mapping) |
| ORFFinder | ORF Identification | 0.4.3 | - | [`act_orffinder`](#env-mapping) |
| Panaroo | Pangenome Analysis | 1.6.0 | - | [`env_ann`](#env-mapping) |
| parsnp | Phylogeny Analysis | 2.1.5 | - | [`env_plasmid1`](#env-mapping) |
| phispy | Prophage Detection | 4.2.21 | - | [`env_ann`](#env-mapping) |
| plasmidFinder | Plasmid Identification | 2.1.5 | - | [`env_ann`](#env-mapping) |
| Porechop | Adapter Trimming | 0.2.4 | - | [`env_qc`](#env-mapping) |
| prodigal | Gene Prediction | 2.6.3 | - | [`env_ann`](#env-mapping) |
| prodigal | Gene Prediction | 2.6.3 | - | [`env_checkm2`](#env-mapping) |
| prodigal | Gene Prediction | 2.6.3 | - | [`env_phage`](#env-mapping) |
| prokka | Genome Annotation | 1.15.6 | - | [`env_ann`](#env-mapping) |
| pyani | ANI Calculation | 0.3.0 | - | [`env_evo`](#env-mapping) |
| QUAST | Assembly Assessment | 5.3.0 | - | [`env_ann`](#env-mapping) |
| samtools | File Manipulation | 1.18 | - | [`env_metawrap`](#env-mapping) |
| samtools | File Manipulation | 1.23 | - | [`env_qc`](#env-mapping) |
| samtools | File Manipulation | 1.23.1 | - | [`env_var`](#env-mapping) |
| semibin2 | Genome Binning | 2.2.1 | - | [`env_ann`](#env-mapping) |
| sniffles | Variant Calling | 2.7.3 | - | [`env_var`](#env-mapping) |
| snippy | Variant Calling | 3.1 | - | [`env_evo`](#env-mapping) |
| spades | Genome Assembly | 4.2.0 | - | [`env_asm`](#env-mapping) |
| Trimmomatic | Read Trimming | 0.4 | - | [`env_qc`](#env-mapping) |
| tRNAscan-SE | tRNA Prediction | 2.0.12 | - | [`env_ann`](#env-mapping) |
| Unicycler | Genome Assembly | 0.5.1 | - | [`env_asm`](#env-mapping) |
| Vegan | Ecological Analysis | - | - | [`env_ann`](#env-mapping) |
| virsorter2 | Viral Detection | 2.2.4 | YES | [`env_phage`](#env-mapping) |

## 2. Environment Mapping
<a id="env-mapping"></a>
This table details the actual paths and owners for each environment alias.

| Environment Alias | Environment Path | Python | Maintained by |
| :--- | :--- | :--- | :--- |
| `env_ann` | `/hdd1/shared_envs/chelijia/env_annotation` | 3.9.15 | @chelijia |
| `env_asm` | `/hdd1/shared_envs/chelijia/env_assembly` | 3.10.20 | @chelijia |
| `env_bacphlip` | `/hdd1/shared_envs/chelijia/env_bacphlip` | 3.8.20 | @chelijia |
| `env_checkm2` | `/hdd1/shared_envs/chelijia/env_checkm2` | 3.12.13 | @chelijia |
| `env_evo` | `/hdd1/shared_envs/chelijia/env_evo` | 3.9.19 | @chelijia |
| `env_gtdbtk` | `/hdd1/shared_envs/chelijia/env_gtdbtk` | 3.13.12 | @chelijia |
| `env_metawrap` | `/hdd1/shared_envs/chelijia/env_metawrap` | 2.7.15 | @chelijia |
| `env_phage` | `/hdd1/shared_envs/chelijia/env_phage` | 3.8.15 | @chelijia |
| `env_plasmid1` | `/hdd1/shared_envs/chelijia/env_plasmid1` | 3.10.20 | @chelijia |
| `env_qc` | `/hdd1/shared_envs/chelijia/env_qc` | 3.10.21 | @chelijia |
| `env_var` | `/hdd1/shared_envs/chelijia/env_variation` | 3.11.15 | @chelijia |
---

## 3. Shell Configuration (Recommended)
To make your workflow more efficient, you may add these aliases to your `~/.bashrc` file.

```bash
# --- Lab Server Environment & Database Configuration ---

# 1. Environment Activation Aliases
alias act_ann='conda activate /hdd1/shared_envs/chelijia/env_annotation'
alias act_asm='conda activate /hdd1/shared_envs/chelijia/env_assembly'
alias act_bacphlip='conda activate /hdd1/shared_envs/chelijia/env_bacphlip'
alias act_checkm2='conda activate /hdd1/shared_envs/chelijia/env_checkm2'
alias act_evo='conda activate /hdd1/shared_envs/chelijia/env_evo'
alias act_gtdbtk='conda activate /hdd1/shared_envs/chelijia/env_gtdbtk'
alias act_metawrap='conda activate /hdd1/shared_envs/chelijia/env_metawrap'
alias act_phage='conda activate /hdd1/shared_envs/chelijia/env_phage'
alias act_plasmid1='conda activate /hdd1/shared_envs/chelijia/env_plasmid1'
alias act_qc='conda activate /hdd1/shared_envs/chelijia/env_qc'
alias act_var='conda activate /hdd1/shared_envs/chelijia/env_variation'

# 2. Database Path Variables
export ANTISMASH_DB="/hdd1/shared_db/chelijia/antismash_db"
export BAKTA_DB="/hdd1/shared_db/chelijia/bakta_db"
export CHECKM_DB="/hdd1/shared_db/chelijia/checkm_db"
export CHECKM2_DB="/hdd1/shared_db/chelijia/checkm2_db"
export EGGNOG_DB="/hdd1/shared_db/chelijia/eggnog_db"
export GTDBTK_DB="/hdd1/shared_db/chelijia/gtdbtd_db"
export IPHOP_DB="/hdd1/shared_db/chelijia/iphop_db"
export KRAKEN2_DB="/hdd1/shared_db/chelijia/kraken2_db"
export MOB_SUITE_DB="/hdd1/shared_db/chelijia/mob_suite_db"
export VIRSORTER_DB="/hdd1/shared_db/chelijia/virsorter_db"
