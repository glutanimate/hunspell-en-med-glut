## Hunspell Dictionary of English Medical Terms

### Overview

This is a dictionary of English medical terms for Hunspell. It is based on two prominent medical dictionary projects:

 - [OpenMedSpel](http://www.e-medtools.com/openmedspel.html) by e-MedTools
 - [MTH-Med-Spel-Chek by Rajasekharan N. of MT-Herald](http://mtherald.com/free-medical-spell-checker-for-microsoft-word-custom-dictionary/)

The two sources have been merged, deduplicated, corrected, and converted into a Hunspell dictionary file.

### Details

    Number of Terms:    90142
    Contents:           drug names (up-to-date with FDA-approvals as of 2014-04-02, trade and generic names),
                        anatomical terms, dermatological terms, internal medicine terms, surgical terms,
                        DSM-IV terms, ICD-9 terms, and many more
    Author:             (c) 2014-2017 Aristotelis P. (https://github.com/Glutanimate)
    Original Authors:   (c) 2007-2014 R. Robinson <info@e-medtools.com>, 
                        (c) 2009-2014 Rajasekharan N. <https://plus.google.com/u/0/+Rajasekharan-N/>
    Original Sources:   - OpenMedSpel by R. Robinson of e-MedTools (Version 2.0.0, released 2014-01-21)
                          <http://www.e-medtools.com/openmedspel.html>
                        - MTH-Med-Spel-Chek by Rajasekharan N. of MT-Herald (released 2014-04-02)
                          <http://mtherald.com/free-medical-spell-checker-for-microsoft-word-custom-dictionary/>
    License:            GNU GPL v3 (see LICENSEs for more information)

### Installation

    git clone https://github.com/Glutanimate/hunspell-en-med-glut.git
    cd hunspell-en-med-glut
    sudo cp en_med_glut.dic '/usr/share/hunspell/en_med_glut.dic'
    sudo mkdir -p /var/lib/dictionaries-common/hunspell
    sudo cp hunspell-en-med-glut /var/lib/dictionaries-common/hunspell/hunspell-en-med-glut

###Usage
 
From the command-line:

    hunspell -d en_US,en_med_glut -a < input_file.txt

### Warranty

This software comes with no warranty of any kind. Some misspelled words might be included.

### Issues with LibreOffice

The following bugs might prevent this dictionary from working properly with LibreOffice:

- https://bugs.launchpad.net/ubuntu/+source/language-support-extra-de/+bug/363619
- https://bugs.launchpad.net/ubuntu/+source/openoffice.org/+bug/329968
- https://bugs.launchpad.net/medicalterms/+bug/401423

If you are experiencing any of these you might want to try [my workaround dictionary](https://github.com/Glutanimate/hunspell-en-med-glut-workaround), instead.