---
title: 'How to download SRA data, and convert to FASTQ'
author: Jin Choi
layout: post
permalink: /How-to-download-SRA/
dsq_thread_id:
  - 1681486643
categories:
  - Tech
---
0. Installed the program followed by tutorial http://khmer-protocols.readthedocs.org/en/v0.8.4/metagenomics/1-quality.html

1. Download SRA file from the web for the data. 
go to ncbi
choose SRA at search. add keyword and search
find FTP address and copy into computer by using 

<pre><code>
$ ncftp ftp://ftp-trace.ncbi.nlm.nih.gov/sra/sra-instant/reads/ByRun/sra/SRR/SRR492/SRR492065
</code></pre>
2. And convert SRA into FASTQ. fastq-dump --gzip SRR492065.sra
Now I have SRR492065.fastq.gz

