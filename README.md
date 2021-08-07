# EMDrama

This repository contains the **SimpleText** files for the texts in the
**Early Modern Drama Corpus** from the Visualizing English Print (VEP project).

**Quickstart:** If you want to download the files, press the "Code" button
(upper right above the README) and select "Download ZIP". This way you can get
the files without using GIT.

If you are a GIT user, you can also clone this repository. If you don't know what
that means, use the "Download ZIP" option from the "Code" button above.

## What is this?

The [Visualizing English Print (VEP)](http://vep.cs.wisc.edu/) project was an effort
to scalable, digital scolarship of Early Modern texts possible. The project ran
from 2011-2016. The project is now over, but we are trying to make the things we
created available.

The [Early Modern Drama Corpus](LINK) was a component of VEP sought to identify the "plays"
written during the time period (see LINK for more explanation). Prof. Jonathan Hope
lead a team that identified 1554 texts. Metadata for these texts is available at LINK.

[Text Creation Partnership (TCP)](https://textcreationpartnership.org/) had made available
transcriptions of 1292 of the 1554 texts. We say "had" because we used the TCP as of
the summer of 2015. It could be that more texts are now available, or that updated
versions have become available.

**This Repository** contains the *SimpleText* versions of the 1292 documents.
That is, if you copy this repository, you will have 1292 `.txt` files
(in VEP SimpleText format). If you want something other than the SimpleText files,
you will need to look elsewhere. If you want less than the whole thing, you may want
to look elsewhere. See below for suggestions...

**SimpleText** is a simplified file format that was developed by the VEP project
in order to make certain kinds of analysis convenient. It is derived from the original
XML files available from the TCP. It purposefully throws away information
in the source files to make it convenient and consistent to perform analysis on the words.
Metadata is stored separately. It seeks to make consistent and transparent access to the
information in the TCP files. If there are errors, they are reproduced.
If we introduce errors, we do it consistently.

Briefly, SimpleText files are ASCII files (a limited character set) that include the
transcribed "words" without any metadata. Some limited standardization has been done to
improve consistency LINK.
But the format and its process were designed for simplicity, convenience, and traceability.
It was intended to help enable consistent, corpus scale inquiries (which necessarily mean
computation analysis).
If you are looking for a format that is better for humans to read, or has extensive
metadata, look elsewhere.

These documents are **split**, in an attempt that they contain only the dramatic work
itself. The source TCP file may contain multiple works, or other material
(e.g., frontmatter).
A single TCP file may create a number of different "play" files, and may contain
text not included in any file. See *Filename Conventions* below.

This **version** of the files was dated September 14, 2016. That is, we believe that
these files were processed (converted by a team member from the TCP XML sources on hand)
on (or before) that date. We are not actually sure which "version" of the TCP XML files were
used.

## The File Naming Convention

The `SimpleText` folder has 1292 files (one for each work). Each is a `.txt` file.

The file names begin with the TCP identifier. If the file contains less than the
entirety of the content the portion is included in the file name. For example:

+ `A00969.headed.txt` is Shakespeare's "The Two Noble Kinsmen" - and it is the
    entirety of the "headed" section of TCP file A00969.
+ `A11954.headed_014_play_001.txt` is Shakespeare's "The Tempest" from the First Folio.
    The First Folio is TCP id A11954, and it contains many plays.
    This work is the 14th "chunk" of the TCP file, and the TCP called the "chunk"
    a "play".
    To be more precise, in the TCP XML file, this is a `play` entity from which the
    work was extracted.
    (We use "chunk" in scare quotes because we lack a better word for it.
    "Near-top level XML entity that contains text" might be a better description).
+ `A01227.headed_003_part_001.txt` is the play "Phillis and Amyntas".
    Even though it is the only play in the TCP file, the TCP file contains other
    contents, so we have only included the contents of the 3rd "chunk" which is a
    `part` entity.

## What else can I get?

Again, this repository has only the SimpleText versions of the Drama Corpus.

If you want the **metadata** ours is available LINK.

If you want an individual file, it can be inconvenient to use GitHub to get it.
You can get links to the individual files using the LINK.

If you want more extensive information about each TCP document, you may want to consult
the [EarlyPrint](https://earlyprint.org/) project. They have a very complete archive
of extensively annotated texts. Early Print has a very contrasting set of goals LINK
from SimpleText.

If you want SimpleText (or MetaData) for more of the TCP
(i.e., everything available to us in the Summer of 2015), you can find that at LINK.
Be warned: those files are not "split" - there is a single SingleText document for
each TCP document.

If you want the source XML files, you can get those from other sources, including the
TCP. If you want to see the page images, you will need to go elsewhere.

## What if I have Questions?

Unfortunately, the VEP project is over.
However, the PIs still care about it so you can write to us.

Note: if you find an "error", remember that our goal is to be consistent
and transparent. If there is an error in the original transcription, we
intentionally reproduce it. If we introduce an error in extracting and
converting the transcriptions, we do so consistently.

If you want a "corrected" set of texts, look to the
[EarlyPrint](https://earlyprint.org/) project.
