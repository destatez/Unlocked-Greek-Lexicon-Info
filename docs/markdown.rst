.. _markdown:

Markdown
========
The lemma files for en_ugl are defined in Markdown format. This format/language is a convenient means to specify the desired format of the **visual output** for the project. When you select a lemma file on the DCS web you will see this visual form, though the final, published, visual form may be slightly different. When editing a file, you will be working in the Markdown language environment. This document will endeavor to specify the required Markdown format and content of each lemma file to achieve the project-desired output, consistently across all lemmas for all editors. Markdown is blank line sensitive which means that data within a marker can be entered on multiple consecutive lines and will be merged together from a syntax checking and the visual output perspective. A blank line must be entered between data lines to have that data treated as separate from a syntax checking and the visual output perspective. Markdown also provides a way to add emphasis to data that is entered. Text that is enclosed within a single “*” or a single “_” will be italicized. Text that is enclosed within double “*” or double “_” will be displayed bold. These can be combined to achieve both forms of emphasis. The following example will be displayed as below:
::

  This **bold data**
  is entered *with italics* on
  multiple consecutive lines


This **bold data** is entered *with italics* on multiple consecutive lines

Syntax Checker
--------------
A Syntax Checker has been developed to read a lemma markdown file and determine whether it meets the requirements of this document. A change log for that Syntax Checker script, in the form of a Google Doc, can be found at `this link <https://docs.google.com/document/d/1wugi6DJIDEq2tu_eMro3uXWCPn2zNB0kLMnRtGh_VmI/edit?usp=sharing>`_

Markers
-------
The Markdown format is achieved with the use of markers (marker lines). Any line which starts with a pound sign, “#” or an asterisk, “*”, is considered a marker. Apart from the first line, there must be at least one blank line before and after each marker. These markers should not be altered or reordered so that consistency across the project can be maintained. Only 4 of these markers allow/require data to be entered as part of the actual marker line. These are:

#. \* Strongs: <Strongs-plus identifier>, see `Strongs <https://ugl-info.readthedocs.io/en/latest/markdown.html#strongs-gddddd>`_ , below.

#. \* Instances in the New Testament: <instance count>, see `Instances Count <https://ugl-info.readthedocs.io/en/latest/markdown.html#instances-in-the-new-testament-count>`_ , below.

#. \* All Scriptures cited: "Yes" or "No",  see `All Scriptures cited <https://ugl-info.readthedocs.io/en/latest/markdown.html#all-scriptures-cited-yes-no>`_ , below.

#. \#\#\# Sense <sense number>:, see `Sense <https://ugl-info.readthedocs.io/en/latest/markdown.html#sense-sense-number>`_ , below.

.. note:: As was discussed in the  `Content <http://ugl-info.readthedocs.io/en/latest/assignments.html#content>`_ section, there is a link labeled **refs** for each lemma in its Greek letter Instance Table of Contents web page which provides a list, in our project's format, of each of the references to that lemma.


References
----------

