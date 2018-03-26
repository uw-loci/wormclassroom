---
layout: page
permalink: /protein-sequencing-tools
---
Here are some brief instructions for using some amino acid sequencing
tools. There are \"Help\" pages in each program\'s website. This page is
just a place for you to get started. Once you are familiar with the
program, you can experiment with different parameters or settings.

LALIGN
------

[Go to LALIGN
Server](http://www.ch.embnet.org/software/LALIGN_form.html)

Keep \"default\" setting unless specified below.

1.  Change the \"Choose the alignment method\" to \"Global without
    end-gap penalty\".
2.  Change \"Number of reported sub-alignments\" to 1.
3.  Copy your two sequences and paste them to the two text fields
    respecitivly. Note: your input sequence need to match the \"Input
    sequence format\" of your chice. Choose \"plain text\" if your
    sequence only contains plain amino acid sequence (no \"\<\", \";\"
    \-- symbols).
4.  Then run LALIGN
5.  Result:
    -   You will see the percentage of identities and the two sequences
        aligned parallelly. Sequence1 will show on top of sequence2.
    -   By default: \":\" means two amino acids or nucleotides are the
        same within the two sequences. \".\" means the second a.a or
        nucleotide is a conservative replacement of the first one, \" \"
        means non-conservative replacements.
6.  Note: this tool is not very senstitive which means if your two
    sequences contains thousands of amino acids or nucleotides and only
    one of the a.a. or nucleotide is different in these two sequences,
    it will show 100% identity. However, you can still find the
    difference by carefully checking the comparison result.

SIM + LALNVIEW
--------------

[Go to SIM Alignment Tool](http://web.expasy.org/error/removed.html)

Use default value unless specified below.

1.  Select \"User-entered sequence\"
2.  Parameters
    -   Number of alignments to be computed: 1
3.  Result:
    -   -Will show the percentage of identity between two sequences.
    -   \"\*\" under each comparison means these two amino acids or
        nucleotides are the same. Thus, if you want to find differences
        between two sequences, find the one without \"\*\".
4.  Note: Same as LALIGN, if you have thousands of amino acids or
    nucleotide in the sequence and only one difference between two
    sequences, this program will show 100% identity between these two
    sequences. However, by looking into the result, you are able to find
    the only one difference between the two sequences.

DOTLET
------

[Go to DOTLET](http://alggen.lsi.upc.es/softpublic/dotlet/Dotlet.html)

The \"[need
help?](http://ccg.vital-it.ch/java/dotlet/dotlet_help.html)\" page is
very helpful

1.  Enter your sequence by pressing \"input\" botton, a dialog will show
    that allows you to pick a name for your sequence. Paste your
    sequence into the text box. Hit \"ok\". Then press \"input\" botton
    again to enter the second sequence. Repeat this process if needed.
2.  Then pick two sequences you want to compare with.
3.  Hit \"compute\" to get the comarison result.
4.  Result:
    -   See \"[need
        help?](http://ccg.vital-it.ch/java/dotlet/dotlet_help.html)\"
        for result interpretation.
5.  Note:
    -   For this program, it might not be easy to understand the
        histogram if you are a first time user. Try to copy two totally
        different sequences (with big variatiation between two
        sequences, such as in length), compute the differences and get a
        sense on how the histogram is like. Then you can start to work
        on two very similar sequences and get a better sense on how they
        differ from each other.
    -   You always can use the \"Alignment\" tool down in the bottom to
        compare two sequences by doing one by one comparison.
