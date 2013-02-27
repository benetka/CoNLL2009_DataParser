#CoNLL 2009 Data Parser

Easy helper application for parsing data in CoNLL 2009 format (http://ufal.mff.cuni.cz/conll2009-st/task-description.html#Dataformat). I use this app for parsing output of the [Semantic Role Labeling Tagger in GATE](https://github.com/jendarybak/GATE-SRL).

## Data Format

####Columns:
ID FORM LEMMA PLEMMA POS PPOS FEAT PFEAT HEAD PHEAD DEPREL PDEPREL FILLPRED PRED APREDs

####Description of the columns
ID, FORM, LEMMA, POS, FEAT, HEAD and DEPREL are the same as in the CoNLL-2006 and CoNLL-2007 Shared Tasks.

FEAT is a set of morphological features (separated by |) defined for a particular language, e.g. more detailed part of speech, number, gender, case, tense, aspect, degree of comparison, etc.

The P-columns (PLEMMA, PPOS, PFEAT, PHEAD and PDEPREL) are the autoamtically predicted variants of the gold-standard LEMMA, POS, FEAT, HEAD and DEPREL columns. They are produced by independently (or cross-)trained taggers and parsers.

PRED is the same as in the 2008 English data. APREDs correspond to 2008's ARGs. FILLPRED contains Y for lines where PRED is/should be filled.

(Taken from: http://ufal.mff.cuni.cz/conll2009-st/task-description.html#Dataformat)