Greek Lemma Link
^^^^^^^^^^^^^^^^
There is a required format needed to specify a reference to a different Greek lemma within the body of this file. When to add these will be discussed under the appropriate marker discussions, below. The basic link format is in the form: [<Greek form of another lemma>](../<Strongs-Plus Identifier of that lemma>/01.md). Each instance of a link is made up of different pieces of associated data. Each link is required to have its associated referenced lemma’s “Definition” or “Gloss” from that lemma's UGL data which best fits the current context. This data piece must follow the corresponding specification of the link with a colon.  Optional textual narrative and/or `Sense Link`_ data pieces should follow this definition/gloss data with a semicolon. This narrative text and Sense Link can appear in any order after that semicolon, with no separator required between the narrative and Sense Link.  A comma should be used to separate each instance of a Greek Lemma Link.
The different formats for this are:
::

 {Basic form with no narrative or Sense Link}:
  [<Greek form of another lemma>](../<Strongs-Plus Identifier of that lemma>/01.md): <Definition or Gloss for that lemma>
   e.g.
    [πύργος](../G44440/01.md): a tower, [ἁγνός](../G00530/01.md): free from ceremonial defilement

 {Basic form with textual narrative}:
  [<Greek form of another lemma>](../<Strongs-Plus Identifier of that lemma>/01.md): <Definition or Gloss for that lemma>; <textual narrative>
   e.g.
    [πύργος](../G44440/01.md): a tower, [ἁγνός](../G00530/01.md): free from ceremonial defilement; to be clean from a Jewish ceremonial standpoint

 {Basic form with a Sense Link}:
  [<Greek form of another lemma>](../<Strongs-Plus Identifier of that lemma>/01.md): <Definition or Gloss for that lemma>; <Sense Link>
   e.g.
    [πύργος](../G44440/01.md): a tower, [ἁγνός](../G00530/01.md): free from ceremonial defilement; [Sense 1.1](#sense-11) 

 {Basic form with a Sense Link and textual narrative}:
  [<Greek form of another lemma>](../<Strongs-Plus Identifier of that lemma>/01.md): <Definition or Gloss for that lemma>; <textual narrative> 
  <Sense Link>
   e.g.
    [πύργος](../G44440/01.md): a tower, [ἁγνός](../G00530/01.md): free from ceremonial defilement; to be clean from a Jewish ceremonial standpoint [Sense 1.1](#sense-11) 


Scripture Links
^^^^^^^^^^^^^^^
References to passages of Scripture, Old Testament, New Testament, of Septuagint also have a fixed format. When to add these will be discussed under the appropriate marker discussions, below. The format for this is:
::

  [<Standard book name> <chapter number>:<verse number>](<USFM book name> <chapter number>:<verse number>)

Note: <Standard book name> and <USFM book name> entries have a defined set of values in a predefined format as documented in the `USFM Names <http://ugl-info.readthedocs.io/en/latest/abbreviations.html#usfm-names>`_ section. 
   
Each instance of a reference should be separated with a comma when a list of verses is desired.  A range of verses can be specified with a dash, "-", supplied between the start and the end of the range.  Sequential references in the same book or same chapter of the same book can be abbreviated in their Standard form, though their USFM form must be complete for each reference. These sequential, abbreviated, references cannot be separated by references to other books.
e.g.
::


   Example of a list of verse referenes:
     [1Cor 3:5](1co 3:5), [4:4](1co 4:4), [5](1co 4:5)

   Example of a range of verses reference:
     [Mark 12:36](mrk 12:36)-[38](mrk 12:38)

   Example of a range of verses reference within a list of other verse references:
     [Matt 22:43](mat 22:43), [45](mat 22:45), [Mark 12:36](mrk 12:36)-[38](mrk 12:38), [Luke 20:42](luk 20:42), [44](luk 20:44)

Hebrew Lemma Links
^^^^^^^^^^^^^^^^^^

There is also a fixed format for a reference to a Hebrew Lemma file. When to add these will be discussed under the appropriate marker discussions, below. The basic link format is in the form: [<Hebrew lemma]( //en-uhal/<Hebrew Strongs ID for that lemma>). Additional data may be added for each of the Hebrew lemma links. A single definition or gloss for the lemma will follow that link and be preceded by a colon. This is optional and not a requirement for these Hebrew lemma links, as it is for the Greek lemma links. Following this definition/gloss may be narrative text and/or a sense link. These should be preceded with a semicolon. This narrative text and Sense Link can appear in any order after that semicolon, with no separator required between the narrative and Sense Link. A comma should be used to separate each instance of a Hebrew Lemma Link.
The formats for the different options are as follows (using a 4-digit Strong’s number):
::

 {Hebrew lemma reference with no definition and no textual narrative}:
  [<Hebrew lemma]( //en-uhal/<Hebrew Strongs ID for that lemma>)
  e.g.
   [בַּעַל](//en-uhal/H1167), [בֹּשֶׁת](//en-uhal/H1322), [נפל](//en-uhal/H5307), [שׂום](//en-uhal/H7760)

 {Hebrew lemma reference with a definition and with no textual narrative}:
  [<Hebrew lemma]( //en-uhal/<Hebrew Strongs ID for that lemma>): <Hebrew Lemma gloss>
  e.g.
   [בַּעַל](//en-uhal/H1167), [בֹּשֶׁת](//en-uhal/H1322): shame, [נפל](//en-uhal/H5307), [שׂום](//en-uhal/H7760)

 {Hebrew lemma reference with no definition but with a textual narrative}:
  [<Hebrew lemma]( //en-uhal/<Hebrew Strongs ID for that lemma>); <textual narrative>
  e.g.
   [בַּעַל](//en-uhal/H1167), [בֹּשֶׁת](//en-uhal/H1322); this can also refer to a shameful thing, [נפל](//en-uhal/H5307), [שׂום](//en-uhal/H7760)

 {Hebrew lemma reference with both a definition and a textual narrative}:
  [<Hebrew lemma]( //en-uhal/<Hebrew Strongs ID for that lemma>)>) : <Hebrew Lemma gloss> ; <textual narrative>
  e.g.
   [בַּעַל](//en-uhal/H1167), [בֹּשֶׁת](//en-uhal/H1322): shame; this can also refer to a shameful thing, [נפל](//en-uhal/H5307), [שׂום](//en-uhal/H7760)

.. note:: This is a slight difference from the format defined earlier in this Phase of the program. If you have had previous lemma files merged into the main repository with the format, “en-uhl” instead of “en-uhal” these will be programmatically corrected before their Final Review.
.. note:: Since the tooling for this other lexicon is not operative, as yet, endeavoring to follow one of these links will results in a 404 error, Page Not Found. 

If you desire to see a specific Hebrew lemma file at this time, enter the following web address in a web browser address bar: 
::

  https://git.door43.org/unfoldingWord/en_uhal/src/branch/master/content/{UHAL Strong’s ID}.md (When doing this make sure you insert the desired Hebrew lemma’s associated Strong’s ID number into the relevant portion of the web address above. The relevant portion being {UHAL Strong’s ID}). 
  
  If you wish to view an index of all the Hebrew lemmas and their associated Strong’s ID numbers enter the following web address in a web browser address bar:
  
   https://git.door43.org/unfoldingWord/en_uhal/src/branch/master/content

Sense Link
^^^^^^^^^^

A link reference to a specific Sense definition for the current Lemma can be made whereever textual narrative is allowed. This was discussed above and will be alluded to in the discussion of content for the different UGL markers, below. These have a fixed format as shown below:
::

  [<visual expression of sense number>](<linking expression of sense number>)
    Where <linking expression of sense number> combines the following characters:
      “#sense-” & sense number with periods removed
 e.g.
  {for reference to Sense 1.0, 1.1, and 3.1.2}
     [Sense 1.0](#sense-10), [Sense 1.1](#sense-11), [Sense 3.1.2](#sense-312),
  
UGL Markers
-----------
The UGL markers will be identified below. They should remain as entered and they should not be reordered. An example follows this discussion.

1. # <Greek lemma>
^^^^^^^^^^^^^^^^^^
The first line of each lemma file is a marker identifying its lemma. The initial format which came from the originating Abbott Smith lexicon uses a dash before the second term. For consistency and alignment with newer lexica, change these to replace the **<space>–** with **,<space>**. This line should be terminated with a period. e.g.
::

  # ἄμφοδον -ου, το 

should be changed to:
::

  # ἄμφοδον, ου, το. 

2. Comment Markers
^^^^^^^^^^^^^^^^^^
Markdown does support specification of comments. Lines 3 and 4 of each lemma file have two comment lines. They start with “<!—“ and end with “-->”. This format specifies non-visible comments, that is comments that are in the lemma file but are not shown in the visual form. These two comment lines must remain in the file as entered:
::

   <!-- Status: S2=NeedsEdits -->

   <!-- Lexica used for edits:   -->

Editing for the first of these is only allowed for the value given to S2 (Stage 2 of project) and for the specification of the lexica that were used for editing the file, in the second comment. The valid values for S2 are:
  * NeedsEdit  {initial value when you start editing}
  * NeedsReview  {value you must enter before performing the git commit for your edits}
  * NeedsFinalCheck {Reviewer enters this when 1st Review is complete}
  * ReadyforPublication {Final Reviewer enters this when Final Check/2nd Review is complete}
  
The list of lexica should be entered as abbreviations per the list shown in the   `Lexica <http://ugl-info.readthedocs.io/en/latest/abbreviations.html#lexica>`_ section.

3. ## Word data 
^^^^^^^^^^^^^^^
This is a content/format marker with only other markers associated with it, so no data should be entered for it.

4. * Strongs: Gddddd. 
^^^^^^^^^^^^^^^^^^^^^
Identifies the Strong’s-Plus ID, with the 5-digit **ddddd** notation, for the lemma and was generated by the lemma file creation tool and should remain unchanged with the exception of adding a terminating period.

5. * Alternate spellings 
^^^^^^^^^^^^^^^^^^^^^^^^
This is the first marker where editing is allowed to add data to supply any variant or alternative spellings identified in the referenced lexica. This data should be entered as simple Greek text with no surrounding bracketing or parenthesis as discussed in `Greek Lemma Link`_ for referencing other Greek lemmas from this file, since that reference would point back to the current lemma file. Each instance that is specified should be separated with a comma. No additional data is required but any needed textual narrative for an instance should be separated from the Greek by a semicolon. If data is present it should data be terminated with a period.

6. * Principle Parts: 
^^^^^^^^^^^^^^^^^^^^^
This marker should be left empty for this Stage of the project.

7. * Part of speech: 
^^^^^^^^^^^^^^^^^^^^
This marker's data should be left empty for manual editing of each lemma file. A software tool will be run near the end of this Stage of the project which will populate this marker’s data with all of the POS instances that are found in Alan Bunnig’s spreadsheet  containing the entire UGNT. 

8. * Instances in the New Testament: <count> 
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
This count value should be left as-is since that instance count was based upon the data from the UGNT. The text for this marker may erroneously be **Instances in Scripture** or **Instances in the NT** and should be updated to be **Instances in the New Testament**. If there are more than 1 instance of the lemma in a specific verse, this should be identified with the addition of the text “{in xx verses}”, where xx is the number of unique verses that contain this lemma. The specific verses where this occurs will be noted as defined in `21. #### Citations:`_, below. This should data be terminated with a period. The formats for specifying this data are:
::

  {Where only one instance of this lemma is found in each verse}
    * Instances in the New Testament: 7.

  {Where there are 2 instances of this lemma found in 2 different verses}
    * Instances in the New Testament: 7 {in 5 verses}.


9. * All Scriptures cited: Yes/No
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
This marker should be followed with the word **Yes** or **No**, indicating whether every instance count reference appears in one of more of the data sections for the `21. #### Citations:`_, below. This line should be terminated with a period.

10. ## Etymology: 
^^^^^^^^^^^^^^^^^
This marker's data should contain any `Greek Lemma Link`_ that is etymologically tied to this lemma. Where present this data should be terminated with a period.

11. * LXX/Hebrew glosses: 
^^^^^^^^^^^^^^^^^^^^^^^^^
This marker's data should contain any associated data that was propagated from the A-S lexicon. That propagation may have placed this data under other markers in this file, and if so, it should be moved back to this marker's data. There may be no LXX/Hebrew gloss data for a given lemma file. Remove or expand any abbreviations that may remain and check the format for all scripture references against `Scripture Links`_. The LXX book references from Abbott-Smith were generally in the format **<LXX book>.<chapter>.<verse>**. These should be reformatted to reflect the documented reference format for the `USFM Names <https://ugl-info.readthedocs.io/en/latest/abbreviations.html#usfm-names>`_ portion of these UGL documents. An LXX/Hebrew gloss contains, at a minimum, a Scripture link and/or a Hebrew lemma link. A space should be used to separate these two if both are present for a single LXX/Hebrew gloss instance. Each instance must be separated from other instances by a comma, even if one instance has only a Hebrew lemma link, one instance has only a Scripture link, or one instance has both links. Each of these comma-separated instances may have leading textual narrative/discussion which must be preceded by a semicolon (;). No special punctutation is needed to transition from this narrative text to one or both of the links for this instance.  Where present this data should be terminated with a period. Examples of the different forms of this data are:
::

  {Scripture links only}
    [Exod 22:11](exo 22:11), [10](exo 22:10), [Amos 3:3](amo 3:3), [4](amo 3:4).

     {Scripture and Hebrew links with leading narrative}
           ;in LXX [Num 24:2](num 24:2) [ראה](//en-uhal/H7200), [Job 10:4](job 10:4), [39:26](job 39:26).

     {Scripture and Hebrew links with leading narrative and trailing gloss}
           ;in LXX [Num 24:2](num 24:2) [ראה](//en-uhal/H7200) : to see, [Job 10:4](job 10:4), [39:26](job 39:26).

      {Hebrew link only with leading narrative and trailing gloss}
           ;in LXX chiefly for [רעע](//en-uhal/H7489) : evildoer.

      {2 instances of Hebrew links only with leading narrative and trailing gloss}
      ;in LXX chiefly for [רעע](//en-uhal/H7489) : evildoer, ;in LXX also for [רֹעַ](//en-uhal/H7455) : evil.

12. * Time Period/Ancient Authors: 
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
This marker should have no data supplied for this stage of the project.

13. * Related words: 
^^^^^^^^^^^^^^^^^^^^
This marker's data should contain any other Greek lemmas that are identified by the other lexica, as being related to this lemma, but which are not etymologically related and do not qualify as being a synonym or antonym. These should be formatted per `Greek Lemma Link`_, above. Project time and schedule does not give us the freedom to perform our own research on this topic so we must rely solely upon the other lexica. Any Greek lemma reference identified by other lexica that is not a UGL-defined lemma should be omitted from this lexicon. To determine if a lemma is a UGL-defined lemma you will need to open up the associated Greek letter’s Word Sort TOC file, as discussed in `<http://ugl-info.readthedocs.io/en/latest/assignments.html#To more easily access these individual lemma files>`_ . The lemma must appear in that TOC file to be a UGL-defined lemma and if so, you can see the Strongs-Plus ID for it. Multiple links should be separated by a comma. A period should terminate this data when present.

14. * Antonyms for all senses: 
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
This marker's data should contain any other Greek lemmas that are identified by the other lexica as antonyms. These should be formatted per `Greek Lemma Link`_, above. Project time and schedule does not give us the freedom to perform our own research on this topic so we must rely solely upon the other lexica. Any Greek lemma reference identified by other lexica that is not a UGL-defined lemma should be omitted from this lexicon. To determine if a lemma is a UGL-defined lemma you will need to open up the associated Greek letter’s Word Sort TOC file, as discussed in `<http://ugl-info.readthedocs.io/en/latest/assignments.html#To more easily access these individual lemma files>`_ . The lemma must appear in that TOC file to be a UGL-defined lemma and if so, you can see the Strongs-Plus ID for it. Multiple links should be separated by a comma. A period should terminate this data when present.


15. * Synonyms for all senses: 
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
This marker's data should contain any other Greek lemmas that are identified by the other lexica as synonyms. These should be formatted per `Greek Lemma Link`_, above. Project time and schedule does not give us the freedom to perform our own research on this topic so we must rely solely upon the other lexica. Any Greek lemma reference identified by other lexica that is not a UGL-defined lemma should be omitted from this lexicon. To determine if a lemma is a UGL-defined lemma you will need to open up the associated Greek letter’s Word Sort TOC file, as discussed in `To more easily access these individual lemma files <http://ugl-info.readthedocs.io/en/latest/assignments.html#To more easily access these individual lemma files>`_ . The lemma must appear in that TOC file to be a UGL-defined lemma and if so, you can see the Strongs-Plus ID for it. Multiple links should be separated by a comma. A period should terminate this data when present.

16. ## Senses: 
^^^^^^^^^^^^^^
The only permitted data for this marker is one or more Sense markers with their associated sub-markers. Editors should start with the structure and content embedded in the files from the Abbott-Smith lexicon. After review and analysis of the sense data from the other lexica this Abbott-Smith starting point can be expanded with additional sense and sub-sense markers, can be down-sized with the removal of sense and sub-sense markers, and/or merely modified to update the Definitions and/or Glosses with the same number of sense and sub-sense markers. 

17. ### Sense <sense number>:  
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
The only permitted data for this marker is the in-line Sense number with a colon as the line terminator and the four sense sub-markers with their associated data. The sense number starts at 1.0 and increments at the decimal digit, the number preceding the decimal point, for each significant sense and increments at the fractional level to differentiate sub-senses of each significant sense. The sense number, and thus the senses, can vary from a single sense with the number 1.0, to complex sub-senses which could be in the form, 3.8.5, which would be the third significant sense, it’s eighth sub-sense, and that sub-sense’s fifth sub-sub-sense. It is recommended that you limit your sense levels to only two decimal digits as, 2.4, but three levels is the maximum, if required for completeness and accuracy. These sense numbers must occur in numerical order in the file, with no missing intermediate numbers; ### Sense 2.4 followed by ### Sense 2.6 would be flagged as a syntax error, since ###Sense 2.5 is missing. Every ### Sense marker is followed only by sub-markers, with no data specified for this marker. Each of the following sub-markers must be present and in the prescribed order given below.

.. note:: Many lexica use a sense numbering system that includes letters and possibly Greek letters, e.g. 1bα. This lexicon will use only numbers for each of the level of senses appropriate for the lemma, with a decimal point separating the sense from the sub-sense and then the sub-sub-sense numbers.

18. #### Definition: 
^^^^^^^^^^^^^^^^^^^^
This marker's data should contain the top-level definition for this Sense. It can be expressed as a full sentence or as a clause with multiple instances separated by a comma. Narrative text and/or `Sense Link`_ can be provided and must follow its associated definition data instance with a semicolon.  No termination mark should be entered. Some examples of this clausal form are:
::

  Aromatic substance burned as incense, An altar for burning incense
   
  To burn incense as an offering to a deity; this does not always refer to an incense offering to Yahweh, to burn incense on an altar

19. #### Glosses: 
^^^^^^^^^^^^^^^^^
This marker's data should contain one or more one-word meanings for this sense. Multiple instances should be separated by a comma. Any narrative text and/or `Sense Link`_ should follow its associated gloss data instance with a semicolon.  No termination mark should be entered.

20. #### Explanation: 
^^^^^^^^^^^^^^^^^^^^^
This marker's data should be left empty for this Stage of the project, unless there is discussion needed to explain the *context* of the Definition and/or Glosses. Multiple instances should be separated by a comma. No termination mark should be entered.

21. #### Citations: 
^^^^^^^^^^^^^^^^^^^
This marker’s data should contain each Scripture reference associated with this sense of the lemma. For a sense with many references, you may choose a subset of those that you believe would be most beneficial for the users of this lexicon. Omitting some for the sake of brevity would be the reason to specify No for the `9. * All Scriptures cited: Yes/No`_ . Each citation instance must be made up of only one `Scripture Links`_, defined above. Optionally a citation instance can be preceded by a narrative discussion or by either or both of the actual UGNT Greek text and an English translation, the latter should be suffixed with the translation source identified as three to four capital letters enclosed in parenthesis: e.g. (ULT),(NASB),(ESV),or (NIV). If narrative discussion is entered this should be preceded with a tilde, “~”. This narrative discussion may include a single `Greek Lemma Link`_ or a single `Hebrew Lemma Links`_ but these must follow their documented syntax. An exception to this is that *this* Greek lemma link does not require a gloss or definition, but if it is present, it should be preceded by a comma, and not a colon as in the standard form. If a gloss or definition for a Hebrew lemma link is provided, it should be preceded by a comma, and not a colon as in its standard form. If any narrative discussion is entered it should precede the UGNT text or English translation. If entered, there should be a semicolon preceding the UGNT text and a semicolon preceding the English translation, if entered. It should be noted that if the UGNT text is entered it would be most beneficial for the downstream translators to have this Greek entered in Greek lemma link format to support hotlinks to the lemmas for each of those Greek words. For this case of entering Greek lemma links, no gloss/definition data should follow each link. Also, where the current Greek lemma occurs within that UGNT text, that Greek word should not be in Greek lemma link format since that hotlink would send the translator back to the current lemma file. It should be entered as simple Greek text. If any or all of these three preceding data pieces are entered they should be separated from their Scripture link with a colon. It should be noted that any narrative discussion is terminated by either a semicolon if there is inserted UGNT and/or English translation or by a colon if neither of these is inserted. To not overburden the translators and not have a congested file, the UGNT text and English translation should be entered for only the first citation link instance. Multiple citation instances must be separated by a comma. No termination mark should be entered for this data except for the citation data of the last Sense level in the lemma file. For this last citation data in the file, it should be terminated with a period. As discussed in `8. * Instances in the New Testament: <count>`_, above, annotations to this citation data should be made to identify which references have more than 1 instance of this lemma. This identification must be enclosed within curly brackets “{}”. It may be just standard textual narrative or it may include one or more Sense links. As with other marker data, this data can span multiple, consecutive, lines in the file with no blank lines between them. Examples of the format for this annotation are:
::

     {Under Sense 1.0 of lemma καινός, G25370}
  [Luke 5:36](luk 5:36){3 instances, all for this Sense}

    {Under Sense 2.0 of lemma καινός, G25370}
  [Rev 3:12](rev 3:12){2 instances, both for this Sense}

     {Under Sense 4.0 of lemma καλέω, G25640 where the passage is not cited in any other Sense Citation data}
  [Rom 8:30](rom 8:30){2 instances, one(1) for this Sense, one(1) not cited}

     {Under Sense 1.0 of lemma κἄν, G25790}
  [Luke 12:38](luk 12:38){2 instances, one(1) for this Sense and one(1) for [Sense 2.0](#sense-20)} 
     {Under Sense 2.0 of lemma κἄν, G25790}
  [Luke 12:38](luk 12:38){2 instances, one(1) for this Sense and one(1) for [Sense 1.0](#sense-10)}

      Example with preceding narrative discussion only, without a Greek or Hebrew lemma link:
  ~Gabbatha, the Greek transliteration of an uncertain Aramaic word: [John 19:13](jhn 19:13)

      Example with preceding narrative discussion only, which includes a Greek lemma link without a gloss:
  ~Gabbatha, the Greek transliteration of an uncertain Aramaic word used as the equivalent of [λιθόστρωτον](../G30380/01.md): [John 19:13](jhn 19:13)

      Example with preceding narrative discussion only, which includes a Greek lemma link with a gloss:
  ~Gabbatha, the Greek transliteration of an uncertain Aramaic word used as the equivalent of [λιθόστρωτον](../G30380/01.md), stone pavement: [John 19:13](jhn 19:13)

      Example with preceding UGNT and English Translation, only:
  ;[καὶ](../G25320/01.md) [γὰρ](../G10630/01.md) [ὁ](../G35880/01.md) [θεὸς](../G23160/01.md) [ἡμῶν](../G14730/01.md) [πῦρ](../G44420/01.md) καταναλίσκον, 
  ;"For our God is a consuming fire." (ULB)
  :[Heb 12:29](heb 12:29)

      Example with preceding narrative discussion, UGNT, and English Translation:
  ~This addresses a significant aspect of God
  ;[καὶ](../G25320/01.md) [γὰρ](../G10630/01.md) [ὁ](../G35880/01.md) [θεὸς](../G23160/01.md) [ἡμῶν](../G14730/01.md) [πῦρ](../G44420/01.md) καταναλίσκον, 
  ;"For our God is a consuming fire." (ULB)
  :[Heb 12:29](heb 12:29)


Example Markdown file:
^^^^^^^^^^^^^^^^^^^^^^

::


    # κακῶς.

    <!-- Status: S2=NeedsReview -->
    <!-- Lexica used for edits: BDAG, FFM, LN, A-S -->

    ## Word data

    * Strongs: G25600.

    * Alternate spellings:

    * Principle Parts: 

    * Part of speech: 

    [Adverb](http://ugg.readthedocs.io/en/latest/adverb.html).

    * Instances in the New Testament: 16.

    * All Scriptures cited: Yes.

    ## Etymology: 

    [κακός](../G25560/01.md): bad, evil.

    * LXX/Hebrew glosses: 

    * Time Period/Ancient Authors: 

    * Related words: 

    * Antonyms for all senses:

    * Synonyms for all senses: 

    ## Senses 

    ### Sense 1.0:

    #### Definition: 

    Suffer physical harm

    #### Glosses:

    #### Explanation:

    #### Citations:

    ### Sense 1.1:

    #### Definition: 

    Suffer physical harm without identifying magnitude

    #### Glosses:

    ill, sick

    #### Explanation:

    #### Citations:

    [καὶ](../G25320/01.md) [ἀπῆλθεν](../G05650/01.md) [ἡ](../G35880/01.md) [ἀκοὴ](../G01890/01.md) [αὐτοῦ](../G08460/01.md) [εἰς](../G15190/01.md) [ὅλην](../G36500/01.md) [τὴν](../G35880/01.md) [Συρίαν](../G49470/01.md) [καὶ](../G25320/01.md) [προσήνεγκαν](../G43740/01.md) [αὐτῷ](../G08460/01.md) [πάντας](../G39560/01.md) [τοὺς](../G35880/01.md) κακῶς [ἔχοντας](../G21920/01.md) [ποικίλαις](../G41640/01.md) [νόσοις](../G35540/01.md) [καὶ](../G25320/01.md) [βασάνοις](../G09310/01.md) [συνεχομένους](../G49120/01.md) [καὶ](../G25320/01.md) [δαιμονιζομένους](../G11390/01.md) [καὶ](../G25320/01.md) [σεληνιαζομένους](../G45830/01.md) [καὶ](../G25320/01.md) [παραλυτικούς](../G38850/01.md) [καὶ](../G25320/01.md) [ἐθεράπευσεν](../G23230/01.md) [αὐτούς](../G08460/01.md)
    "The news about him went out into all of Syria, and the people brought to him all those who were sick, ill with various diseases and pains, those possessed by demons, and the epileptic and paralytic. Jesus healed them." (ULB) 
    [Matt 4:24](mat 4:24),  [Matt 8:16](mat 8:16),  [Matt 9:12](mat 9:12),  [Matt 14:35](mat 14:35),  [Mark 1:32](mrk 1:32),  [Mark 1:34](mrk 1:34),  [Mark 2:17](mrk 2:17),  [Mark 6:55](mrk 6:55),  [Luke 5:31](luk 5:11),  [Luke 7:2](luk 7:2).

    ### Sense 1.2:

    #### Definition: 

    Suffer physical harm and identifying its magnitude

    #### Glosses:

    suffer severely

    #### Explanation:

    #### Citations:

    [καὶ](../G25320/01.md) [ἰδοὺ](../G37080/01.md) [γυνὴ](../G11350/01.md) [Χαναναία](../G54780/01.md) [ἀπὸ](../G05750/01.md) [τῶν](../G35880/01.md) [ὁρίων](../G37250/01.md) [ἐκείνων](../G15650/01.md) [ἐξελθοῦσα](../G18310/01.md) [ἔκραζεν](../G28960/01.md) [λέγουσα](../G30040/01.md) [Ἐλέησόν](../G16530/01.md) [με](../G14730/01.md) [κύριε](../G29620/01.md) [υἱὸς](../G52070/01.md) [Δαυείδ](../G11380/01.md) [ἡ](../G35880/01.md) [θυγάτηρ](../G23640/01.md) [μου](../G14730/01.md) κακῶς [δαιμονίζεται](../G11390/01.md) 
    'Behold, a Canaanite woman came out from that region. She shouted out and said, "Have mercy on me, Lord, Son of David! My daughter is severely demon-possessed."' (ULB) 
    [Matt 15:22](mat 15:22),  [Matt 17:15](mat 17:15),  [Matt 21:41](mat 21:41).  

    ### Sense 2.0:

    #### Definition: 

    To be morally evil

    #### Glosses:

    wickedly, speak wrongly

    #### Explanation:

    #### Citations:

    [ἀπεκρίθη](../G06110/01.md) [αὐτῷ](../G08460/01.md) [Ἰησοῦς](../G24240/01.md) [Εἰ](../G14870/01.md) κακῶς [ἐλάλησα](../G29800/01.md) [μαρτύρησον](../G31400/01.md) [περὶ](../G40120/01.md) [τοῦ](../G35880/01.md) [κακοῦ](../G25560/01.md) [εἰ](../G14870/01.md) [δὲ](../G11610/01.md) [καλῶς](../G25730/01.md) [τί](../G51010/01.md) [με](../G14730/01.md) [δέρεις](../G11940/01.md) 
    "Jesus answered him, "If I spoke wrongly, testify about the wrong, but if rightly, why do you hit me?"" (ULB)  
    [John 18:23](jhn 18:23),  [Acts 23:5](act 23:5),  [Jas 4:3](jas 4:3).

Valid part of speech, POS, entries:
-----------------------------------
The following is a list of the valid values for Textual Representation and their corresponding UGG Filename. See the `UGG <https://ugg.readthedocs.io/en/latest/front.html>`_  for clarification.

.. csv-table:: 
   :header: "Textual representation", "UGG filename"
   :widths: 40, 30
   
    Noun, noun
    Adjective used substantively as a Noun, noun_substantive_adj
    Adjective used predicatively as a Noun, noun_predicate_adj
    Proper noun_indeclinable, proper_noun_indeclinable;
    Adjective, adjective
    Adjective ascriptive, adjective_ascriptive
    Adjective restrictive, adjective_restrictive
    Determiner, determiner
    Determiner article, determiner_article
    Determiner demonstrative, determiner_demonstrative
    Determiner differential, determiner_differential
    Determiner possessive, determiner_possessive
    Determiner quantifier, determiner_quantifier
    Determiner number, determiner_number
    Determiner ordinal, determiner_ordinal
    Determiner relative, determiner_relative
    Determiner interrogative, determiner_interrogative
    Pronoun, pronoun
    Pronoun demonstrative, pronoun_demonstrative
    Pronoun personal, pronoun_personal
    Pronoun reflexive, pronoun_reflexive
    Pronoun reciprocal, pronoun_reciprocal
    Pronoun indefinite, pronoun_indefinite
    Pronoun relative, pronoun_relative
    Pronoun interrogative, pronoun_interrogative
    Verb, verb
    Verb transitive, verb_transitive
    Verb intransitive, verb_intransitive
    Verb linking, verb_linking
    Verb modal, verb_modal
    Verb periphrastic, verb_periphrastic
    Interjection, interjection
    Interjection exclamation, interjection_exclamation
    Interjection directive, interjection_directive
    Interjection response, interjection_response

