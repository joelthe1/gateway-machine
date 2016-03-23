# The Gateway Machine
An MT engine which aims to map Gateway language Bibles to mapped target languages.

###Goal
To make an reasonably accurate machine translation system that translates the Bible from and to any set of mapped languages.

###Proposed Approach
1) Perform Part-of-Speech (POS) tagging of the corresponding source Gateway language Bible.
2) Build/Translate a relevant (to those used in the Bible) lexicon and it's usages in the target language.
3) Machine generates a mapped output based on the words and tags from the source text to the target text. Improvisations can be made (per language) to generate a more accurate result.

###Intuition
Exploit the fact that the source text is constant. This allows us to restrict the initial (seed) translation to be minimal and that the source text need not be tagged separately each time a translation is carried out.

###Pros
1) Could yield more accurate and reliable results.
2) The source text need only be tagged once (per Gateway language).
3) Only a subset of the target language lexicon with usages need be translated manually.

###Cons
1) Needs manual tagging of source text, if not already done.
2) Needs the manual translation of lexicon with usages in target language.
3) Output accuracy needs to be experimentally verified.
