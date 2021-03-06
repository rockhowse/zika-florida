#### Data
[Sequences](https://github.com/andersen-lab/zika-florida/tree/master/consensus_sequences) | [Alignments](https://github.com/andersen-lab/zika-florida/tree/master/alignments) | [Trees](https://github.com/andersen-lab/zika-florida/tree/master/trees) | [BAMs](https://www.dropbox.com/sh/87bnqj83mwgw8br/AADWjkfL5bZ22XvemlMOUhBOa?dl=0)

#### Samples

| Scripps ID | Patient ID | Sample type | Quality score | % Coverage | Location of infection     |
| :---       |       :--- | :---        | :---          |       :--- | :---                      |
| ZF1        |        001 | Saliva      | ***           |      99.71 | Martinique                |
| ZF8        |        008 | Urine       | ***           |      90.07 | Puerto Rico               |
| ZF10       |        010 | Urine       | ****          |      97.69 | USA     |
| ZF16       |        016 | Urine       | ***           |      99.88 | Puerto Rico               |
| ZF21       |        021 | Urine       | ***           |      97.45 | USA     |
| ZF22       |        022 | Urine       | ***           |      97.77 | USA     |
| ZF30       |        030 | Urine       | ***           |      99.75 | USA     |
| ZF32       |        032 | Urine       | ***           |      99.75 | USA     |
| ZF38       |        038 | Urine       | ***           |      99.76 | USA     |
| ZF39       |        039 | Urine       | ****          |      99.75 | USA     |
| ZL2        |     Hu0015 | Saliva      | ***           |      99.75 | USA     |
| ZM1        |       7501 | Mosquito    | ****          |      99.75 | USA     |
| ZM2        |       7719 | Mosquito    | ****          |      99.74 | USA     |
| ZM3        |       7727 | Mosquito    | ****          |      99.83 | USA     |
| ZM4        |   16-10416 | Mosquito    | ****          |      99.72 | USA     |
| ZM5        |    16-3125 | Mosquito    | **            |      96.63 | USA     |
| ZC188      |  423568715 | Serum       | ****          |      98.26 | Columbia                  |
| ZC192      |  423401315 | Serum       | ****          |      98.36 | Columbia                  |
| ZC204      |  424439915 | Serum       | ****          |      99.74 | Columbia                  |
| ZC207      |  423217515 | Serum       | ****          |      96.68 | Columbia                  |	

### Quality
```
**** Complete coding sequence, no apparent contamination in aligned bam file
***	Complete coding sequence, some contamination in aligned bam file (confident in consensus)
**	Partial coding sequence, no apparent contamination in aligned bam file
*	Partial coding sequence, some contamination in aligned bam file
```

#### Sequencing
* Library construction was performed using an amplicon-based approach [amplicon-based approach](https://docs.google.com/document/d/1PilT4w5jHO-ROsE8TL5WBGa0wSCdTHAsNl1LIOYiTgk).
* Sequencing was performed on the MiSeq.

#### Coding-complete genomes
* Downloaded from NCBI, ViPR, and NextStrain. Only new genomes are added to later folders.
* Consensus sequences sequenced in our lab are added to the root of the 'consensus_sequences' folder.

#### Alignments
* Created using MAFFT.
* Trimmed to just contain the ORFs.

#### Maximum likelihood trees
* Created using the fast algorithm in RAxML using 200 bootstraps.
* Orange = travel-associated cases; Red = local transmissions.
* We root trees on KX447517 from French Polynesia.

#### Time-scaled trees 
* Made with BEAST using the following parameters:
 * Uncorrelated relaxed clock with lognormal distribution, CTMC rate prior.
 * GTR<sub>&#915;</sub> substitution model with codon partitioning.
 * SkyGrid, 50 parameters, time at last point = 4.
 * 30,000,000 states.

**Disclaimer**. Please note that this data is still based on work in progress and should be considered preliminary. If you intend to include any of these data in publications, please let us know – otherwise please feel free to download and use without restrictions. We have shared this data with the hope that people will download and use it, as well as scrutinize it so we can improve our methods and analyses. Please contact us if you have any questions or comments – we’ll buy beers for #ResearchParasites that spot flaws and faults in the data and come up with improvements!
