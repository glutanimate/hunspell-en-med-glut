## README for hunspell-en-med-glut


###Overview

    Description:        Hunspell dictionary of English medical terms
    Terms:              90142
    Author:             Glutanimate (https://github.com/Glutanimate)
    Original Authors:   R. Robinson <info@e-medtools.com>, 
                        Rajasekharan N. <https://plus.google.com/u/0/+Rajasekharan-N/>
    Sources:            - OpenMedSpel by R. Robinson of e-MedTools 
                          <http://www.e-medtools.com/openmedspel.html>
                        - Raj&Co-Med-Spel-Chek by Rajasekharan N. of Raj&Co
                          <http://rajn.co/free-medical-spell-checker-for-microsoft-word-custom-dictionary/>
    License:            GNU GPL v3 (see LICENSE for more information)


###Description

This is a Hunspell dictionary of English medical terms. It is based on two prominent medical dictionary projects:

 - [OpenMedSpel](http://www.e-medtools.com/openmedspel.html) by e-MedTools
 - [Raj&Co-Med-Spel-Chek by Rajasekharan N. of Raj&Co](http://rajn.co/free-medical-spell-checker-for-microsoft-word-custom-dictionary/)

the two sources have been merged, deduplicated, corrected and converted into a Hunspell dictionary file.

###Installation

    git clone https://github.com/Glutanimate/hunspell-en-med-glut.git
    cd hunspell-en-med-glut
    sudo cp en_med_glut.dic '/usr/share/hunspell/en_med_glut.dic'
    sudo mkdir /var/lib/dictionaries-common/hunspell
    sudo cp hunspell-en-med-glut /var/lib/dictionaries-common/hunspell/hunspell-en-med-glut
    
###Usage

    # hunspell -d en_US,en_med_glut -a < input_file.txt
    

Note: This might not work properly with LibreOffice/OpenOffice because of a number of bugs (1). If that's the case for your system use [my workaround](https://github.com/Glutanimate/hunspell-en-med-glut-workaround) instead.

###Warranty

This software comes with no warranty of any kind. Some misspelled words might be included. If you find any mistakes please report them through the [issues tracker](https://github.com/Glutanimate/hunspell-en-med-glut/issues).

###Sources

(1): 

https://bugs.launchpad.net/ubuntu/+source/language-support-extra-de/+bug/363619

https://bugs.launchpad.net/ubuntu/+source/openoffice.org/+bug/329968

https://bugs.launchpad.net/medicalterms/+bug/401423
