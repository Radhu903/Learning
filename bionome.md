```
(base) radhu@Radhu:~/Documents/1_RawReads$ cd..
cd..: command not found
(base) radhu@Radhu:~/Documents/1_RawReads$ cd ..
(base) radhu@Radhu:~/Documents$ conda install -c bioconda bwa
Collecting package metadata (current_repodata.json): done
Solving environment: done

## Package Plan ##

  environment location: /home/radhu/miniconda3

  added / updated specs:
    - bwa


The following packages will be downloaded:

    package                    |            build
    ---------------------------|-----------------
    bwa-0.7.17                 |       h5bf99c6_8         608 KB  bioconda
    openssl-1.1.1l             |       h7f8727e_0         2.5 MB
    ------------------------------------------------------------
                                           Total:         3.1 MB

The following NEW packages will be INSTALLED:

  bwa                bioconda/linux-64::bwa-0.7.17-h5bf99c6_8

The following packages will be UPDATED:

  openssl            conda-forge::openssl-1.1.1k-h7f98852_0 --> pkgs/main::openssl-1.1.1l-h7f8727e_0


Proceed ([y]/n)? y


Downloading and Extracting Packages
bwa-0.7.17           | 608 KB    | ################################################################################################################################################################ | 100% 
openssl-1.1.1l       | 2.5 MB    | ################################################################################################################################################################ | 100% 
Preparing transaction: done
Verifying transaction: done
Executing transaction: done
(base) radhu@Radhu:~/Documents$ conda install -c bioconda samtools
Collecting package metadata (current_repodata.json): done
Solving environment: done

## Package Plan ##

  environment location: /home/radhu/miniconda3

  added / updated specs:
    - samtools


The following packages will be downloaded:

    package                    |            build
    ---------------------------|-----------------
    bzip2-1.0.8                |       h7b6447c_0          78 KB
    c-ares-1.17.1              |       h27cfd23_0         108 KB
    htslib-1.13                |       h9093b5e_0         2.2 MB  bioconda
    krb5-1.19.2                |       hac12032_0         1.2 MB
    libcurl-7.78.0             |       h0b77cf5_0         338 KB
    libdeflate-1.7             |       h27cfd23_5          55 KB
    libedit-3.1.20210714       |       h7f8727e_0         165 KB
    libev-4.33                 |       h7b6447c_0         112 KB
    libnghttp2-1.41.0          |       hf8bcb03_2         667 KB
    libssh2-1.9.0              |       h1ba5d50_1         269 KB
    samtools-1.13              |       h8c37831_0         397 KB  bioconda
    ------------------------------------------------------------
                                           Total:         5.5 MB

The following NEW packages will be INSTALLED:

  bzip2              pkgs/main/linux-64::bzip2-1.0.8-h7b6447c_0
  c-ares             pkgs/main/linux-64::c-ares-1.17.1-h27cfd23_0
  htslib             bioconda/linux-64::htslib-1.13-h9093b5e_0
  krb5               pkgs/main/linux-64::krb5-1.19.2-hac12032_0
  libcurl            pkgs/main/linux-64::libcurl-7.78.0-h0b77cf5_0
  libdeflate         pkgs/main/linux-64::libdeflate-1.7-h27cfd23_5
  libedit            pkgs/main/linux-64::libedit-3.1.20210714-h7f8727e_0
  libev              pkgs/main/linux-64::libev-4.33-h7b6447c_0
  libnghttp2         pkgs/main/linux-64::libnghttp2-1.41.0-hf8bcb03_2
  libssh2            pkgs/main/linux-64::libssh2-1.9.0-h1ba5d50_1
  samtools           bioconda/linux-64::samtools-1.13-h8c37831_0


Proceed ([y]/n)? y


Downloading and Extracting Packages
samtools-1.13        | 397 KB    | ################################################################################################################################################################ | 100% 
htslib-1.13          | 2.2 MB    | ################################################################################################################################################################ | 100% 
bzip2-1.0.8          | 78 KB     | ################################################################################################################################################################ | 100% 
libdeflate-1.7       | 55 KB     | ################################################################################################################################################################ | 100% 
libcurl-7.78.0       | 338 KB    | ################################################################################################################################################################ | 100% 
libev-4.33           | 112 KB    | ################################################################################################################################################################ | 100% 
c-ares-1.17.1        | 108 KB    | ################################################################################################################################################################ | 100% 
libssh2-1.9.0        | 269 KB    | ################################################################################################################################################################ | 100% 
libnghttp2-1.41.0    | 667 KB    | ################################################################################################################################################################ | 100% 
krb5-1.19.2          | 1.2 MB    | ################################################################################################################################################################ | 100% 
libedit-3.1.20210714 | 165 KB    | ################################################################################################################################################################ | 100% 
Preparing transaction: done
Verifying transaction: done
Executing transaction: done
(base) radhu@Radhu:~/Documents$ cd ..
(base) radhu@Radhu:~$ samtools

Program: samtools (Tools for alignments in the SAM format)
Version: 1.13 (using htslib 1.13)

Usage:   samtools <command> [options]

Commands:
  -- Indexing
     dict           create a sequence dictionary file
     faidx          index/extract FASTA
     fqidx          index/extract FASTQ
     index          index alignment

  -- Editing
     calmd          recalculate MD/NM tags and '=' bases
     fixmate        fix mate information
     reheader       replace BAM header
     targetcut      cut fosmid regions (for fosmid pool only)
     addreplacerg   adds or replaces RG tags
     markdup        mark duplicates
     ampliconclip   clip oligos from the end of reads

  -- File operations
     collate        shuffle and group alignments by name
     cat            concatenate BAMs
     merge          merge sorted alignments
     mpileup        multi-way pileup
     sort           sort alignment file
     split          splits a file by read group
     quickcheck     quickly check if SAM/BAM/CRAM file appears intact
     fastq          converts a BAM to a FASTQ
     fasta          converts a BAM to a FASTA
     import         Converts FASTA or FASTQ files to SAM/BAM/CRAM

  -- Statistics
     bedcov         read depth per BED region
     coverage       alignment depth and percent coverage
     depth          compute the depth
     flagstat       simple stats
     idxstats       BAM index stats
     phase          phase heterozygotes
     stats          generate stats (former bamcheck)
     ampliconstats  generate amplicon specific stats

  -- Viewing
     flags          explain BAM flags
     tview          text alignment viewer
     view           SAM<->BAM<->CRAM conversion
     depad          convert padded BAM to unpadded BAM

  -- Misc
     help [cmd]     display this help message or help for [cmd]
     version        detailed version information

(base) radhu@Radhu:~$ bwa

Program: bwa (alignment via Burrows-Wheeler transformation)
Version: 0.7.17-r1188
Contact: Heng Li <lh3@sanger.ac.uk>

Usage:   bwa <command> [options]

Command: index         index sequences in the FASTA format
         mem           BWA-MEM algorithm
         fastmap       identify super-maximal exact matches
         pemerge       merge overlapping paired ends (EXPERIMENTAL)
         aln           gapped/ungapped alignment
         samse         generate alignment (single ended)
         sampe         generate alignment (paired ended)
         bwasw         BWA-SW for long queries

         shm           manage indices in shared memory
         fa2pac        convert FASTA to PAC format
         pac2bwt       generate BWT from PAC
         pac2bwtgen    alternative algorithm for generating BWT
         bwtupdate     update .bwt to the new format
         bwt2sa        generate SA from BWT and Occ

Note: To use BWA, you need to first index the genome with `bwa index'.
      There are three alignment algorithms in BWA: `mem', `bwasw', and
      `aln/samse/sampe'. If you are not sure which to use, try `bwa mem'
      first. Please `man ./bwa.1' for the manual.

(base) radhu@Radhu:~$ conda install -c bioconda sambamba
Collecting package metadata (current_repodata.json): done
Solving environment: failed with initial frozen solve. Retrying with flexible solve.
Solving environment: failed with repodata from current_repodata.json, will retry with next repodata source.
Collecting package metadata (repodata.json): done
Solving environment: done

## Package Plan ##

  environment location: /home/radhu/miniconda3

  added / updated specs:
    - sambamba


The following packages will be downloaded:

    package                    |            build
    ---------------------------|-----------------
    sambamba-0.6.6             |                2         1.1 MB  bioconda
    ------------------------------------------------------------
                                           Total:         1.1 MB

The following NEW packages will be INSTALLED:

  sambamba           bioconda/linux-64::sambamba-0.6.6-2


Proceed ([y]/n)? y


Downloading and Extracting Packages
sambamba-0.6.6       | 1.1 MB    | ################################################################################################################################################################ | 100% 
Preparing transaction: done
Verifying transaction: done
Executing transaction: done
(base) radhu@Radhu:~$ sambamba
sambamba 0.6.6

Usage: sambamba [command] [args...]

    Available commands: 'view', 'index', 'merge', 'sort',
                        'flagstat', 'slice', 'markdup', 'depth', 'mpileup'
    To get help on a particular command, just call it without args.

Leave bug reports and feature requests at
https://github.com/lomereiter/sambamba/issues

(base) radhu@Radhu:~$ ^C
(base) radhu@Radhu:~$ 
```
