# **Project Update (03/01/2019)**
Note: Tick mark means completed tasks. Will be removed in the latter project update documents.
## Parikh (HIV mutation analysis)
*Summary: Finding mutations in  HIV RT sequences resistant to drugs from clinical trails and MP samples*
- [ ] 1. Check automation of Contamination Analysis pipeline on ASPIRE samples
- [ ] 2. Work on transferring Contamination Analysis pipeline to NextFlow for packaging
- [ ] 3. Work on manuscript on Mutation Analysis & Contamination Analysis 
- [ ] 4. HIV Mutation Pipeline Update1: Include the code of collecting random virion sequences with condtion of Sample > 25K virions, then randomly select 25K virions.
- [ ] 5. HIV Mutation Pipeline Update2: Include the steps for overlap pairs in paired end library. Reference for virion assembly still need to be provided by Kerri to test run this update.
- [ ] 6. Complete rest of the priorities in their Priority list i.e. 4,5 and 6. (Reference and Library prep info still need ot be provided by Kerri)

## Kevin Joseph (HIV sequence integration in Human analysis)
*Summary: Finding HIV human junctions and assembly of pro-virus*

### Human+HIV junction region:

- [x] 1. Give presentation on final HIV+Human integration region pipeline
- [x] 2. Run the pipeline on all GKISA samples and test them
- [x] 3. Obtain paritally aligned reads with no signature sequence and share them with Kevin to find out what they are
- [ ] 4. Conduct test on cutoff position for HIV+Human integration at different percentage coverage vs. length of integration region
- [x] 5. Run Pipeline on other KISA samples

### Bringing together the results of Integration Assembly and Provirus Assembly

- [x] 1. Rerun provirus assmebly for samples (KSISA+NFL) using same ACH2 reference used for assembly of integration region
- [ ] 2. For samples which were assembled into provirus sequences, concatenate the assembly of integration region

### Presentation to Dr. Mellors
 [ ] 1. Work on slides to present the pipelines worked on junction region and provirus assembly

## Prepare for Workshop/Training of CORE group on HIV projects

### Chandran Group Workshop: Rahil Sethi
- [x] 1. Continue with the remainder of HIV mutation pipeline
- [x] 2. Discuss if they were able to run and understand each step of the pipeline
- [x] 3. Introduce them with HIV Contamination Analysis pipeline
- [x] 4. Give Traning sesison on complete HIV Contamination Pipeline
- [ ] 5. Make Training ppt on Human+HIV integration project
- [ ] 6. Make Training ppt on Provirus assembly project
