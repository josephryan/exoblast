<font color=red>NOTE: I recommend BUSCO over exoblast.</font>

exoblast
=======

DESCRIPTION
-----------

exoblast is being actively developed and tested. Please use with caution. I appreciate hearing about your experience with the program.

exoblast compares genome assemblies using sequence similarity to transcript or protein sequences from a different species.

INSTALLATION
------------

To install this program and documentation type the following:

    perl Makefile.PL
    make
    make install

RUN
---

    exoblast --query=FASTA_FILE --blast=tblastn_OR_tblastx --out=PREFIX_FOR_OUTFILES --assembly=FASTA_ASSEMBLY1 --assembly=FASTA_ASSEMBLY2 [--assembly=ADDITIONAL_ASSEMBLY ...] [--num_queries=NUMBER_OF_QUERIES] [--eval=EVAL] [--threads=NUM_THREADS] [--blastdb=USE_EXISTING_BLASTDB] [--saveblastdb=PATH/FILE_TO_SAVE_GENERATED_BLASTDB] [--randomseed=RANDOMSEED_FOR_PICKING_QUERY_SEQS] [--min_contig_size=IGNORE_ASSEMBLED_SEQS_SHORTER_THAN_THIS] [--version] [--help]

TEST
----

exoblast --query=exoblast_test_files/prots.fa --assembly=exoblast_test_files/assembly1.fa --assembly=exoblast_test_files/assembly2.fa --blast=tblastn --out=test.exoblast


DOCUMENTATION
-------------

    perldoc exoblast

DEPENDENCIES
------------

This program requires Perl

It also requires BLAST+:

   http://blast.ncbi.nlm.nih.gov/Blast.cgi?PAGE_TYPE=BlastDocs&DOC_TYPE=Download


CITATION
------------

    Ryan, Joseph F., exoblast, (2014), GitHub repository, https://github.com/josephryan/exoblast

COPYRIGHT AND LICENSE
------------

Copyright (C) 2014, Joseph F. Ryan

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program in the file gpl.txt.  If not, see
http://www.gnu.org/licenses/.

