<h1 style="color:black;">About</h1>
<p style="color:black;">For more instructions on how to download IGenotyper and a more detailed explanation on how to run IGenotyper go to the IGenotyper github site: .</p>
<p style="color:black;">This repository is a more detailed analysis on the IGenotyper and it's output.</p>
<p></p>
<h1>Quick start</h1>
```
IG-make-ref reference/hg19.fasta
IG --phase <pacbio bam file> <output>
IG --assemble <pacbio bam file> <output>
IG --detect <pacbio bam file> <output>
```
<h1>Input to IGenotyper</h1>
<h2>RSII</h2>
<p> If you are using RSII data, you'll have to turn the raw bax files to a bam file. You can do this using the bax2bam tool (https://github.com/PacificBiosciences/bax2bam)</p>
<h2>Sequel+</h2>
<p>The BAM file from the Sequel machines can be used as input into IGenotyper</p>
<h2>Difference between RSII and Sequel data</h2>
<p>One if the steps in IGenotyper is to create CCS reads. The CCS reads are of lower quality in RSII and cannot use be used to validate the genes extracted from the assembly.</p>
