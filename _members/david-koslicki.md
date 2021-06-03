---
title: David Koslicki # fill out your name

# name variations to include when generating list of this person's papers
search:
 - David
 - Koslicki

# if image not specified, default will automatically be used
image: images/team/Koslicki-David.jpg ## the path of your profile photo, please put it under 'images/team' and name it as firstname-lastname.jpg

# role must be included or person won't appear on team page
role: pi ## options: pi-Principal Investigator, postdoc-Postdoctoral Researcher, phd-PhD Student, masters-Master's Student, undergrad-Undergraduate Student, highschool-High School Student, programmer-Software Engineer

# add person to alumni group
# group: alum ## comment it if you're not alumni

# contact info and social media links
email: dmk333@psu.edu ## fill out your email
website: https://www.linkedin.com/in/david-koslicki-86174b97/ ## fill out the address of your pesonal website if you have or your linkedin profile if you like
github: dkoslicki ## your github account if you like to put it on your profile
google: Oz90sQsAAAAJ
twitter: DavidKoslicki ## your twitter account if you like to put it on your profile
instagram: koslickid ## your instagram account if you like to put it on your profile
youtube: dmkoslicki ##https://www.youtube.com/channel/UC4ocxPwjndh1c9xr0HyD27Q  ## your youtube account if you like to put it on your profile

---
[comment]: Fill out your description below 

With the advent of high-throughput sequencing technology, it is becoming
increasingly easy to generate large amounts of biological data. However,
it is also becoming increasingly more difficult to extract scientific
knowledge from such datasets due to their size, noisiness, and a
currently incomplete understanding of what such datasets are composed of
(e.g. never before seen bacteria in a metagenomic community of
microorganisms). **My passion and main research area is the development
of efficient algorithms to extract insight from \*-omics data**. This
puts my research squarely at the intersection of biology, mathematics,
and computer science. I am particularly interested in the entire arc of
developing a computational biology method: rigorous mathematical
justification of a method, implementing the method into a tool usable by
the community, applying the tool to pressing scientific problems, and
finally using the results to inform further development of computational
techniques.

I have spent the majority of my career developing such computational
techniques. During this time, I have predominantly worked on the
analysis of metagenomic data (Sczyrba et al. 2017; D. Koslicki et al.
2015; Chatterjee et al. 2014; D. Koslicki and Falush 2016; Koslicki and
Zabeti, n.d.; D. Koslicki, Foucart, and Rosen 2014; D. Koslicki, S.
Foucart, and G. Rosen 2013), reference-free and alignment-free analysis
of genomic data (Holzinger et al. 2014; D. Koslicki 2011; D. Koslicki
and D.J. Thompson 2014; Mangul and D. Koslicki 2016), and Markov chains
with their application to models of molecular evolution (D. Koslicki
2012; D. Koslicki and Denker 2016). In the future, I will continue to
work on enabling the extraction of knowledge from large biological
datasets through efficient computation.

# Current research: Efficient computation in biology

My current research involves the development of typically discrete
algorithms (often with an optimization component) to analyze genomic
data. Much of my research is concerned with how to effectively utilize
*k*-mers (contiguous subsequences of DNA of length *k*) to **analyze
metagenomic data sets**. However, I also have an interest in a more
systems-scale analysis of biological data including the analysis of gene
regulatory networks (Ansariola, Megraw, and D. Koslicki 2018) and
sensitivity analysis of networks of interacting organisms (D. Koslicki
and Novak 2017). Two short vignettes will illustrate the flavor of my
research.

The first illustrates the mutually beneficial relationship between
biology and computational sciences that I particularly enjoy. When
working on a technique to profile metagenomic communities (i.e.
answering the question “what organisms are present in a given community
of microorganisms?”) a colleague and I were able to discover new
insights in the field of compressive sensing. Not only did the
biologists get a fast, efficient computational technique (D. Koslicki,
S. Foucart, and G. Rosen 2013), but we were able to prove that the
underlying algorithm performed better on the problems of interest than
the celebrated Orthogonal Matching Pursuit (OMP) and related compressive
sensing algorithms (Foucart and D. Koslicki 2014). This line of research
has been continued, with the resulting computational techniques
comparing favorably in a recent comparison of metagenomic tools (Sczyrba
et al. 2017).

Secondly, motivated by the computational bottleneck experienced when
comparing the similarity of communities of microorganisms, I was able to
develop a new, linear-time algorithm for the computation of the
widely-used UniFrac metric as well as make connections between its
computation and the Monge property for greedy algorithms (McClelland and
D. Koslicki 2017). Not only is this algorithm faster than the current
state of the art, but it also proves, for free, additional biological
insight in the form of so-called differential abundance vectors. This
underlying algorithm has since been implemented into the popular (cited
over 10,000 times) QIIME computational framework.

