UPDATE - autoQC development has moved to the CAMDU fork at https://github.com/warwickcamdu/auto_qc .



[![DOI](https://zenodo.org/badge/169840753.svg)](https://zenodo.org/badge/latestdoi/169840753)  [![Scaladoc](https://javadoc-badge.appspot.com/uk.ac.warwick.camdu/nscala-time_2.11.svg?label=javadoc)](https://erickmartins.github.io/auto_qc/) [![Build Status](https://travis-ci.com/erickmartins/auto_qc.svg?branch=master)](https://travis-ci.com/erickmartins/auto_qc)



ImageJ plugin auto_qc


Continuing development by Erick Ratamero, experimental input from Claire Mitchell  
https://www.warwick.ac.uk/camdu


Based on the .py scripts from Erick Ratamero:  
https://github.com/erickmartins/autoQC_jython


Auto-generated Javadoc is available:  
https://erickmartins.github.io/auto_qc/


Initial work by group 4 of the NEUBIAS trainingschool 11:  
Erick Ratamero, Cesar Augusto Valades Cruz, Christopher Schmied, Jan Eckhardt, Paul Stroe.

==========================================================================================

Usage Instructions:

autoPSF: expects Z-stacks with sub-resolution fluorescent beads.  Multichannel stacks are fine; you can pick which channel to use as a parameter.

autoFOV: expects single 2d images of a fluorescent slide (uniform sample).  Multichannel images also fine, will operate over each individual channel and save all results.

autoColoc: expects 4d images (XYCZT) of larger-than-resolution fluorescent beads.  

autoStageRepro: expects 3d images (timelapse). Each timepoint should be recorded after translating the stage and moving it back to its original position.

If you're using files from multiple folders, outputs will be saved on the folder where the first file is.  

You can operate over multiseries files - the match string parameter tells the program what substring it should look for. For example, if you have a multiseries file and you wan to run autoPSF only over series containing "psf" on their names, use "psf" as the match string parameter.

Note that, for multiseries files (e.g. mvd2), the same calibration is used for all series - do not mix different objectives on the same file!    

When in doubt, consult the [MetroloJ Manual](http://imagejdocu.tudor.lu/lib/exe/fetch.php?media=plugin:analysis:metroloj:metroloj.pdf) for detailed protocols.   

For OMERO stuff, you need the [OMERO Plugin for ImageJ](https://www.openmicroscopy.org/omero/downloads/). 





==========================================================================================
Citations:


Based on ImageJ:  
Schneider, C. A.; Rasband, W. S. & Eliceiri, K. W. (2012), "NIH Image to ImageJ: 25 years of image analysis", Nature methods 9(7): 671-675, PMID 22930834

Used to run Fiji in the background:  
Schindelin, J.; Arganda-Carreras, I. & Frise, E. et al. (2012), "Fiji: an open-source platform for biological-image analysis", Nature methods 9(7): 676-682, PMID 22743772, doi:10.1038/nmeth.2019


Uses the following plugins:  

bioformats (https://www.openmicroscopy.org/bio-formats/)  
Melissa Linkert, Curtis T. Rueden, Chris Allan, Jean-Marie Burel, Will Moore, Andrew Patterson, Brian Loranger, Josh Moore, Carlos Neves, Donald MacDonald, Aleksandra Tarkowska, Caitlin Sticco, Emma Hill, Mike Rossner, Kevin W. Eliceiri, and Jason R. Swedlow (2010) Metadata matters: access to image data in the real world. The Journal of Cell Biology 189(5), 777-782. doi: 10.1083/jcb.201004104


Uses code from:

MetroloJ (http://imagejdocu.tudor.lu/doku.php?id=plugin:analysis:metroloj:start)  
Cédric Matthews and Fabrice P. Cordelieres, MetroloJ : an ImageJ plugin to help monitor microscopes' health, in ImageJ User & Developer Conference 2010 proceedings

TrackMate (https://imagej.net/TrackMate)  
Tinevez, JY.; Perry, N. & Schindelin, J. et al. (2016), "TrackMate: An open and extensible platform for single-particle tracking.", Methods 115: 80-90, PMID 27713081


==========================================================================================
Acknowledgements

Special thanks goes to:

- Robert Haase
- Jean-Yves Tinevez

For their help and guidance

NEUBIAS and NEUBIAS TS11 organisers for creating the environment

==========================================================================================


