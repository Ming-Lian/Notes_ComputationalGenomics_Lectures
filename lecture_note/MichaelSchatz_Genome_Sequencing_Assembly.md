# Assembly theory

## Assembling a Genome
        
![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_01.png)
        
Why are genomes hard to assemble?
        
1. Biological

    (Very) High ploidy, heterozygosity, repeat content

2. Sequencing

    (Very) large genomes, imperfect sequencing

3. Computational

    (Very) Large genomes, complex structure

4. Accuracy

    (Very) Hard to assess correctness
        
Detangle graph with long reads, mates, and other links
        
![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_02.png)
        
![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_03.png)
        
![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_04.png)
        
## De Bruijn and Overlap graph

![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_05.png)

![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_06.png)

![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_07.png)
        
## Ingredients for a good assembly
        
![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_08.png)

- Coverage

    Typical sequencing coverage
  
    ![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_09.png)

    ![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_10.png)

    ![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_11.png)

    ![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_12.png)

    ![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_13.png)

    ![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_14.png)

- Read Length

    Coverage and Read Length

    ![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_15.png)

- Error

    ![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_16.png)

    ![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_17.png)

- Repeats composition

    ![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_18.png)

    ![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_19.png)

![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_20.png)
    
# Whole Genome Alignment & visualization

Goal of WGA

> For two genomes, A and B, find a mapping from each position in A to its corresponding position in B
>
> ![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_21.png)

Not so fast...

> Genome A may have insertions, deletions, translocations, inversions, duplications or SNPs with respect to B (sometimes all of the above)
>
> ![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_22.png)

WGA visualization

> ![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_23.png)
>
> ![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_24.png)
>
> ![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_25.png)
>
> ![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_26.png)

# Genome assemblers

## ALLPATHS-LG: recommended for Illumina-only projects

![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_27.png)

![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_28.png)

![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_29.png)

![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_30.png)

## Celera Assembler: recommended for PacBio projects

### Assembly Complexity

![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_31.png)

![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_32.png)

### Long Read Sequencing Technology

![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_33.png)

- Moleculo Sequencing

    Clever library preparation technique to turn a short read sequencer into a quazi-long read sequencer

    ![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_34.png)

    ![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_35.png)
  
- PacBio SMRT Sequencing

    Imaging of fluorescently phospholinked labeled nucleotides as they are incorporated by a polymerase anchored to a Zero-Mode Waveguide (ZMW)

    ![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_36.png)

- Oxford Nanopore MinION

    ![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_37.png)
   
### Consensus Accuracy and Coverage

![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_38.png)

![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_39.png)

![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_40.png)

![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_41.png)

![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_42.png)

# Application: Her2 amplified breast cancer

![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_43.png)

SK-BR-3: Most commonly used Her2-amplified breast cancer cell line

<aside>
❓ Can we resolve the complex structural varia4ons, especially around Her2?
</aside>

Improving SMRTcell Performance

![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_44.png)

![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_45.png)

## Structural variant discovery with long reads

![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_46.png)

![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_47.png)

PacBio and Illumina coverage values are highly correlated but Illumina shows greater variance because of poorly mapping reads

![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_48.png)

Confirmed both known gene fusions in this region

![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_49.png)

Joint coverage and breakpoint analysis to discover underlying events

![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_50.png)

Cancer lesion Reconstruction

![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_51.png)

## Oncogene Analysis

![](../pictures/MichaelSchatz_Genome_Sequencing_Assembly_52.png)