On a broader level, I am also interested in the fair and open assessment
of computational techniques and the development of “standard practices”
in computational biology. As an organizing committee member, co-author,
and participant of the CAMI (Critical Assessment of Metagenomic
Interpretation) initiative, I have helped to perform the largest
comparison of metagenomic computational techniques to date (Sczyrba et
al. 2017). Through this initiative, I have helped to set standards (in
terms of formats, metrics, etc.) for this relatively young field and
have seen these standards adopted by the community.

Given the interdisciplinary nature of my work, it is by necessity highly
collaborative. I maintain active research collaborations with
researchers in mathematics (Texas A&M, Ohio State), computer science
(UCLA, Helmholtz, Royal Institute of Technology), and biology (Oregon
State, UCLA, Royal Institute of Technology). One advantageous way to
maintain these collaborations has been working with students in these
departments and ensuring they are engaged in the biology while also
thoroughly immersed in computational expertise.

# Education, outreach, and community involvement

Along with the aforementioned CAMI involvement, I am also an organizer
and member of the OSU Microbiome Initiative (OMBI) which hosts research
symposia, training workshops, and also engages with the community
through public lectures and even a microbiome art exhibit. I also
actively engage with the computational biology community through my
position as an organizer of the Computational Genomics Summer Institute
(CGSI) at UCLA. In its third year of existence, this Summer institute
hosts a multi-part program that includes an (internationally recognized
and attended) conference of genomics methods developers, as well as
short courses and a long course that focus on different aspects of
computational biology methods development.

Given the increasing importance of computational education, I have also
prioritized the training of students in this field. With colleagues in
my department, I have developed a new mathematical biology minor,
assisted in the development of a university-wide data sciences graduate
major, and have also developed and helped to develop three ongoing
courses that emphasize mathematical, statistical, and computer science
approaches to the analysis of biological systems and data.

# Ongoing and Future research

In the near term, I will continue working on several problems that flow
naturally from my current research. These include: (1) rapid metagenomic
community profiling through locality sensitive hashing coupled with a
model of molecular evolution for biological relevancy, (2) metagenomic
community analysis through biodiversity minimization (an extension of
nonconvex ℓ<sub>*q*</sub>-minimization), and (3) refinement of
semidefinite relaxation approaches to the computation of the cut-norm
for the identification of network motifs in gene regulatory networks.

In the medium term, an exiting area of future research involves a
project very recently funded by the National Center for Advancing
Translational Sciences (NCATS), an institute and center of the NIH. This
project is a part of the Biomedical Data Translator program that seeks
to couple machine learning techniques to the myriad of biological data
repositories to create an interactive reasoning tool. This reasoning
tool will be used by biologists and clinicians via natural language
queries, after which the reasoning tool will query, collate, and infer
answers to the user queries. The overarching goal is to accelerate
knowledge discovery and spark the next generation of biomedical
translation for the understanding and treatment of disease. This is
accomplished by helping researchers to make connections and discover new
insights without requiring them to manually wade through massive
biological databases. On this project (which is joint with the Institute
of Systems Biology and Ohio State University), I will be mainly
concerned with the algorithmic aspects of how to automate the question
answering and reasoning components of this tool: so this project deals
with **knowledge representation and reasoning with graph databases**.
Our current implementation utilizes Markov chains, graphical models, and
measures of semantic similarity.

In the long term, I am particularly interested in the problem of
**microbial dark matter**. By some estimates, upwards of 90% of
microorganisms cannot yet be cultured in the lab and a significant
percentage of metagenomic data consists of DNA sequences of unknown
origin and function. This is an area of “unknown unknowns” where
scientists hesitate to even postulate what exists in these portions of
such datasets. Nonetheless, a number of recent exciting biomedical
advancements have come from the focused study of parts of this “dark
matter”: the revolutionary CRISPR/Cas9 gene editing approach, the
MRSA-fighting antibiotic Lugdunin, and the antibiotic Teixobactin were
all discovered in this fashion. One approach to facilitate such
discovery is through the computational analysis of metagenomic samples.
From an algorithmic viewpoint, this presents a unique challenge as the
goal is to identify, classify, and infer the function of genuinely novel
data in the form of DNA sequences. To approach this problem, we need
computational techniques that are capable of extracting from these
fragmented, noisy datasets portions that correspond to novel organisms,
assemble their genomes, and infer their functions. I am attempting just
this via what I term “profile informed assembly” whereby the very
difficult process of metagenomic genome assembly is made easier by
incorporating the results of the profiling step to partition the data
into “known knowns” and “known unknowns.”

