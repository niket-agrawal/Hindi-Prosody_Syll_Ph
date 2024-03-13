## Prosody, Syllables, Phonemes and IPA for Hindi words (Python3)

### ```input.py```

To syllabilfy and find IPA for whole file, e.g.```sample_text.txt```,

- Step 1 - ```cd``` to folder Hindi-Prosody_Syll_Ph
- Step 2 - Execute: ```python src/input.py```. It will generate GUI and user can feed the words or files as input and the output will generated in GUI as well as in the form a text file.
- Step 3 - Then select your file from file input/output dialog box. Your file should contain only one word per line.
- Step 4 - It will generate 2 files in data directory: ```PLS_XML_W3C_Format_Lexicon.txt``` and ```PLS_XML_W3C_Format_Lexicon.txt```. It will also generate 2 additional files (exceptions) ```rejected_items_phoneme.txt``` and ```rejected_items_labeling.txt```
- Note: Please note that the code in current from does contains some bugs and is not able to syllabify words containing two consecutive vowels at the end, among some other bugs. For all such bugs, it raises and exception and appends such words to rejected words list.

This package adapts from a Python2 code for Hindi language (Python3). 
Credits to [somnat/Hindi-word-prosody](https://github.com/somnat/Hindi-word-prosody)

### Hindi-Word-Prosody
- Pronunciation lexicon is one of the essential resource for building a Speech-to-Text(STT)  or Text-to-Speech (TTS). 
- This library is intended for generating the phonemic sequence for a given Hindi graphemic input along with its word-level prosodic structure. 
- The prosodic structure includes the syllable boundaries as well as the syllable weight.
- The Heavy and Super heavy syllables are generally the stressed syllables. However, in some cases heavy syllables are not stressed. The above library includes all the rules to correctly capture the prosodic structure.
- Hindi is a morphologically rich language. Therefore, all derived words and compound words delete schwa at morphological boundaries.

For example: कमला becomes 'kam.la: where "." is the syllable boundary and ' specifies the stressed syllable.

#### More details can be found in the following paper. 


### Citations

Please cite Hindi-Word-Prosody in your publications if it helps your research.
The following is a [BibTeX](http://www.bibtex.org/) and plaintext reference for our
[Hindi-Word-Prosody](https://cdn.iiit.ac.in/cdn/ltrc.iiit.ac.in/icon2017/proceedings/icon2017/pdf/W17-7502.pdf).


### Dependencies
- tkinter

