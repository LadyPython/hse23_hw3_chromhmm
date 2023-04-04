# hse_hw3_chromhmm

[Colab](https://colab.research.google.com/drive/1tRSkUK2sim7ZU-LQ-4HmAPjhleMMQDxz?usp=sharing)

Клеточная линия: **HMEC**

Список 10-ти гистоновых меток:
1. wgEncodeBroadHistoneHmec**Ctcf**StdAlnRep1
2. wgEncodeBroadHistoneHmec**H3k27ac**StdAlnRep1
3. wgEncodeBroadHistoneHmec**H3k27me3**StdAlnRep1
4. wgEncodeBroadHistoneHmec**H3k36me3**StdAlnRep1
5. wgEncodeBroadHistoneHmec**H3k4me1**StdAlnRep1
6. wgEncodeBroadHistoneHmec**H3k4me2**StdAlnRep1
7. wgEncodeBroadHistoneHmec**H3k4me3**StdAlnRep1
8. wgEncodeBroadHistoneHmec**H3k79me2**AlnRep1
9. wgEncodeBroadHistoneHmec**H3k9ac**StdAlnRep1
10. wgEncodeBroadHistoneHmec**H4k20me1**StdAlnRep1

Контроль: wgEncodeBroadHistoneHmec**Control**StdAlnRep1

[cellmarkfiletable.txt](/cellmarkfiletable.txt)
[Папка с выдачей ChromHMM](/data)

## ChromHMM

Emission | Overlap | Transition 
--- | --- | ---
![Image](/data/emissions_15.png) | ![Image](/data/HMEC_15_overlap.png) | ![Image](/data/transitions_15.png)

RefSeqTSS | RefSeqTES  
--- | --- 
![Image](/data/HMEC_15_RefSeqTSS_neighborhood.png) | ![Image](/data/HMEC_15_RefSeqTES_neighborhood.png)

N | Name | Histones | Refs
--- | --- | --- | ---
1 | Active Promoter | H3k79me2 | RefSeqExon, RefSeqGene, RefSeqTES
2 | Weak Promoter | H3k36me3, H3k79me2 | RefSeqExon, RefSeqGene, RefSeqTES
3 | Inactive/poised | Promoter H3k79me2 | RefSeqGene
4 | Strong enhancer | H3k27ac, H3k4me2, H3k4me1, H3k79me2 | RefSeqGene
5 | Strong enhancer | H3k27ac, H3k4me1 | RefSeqExon, RefSeqGene, RefSeqTES
6 | Weak/poised enhancer | H3k4me1 | laminb1ladsa
7 | Weak/poised enhancer | H3k27ac, H3k4me2, H3k4me1 | 
8 | Insulator | H3k27ac, H3k9ac, H3k4me2, H3k4me1 | 
9 | Transcriptional transition | H3k27ac, H3k9ac, H3k4me3, H3k4me2 | RefSeqExon, CpGIslands, RefSeqTES, RefSeqTSS, RefSeqTSS2Kb
10 | Transcriptional elongation | H3k27ac, H3k9ac, H3k4me3, H3k4me2, H3k79me2 | RefSeqExon, CpGIslands, RefSeqGene, RefSeqTES, RefSeqTSS2Kb
11 | Weak transcribed | H3k4me3, H3k4me2, H3k4me1 | RefSeqExon, CpGIslands, RefSeqTES, RefSeqTSS, RefSeqTSS2Kb
12 | Polycomb-repressed | H3k4me3, H3k4me2, H3k4me1, H3k27me3 | RefSeqExon, CpGIslands, RefSeqTES, RefSeqTSS, RefSeqTSS2Kb, laminb1ladsa
13 | Heterochromatin; low signal | ~H3k27me3 | laminb1ladsa
14 | Repetitive/Copy Number Variation | | laminb1ladsa
15 | Repetitive/Copy Number Variation | Ctcf | laminb1ladsa

<img width="980" alt="image" src="https://user-images.githubusercontent.com/6313540/229896224-5a6e5dd5-35ad-456b-bcd6-5fd9e9f33e47.png">