I look forward to engaging with these problems while also pursuing
future collaborative opportunities.

Ansariola, M., M. Megraw, and D. Koslicki. 2018. “<span
class="nocase">IndeCut evaluates performance of network motif discovery
algorithms</span>.” *Bioinformatics* 34 (9).

Chatterjee, S., D. Koslicki, S. Dong, N. Innocenti, L. Cheng, Y. Lan, M.
Vehkaperaand M. Skoglundand L.K. Rassmussen, E. Aurell, and J. Corander.
2014. “<span class="nocase">SEK: sparsity exploiting *k*-mer based
estimation of bacterial community composition</span>.” *Bioinformatics*
30 (17): 2423–31.

D. Koslicki. 2011. “<span class="nocase">Topological entropy of DNA
sequences.</span>” *Bioinformatics* 27 (8): 1061–67.
<https://doi.org/10.1093/bioinformatics/btr077>.

D. Koslicki. 2012. “<span class="nocase">Substitution Markov chains with
applications to molecular evolution</span>.” PhD thesis, State College,
PA, USA: Pennsylvania State University.

D. Koslicki, S. Chatterjee, D. Shahrivar, A. Walker, S. Francis, L.
Fraser, M. Vehkaperä, Y. Lan, and J. Corander. 2015. “ARK: Aggregation
of Reads by k-Means for Estimation of Bacterial Community Composition.”
*PLoS ONE* 10 (10): e0140644.

D. Koslicki, and D.J. Thompson. 2014. “Coding Sequence Density
Estimation via Topological Pressure.” *Journal of Mathematical Biology*,
1–25. <https://doi.org/10.1007/s00285-014-0754-2>.

D. Koslicki, and M. Denker. 2016. “Substitution Markov Chains and Martin
Boundaries.” *Rocky Mountain Journal of Mathematics* 46 (6): 1963–85.

D. Koslicki, and D. Falush. 2016. “MetaPalette: A k-Mer Painting
Approach for Metagenomic Taxonomic Profiling and Quantification of Novel
Strain Variation.” *mSystems* 1 (3): e00020–16.

D. Koslicki, S. Foucart, and G. Rosen. 2014. “<span
class="nocase">WGSQuikr: fast whole-genome shotgun metagenomic
classification</span>.” *PLoS ONE* 9 (3): e91784.

D. Koslicki, and M. Novak. 2017. “Exact Probabilities for the
Indeterminacy of Complex Networks as Perceived Through Press
Perturbations.” *Journal of Mathematical Biology* Online ahead of print:
[doi.org/10.1007/s00285-017-1163-0](doi.org/10.1007/s00285-017-1163-0)
(July). <https://doi.org/10.1007/s00285-017-1163-0>.

D. Koslicki, S. Foucart, and G. Rosen. 2013. “<span
class="nocase">Quikr: a Method for Rapid Reconstruction of Bacterial
Communities via Compressive Sensing</span>.” *Bioinformatics* 29 (17):
2096–2102.

Foucart, S., and D. Koslicki. 2014. “<span class="nocase">Sparse
recovery by means of nonnegative least squares</span>.” *IEEE Signal
Processing Letters* 21 (14): 498–502.

Holzinger, A., M. Hortenhuber, C. Mayer, M. Bachler, S. Wassertheurer,
A.J. Pinho, and D. Koslicki. 2014. “On Entropy-Based Data Mining.” In
*Interactive Knowledge Discovery and Data Mining in Biomedical
Informatics*, 209–26. Springer Berlin Heidelberg.

Koslicki, D, and H Zabeti. n.d. “Improving Min Hash via the Containment
Index with Applications to Metagenomic Analysis. bioRxiv. 2017.”
*Publisher Full Text*.

Mangul, S., and D. Koslicki. 2016. “Reference-Free Comparison of
Microbial Communities via de Bruijn Graphs.” *ACM-BCB, IEEE/ACM Trans.
On Computational Biol. And Bioinf.*

McClelland, J., and D. Koslicki. 2017. “<span class="nocase">EMDUnifrac:
Exact linear time computation of the Unifrac metric and identification
of differentially abundant organisms</span>.” *Journal of Mathematical
Biology*, no. In print.

Sczyrba, A., P. Hofmann, P. Belmann, D. Koslicki, and …and A. McHardy,.
2017. “Critical Assessment of Metagenome Interpretation - a Benchmark of
Metagenomics Software.” *Nature Methods* 14 (11): 1063–71.

