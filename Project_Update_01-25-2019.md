# **Project Update (01/25/2019)**
Note: Tick mark means completed tasks. Will be removed in the latter project update documents.
## Parikh (HIV mutation analysis)
*Summary: Finding mutations in  HIV RT sequences resistant to drugs from clinical trails and MP samples*
- [x] 1. Priority1: Select/Provide concensus seq of random sampling of UMIs (50) from s25 (DS6) then provide UPGMA tree for analysis in ITOL.
- [x] 2. Priority2: Supervise William S. to reanalize Serial Dilution I and II datasets with the current HIV mutation pipeline and in generating table for read counts per virion (all & assembled ones) for these samples.
- [x] 3. Priority 3 (MTN): Build consensus of Assembled virions for each sample in MTN study (with IUPAC base names and 80% major base cutoff) and build UPGMA Tree of Sanger vs. Consensus for all samples in the study.
- [x] 4. Priority 3 (IPM): Build consensus of Assembled virions for each sample in IPM study (with IUPAC base names and 80% major base cutoff) and build UPGMA Tree of Sanger vs. Consensus for all samples in the study.
- [x] 5. Run Contamination Analysis on MTN including DS23 MTN samples (Status: Between and Within Sample analysis Finished, contaminatant detection and UPGMA validation left)
- [x] 6. Run Contamination Analysis on IPM including DS23 IPM samples (Status: Between and Within Sample analysis Finished, contaminatant detection and UPGMA validation left) 
- [ ] 7. HIV Mutation Pipeline Update1: Include the code of collecting random virion sequences with condtion of Sample > 25K virions, then randomly select 25K virions.
- [ ] 8. HIV Mutation Pipeline Update2: Include the steps for overlap pairs in paired end library. Reference for virion assembly still need to be provided by Kerri to test run this update.
- [ ] 9. Complete rest of the Priorities: 4,5 and 6.

## Kevin Joseph (HIV sequence integration in Human analysis)
*Summary: Finding HIV human junctions and assembly of pro-virus*

### Human+HIV junction region:

- [x] 1. Write code to generate statistics on alignment of reads to HIV, such that it includes #Reads paritally aligned and carry signature sequence in the same place where reference genome has.
- [x] 2. Generate pipleline for finding Human+HIV junction region:

Reads --> Align to HIV reference --> Collect partially aligned read ids (softclipped) with signature sequence in them --> Obtain R1 and R2 sequences for such read ids --> Align such reads to HIV+hg19 genome -->
a. Find region with max coverage --> Traverse upstream and downstream of the max coverage region until coverage >= 5% of max coverage --> Assemble reads in such region using samtools/bcftools --> 
Count # reads in fwd and reverse direction in such region to get strand of assembly --> Reverse complement assembly if (-) strand: Human region of integration site
b. Assemble reads in region from start of HIV reference to the last base after which the alignment begins. Use consensus building tool with 75% major base cutoff
c. Assemble reads from 1st base of alignment on HIV reference to base where coverage >= 5% of max coverage.
d. Join b and c assemblies to get provirus region of integration site.  
- [x] 3. Construct bash script pipeline for above workflow
- [x] 4. Test on GKISA2_S6 (works well)
- [ ] 5. Rerun pipeline on GKISA samples
- [ ] 6. Once established the pipeline, run the pipeline on other datasets for HIV+Human junction
- [ ] 7. Conduct test on cutoff position for HIV+Human integration at different percentage coverage vs. length of integration region
- [ ] 8. Run Pipeline on other KISA samples

### Bringing together the results of Integration Assembly and Provirus Assembly

- [ ] 1. For MS6369218-500v2, and probably for other datasets with KISA and NFL assays, once decided on results of Human+HIV integration region and provirus assembly, discuss strategy to bring them together as one assembly.


## Prepare for Workshop/Training of CORE group on HIV projects

### Chandran Group Workshop: Rahil Sethi
- [x] 1. Continue with the remainder of HIV mutation pipeline
- [x] 2. Discuss if they were able to run and understand each step of the pipeline
- [ ] 3. Introduce them with HIV Contamination Analysis pipeline
- [ ] 4. Make Training ppt on Human+HIV integration project
- [ ] 5. Make Training ppt on  Provirus assembly project
