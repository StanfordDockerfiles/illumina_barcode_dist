# illumina_barcode_dist
Tabulates the frequencies at which each barcode seen in the Illumina unmatched reads is present

Will output a single, tab-delimited file named barcode_distribution.txt with the fields being 1) Barcode, 2) Freq, and 3) Relative_Freq%. For paired-end sequencing, you only need to supply one of the FASTQ files. By defualt, only a subset of the reads are sampled (configurable). Note that if the original sample sheet used in demultiplexing did not contain any barcodes, then the sample numbers are present in the read headers instead of barcode sequence. As a result, sample numbers would be written in the 'Barcode' column of the output file instead.
