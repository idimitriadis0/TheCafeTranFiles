# CafeTran Espresso ChangeLog

Find CafeTran Espresso's version announcements, all gathered in one place.

To get notified about new CafeTran updates, use the "Follow" button in the [CafeTran News page](https://cafetran.freshdesk.com/support/discussions/forums/6000148195).

*The ChangeLog is being curated by [Jean Dimitriadis](https://www.proz.com/translator/2042360) (EN-FR/EL-FR translator).
Entries from 20130701 through to 20151128 have been curated by [Michael Beijer](http://beijer.uk) and [Hans Lenting](http://www.niederlaendisch.nl/).*

<!--- Shortened link to this document: --->

**Important! Do not update before exporting your current projects. Please complete all your translation projects in your current CafeTran version before updating.**


## 11.0 - Poppy Seed Roll (20211203)

- Tracking Changes. This new feature is available via the Edit >  Track Changes > Manage menu. See the Changes tab after activation.  There, you can Accept and Reject changes to the current target segment.
- Filtering on tracked changes via the Filter menu.
- Accepting or rejecting all tracked changes in one task via the Task menu.
- Color settings for the changes in the View > Colors > Added/Deleted text color.
- New bright and dark image-based themes - see the View > Themes menu.
- Fixed spoken segments synchronization issue in Amazon Polly Text to Speech implementation.
- Fixed an issue with the spell checker dictionaries. It affects  CafeTran on Mac with Apple M1 chip only - reinstallation is required.

The 11.0.1 update to CafeTran adds the following:

  - the support for Cornish (kw-GB) language.
- a case-insensitive QA translation consistency check.
- tags protection in locked fragments.
- fixed an issue with quotes in IBM Watson API implementation.

  

You can update following the steps in the announcement post above

## 10.9.1 - Apple Charlotte (20211002)

- Added interface to Amazon Polly (Text to Speech) web service available via the API key. Text To Speech (TTS) integration in CafeTran enables the translators to listen to the currently-translated source language segment. It can be set either automatic or manual with the option to listen to target language segments (e.g during the review) as well. Amazon Polly supports over 30 languages and a selection of voices. It also offers the free tier for the first 12 months. Please check [here](https://aws.amazon.com/polly/) for details. After receiving the API secret and access keys from Amazon, you need to paste them in CafeTran's Preferences > Web services tab > Amazon Polly (TTS) > the API key button > the API Access and Secret key fields.
- Added interface to Amazon Translate MT available via the API key (the API keys for Amazon Translate MT and Amazon Polly TTS are the same).
- Marking of term patterns in source segment editor.
- Adjustments for some special characters in the Prompter function.
- Improved handling of xliff files created in other tools.

## 10.9 - Apple Charlotte (20210820)

- First CafeTran release for Mac's Apple M1 chip architecture (https://www.cafetran.com/download-for-mac/).
-  Updated libraries for Apple M1 chip.

- Equals character in the non-translatable fragments can be escaped with the backslash.
- Fixed an issue with the non-translatable fragments containing numbers.
- Fixed the tagging issue in Adobe InDesign filter.
- Single-click addition of the selected terms to the glossary or translation memory. It works as follows:

1. Select a term in the source segment.

2. Select its translation in the target segment.

3. Click the chosen glossary or translation memory pane to add the new entry there.  

 Skipped read-only resources during Search and Replace action.

- Blocked Split and Join segments action during the translation of subtitles.
- Fixed the whole segment deletion by Backspace when selecting the text with the boundary tags.
- Updated interface to IBM Watson Machine Translation API. 
  You need to set the API key and URL address for IBM Watson MT in CafeTran's Preferences > MT services tab > API key button. The API key and URL can be generated and copied from IBM website after signing up there.

- Changing tabs divider orientation does not require restart.

- Reduced width of the segment editor toolbars for smaller laptop screens in the compact windows layout.

- Fixed the issue with the display of the converted non-translatable fragments in F4 pop-up panel.

- Converted non-translatable fragments are shown in the auto-assembling result.

- Automatic transfer of the number being the source segment to target segment editor if the segment is empty.

## 10.8.3 Cornetto (20210226)

* Improved display of formatting in the grid for external xliff files.

* Display of Rendezvous memory server IP address in Preferences > Memory server tab.

* Fixed processing of TM fragments in the Rendezvous TM server.

* "Read only" and "Terms consistency check" glossary options set via the pop-up menu are preserved at program's exit.

* Keeping the contents of the edited and unconfirmed segment after the return from the filter view.

* Fixed a segmentation issue in the segments ending with the quotation marks.

* Check for tab characters in TMX memories during the conversion to the glossary format.

* Locale-specific conversion of numbers with the thousands (grouping) separator.

* Conversion of non-translatable fragments to let the user adjust them to the target language equivalents. For example, to change dates from the US format to the international format, the following non-translatable can be defined:  
      
  |(\\d)(\\d)/(\\d)(\\d)/(\\d)(\\d)(\\d)(\\d)=(3)(4)-(1)(2)-(\\5)(\\6)(\\7)(\\8)  

  \- | the pipe character at the start indicates the non-translatable fragment pair is in a special format (a regular expression).
  \- = is a separator between source and target language non-translatable fragments.  
  \- \\d means a digit in the source fragment.  
  \- () the characters to move or reorder need to be placed between brackets.  
  \- Some punctuation characters (e.g the full stop) need to be preceded by the backslash in the source fragment.  
  \- Reordering of characters in the target language fragment is controlled by the numbers in brackets. The numbers refer to the groups in brackets in the source fragment, counting from the left. All the other characters in the target fragment are in their usual form.

  The new build of the 10.8.3 update has the following changes:

-   fixes an issue with the transfer of some non-translatable fragments.
-   updates the links to online spell-checker glossaries.
-   adds the Sicilian language to the list of supported languages.

## 10.8.2 Cornetto (20210118)

- Added the MT websites of ModernMT, Systran and MyMemory as web resources.*
- The menu action (and the keyboard shortcut) in View > Segment editors > Request focus in target segment editor can cycle the focus between CT target segment editor and the source segment box on the MT resource webpage. This is convenient for those web resources that require focus in the source language box to trigger the automatic translation process.
- Text shortcuts can also be inserted after typing a punctuation character.
- Ms Excel filter allows for empty cells in target language column.
- The tab character symbol is always visible in the segments editors.
- Some minor fixes and improvements.

\* The transfer of the source text for translation into the text boxes on the web pages of some MT service providers via the keyboard shortcut canterm patterns work only after the focus is set on the given webpage (e.g via the mouse click).  

## 10.8.1 Cornetto (20201007)

- Recognition of previously-matched patterns inside term patterns - nested patterns.
- Loading of multiple .sdltm memories from .sdlppx packages.
- Fixed saving of glossaries with some unusual characters in the location path.

## 10.8 Cornetto (20200916)

- Term patterns. This new feature allows the user to create complex terms consisting of fixed and changeable parts both on the source and target language side. For example, see this simple term pattern in the glossary:

  I like {1}=Me gusta {1}

  If the source language segment includes the above pattern (e.g I like coffee very much), CafeTran will translate it into the target language provided that the variable part (e.g "coffee") can be found as the term or fragment in any of your glossaries, memories or lists of non-translatable fragments. See another example:

  "{1}" = “{1}” to match and replace the double quotes with the curly ones in the terms found in the current segment.

  The matched patterns are displayed in the Matchboard with the PA label.

- Display of auto-adjusted (AA label) fragments in the Matchboard.

- New keyboard shortcut for placing the consecutive tags: type x followed by Esc key.

- Cell segmentation option for the Excel filter.

- Saving the ignored spelling mistakes in the project.

- Option for the Prompter to use the segment editor font.

- Workflow option to transfer automatically source segments with no letters to target segments.

- Display of the notes in mxliff projects.

- New Dashboard command in the Dashboard menu. It deselects the resources in the Dashboard.

- The right-click Dashboard option to remove all the selected resources in the panel.

- Fixed an import issue in the Excel filter.

- Fixed a glossary path issue with non-Latin characters.

- Some UI improvements.

- Added Iloko, Hiligaynon and Tagalog languages.

## 2020 10.7.5 Doughnut (2020050)

- Binding of project templates to external projects.
- Automatic update of the current project template when a resource is added or removed, preference changed.
- Automatic selection of the project template in the Dashboard together with the selection of the project.
- Fixed an issue with the consistent display of details in (unfolded) hidden tags during automatic matching.
- Display of the duplicate entries when browsing through read-only translation memories.
- Matchboard font's bold style option.
- "Translate" button action takes the current segment for MT search when there is no selection.
- Hidden Dashboard menu during "Replace document" action.
- Keyboard shortcut for ‘Show invisible characters" action (CTRL+SHIFT+V).

## 2020 10.7.4 Doughnut (20200409)

- Updates to CTE interface for ProZ.com API.
- Updates to CTE interface for DeepL.com API to include new languages: Japanese, Chinese, Portuguese (Brazil) and Portuguese (Portugal).

## 2020 10.7.3 Doughnut (20200402)

- Separate setting of the Matchboard font - see the menu View > Font > Matchboard.
- Added Kongo and Lingala languages.
- Display of notes in .txlf files.
- Various UI adjustments and fixes.

## 2020 10.7.2 Doughnut (20200311)

- The border around the highlighted terms and fragments in the source segment editor.
- The option to run QA tasks on the filtered segments - see Edit > Preferences > QA > QA for filtered segments.
- Pausing session progress - see the STOP/START button in the Statistics pane.
- Small UI adjustments.

## 2020 10.7.1 Doughnut (20200127)

- New custom formatting (m) tag to mark/highlight part of the target segment. The default yellow color of the highlight can be changed via the menu View > Colors > Highlight color.\
- Changing the color of toolbar icons is possible via View > Colors > Icons color.
- Fixed automatic memory matching in the Clipboard workflow.
- Small UI adjustments. TODO examples

## 2020 10.7 Doughnut (20200114)

- Icons for high resolution screens.
- Improvements to Word and HTML filters - starting from new projects.
- Shown context notes in the grid in mqxliff projects.
- Addition of custom formatting (bold, italics, underline, subscript and superscript) possible in Excel projects.

## 2019 10.6.6 Brownie (20191218)

- Added the option of filtering repeated and propagated segments from the current segment - see the Filter menu.  Also, hold the CTRL key while clicking at a segment in the grid to activate this filter.
- Added East Franconian (vmf) and Neapolitan (nap) as project languages.
- Fixed an issue with column names in the alternative MySQL database for Total Recall.
- Fixed an issue with the adjustment of segment editors divider in the Compact Layout.

## 2019 10.6.5 Brownie (20191203)

- Added segment skipping options and term prefix settings to Project Templates.
- Faster opening of Project Templates.
- Stopping at the last segment during navigation even if this segment is set for skipping. It also eliminates the blank editor after the last skipped segment. 
- Addition of Approved (A) and Rejected (R) segment status in the status column at bilingual export to Word. The letter for Checked/Reviewed status has been changed from R to C in the status column of bilingual Word document. 
- Option to ignore segment status at bilingual document import - see it Preferences > Workflow tab. 

## 2019 10.6.4 Brownie (20191119)

- Options to exclude space and newline characters from showing when the invisible characters display is on - see Edit > Invisible characters menu.
- Options to set separate background colors for the grid and the editor - see View > Colors menu.
- Fixed an issue during the creation of sdlrpx packages.
- Fixed a Prompter issue with the tiling window managers on Linux.

## 2019 10.6.3 Brownie (20191104)

- Display of basic formatting (bold, underline and italic) in the grid for Word-based sdlxliff files.
- Removed the Start button. Now, CafeTran begins the translation right after the creation of the new project.
- Removed the exit confirmation panel when clicking at the Close window icon.

## 2019 10.6.2 Brownie (20191023)

- The option to include hidden non-translatable fragments in matching results and auto-assembling - see the menu Resources > Non-translatable fragments > Match hidden non-translatable fragments. The ability to hide a part of the segment was introduced in CafeTran Espresso 10.6.

## 2019 10.6.1 Brownie (20191014)

- Hidden non-translatable fragments (both literal phrases and regular expressions). Just append the ^ character to your non-translatable fragment to hide it behind the tag and let it transfer to the target segment like the regular tags. To disable hiding of tags temporarily, use the menu Resource > Non-translatable fragments > Show hidden non-translatable fragments.
- Hide tag details option in the menu Action > Tags. It toggles the display of the tags in more detail for xliff-based projects and the contents of hidden tags in native projects.
- Ignoring a spelling mistake for the current session - right click at the misspelled word and choose the "Ignore" item.
- Fixed a text orientation issue with the export of Word documents translated from a RTL source language.
- Normalization of double byte numbers to pass QA numbers check

## 2019 10.5.1 Croissant (20190909)

- Improved sorting of matches by quality in the Matchboard.
- Fixed handling of some formatting (color) tags in Ms PowerPoint filter.
- Automatic insertion of Machine Translation results prioritizes the auto-insert thresholds set for the Memory matches and Auto-assembling in Preferences.
- Some tuning for the new Java 13 version.

## 2019 10.5 Croissant (20190507)

- Automatic fragment adjustment for Machine Translation matches - see it in Edit > Preferences > MT services tab.  With this option on, CafeTran replaces the MT fragments with the synonyms in your glossary/TM that are actually used in the current session.  If the replacement takes place, the MT tabs show both the original MT result and the modified one.
- Fixed an issue with some special characters in MT results.
- Choosing a color for Dashboard panels - View > Colors > Dashboard color.
- Showing line breaks in the grid when the Search filter is used.
- Letting user overwrite the existing return .sdlrpx package.
- The cursor set at the start of the target segment after the source segment transfer.

## 2019 10.4.1 Croissant (20190424)

- The option to open the export folder when exporting to the package.
- Literal recognition of single character non-translatable fragments without the need for regular expressions.
- The option to turn off the conversion of html formatting tags to the source document formatting at export - see Preferences > Workflow tab.

## 2019 10.4 Croissant (20190417)

- When transferring MT or TM result, the cursor is positioned at the start of the target segment.
- Addition of several non-translatable terms to the glossary in one "Add term to glossary" action.
- Filtering on fuzzy matches - see Filter > Origin > Fuzzy matches.
- Support for the new Microsoft Translator MT API version 3.0.
- Support for IBM Watson Language Translator MT API. The API key can be received at IBM website (https://www.ibm.com/watson/services/language-translator/). Please check if your language pair is supported. During the registration at IBM site, choose Frankfurt as the deployment region/location.
- Change of the Preferences interface for setting API keys in MT Services tab.

## 2019 10.3.2 Croissant (20190328)

- Prevention against the change of the package folder during the export to package (via the menu Project > Export and exchange > To package... ). Previously, when the user chose another package folder, CafeTran created a wrong package, possibly with large files stalling the program.

## 2019 10.3.1 Croissant (2019032)

- Clicking on a segment in the gird sets this segment for edition in the target segment editor. It works the same as clicking on a segment number.
- Some additional word dividers do not need to be escaped by the backslash character in the Glossary preferences.
- A right-click option to display Machine Translation results last in the Matchboard.

## 2019 10.3 Croissant (20190323)

-  Added punctuation to ideographic characters count in Statistics for CJK languages.
-  If the Human Translation (HT) and Edited Segment (*) labels are deactivated (in View > Segment Labels menu), the TM match percentage keeps being displayed in the grid even for edited/changed segments.
-  Added the "Additional word dividers" field to the Glossary options - see Preferences > Glossary tab.
-  Added a confirmation panel before the removal of the current document during the "Replace document" action.

## 2019 10.2.2 Croissant (20190313)

- When CJKV language is set in the project, the Statistics function shows the number of ideographic characters.
- Unfolding of text shortcuts after the full stop.
- Fixed an issue with handling of TTX files.
- Improved setting of the target language code in the exported Word documents.

## 2019 10.2.1 Croissant (20190308)

- Disabling of auto-propagation of the segment  (nP label in the grid) replaces its previously set auto-propagation state (P label in the grid).
- Fixed an issue with auto-tagging of numbers.
- Automatic appending of the space in the target segment if the source segment ends with the full width question mark, exclamation mark, colon or semi-colon (e.g. in Japanese).

## 2019 Croissant 10.2 (20190304)

- Term or Fragment Matches with higher or lower priority of the given glossary/memory have the brighter or darker shade of its highlight color.
- Fixed keyboard shortcuts issue with segment editors in the detached mode.
- Search after listing misspelled words with the "whole words" option turned on automatically.
- On some Glossary menu actions (e.g. join, merge, sort) CafeTran displays glossary selection panel, when no glossary is selected in the active tab.
- Glossary "Prefix matching" option for CJK languages.
- "Keep out of auto-assembling" memory option can also be selected in the Priority box of the TM options panel.

## 2019 10.1.2 Croissant (20190223)

- Fixed automatic tagging of non-translatable fragments surrounded by brackets.
- Distinction between exact fragment matches, exact segments matches and context matches in the Matchboard. Fragment matches are marked as "Fragm" and Context matches have the CTX label.

## 2019 10.1.1 Croissant (20190220)

This update adds two shortcut options useful for French translators during typing - see the menu Resources > Text shortcuts:

- Change double straight quotes to guillemets in French.
- Add non-breaking space before some French punctuation characters.

If the above options are on, they get activated automatically with French as the target language of the current project. The default shortcut to surround the word at the cursor with guillemets (CTRL + SHIFT + Quote) remains unchanged.

## 2019 10.1 Croissant (20190218)

The major changes in this version:

- Automatic tagging of non-translatable fragments in Machine Translation and Auto-assembling results.
- Automatic transfer of source segments that contain non-translatable fragments and numbers only - an option in Edit > Preferences > Workflow tab.
- Added "Sort by length" (long segments first) filter.

## 2019 10.0.1 Croissant (20190130)

- Conversion of some HTML entities (e.g. &gt; &amp;) during the transfer of the Machine Translation result to the target segment editor.
- Recognition of terms at g tag in sdlxliff files.
- Prompter recognizes words with the hyphen during automatic case adjustment.
- Added Bislama language to the list of project languages.

## 2019 10.0 Croissant (20190117)

This version is the summary of all the updates to the CTE 2018 Akua and CTE 2019 Forerunner (aka Beta) version.

The major changes in this version:

- Easier selection of a single translation memory from the list of loaded TMs in the Memory menu for various tasks.
- Recognition of .xhtml file extension for HTML filter.
- Uniform color for search buttons in the search bar.
- Adjustment to transfer the translation from Ms Bing Translator web page due to its recent change.
- New "Transfer MT from web page" button in the source segment toolbar.  It transfers the translation from the selected Machine Translation web page (e.g DeepL, Google Translate, Bing Translator).
- Locked segment can be exported to translation memories either vie Project > Export and exchange > To TMX memory or via Memory > Import > Import segments from project.
- Access to DeepL Pro Machine Translation service via its API key. See this option in Edit > Preferences > MT services tab.
- Displaying match score information for the target segments included in .txml translation projects.
- Added the right-click pop-up menu to Frequent words feature with the minimal and maximal fragment length settings.
- Frequent words feature is activated automatically at the start of the project when "Extract frequent words from current segment" option is on.
- Resizing of the Preferences dialog is remembered now.
- Repeated segments in the filter are sorted in the order of their occurrence.
- Project Template files are selected directly via the File Chooser.
- Option to turn off the "greedy" exact matching for translation memories - see it in the TM options panel. With this option off, CafeTran does not stop the search at the found exact match(es) for the current segment, but it continues looking for fuzzy matches and fragments. Switching off this option is not recommended for slower computers and huge translation memories.
- Automatic removal of the misspelled words from the Auto-completion list.
- Splitting and joining of adjacent segments in the Filter mode as well.
- Adjustments to the MS Word filter.
- Approved segment status - see the status selection box in the target segment toolbar. Approved segments are marked with the red border around the status cell in the grid. The new segment status maps to "Translated" status in the external sdlxliff files. There is also a new filter for "Approved" and "Not approved" segments.
- Updated target segment editor bindings to web editors on the refreshed MT websites.
- Added import of Multiterm XML glossaries - see the Memory > Import menu.
- Added two window layouts for higher resolution screens - see the menu View > Window layout > Layout 4 and 5 Desktop. Layout 4 is the default for new CafeTran installation on high resolution screens while Layout 5 resembles, more or less, panels arrangement found in some other CAT tools.
- The frequently-requested layout that integrates editors and the grid - see View > Window Layout > Layout 6 Compact. Although it is recommended for reviewing your translations, some translators might wish to use it for translating too, as it is a popular layout in other tools.
- QA > Initial capitalization check catches the false positives that start with numbers.
- The status of the current segment in Layout 6 Compact is displayed in the corner of the editor.
- Clicking at the segment status label in the Filter view switches back to the normal (unfiltered) view.
- A keyboard shortcut (CTRL+SHIFT+H) to hide editor toolbars if needed.
- Improved sorting of resources in the Dashboard.
- Saving of "Replace punctuation characters" and "Replace characters at source transfer" options in Project Templates.
- Check for the maximum difference in length between source and target segments (menu QA > Length difference check).
- Check for the maximum number of characters in the target segments (menu QA > Maximum segment length check).
- Check for the consistency of non-translatable fragments in the source and target segments (menu QA > Non-translatable fragments check).
- Some improvements to the LibreOffice filter.
- Import of the editable drawings in the Ms Excel filter.
- Corrected project's language code for Irish Gaelic.
- New QA > Length difference check in the number of characters.
- New Filter > Segments with numbers.
- Fixed an issue while closing resources with duplicate names.
- Import of SDLTB termbases.
- Extension of the "Transfer tags to matches" option for the matches found in Machine Translation results.
- Showing context in the filtered view of Layout 6 Compact.
- Fixed closing of the tabs after changing their position via drag and drop.
- Fixed the display of exact and fuzzy matches in the Matchboard for Translation Memories with the option "Keep out of auto-assembling" on.
- Added the "Minimal prefix length" option in Edit > Preferences > Glossary tab.
- Autopilot. This may be a very handy feature during the Review or QA phase of translation. You can also use it when translating short, repetitive/similar phrases or numbers. It allows hands-free navigation with the set delay between the segments. The default delay of 2000 milliseconds (2 seconds) can be increased in Edit > Preferences > General tab. Activation/deactivation of the Autopilot is done via the Action menu. After that, you will notice the Autopilot button in the target segment editor. Click this button to turn on/off the Autopilot. Going to the next segment triggers off its functioning. To suspend it for a while (e.g for the correction of the current segment), press the Esc key or click the mouse on the target segment editor.
- Automatic transfer of numbers being the full segments which end with the white space character.
- Recognition of language variants in SDLTB termbases.
- Support for subtitles (.itt and .srt file formats).
- Added video resource preview for translation of subtitles.
- Added an option to set the variable delay for Autopilot. The default setting in Edit > Preferences is 1000 millisecond per 10 characters in the current segment.
- Added the menu option to turn on/off automatic searching - useful with Autopilot during the review - see it the Action menu.
- Glossaries selection at QA > Terms consistency check.

## 2019 Forerunner (20180907)

- Autopilot. This may be a very handy feature during the Review or QA phase of translation. You can also use it when translating short, repetitive/similar phrases or numbers. It allows hands-free navigation with the set delay between the segments. The default delay of 2000 milliseconds (2 seconds) can be increased in Edit > Preferences > General tab. Activation/deactivation of the Autopilot is done via the Action menu. After that, you will notice the Autopilot button in the target segment editor. Click this button to turn on/off the Autopilot. Going to the next segment triggers its functioning. To suspend it for a while (e.g for the correction of the current segment), press the Esc key or click the mouse on the target segment editor.
- Automatic transfer of numbers being the full segments which end with the white space character.
- Recognition of language variants in SDLTB termbases.

The new build of CTE 2019 Forerunner (**2018091401**) is available for download. It features the following major changes:

- added an option to set the variable delay for Autopilot. The default setting in Edit > Preferences is 1000 millisecond per 10 characters in the current segment. You can adjust it as preferable.
- fixed a search off by one segment issue with Autopilot.
- added the menu option to turn on/off automatic searching - useful with Autopilot during the review - see it the Action menu.
- fixed an issue with the "Transpose selection to the right".

The new build of CTE 2019 Forerunner (**2018092101**) is available for download. It features the following:

- recognition of synonyms in .sdltb termbases.
- glossaries selection at QA > Terms consistency check.
- including non-translatable duplicates from the current segment in the F4 list.

The new build of CTE 2019 Forerunner (**2018092401**) is available for download, with the following improvements to the spell-checker function.

- recognition of words with the curly apostrophe (instead of the typewriter/straight apostrophe) inside.
- ignoring short (fewer than 4 characters in length) upper-case words.
- improved display of Task > List words with unknown spelling - see the buttons to add - easily the listed words to user's spell-checker dictionary.

The latest build (**2018092701**) makes ignoring short upper-case acronyms optional in Preferences > QA tab. Other improvements:

- An option to set the maximal length of the upper case acronyms to skip during spell checking.
- Task > List of words with unknown spelling: the buttons in the list have two functions now - click to add the word to the spell checker dictionary or hold CTRL key + click to search the misspelled word in target segments.
- Change of the glossary Prefix matching option in Preferences > Glossary tab causes the automatic reload of the glossaries.
- Saving notes in external .xliff or .xlf files that follow XLIFF 1.2 specification.

The new build of CTE 2019 Forerunner (**2018092901**) is available for download, with the following:

- Fixed Task > Remove notes function for some external xliff files (e.g. mqxliff).
- Remembering the choices in QA > Check all panel.

The new build of CTE 2019 Forerunner (**2018100401**) is available for download, with the following:

- Added "Adjust start punctuation" command/shortcut in the menu Edit > Target segment.
- Added "Clone" function to "Term Editor". It enables the creation of a new term based on the currently edited term.
- Holding the CTRL key while closing the "New Term" dialog via the Close dialog switches to the "New fragment" dialog. The switch also works while closing the "New fragment" dialog.
- Highlighting of non-translatables overwrites the highlight color of glossary or TM matches.

The new build (**2018100402**) has the Clone button grayed initially.

Τhe new build of CTE 2019 Forerunner (**2018100901**) is available for download, with the following:

- Automatic case adjustment (e.g to lower or upper case) during Auto-completion.
- New tasks (in the Task menu): Bookmark segments and Unbookmark segments (e.g. for bookmarking filtered segments).
- New Filter: Unbookmarked segments.
- Task > TMX Memory > Remove TMX filtered units can also detect the same contents in the filtered project segments (not in the TMX edit mode), and remove such segments from the TMX Memory.
- New Term Dialog can add multiple entries to the glossary - separated by the new line.
- Export of filtered segments as a bilingual Word document. The return import is also possible into exactly the same filter only.
- TMX Memory edit mode: Export and Import as a bilingual Word document.
- Fixed some minor issues.

The "Remove TMX filtered units" feature in latest build (**2018101001**) works with multilple TM selection too.

The new build of CTE 2019 Forerunner (**2018101601**) is available for download, with the following:

- Added Java memory usage indicator in the Help > About panel. The feature helps to determine the size of Java memory assigned for CafeTran.

The new update (**2018102501**) has just been uploaded. It features the following:

- enhancements to the Auto-complete feature (e.g. autocompletion in the middle of words, full MT results).
- filtering out of the deleted text in Ms Word and LibreOffice source documents with the track changes enabled (only for the new projects).
- restored Import and Export of Preferences in the Preferences panel.
- TM pane is refreshed after the deletion of the segments from the memory.

**As there are changes to the filters, please complete any unfinished Word or LibreOffice projects before updating**.

The new build (**2018103001**) of CafeTran Forerunner 2019 is available for download. It adds the following:

- Options to turn off the automatic case adjustment and overwriting during auto-completion - see the new Prompter tab in Preferences.
- Added "Rejected" status for proofreaders. It also maps to the similar status in sdlxliff and mqxliff files.
- CafeTran "Approved" status maps the the similar status in in sdlxliff files and mqxliff files now.
- CafeTran "Checked" status maps to the Translated status in sdlxliff files and the Confirmed status in mqxliff files now.

The new update (**2018110201**) of CafeTran 2019 Forerunner has just been made available for download with the following changes:

- Statistics for checked, rejected and approved segments.
- Removing the two-word (typed) phrase from the Prompter if one of the words is a spelling mistake.
- Some improvements to Ms Excel filter.
- Added the "es" language code (neutral - without a country variant) for Spanish spoken in the US.
- Keeping the punctuation character when replacing a word during auto-completion.
- Option to propagate the current segment status during auto-propagation.

The new update (**2018110802**) of CafeTran 2019 Forerunner is available for download with the following change:

- options for QA checks are stored in Project Templates.

The new update (**2018111601**) of CafeTran 2019 Forerunner is available for download. The changes are as follows:

- highlighting punctuation characters in TM exact matches which are defined in "Do not match" option.
- replacing background color with strike-through line for the missing words at the comparison between the current segment and fuzzy matches.
- 4"R" symbol in the grid for repeated segments regardless of their propagation status.
- marking segments edited in the current session - see the red asterisk in the grid.
- showing the origin of the translation in the grid:
  - Machine Translation - see the MT symbol.
  - CafeTran's Auto-assembling - see the CT symbol.
  - Human Translation - see the HT symbol.

CafeTran handles the origin state automatically. For example, Machine Translations or Exact/Fuzzy matches switch to Human Translation (HT) state after their edition. Currently, the origin is stored permamently in CafeTran's projects only, as projects coming from other translation tools may not have this concept. There are also new filters corresponding to the new states:

- Segments edited in the current session - see Filter > Status menu.
- Human Translation (HT) - see Filter > Origin menu.
- AI Translation (MT+TM) - see Filter > Origin menu.

The new update (**2018111901**) of CafeTran 2019 Forerunner is available for download with the following:

- quick access to recently used Project Templates via the Dashboard menu. Their usage is remembered starting from this update.
- improved dark theme for Nimbus look and feel.

The new update (**2018112201**) of CafeTran 2019 Forerunner has been available for download.  The new features:

- handling of some Unicode symbols (e.g Trademark**™**, Copyright©, Registered trademark®) during fuzzy matching.
- handling of CDATA sections in some external xliff files.

The new update (**2018112701**) of CafeTran 2019 Forerunner is available with the following changes:

- a new filter for ITT subtitles file. SRT subtitles file filter should be ready for the next update.
- options for displaying various segment labels in the grid - see the menu View > Segment labels.

Google Translate website has changed so CafeTran's interfacing to it needed updating as well. The update **2018112901** is available for download.

The new update (**2018120602**) of CafeTran 2019 Forerunner is available with the following features:

- an filter option to define a notes column for the import of Ms Excel documents.
- an option to export target documents into a shared folder - across multiple projects. See Edit > Preferences > Workflow tab > Shared export folder check box.  After turning this option on, CafeTran remembers the last Export location for the subsequent projects.
- added a movie resource - see the menu Resources > Open movie... . The movie resource can be useful during the translation of subtitles. You can also watch movies for fun, while translating, if you are good at multitasking.
- added YouTube web resource.

The new movie resource feature depends both on the Java version and the operating system (or its version). In particular, not all Linux distributions can work with this feature. Generally, Java developers try to catch up with the latest versions of video codec libraries on your operating system.

The new update (**2018121001**) of CafeTran 2019 Forerunner is available with the following features:

- case-insensitive language codes mapping for segmentation .srx files.
- the option Filter > Source and Target segments preview also determines the language of export/conversion of the project to the text and html formats.

The update **2018121301** of CafeTran 2019 Forerunner is available with Portuguese and Russian languages included in DeepL API.

The update **2019010501** of CafeTran 2019 Forerunner is available with the following:

- added LanguageTool as a Web resource (see it the menu Resources > Web). The Translate and Transfer buttons for querying and transferring MT web results work for this QA web resource as well.

- added support for Java 12 (to be released in March). The early access (ea) of this new Java version fixes an issue on MacOS Mojave with the insertion of accented characters via Mac pop-up characters window. If you insert the accented characters through this method on your Mac,  you need to update CafeTan by downloading and installing again to have this issue fixed. Otherwise, there is no need to reinstall the program, which works with the current Java 11.



## 2018 Akua Update 12 (20180901)

- Extension of the "Transfer tags to matches" option for the matches found in Machine Translation results.
- Showing context in the filtered view of Layout 6 Compact.
- Fixed closing of the tabs after changing their position via drag and drop.
- Fixed the display of exact and fuzzy matches in the Matchboard for Translation Memories with the option "Keep out of auto-assembling" on.
- Added the "Minimal prefix length" option in Edit > Preferences > Glossary tab.

## 2018 Akua Update 11 (20180730)

- Some improvements to the LibreOffice filter.
- Import of the editable drawings in the Ms Excel filter.
- Display of regular expression matches instead of the regular expression patterns in the Matchboard.
- Corrected project's language code for Irish Gaelic.
- New QA > Length difference check in the number of characters
- New Filter > Segments with numbers.
- Fixed an issue while closing resources with duplicate names.
- Import of SDLTB termbases.

The new build (**2018080601**) of update 11 is available with the following:

- fixed a glitch in the display of Total Recall tables in the Dashboard.
- fixed recording/remembering of the selected words (with the mouse) for the latest Java version.
- fixed the addition of comments in some sdlxliff files.

The new build (**2018082301**) of update 11 is available with the following:

- import of SDLTB termbases (see the new menu Memory > Import > Import SDLTB termbase...).

Issue with trunctacted text in imported SDLTB termbases fixed in build **2018082401**.

The new build (**2018082501**) of update 11 is available. It has a modified algorithm in the optional feature "Team Auto-assembling with the Machine Translation".

## 2018 Akua Update 10 (20180612)

- Check for the maximum difference in length between source and target segments (menu QA > Length difference check).
- Check for the maximum number of characters in the target segments (menu QA > Maximum segment length check).
- Check for the consistency of non-translatable fragments in the source and target segments (menu QA > Non-translatable fragments check).

The new build (**2018061501**) of update 10 is available. It adds the editor's support for the Windows context menu key found on some keyboards.

The issue with double percentage symbol for context matches in the Matchboard is fixed in the latest build (**2018062001**).

## 2018 Akua Update 9 (20180604)

- The status of the current segment in Layout 6 Compact is displayed in the corner of the editor.
- Clicking at the segment status label in the Filter view switches back to the normal (unfiltered) view.
- A keyboard shortcut (CTRL+SHIFT+H) to hide editor toolbars if needed.
- Improved sorting of resources in the Dashboard.
- Saving of "Replace punctuation characters" and "Replace characters at source transfer" options in Project Templates.

The new build (**2018060601**) of update 9 is available. The right-click Matchboard option "Shorten match information" is further enhanced by reducing the resource name to two letters and omitting the percentage symbol next to fuzzy matches. The change saves some more vertical space in the Matchboard, which is important for smaller screens.

## 2018 Akua Update 8 (20180521)

- The frequently-requested layout that integrates editors and the grid - see View > Window Layout > Layout 6 Compact. Although it is recommended for reviewing your translations, some translators might wish to use it for translating too, as it is a popular layout in other tools.
- QA > Initial capitalization check catches the false positives that start with numbers.

The new build (**2018052201**) of update 8 is available. There is a slight change in highlighting of the current segment status for the new Layout 6 Compact. Now, the status marking of the currently-edited segment is limited to its status box only. The previous highlighting of the whole row gave the impression that the edited segment was empty.

There is a new build (**2018052301**) of update 8 available.  In this update, the search back and forward arrows are moved from the top search bar to the search field below. The change allows for narrowing the main window for even more compact view. For example:

1. Set the View > Window layout >  Layout 6 Compact and undock the Matchboard to the tabs below.
2. Switch the editors orientation to the vertical one, unchecking View > Segment editors > Horizontal segment editors.
3. Resize the main windows as much as you can to see how compact CafeTran can be.

There is a new build (**2018052501**) of update 8 available. It changes the filters by showing the standalone space at the start of some formatting tags, instead of hiding it inside the tag as before.

Important! Please finish all the projects before applying this update to CafeTran's filters. Otherwise, the export to the target language document may fail in the projects started with the previous updates.

A new build (**2018052801**) of update 8 is available. There is a slight change to the Layout 6 Compact. The status of the currently-edited segment in this layout is shown in the grid's toolbar now. It saves some horizontal space in the grid just above the editors.

## 2018 Akua Update 7 (20180504)

- Added two window layouts for higher resolution screens - see the menu View > Window layout > Layout 4 and 5 Desktop. Layout 4 is the default for new CafeTran installation on high resolution screens while Layout 5 resembles, more or less, panels arrangement found in some other CAT tools.

The new build (**2018050701**) of update 7 is available. It adds the option to block auto-propagation from locked segments - see it in Edit > Preferences > Auto-propagation tab.

## 2018 Akua Update 6 (20180427)

- Approved segment status - see the status selection box in the target segment toolbar. - Approved segments are marked with the red border around the status cell in the grid. The new segment status maps to "Translated" status in the external sdlxliff files. There is also a new filter for "Approved" and "Not approved" segments.
- Updated target segment editor bindings to web editors on the refreshed MT websites.
- Added import of Multiterm XML glossaries - see the Memory > Import menu.

The new build (**2018042801**) of update 6 is available. It lets you import converted Multiterm XML glossaries via the Memory > Import menu.

##  2018 Akua Update 5 (20180409)

- Option to turn off the "greedy" exact matching for translation memories - see it in the TM options panel. With this option off, CafeTran does not stop the search at the found exact match(es) for the current segment, but it continues looking for fuzzy matches and fragments. Switching on this option is not recommended for slower computers and huge translation memories.
- Automatic removal of the misspelled words from the Auto-completion list.
- Splitting and joining of adjacent segments in the Filter mode as well.
- Adjustments to the MS Word filter.

The new build (**2018041101**) of update 5 is available. It adds the support for Java 10.

The new build (**2018041901**) of update 5 is available with the following fixes and changes:

- option to omit setting of the Translated status for target segments during the export to sdlrpx package.
- option to show only the first segment in the "Repeated and propagated segments" filter.
- clicking at the Exact match in the TM tab replaces the current target segment with the Exact match.
- fixed trimming of leading and trailing spaces at the transfer of the auto-assembling result.

## 2018 Akua Update 4 (20180330)

- Added the right-click pop-up menu to Frequent words feature with the minimal and maximal fragment length settings.
- Frequent words feature is activated automatically at the start of the project when "Extract frequent words from current segment" option is on.
- Resizing of the Preferences dialog is remembered now.
- Repeated segments in the filter are sorted in the order of their occurrence.
- Project Template files are selected directly via the File Chooser.

## 2018 Akua Update 3 (20180323)

- Access to DeepL Pro Machine Translation service via its API key. See this option in Edit > Preferences > MT services tab.
- Displaying match score information for the target segments included .txml translation projects.

The new build (**2018032401**) of update 3 is available with the following:

- Displaying match percentage for the target segments included in .mqxliff translation projects.

## 2018 Akua Update 2 (20180312)

- Adjustment to transfer the translation from Ms Bing Translator web page due to its recent change.
- New "Transfer MT from web page" button in the source segment toolbar.  It transfers the translation from the selected Machine Translation web page (e.g DeepL, Google Translate, Bing Translator).
- Locked segment can be exported to translation memories either vie Project > Export and exchange > To TMX memory or via Memory > Import > Import segments from project.

The new build (**2018031301**) of update 2 is available. It adds the surrounding tags insertion at the transfer of non-translatable fragments to the target segment via F4 pop-up panel.

The new build (**2018031501**) of update 2 is available with the following: Automatic recognition of segment words preceded by the curly apostrophe.  The user needs to remove the curly apostrophe from the "Do not match" list in Edit > Preferences >  Memory tab to have it matched.

## 2018 Akua Update 1 (20180301)

- Easier selection of a single translation memory from the list of loaded TMs in the Memory menu for various tasks. The user does not need to select the TM tab first to indicate the specific TM.
- Recognition of .xhtml file extension for HTML filter.
- Uniform color for search buttons in the search bar.
- In "Shorten match information" option of the Matchboard, the length of the shortened resource name is increased to 4 characters.

The 4-letter short names for MT services are in the new build (*2018030401*). The build also lets the user change the color of the Search bar at the top of the UI via View > Colors > Searchbar color menu.

The new build (**2018030502**) of update 1 is available. It improves Ms PowerPoint filter by including diagrams' data for translation. Please perform the update as described in the announcement above. If you are in the middle of PowerPoint document translation, please update after you finish your current project.

## 2018 Akua (20180118)

*Important! The update features some improvements to MS Word filter. Please complete all your Word translation projects in your current CafeTran version before updating.*

This is a product of all-year development with numerous additions. It goes without saying that most of them took the final shape with your excellent feedback. Thank you!

 To name some major new features:

 - important improvements in various areas such as user interface, documents filers, memory and glossary matching with the display of the results in the Matchboard.
 - added locked and version segment (a simple form of segment versioning) statuses.
 - new Tasks and QA functions
 - switch to the new Google Cloud Translation API which uses the neural machine translation model.
 - added Project Templates.
 - caching of translation results from all MT services available.
 - automatic fragments adjustment. This a new and experimental feature which picks fragments/terms from the current segment and updates their priority on the fly. It can also adjust to some slight changes in the fragments (e.g. plural forms) creating virtual fragment pairs if they do not exist in your resources. It also detects term’s synonym usage adjusting its priority automatically.
 - improved handling of comments in non-CafeTran projects.
 - added DeepL Machine Translation online service as a web resource (see the menu Resources > Web > DeepL). The Translate button in the source segment toolbar copies the source segment (or selection) to the internal web browser to look up the segment or the selected phrase in the Machine Translation web resource which is currently selected in the tab.
 - switch to the newest Java 9 release while still maintaining support for Java 8 on all major operating systems (Windows, Mac and Linux).
 - optional masking of non-translatable fragments for MT online services.
 - binding with MT editors on web pages such as Google Translate, Bing Translator, DeepL. See the binding option in Edit > Bind external editor and choose an editor in Edit > Preferences > General tab > External editor box. This new binding feature is dependent on the external website. If its web page or address changes, binding with the editor on that page will stop working.
 - action to transfer the MT result from a web page to the target segment - see the menu Translate > Transfer MT from web page. This transfer action (via the keyboard shortcut) can also be used when editors binding is off.
 - dragging of tabs with resources to change their position in the user interface.
 - CafeTran themes and the Dashboard have been refreshed to look modern and eye-friendly.
 - export to bilingual Word documents from external (non-CafeTran) projects.
 - connection to Youdao MT online resource via the web browser interface.

The new build (**2018013001**) is available for download that improves parallel loading of multiple resources at the project’s start.


## 2018 Forerunner (20171130)

*Important! The update features some improvements to MS Word filter. Please complete all your Word translation projects in your current CafeTran version before updating.*

What’s new:

- display of actual segment numbers in the Filter and QA view.
- segmenting on LibreOffice headings.
- option to use only high priority fragments when teaming Auto-assembling result with Machine Translation.
- separate joining of source and target segments which have already been created in the Alignment workflow.
- deleting segments in the Alignment workflow.
- keeping the newline characters in sdlxliff segments.
- set the 2000 character limit for the automatic look-up of the current segment to avoid delays.
- export to bilingual Word documents from external projects.
- distinguishing between 100% translated units and approved/checked segments in sdlxliff projects.
- connection to Youdao MT online resource via the web browser interface.
- option to add invisible characters in the form of Unicode numbers to the “Do not match” list.
- sorting of TMX memories in the edit mode.

The new build of CTE 2018 Forerunner (**2017120401**) is available for download with the following:

- fixed a join segment issue with the simultaneous joining of both source and target segment.
- removed the Filter for kWord documents as this KOffice suite has been obsoleted.
- “Translated” status via the Task menu can be applied to the filtered segments only.

The new build of CTE 2018 Forerunner (**2017120601**) is available for download with the following:

- improvements in handling complex formatting for Ms Word filter*.
- added “Show glossary fields” right-click option for the Matchboard.

Also, in older builds, CT always joined existing segments ignoring any changes in the target segment editor. In the recent builds, it takes changes in the editor into account before the Join segment action if the target segment is new (not created yet).

Before the latest update, CafeTran sometimes merged some complex formatting across segments. For example, if one segment finished bolded and underlined, the following segment might continue with that double formatting even though bold was dropped leaving only the underlined part. This has been improved.

In the latest build of CafeTran 2018 - Forerunner version (**2017120901**), the font of the status column is larger to be able to click at the segment number and activate it more easily.

The new build of CTE 2018 Forerunner (**2017121501**) is available for download with the following:

- Memories and glossaries in the Dashboard are sorted.
- The Search action in the Frequent words list includes looking-up in Machine Translation services.
- New Filter actions: Non-translatable segments and Non-translatable fragments.
- Fixed an issue with doubling of non-translatable numbers in the F4 list.

The latest build (**2017121801**) fixes two DeepL issues (Text was not carried over to the DeepL tab if it contained line breaks or straight single quotes).

The latest build (**2017122101**) corrects the “GO TO CURRENT SEGMENTS” link position. It also features the following improvements:

- added the filter for Vector Graphics (.svg) files.
- automatic removal of non-translatable duplicates in F4 list.
- normalization of source segment apostrophes for the “Prefix matching” feature (all the major variants of apostrophes appearing in the source segments are internally treated as the straight apostrophe to increase the probability of finding the match).
- fixed the display of the source document name in the title bar in newly created projects.
- change of the “New project” icon in the Dashboard after the selection of the “Multiple document project” option.

The new build of CTE 2018 Forerunner (**2017122201**) is available for download with the following:

- fixed an issue with some bullets in the PowerPoint filter.
- corrected the display of source term synonyms in the glossary.

The new build of CTE 2018 Forerunner (**2018010401**) is available for download with the following:

- added an option to export all documents with notes in the glue mode.
- added the display of the background color from Ms Word tables in the grid.
- fixed an issue with auto-scrolling of MT panels when they are joined together.
- fixed an issue with colors while zooming the text in the segment editors.

The new build of CTE 2018 Forerunner (**2018010801**) is available for download with virtual joining of segments in external (created in other tools) projects. The feature allows to join segments in segments’ editor and rearrange their contents comfortably. As soon as the joined segments leave the editor, their number is the same as before joining but their respective text contents is changed (rearranged), hence the virtual aspect of this feature. Use this new feature with care making sure that boundary (opening and closing) tags between joined segments are in place.

Remove target segments feature: One needs to progress with external xliff files cautiously since they internal translation unit structure is often non-standard and not so obvious. With today’s build (**2018010901**) of the CTE 2018 Forerunner update, you can try the “Remove target segments” function on your mqxliff files.

## 2017 Yeddi Update 27 (20171114)

- Compacted tool bars in the Dashboard to gain vertical space.
- View > Toolbars > Hide help tips also hides the workflow tips at the bottom of the Dashboard.
- Access to the web resource or glossary information/settings via the right-click at its name in the Dashboard.
- Added some missing help tips for the recently added functions in the menus.

Additional builds:

- Coffeehouse theme and transparency of Dashboard’s tool bar are adjusted for Linux GTK theme in the latest build (2017111501).

- Latest build 2017111601 fixes the behavior of copy and paste shortcut that transfers text to adjust to DeepL’s new web interface.

## 2017 Yeddi Update 26 (20171110)

- Optional creation of Project Memory and/or Project Glossary while opening projects created in other tools. ProjectTM.tmx and/or ProjectTerms.txt files are created at the location of the project.
- Two new tasks - “Remove notes” and “Remove alternative translations”.
- Fixed an issue with positioning of panel dividers in the Dashboard.
- Fixed an issue with the caret color in the dark GTK look and feel on Linux systems.
- Refreshment of CafeTran themes. The change will be noticeable only after choosing a theme in the View > Themes. New transparent themes (bright and dark) with the slider controlling the transparency effect are very eye-friendly and they look just awesome. Give it a try!

Note: Uniform theme was removed. TMX related tasks have been gathered under Tasks > TMX memory submenu.

The new build of update 26 (201711101) is available for download with the following:

- added the System theme to reflect underlying operating system background color.
- added the “Quick search” icon to the source editor toolbar to toggle Search bar on/off.
- fixed tabs border issue in the GTK theme appearing with the background grid on.

## 2017 Yeddi Update 25 (20171023)

- Dragging of tabs with resources to change their position in the user interface.
- Fixed an issue with transparency of docked tabs in transparent themes.
- Changed the symbol for the tab character to fix an issue with the display of invisible characters. It is a bold red t now.
- Some fine tuning of “Team Auto-assembling with Machine Translation” option.
- Fixed a issue with source segment transfer to Google Translate web resource.
- Fixed a tagging issue in the first segment of the project when “Hide segment boundary tags” is off.

The new build of update 25 (2017102701) is available for download with the following:

- some minor user interface enhancements to adjust to GTK look and feel on Linux.
- simultaneous translating with the supported Machine Translation web resources (via the browser interface).
- The Alt+V keyboard shortcut transferring MT from web page works for docked web MT resources too.

## 2017 Yeddi Update 24 (20171016)

- Binding of MT editors on web pages such as Google Translate, Bing Translator, DeepL. See the binding option in Edit > Bind external editor and choose an editor in Edit > Preferences > General tab > External editor box. This new binding feature is dependent on the external website. If its web page or address changes, binding with the editor on that page will stop working.
- Action to transfer the MT result from a web page to the target segment - see the menu Translate > Transfer MT from web page. This transfer action (via the keyboard shortcut) can also be used when editors binding is off.
- Selection of the glossary during the manual Search when the glossary is joined to another resource under one tab.
- Fixed automatic saving of sdlxliff files after deletion of target segments via the Task menu.
  Option to change the Google’s MT engine (from neural to phrase-based) after the right-click at Google MT panel.

The new build of update 24 (2017101802) is available for download with the following fixes and improvements:

- Fixed a color issue while selecting a text in the back themes on Mac OS - Mac look & feel.
- Showing auto-propagation P mark for non-CafeTran projects - for the current session only.
- Accepting .xlsm (Excel with macros) documents in the MS Excel filter.
- Matchboard option to hide terms and fragments - after right-clicking on the Matchboard panel.
- Fixed a long text display in a pop-up info message when opening some sdlxliff files.

## 2017 Yeddi Update 23 (20171010)

- Masking of non-translatable fragments for MT online services. The feature is on by default and can be deactivated in Edit > Preferences > MT services tab. All non-translatable fragments longer than 3 characters are masked before being submitted for Machine Translation - both via API and the Web interface. You can see the masking effect in MT tabs. The unmasked translation result is displayed in the Matchboard and after the transfer to the target segment. The masking feature does not work with the right-click “Create TMX memory” MT function.
- A new “Find in page” keyboard shortcut in the Edit menu to search for word occurrences on a web page.
- A keyboard shortcut (CTRL+SHIFT+K) for deactivating a filter in the Filter menu.
- Basic order registering and invoicing feature moved from “Project Configuration” panel to the Statistics display.

The new build of update 23 (2017101102) is available for download with the following fixes and improvements:

- Saving the xliff file - in multi-file projects - which has been affected by cross-file auto-propagation automatically at exit.
- Fixed some dialog overlapping issues on Mac OS.
- Trimming of non-translatable fragments at masking them for Machine Translation services.

The new build of update 23 (2017101201) is available for download with the following:

- Added Euroglot as a web resource (see the Resources > Web menu) to CafeTran interface. This online resource requires login but there is a 10 minute free trial as too.


## 2017 Yeddi Update 22 (20171001)

- The update 22 is the first CafeTran version that runs either on Java 8 or the latest Java 9.
- Removed support for the outdated Java 7.
- Java 9 fixes an issue with garbled characters on some web resources (e.g. TM-Town login page) on Mac.

The new build of update 22 (2017100301) is available for download with the following fixes and improvements:

- Fixed an issue with the segments grid display after the “Segment with letters” filter is set.
- Fixed an undo/redo editor’s issue related to Java 9 update.
- Handling TMX translation memories which have the external Document Type Definition (DTD) set.

## 2017 Yeddi Update 21 - 20170901

- Added DeepL Machine Translation online service as a web resource (see the menu Resources > Web > DeepL).
- The Translate button in the source segment toolbar copies the source segment (or selection) to the internal web browser to look up the segment or the selected phrase in the Machine Translation web resource which is currently selected in the tab.

Due to a Java 8 issue on Mac OS, the DeepL web resource is not displayed properly in the internal web browser on Mac systems. The issue has been reported and is probably fixed in Java 9 (official release on 2017.09.21). I will update you on this Java release. Impatient and brave Mac users can already download and install early access builds of Java 9.

The typical workflow with Machine Translation service as a web resource (which is not available via API yet) is as follows:

- Choose MT web resources to work with via the menu Resources > Web or the Dashboard.
- Select the MT web resource in the tab.
- Click the Translate button in the source segment toolbar to copy the current source segment or a selected phrase to the source text box of the MT web resource.
- Select with the mouse the provided machine translation in the target box of the resource in the web browser to transfer it fast to CafeTran’s target segment editor.
- If the target language box of the resource is editable (e.g. DeepL), you can bind it to CafeTran’s target segment editor via Edit > Bind external editor. Then, just edit the translation and press the CTRL+A followed by CTRL+C keyboard shortcuts to transfer the translation and move on to the next segment.

The new build of update 21 (2017090802) is available for download with the following improvements and fixes:

- The editors binding via clipboard on Mac OS works with text areas inside the internal web browser (e.g DeepL web resource). Note that you can place the pipe character “|” in the bound editor to indicate the position of formatting tags.
- Added the support for comments in .txml files.

The new build of update 21 (2017091301) is available for download with the following:

- Fixed the display of percentage in Fuzzy Matches in the Matchboard.
- Fixed a fuzzy match duplication issue during auto-correction.

The new build of update 21 (2017092301) is available for download with the following:

- Fixed the cyclic text transfer via Clipboard in the Clipboard workflow.
- Some polishing of the Dashboard interface.

The new build of update 21 (2017092701) is available for download with the following:

- Block to load multiple memory files which have the same name.
- Interface font size for 1400-1900 resolution screens is two points larger by default.

## 2017 Yeddi Update 20 (20170824)

- Improved handling of comments in non-CafeTran projects.
- Memory fuzzy matches can be edited from the Matchboard directly via the right-click at the yellow link.
- Automatic switching to the TM tab containing the result of the manual search in the translation memory.

The new build (2017082901) of update 20 is available.

- The TM tab should be selected during the manual search even when it contains more (joined) TMs.
- Double-clicking on an auto-completion phrase inserts the phrase into the target segment editor.


## 2017 Yeddi Update 19 (20170708)

- Instant transfer of the selected text from the target segment editor to the Search box.
- Mouse or keyboard selection of a glossary match in the alphabetical Match bar pops up all the additional fields in the glossary entry.

## 2017 Yeddi Update 18 (20170731)

The update 18 brings the following improvements:

- A keyboard shortcut for “Delete segment” in translation memory edit mode.
- Access to Preferences from the Dashboard menu.
- Project > Export and Exchange > To TMX memory… and Memory > Import > Import project segments take the filter state into account during segments’ transfer. For example, the user can open a translation memory in the edit mode, create a range filter by typing segment’s numbers range (e.g. 1000-2000) in the Search field, and then transfer the filtered segments to the new translation memory.
- A new bright theme for Dashboard.
- A few minor fixes.

In today’s build of update 18 - 2017080101, the Document note opens automatically in CafeTran’s projects. Also, when you quit the program and your note has been edited, CafeTran asks in you wish to save it. Please download and apply the update 18 again.

## 2017 Yeddi Update 17 (20170726)

The update 17 includes some fixes and improvements released in the recent builds such as:

- Fuzzy match auto-correction.
- Clearer translation memory info tips when hovering the mouse over a hit in the Dashboard or TM pane.
- Sorting matches by length in the Matchboard - the option available after right clicking at the Matchboard pane.

The following new QA actions have been added:

- Same source with different target check.
- Same target with different source check.

The QA checks above share the same fuzziness as is set in the “Do not match” field of Preferences > Memory tab.

Furthermore, clicking at the number of occurrences of the phrase in the Frequent words list searches for the phrase in the Project’s source segments. It can be useful if you wish to see the full context or filter out all the segments containing a frequent phrase.

## 2017 Yeddi Update 16 (20170705)

* The glossary option in Preferences to display the longest matches only.
* Sorting by length filter action.
* Fixed a display glitch with TM hits - numbers.
  Improved handling of regular expression errors in glossaries.
* Fixed a character escape error when loading tab-delimited glossaries to Total Recall.
* Fixed some status setting and display issues with sdlxliff files.
* **Automatic loading of HTML preview page in CafeTran projects after restart.**
* Fixed a focus issue with the Export dialog.

The new build (2017070601) of the update 16 tackles three issues:

* Matchboard pop-up info hiding when the mouse is off the pop-up panel.
* Regular expression errors handling during auto-assembling that might block the display of the results in the Matchboard.
* Project > Export and Exchange > To Package… panel focus issue.

There is a new build of update 16 (2017072001) available. It improves and adds the following:

* Fuzzy match auto-correction.
* Clearer translation memory info tips when hovering the mouse over a hit in the Dashboard or TM pane.
* Sorting matches by length in the Matchboard - the option available after right clicking at the Matchboard pane.

## 2017 Yeddi Update 15 (20170627)

* **Automatic fragments adjustment.** This a new and experimental feature which picks fragments/terms from the current segment and updates their priority on the fly. It can also adjust to some slight changes in the fragments (e.g. plural forms) creating virtual fragment pairs if their do not exist in your resources. The feature should be very helpful when there are still good matches coming from low quality/priority resources to use in auto-assembling. Then, CafeTran will enhance their status automatically for the current project. Furthermore, it detects term’s synonym usage adjusting its priority automatically.
* Translation Memories panel in the Dashboard can hold up to 100 TMs now.

The second build of this update sets the 3-character limit on the terms/fragments for the automatic adjustment. Please download and repeat the update as described in the announcement post above.

Some more information about this function. Its character is dynamic picking the recently used match for a fragment/term or its synonym as the one with top priority to use in subsequent segments (both in auto-assembling and MT improvement). It can also adjust the basic form of a fragment (e.g. sunny day) to the one you actually use in the segment (e.g sunny days) provided that change is slight - in the form of the regular noun, in this example. Then, CT will use the adjusted fragment in the subsequent segments. So let’s say CT suggests a correct virtual TM fragment (hit) by analyzing the context but your top priority glossary inserts another suggestion (e.g. basic form). If you use the virtual fragment in the current segment, CT will enhance the priority of this virtual fragment to use in the subsequent segments.

The user has been able to replace an automatically inserted translation by right-clicking on it in the target segment if there is an alternative. Then, the new selected translation is used as the top priority match in subsequent segments despite its priority.

The new feature seems to be a fully automated version of this translation/priority replacement feature, which is enhanced by including hits and near-same matches. Is it?
That’s correct. There is no need for the right-click manual action now.

## 2017 Yeddi Update 14 (20170615)

* Changed the size of the Autocompletion panel depending on the screen resolution.
  Adjusted the size of some buttons for UHD screens in Metal look and feel.
* Fixed a tagging issue for embedded objects in MS Word filter.
* Improved hiding of the initial and ending tags with adjacent space.

Important!
If your currently translated MS Word documents contain embedded objects, please complete their translation before applying this update.

The new build of update 14 (2017062001) is available for download with the following enhancements:

- Adding the visual mark for segments that are set not to propagate.
- Clearer user interface font for lower-resolution screens in Nimbus look and feel.
- Correct display of the Matching type option in TM options panel.

## 2017 Yeddi Update 13 (20170609)

Summary of changes added in the recent builds:

* Cmd+A selects the whole text in Metal look and feel on Mac computers.
* For those who find the dark Dashboard too dark on sunny days, the bright option is now available in the Dashboard menu - just uncheck the Coffeehouse theme checkbox.
* Fuzzy match auto-correction also works if the start and/or the end of the current segment is missing in the fuzzy match, and there are matches in TM, glossary or nontranslatables for those missing parts.
* Optional binding of CafeTran to Jarte (a powerful Windows text processor).

New features:

* “Keep out of auto-assembling” option for glossaries can be made permanent by choosing it from the list of priorities.
* The bright Dashboard theme is set automatically along with bright CafeTran themes.
* “Improve auto-assembling with Machine Translation” option can be accessed quickly via the right-click at the MT pane.
* Clicking at “Translate selected fragment” link in the Machine Translation pane shows the original MT result if “Improve auto-assembling with Machine Translation” option is selected.

## 2017 Yeddi Update 12 (20170531)

* The translation results from all MT services are remembered for each segment in the running project to access them fast again (e.g. when reviewing the translation).
* Adding non-translatable terms either from the source or target box in the New term dialog.

The new build (2017060102) of update 12 is available for download. The file chooser does not hide the main interface now as it caused a major issue with choosing files for alignment. Please follow the steps described in the announcement post above to update your installation with the new build.

## 2017 Yeddi Update 11 (20170524)

* Storing the source document location and rate information in the Project template.
* New TMX memory task in the Task menu called “Split TMX units”. It splits translation units at a character or a phrase - set separately for source and target segments.
* Exposing Save and Open file choosers to avoid losing them behind the main application window.
  Search and replace panel is not set as “always on top” now.
* Some little spring changes to the Dashboard theme.
* Fixed the <> characters display issue when they are included in the searched phrase.

Auto-assembling for MT in Preferences after this update:
The feature has been adjusted to the new API as the previous implementation caused some issues. Now you can choose either of the two options - with improved MT version or unchanged MT result, but not both at the same time.

## 2017 Yeddi Update 10 (20170517)

The update 10 is a maintenance update summing up a few builds released after the update 9. * Furthermore, the following fixes and improvements have been made:

* “Replace all” also does the replacement in the target segment being edited. YES
* Auto-correction (via CTRL+Space shortcut) of a spelling mistake at the cursor position instead of the position at the last red-underlined word.
* Fixed an issue with the MS Excel filter when the translator uses an MS Excel glossary as a resource.

## 2017 Yeddi Update 9 (20170508)

* **Project templates**. This update adds the templates feature which stores in a template file the selected CafeTran resources from the Dashboard (Total Recall memories, TMX translation memories, glossaries and Web resources), language pair, windows layout and colors to use for a new project. See the new menu button next to the language pair boxes in the Dashboard to save or load project templates.
* **Total Recall memories with segments in regional variants of a given language are recognized automatically** in the projects with a different variant for the same language.
* Remembering the state of the new previously unconfirmed segments when leaving them unfinished in the target segment editor (e.g. by switching to the Filter view).
* Resetting the preferences does not reset the language pair, the list of recent projects and selected resources in the Dashboard.
* **New segment navigation command - “Add segment to memory and go to next untranslated segment”** (default keyboard shortcut - CTRL+ENTER).

Default Scope search shortcut has been moved by default to : Ctrl+Shift+G (was Ctrl+Enter)

The templates implementation is a new feature and may be further refined in later updates. However in its current form, it gives the user the control over the organization of the template files the same way they manage their other documents in the system (e.g. choosing a folder, moving, renaming and deleting them). So the user can simply assign a folder for the .xml template files wherever he/she wishes and can even share them (e.g. via Dropbox). It also frees CafeTran from additional complexity of the interface such as more interface buttons, menus or a special database for templates. As for the .xml extension, I assume the low probability of mixing .xml templates files with other .xml files just in a folder assigned for templates. To put is simply, you are free to organize your .xml template files as you like. CafeTran can only create and access them. I don’t think any additional template file management features are necessary in CT interface.

The new build of update 9 is available (2017051101) with two minor changes:

* remembering projects’ location settings in project templates.
* keeping target segment editor’s contents when joining current empty target segment with the next non-empty target segment.


## 2017 Yeddi Update 8 (20170426)

* Switch to the new Google Cloud Translation API which uses the neural machine translation model.
* **Navigation between documents in the glue mode. See the “Documents” button in the grid toolbar.**
* Fixed the punctuation issue when recalling segments from Total Recall table. The issue appeared after the user cleared the “Do not match” field in Memory preferences.

The new build (2017042703) of update 8 is available. It makes the keyboard shortcuts for **merging and hiding tags undetermined by default ** as they caused issues with typing some international characters. The user can set them in Preferences > Keyboard shortcuts tab. The build does not change your existing (already set before) shortcuts for the two actions.

## 2017 Yeddi Update 7 (20170419)

* The option for changing UI font size in the View > Font menu.
* **Automatic refresh of the current segment at hiding/merging tags.**
* Thicker border around the current segment in the segments grid.
* Fixed automatic highlighting of the current segment in the HTML source preview.
* **New QA features with word lists**: Find and replace source/target segments. They make it possible to preform multiple replacements both in the source and target segments in a single action. The replacement list is in the simple text format where the searched word is followed by the equals sign '=' and the replacement word. For example: cat=dog.
* A 'Version' status for the current segment in the target segment toolbar. It allows for a simple form of segment versioning. When the Version status is selected, CafeTran stores automatically the previous translation of the current segment in the alternative translation list. Alternative translations are marked as “A” in the segments grid and can be accessed after the right-click at the source segment editor. The feature is for translation projects created in CafeTran Espresso.

## 2017 Yeddi Update 6 (20170410)

* New Auto-propagation option - **Auto-propagation forward only.**
* **In the Filter view, hold CTRL key while clicking the Filter button to stay at the last filtered segment after return to the Normal view**.
* Editing the user’s spell check dictionary or non-translatables sets the cursor at the end of the file.
* Fixed display of percentage numbers in the progress bars in Nimbus look and feel.
* When in the Glue mode, CafeTran displays the red G in the segments grid to indicate the glue mode.

And while in the Filtered view, CafeTran displays the red F in the project segments table.

## 2017 Yeddi Update 5 (20170330)

* Fixed scope of the search to a single document in the unglue mode.
* Consistent naming of the exported target documents in the glue mode.
* Project close confirmation dialog when opening or creating projects.
* Increased interface font size for higher resolution screens.
* If skipping locked segments is active, the search function omits such segment too.
* **Added “Block JavaScript” option** for web resources to deal with a few web pages (usually with numerous ads) which may cause hanging of the whole application.

## 2017 Yeddi Update 4 (20170325)

* Removed single-digit non-translatables from the F4 list.
* The auto-completion keyboard shortcuts start from 1.
* Multiple dots wrap up in the Matchboard results.
* **Mapping Memsource confirmed status to CafeTran checked status.**
* Added the option to **block auto-propagation to other documents in the project.**
* Switch to the new Microsoft Azure API for Microsoft Translate MT service.

## 2017 Yeddi Update 3 (20170310)

* Improved mixing of custom formatting with transferred formatting.
* Fixed calculation of the translation speed per minute in the statistics.
* Added “Session duration” to the statistics.
* Blocked auto-propagation of source segments with numbers when there is no number in the corresponding target segment.
* **Added “Show term information” right-click option to the display of ProZ.com and TM-Town.com search results. **
* **Added the horizontal/vertical docking tabs option to enhance the personal adjustment of the user interface.** It is available in the menu after right-clicking at the tab title. You will need to undock the currently-docked tabs before applying this new option.

## 2017 Yeddi Update 2 (20170302)

* **Added the locked segment status for CafeTran projects.** The locking segment status works in non-CafeTran projects for the current session only. It does not interfere with the segments locked in other tools.
* Two new tasks to lock and unlock filtered segments in CafeTran projects.
* Locked segments do not get converted to the translation memory via Project > Export > To TMX memory… action.
* **Turning on/off the auto-propagation of single segments via the right-click at the source segment pane.** It replaces the auto-propagation blocked by alternative translations.
* **Filtering of Matchboard results via the double-shift shortcut both in the source and target segment editor. The filtering is incremental, that is, you can type or select the first characters of the match and press the Shift key twice. For example, type the first two letters of the matched source fragment and press the shift key twice to display the matches starting with the typed characters.**
* Corrected the filtering of numbers in Excel cells. Please complete any current MS Excel projects before updating.
* **Simplifying the non-translatables glossary format to one column to reuse the entries in other languages.**
* Highlighting of the whole phrases present in the fuzzy match in the order different than in the source segment.


DOUBLE-SHIFT FEATURE
There is an interesting side-effect to this feature. It enables really fast selection of single words to add them to the TM or glossary if they are not present in the Machboard:

Double-shift in the source pane, double-shift in the target pane and add the pair to your resource.

## 2017 Yeddi Update 1 (20170221)

* The Matchboard displays multiple exact matches and the name of the TM being the source of the exact match.
* Corrected the order of imported stories in Adobe Indesign IDML file filter (only for new translation projects).
* Keyboard shortcuts for inserting matches are positioned on the left side of the pop-up panel.
* The Matchboard can display the context for TM fragments and hits the same as in the TM tabs.
* The Matchboard can display additional properties or fields for a TM or glossary match if the mouse is hovered over the match.
* You can edit the matches in the Matchboard after clicking.
* Recalling from Total Recall can recognize words surrounded by non-breaking spaces.
* Fixed the issue which caused that some irrelevant segments were included in hit’s contextual results.

## 2017 Yeddi - 20170201

CafeTran Espresso 2017 Yeddi has been released today. The new version provides translators with the cutting edge assisted translation technologies with the design and focus on translating fast and with fun. It is a summary of ongoing development and the features introduced throughout last year, polished with the invaluable feedback from CafeTran’s users. Apart from numerous fixes and improvements, the Yeddi version comprises the following:

* Mastered subsegment matching and auto-completion.
* Intuitive Matchboard.
* Optional integration with ProZ.com terminology bases.
* Optional integration with TM-Town resources.
* Optional integration with Machine Translation services.
* New Project Dashboard and the user interface for high resolution screens.
* Refreshed dark and white eye-friendly texture themes.
* Improved Auto-assembling algorithm.
* Contextual segments’ retrieval system - “Total Recall” with the support for alternative databases (e.g. MySQL database).
* Flexible docking and joining of numerous resources (translation memories, glossaries and web resources).
* Binding of favorite external editors to enhance the editing process (e.g. with dictation).
* Fuzzy matches auto-correction.
* Auto-tagger: inserting matches along with formatting tags in the target segment.


## 2017 Harbinger RC 4 (20170103)

* The alternative connection to **Yandex Translate MT service** - see the option in Edit > Preferences > MT services tab. Required the API key from Yandex.com after the registration.
* Experimental filter for **xliff 2.0 files**.
* **Automatic switch to preliminary memory matching with large translation memories.**
* Holding CTRL key in New Term/Fragment panels does not erase editor’s contents.
* Fixed the selection of words with German “ß" when changing the case.
* Fixed a language direction issue when importing a glossary into the TM.

AUTO-SWITCH TO PRELIMINARY MEMORY MATCHING
 Τhe threshold segments’ number is set high by default (25000 segments), and you can change it in Edit > Preferences > Memory tab.

To switch off this “feature” (and I think I want to do that - all those darned new things), the only way to achieve that seems to be to increase the preliminary matching threshold to very, very high, like 5,000,000 or even more

TOTAL RECALL ALONG WITH PRELIMINARY MATCHING
Well, I have finally understood how the two TM leveraging features (Total Recall and preliminary matching) can go together.

Total Recall can work as the first-level filter, picking up relevant segments based on the number of word/character occurrences.

Preliminary matching can work as the second-level filter, comparing the source segments with the recalled TM in detail (i.e., in consideration of word/character order).

So, the result of TR + PM can be a very light resource, hence a much quicker retrieval.


## 2017 Harbinger RC 3 (20161222)

* **New Term/Fragment dialog got a button to add a new entry without closing the dialog.** It enables translators to add multiple TM/glossary entries at a time.
* The refreshed dark and white eye-friendly texture themes (menu View > Themes). Image background transparent dark/bright themes are there to reduce eye strain and allow brightness adjustment with the slider in the source segment toolbar.
* Polished Nimbus look and feel becomes default on Windows and Linux systems. It does not replace your current look and feel. You will need to choose it in Preferences > Appearance tab if you wish to try it.
* **New option: View > Tabs > Bottom tabs placement.**

## 2017 Harbinger RC 2 (20161212)

* Improved automatic transfer of term’s surrounding tags with complex tagging in non-CafeTran projects.
* Fixed the display of the glossary matches with source-side synonyms.
* Check and update of file paths in multiple documents (glued) projects when they are moved to another computer.
* Fix to the MS Excel filter - recognizing number-formatted cells which still contain the text instead of numbers.
* Fixed an issue in the Release Candidate 1 with opening the memory via the Memory menu. The matches were only shown when the TM was opened via the Dashboard.
* **This update also includes an experimental feature of synchronizing CafeTran’s target segment editor with some external editors**. It may be particularly useful to the users who enjoy some advanced editing functions in their favorite editing environment. It allows getting the best of both worlds. The details and list of the currently supported editors are shown in this article [https://cafetran.freshdesk.com/solution/articles/6000162841-target-segment-editors](https://cafetran.freshdesk.com/solution/articles/6000162841-target-segment-editors). The feedback from the users who also translate (or dictate) in external editors is welcomed.

## 2017 Harbinger RC 1 (20161205)

* **A glossary can contain non-translatable fragments only - see the option when you add a new glossary**.
* Auto-completion fragments from TMs and glosssaries are sorted by their quality now.
* Unchecking the alphabetic sorting in the Matchboard lets CafeTran sort them in the mixed mode - first by quality followed by (multiple) matches for the same source.
* Trimming double-spaces when transferring matches to the target segment (e.g in the Machine Translation results).

## 2016 Ichiro Update 27 (20161128)

* Fuzzy matches Auto-correction with non-translatable fragments.
* **Auto-tagger**: inserting matches along with formatting tags in the target segment.
* The Matchboard displays full glossary entry even when only its prefix/stem is matched.
* The Matchboard displays one entry for numerous duplicates where both source and target are the same.
* Fixed F2 shortcut for displaying matches in CJK languages.
* **Auto-completion also works when deleting characters via the Backspace key.**
* Check for invalid characters in the project name.

## 2016 Ichiro Update 26 (20161118)

* Switch to the horizontal Total Recall Dashboard panel split when the main window gets very narrow.
* Flow layout of resource names in the Dashboard panels to use the available space better and fit more resources in the panels without scrolling.

## 2016 Ichiro Update 25 (20161109)

* Long matches in the Matchboard switch to the vertical display to save the space.
* Matchboard’s right-click option to shorten match information in the grid.
* The default font scale setting for websites in the View > Font menu.
* Redo/Undo function in the source segment pane.
* Automatic case adjustment of the target segment while typing - an option in the Edit > Target menu.
* A new major feature “**Bind external editor**” (see the option in the menu Edit) with its **AutoNext** function.

Binding the external editor to CafeTran serves two purposes:

1. Enable dictation with CafeTran across all operating systems.
2. Enjoy your favorite typing environment and its functions (e.g. alternative spell checker, grammar-checker).

When you finish dictating or typing of the target segment in the external editor:

On Windows and Linux, press CTRL+A followed by CTRL+ C shortcut.
On Mac OSX, press Command+A, Command+C, Command+TAB shortcut.

The AutoNext function handles the addition of the current segment to the memory and takes the next segment for translation automatically. It also corrects the capitalization of the target segment and its ending punctuation - two frequent errors during dictation.

On each operating system, the above shortcuts can be grouped as one, activated by a voice command if you wish. The detailed description will be available in the Knowledge Base soon.

The AutoNext function has been tested on each operating system in Google Chrome browser using Google Docs “Voice typing” tool which works with lots of languages. The function can be used in other editing environments (e.g. MS Word or LibreOffice) with your preferred dictation program (e.g. Dragon Naturally Speaking).

Hopefully, this new feature will add yet another translation technique, boost and fun to your workflow.

Second build 2016110903:

1. The source segment locking reverted to the previous version because of the mentioned focus change issue.
2. The Total Recall Search buttons are filled with their color now on Linux system.

The second build of this update brought back the ability to select the source segment even when the edit source segment option is off. The behaviour is exactly the same as before - the changes to the source segment in the pane are only for the purpose of the selection and correction with the edit option off.

 Third build (2016111701):
 The new build of update 25 (2016111701) fixes the Dashboard visual issue where the window is too narrow to display the resource names properly. Then CafeTran switches Dashboard orientation. It also arranges the Dashboard panels space better. If you do not want to wait for the next update, please download and install the update 25 again.

## 2016 Ichiro Update 24 (20161102)

1. Sizing and highlighting improvements to the Matchboard.
2. Added the following options to the Matchboard:
   - sort matches alphabetically. If this option is disabled, CafeTran displays the matches sorted by their quality
   - show fuzzy memory fragments
   - show fuzzy glossary terms
   - show auto-assembling result

The above options are accessed via the right-click at the Matchboard.

3. For Mac OSX, there is a new option to wrap tabs - see the menu View > Tabs > Wrap tabs.
4. Consistent colors for resources in their search bar buttons, Matchboard results and Dashboard panels.

Sorting of the Matchboard results broke the display of target language synonyms in today’s update. It is fixed now so please reapply the same update 24.

The additional option to hide the MT results from the Matchboard has just been added as well.

## 2016 Ichiro Update 23 (20161027)

1. Fixed the non-translatable highlighting issue in the source segments containing tags.
2. The rollover undocking icons are placed directly in the docked panels instead of the status bar.
3. The new tab docking option - Dock tab to window vertically - left.

Both the dynamic adjustment of the tab docked at the segment editor and docking tabs to the segments grid should work okay now. Please download and apply the same update 23 again.

## 2016 Ichiro Update 22 (20161022)

1. Fixed sorting of the glossary matches in the order of appearance for CJK languages when the Prefix option is on.
2. Listing non-translatables (F4 keyboard shortcut) in the order of appearance.

and the reported issues fixed later in update 21 as well:

- the segment parser changes dynamically when it detects the change from CJK source language to a language with the word separator.
- the spell checker gets deactivated when the user switches to a target language with no spell-checking dictionary available for it.
- the actual name of the new memory is shown (instead of “New TM”) when creating it in the Dashboard.

## 2016 Ichiro Update 21 (20161017)

This update fixes mainly some reported visual issues and improves a few features:

1. Consistent tags size.
2. Less bright Matchboard colors.
3. Choice between the horizontal and vertical divider when joining tabs in the View > Tabs menu. The horizontal divider is the default one.
4. Improved synchronization between the current segment and its auto-assembling result to avoid timing issues with large memories set in the Automatic mode.
5. Total Recall can function in the Clipboard workflow.
6. In the “Paper/Image document” workflow, the selected Total Recall memory tables open for searching automatically.
7. Added “Hide source segment tags” keyboard shortcut in the Action > Tags menu to toggle tags display (already present in update 20 but not announced there).

Based on your immediate feedback, I pushed a few changes to the last update 21:

* the segment parser changes dynamically when it detects the change from CJK source language to a language with the word separator.
* the spell checker gets deactivated when the user switches to a target language with no spell-checking dictionary available for it.
* the actual name of the new memory is shown (instead of “New TM”) when creating it in the Dashboard.

## 2016 Ichiro Update 20 (20161010)

What’s new:

1. Maintained the font type and size when applying the custom formatting in Word documents (e.g. bold, italics).
2. Added the settings for the font size of tags: View > Font > Tags.
3. Further increase of the button fonts in the main interface for 4K (3840 pixels) resolution screens.
4. ProjectTerms glossary files are saved with the line separator default in the used operating system.
5. Total Recall can connect to MariaDB database (MySQL replacement for Linux systems).
6. Added the Quick search… menu item in the Edit menu to show and hide the Search tool bar.
7. The Matchbar becomes a dockable or floatable Matchboard.

The new Matchboard groups all the matches for the current segment including the matches from the connected Machine Translation resources. The results in the Matchboard can be both clicked and selected to transfer them to the target segment. The match type and the resource name are also shown there. The Matchbar, placed at the top of the Matchboard now, is still functional to quickly display the matches without the need for scrolling in the long list of the matching results. Note the convenient keyboard shortcut when typing in the target segment pane: double SHIFT + the first letter of the source match to narrow down the long list of the results.

8. The improved Auto-assembling algorithm calculating the weight of the match with the following order of preference:

- Context segments
- Exact segments
- Prefix segments (translation memories with the Prefix matching on)
- Context fragments (Exact and Virtual TM fragments with the matched context)
- Exact fragments and terms
- Virtual fragments ('guessed' TM matches with the high number of hits)
- Other Fuzzy fragments and terms (regular expression matches, prefix and stem matches, 'guessed' TM matches with the low number of hits).

If the matches for one word/phrase are of the same type, the set priority of the resource is taken into account.

## 2016 Ichiro Update 19 (20161003)

1. This update provides the implementation of contextual Total Recall system working with the alternative MySQL database. This is a recommended solution for a central database system serving numerous clients on the network or with the storage and recall of very large translation memories consisting of several million segments. Please see this article for connection details.
2. Fixed an issue with hidden rows in Ms Excel files filter.
3. Added the check for empty lines in text glossaries which may block the correct recognition of some entries.
4. Increased the fonts of the main interface buttons for 2K resolution screens.
5. Brought back the optional Autoassembling and Fuzzy matches pop-up panel. See the new checkbox menu Translate > Pop up auto-assembling panel.
6. Fixed a reported minor issue when the user creates a new translation memory in the Dashboard. The file chooser to save this memory appears later on during the translation. It shouldn’t as the file has already been saved during its creation.
7. The correct recognition of Ms Word .docm files containing macros. There is no need to rename them manually now.

## 2016 Ichiro Update 18 (20160916)

- Convenient Total Recall access directly from the Dashboard.
- Removed the remaining space at the end of the segment after Drag & Drop in the 'Automatic space adjustment' function.
- Ability to add untranslatable terms/phrases to glossaries. CafeTran recognizes untranslatables phrases in the glossary when it is preceded by ! character. For example:

!NASA

Since the above term can be untranslatable, you don’t provide its translation in the glossary.

I lowered the resolution of my computer to 1280 to check and the toolbar texts took too much space indeed. The fix is available. Please download again and reapply the update 18 and it should be okay now.

## 2016 Ichiro Update 17 (20160907)

- The ability to open the recently-supported .mqxlz files via Drag & Drop on the Dashboard panel.
- Increased the maximum font point size of the adjustable interface elements to 50 - for convenient adjustment in high resolutions screens.
- Added the “Prefix matching” matching option for glossaries.
- Proper handling of synonyms/alternative terms and other fields in tab-delimited text files opened via the Memory interface (menu Memory > Open memory…)

## 2016 Ichiro Update 16 (20160831)

 The size and state of the Dashboard panels is maintained when you close the project.

- Added support for .mqxlz files. These are zipped .mqxliff files which previously needed to be unzipped and zipped back after the translation. Now, these actions can be performed directly in CafeTran.
- Ability to edit entries (segments or terms) in .txt tab-delimited files when they are loaded via the Memory interface.
- Added the Search option for the ProZ.com users in the “What am I working on?” feature. It enables filtering out the messages containing specific words.


Tmx files and tab-delimited files have been loaded into CafeTran via two separate user interfaces, namely, Memory and Glossary. This led to some confusion and raised a question why to keep the two separate. Ideally, there should be no such a distinction so there is a development effort to let users load and present any type of terminology and translation memory matches via one singe interface from various sources/file types. This can be already done via the Memory > Open memory… menu. The Memory interface does not support regular expressions but I believe that 99% percent of the users do not use such complex structures in their entries. For them, using one common interface could be simpler and more intuitive. No matter where you keep the whole segments, longer fragments and terms (in a tmx file or tab-delimited text file or Total Recall database), they can be loaded into the working Memory and matched the same way.

## 2016 Ichiro Update 15 (20160823)

 Resizable TMs/Glossaries/Resources panels in the Project Dashboard.

- Coffee house style for the Project Dashboard.
- Highlighting of the words occurring in the changed order in fuzzy matches.
- Option to hide all the tags in the current source segment.
- Mapping of the sdlxliff 'Approved' segment status to CafeTran's 'Checked” segment status.
- Optional connection to Slate Desktop Machine Translation service.

You may have used some smaller screen such as 11 inches MacBook Air? Anyway, I have corrected some UI elements of the Project Dashboard for such screens. Please reapply this update.

## 2016 Ichiro Update 14 (20160809)

- lowered fuzzy match calculation when the matched words are present in the segment in a different order.
- translation consistency check - an issue in the similar segments with different numbers only and the Autopropagation option on. Such segments were falsely reported as inconsistent.
- splitting QA trailing and leading spaces check into two independent checks.
- embedded display of Google Maps based on the user’s available location in the new ProZ.com “What I am working on” feature for translators.
- added an option in the Project Segments pane to set the Filter on the found word/phrase directly after performing the search via the Search bar.
- increased font size for the resource name field in the Autoassembly pane.
- another color for the assembled result in the Match bar to distinguish it easier from the TM fuzzy match results.
- a modified “Image background - bright” shaded theme.

## 2016 Ichiro Update 13 (20160802)

- increased font size of some interface elements for high resolution screens.
- the display of the found segments in the project segments pane during the search in multiple documents.
- the Find and Replace panel keyboard shortcut can transfer the selected words either from the source or the target segment pane even when it is kept displayed.
- the “Add segment note” button/keyboard shortcut transfers the selected words either from the source or the target segment pane to the Note editor.
- a new dark theme inspired by the Dracula Look and Feel.
- added the ability to edit or delete comments, add project’s representative words in the new ProZ.com project sharing feature “What are you working on?”. Now the users can also include images and photos describing their current project’s context such as a nice work place or the subject of the translation.

## 2016 Ichiro Update 12 (20160726)

The Ichiro update 12 focuses on CafeTran interface to the new service available for ProZ.com and TM-Town.com users. It enables translators to share the information about their translation projects interactively. CafeTran users can view and post messages via CafeTran without the need to switch to their web browsers. There is also a filter option to view posts coming only from other CafeTran users and reply to such posts. Although ProZ.com emphasizes the promotional aspect of this feature for translators as well as the ability to track their projects history, designing the chat-like interface I focused on the social side of it. Hopefully, in the near future, translators will also be able to share the photos straight from CafeTran’s interface i.e. to show their picturesque translation scenery or the cafe where they enjoy having lunch, and perhaps invite other translators working nearby, in a sort of CafeTran spirit. As it is a new feature, I would be happy to receive any feedback on using it in CafeTran. Thanks!

Other improvements in this update:

- Improved the search function for single and multiple (i.e put in a folder) text files that do not have a specified separator between source and target entries - it is a useful extension of the glossary search. Added the highlighting of the found terms in such files too.
- Minor interface changes such as margins, borders to columns and the look of the buttons in ProZ.com and TM-Town interface.
- Increased the size of the Autocompletion pop-up panel for high resolution screens.

## 2016 Ichiro Update 11 (20160715)

The Ichiro update 11 brings numerous improvements and fixes a few known issues:

- Fixed a rounding issue in the translation speed display of the Statistics panel.
- Added a new panel to the Project dashboard for “Other resources and services”.
- Fixed an issue to the HTML filter (proper filtering of the <script> tag).
- More intuitive display of the search bar with descriptive search buttons.
- Automatic removal of the pipe character that marks stems in the glossary entry when the language pair is reversed - the pipes marking stems on the target side are hidden now.
- Display of the auto-matched source term only instead of all synonyms on the source side for clarity.
- Added “Go to current segment” link in the project segments pane when CafeTran shows search results for phrases in the project segments.
- Saving the “Keep out of the Autoassembling” option in the TMX file to make it persistent for the TM between sessions.
- Updated ProZ.com search term function with the automatic “match exact fragments” option. This option is on by default.
- Integration of the ProZ.com term search exact fragments with the Auto-completion function and the Matchbar for quick access and transfer of the terms to the target segment.
- Added the “What are you working on right now” dialog to ProZ.com interface to share information about your current project and promote the work you do. It will also let you track your project history over time. The ProZ.com users can see the shared information after clicking the #Nowxl8ing button in the ProZ.com service tab.
- Added the third option for “Surround with characters” feature.

## 2016 Ichiro Update 10 (20160610)

- The matches in the Match bar display the name of the resource they come from.
- For source languages without the word separator, the ordering of the matches in the Match bar is based on their order of appearance in the source segment.
- The translation speed per hour in the Statistics is updated continuously taking minutes between hours into account.

I left the CT running for more than one hour and noticed that speed per minute in the Statistics was reset after each next hour instead of summing the minutes. It has just been fixed so please reapply the above update. The current CafeTran build is 2016061001.

## 2016 Ichiro Update 9 (20160606)

 The Ichiro update 9 adds to CafeTran’s interface KudoZ questions and answers of the Proz.com service:

1. The automatically-updated display of KudoZ questions and answers.
2. Asking a KudoZ term question after selecting a term in the source segment pane (the optional right-click at the source segment pane or in the Proz pane).
3. Answering a KudoZ question.
4. KudoZ Q&A display preferences dialog - after the right-click at the Proz pane.
5. Minor Dashboard interface improvements.

## 2016 Ichiro Update 8 (20160519)

The Ichiro update 8 offers the following:

- The new interface for the Frequent Words feature. It is faster, more intuitive and scalable for large projects.
- Improvement to the algorithm which 'guesses' the translation of extracted subsegments - hits.
- Total Recall in context improved to work for languages without a word separator.
- Fixed the synonym separator issue in the display of glossary entries.
- Fixed the Preferences panel display when the text in the “Characters for removal” field is long.

## 2016 Ichiro Update 7 (20160505)

The Ichiro update 7 offers the following:

- Updated list of supported languages for Google Translate, MyMemory MT and Microsoft Translator Machine Translation services.
- Fixed an minor issue with the filtering of AutoCad files on layers. The layer selection box did not pick for filtering the last layer in the list of layers.

## 2016 Ichiro Update 6 (20160422)

The Ichiro update 6 offers the following improvements:

- The alternative connection to Proz.com 6 term bases (KudoZ, KudoZ open glossary, Personal glossaries, GlossPost, Glossary-building KudoZ, Wikiwords). It can be activated and deactivated in the Project Dashboard via Proz.com web service check box. The selection of term bases for the search is done via the right-click at the Proz pane. By default, CafeTran searches all the term bases simultaneously.
- Added filtering on layers to the AutoCad source documents.
- Machine Translation services and Web services can be turned on/off directly in the Project Dashboard > Resources panel. They are also marked with different colors to distinguish them from the Web resources access via the internal web browser.
- The Project field, if activated in Preferences > Definitions, displays the name of the current project in the “New term” or “New fragment” dialogs.

## 2016 Ichiro Update 5 (20160411)

The Ichiro update 5 brings the improvements to the Match bar:

- The Match bar is now placed between the source and target segment pane for faster access.
- It wraps (folds) automatically when the number of matches is large.
- Hovering the mouse triggers the pop-up with matches for quick insertion into the target segment.

The update 5 also fixes the TMX file path issue in the TMX edit mode on the Linux system.

## 2016 Ichiro Update 4 (20160328)

he Ichiro update 4 brings the following improvements and changes:

- Optional fuzzy matching for fragments in Translation Memories. The function performs the look-up of word stems defined in Hunspell spell-check dictionaries.
- Searching Proz.com Term Questions.
- Export of all segments via the system clipboard in the Clipboard Workflow.
- Floating the match bar and search bar together and separately now.
- Automatic transfer of the selected text from web resource panes to the target window.
- Improved the eye-friendly green theme - Image background dark.
- Two new tab docking options which enable to dock tabs to the main window both vertically and horizontally - very useful and nice-looking in large monitors especially.
- The new Project > Replace document… function for the translation of another version of the source document.
- Fixed the drag and drop error on Mac OS X which appeared after updating to the latest Java 1.8.0_77 version.

A minor issue with the display of the pop-up matches has occurred in the latest update. When the main window is not maximized after clicking at the Match bar, the matches popped-up too far from the mouse click. It has been fixed now so please reinstall this update.

I also missed mentioning one new feature present in update 4 - the ability to replace the currently-translated document with its another version. See the menu Project > Replace document. For example, it may be useful when the client corrects something in the document and sends it to you again after you are half way with the translation of the previous version of the document.

## 2016 Ichiro Update 3 (20160317)

The Ichiro update 3 brings the following improvements and changes:

- Added Proz.com Term Search service as a resource.
- The working languages are put at the top of the language lists in the Project Dashboard.
- Correct language mapping in non-CafeTan xliff projects where there is no country code.
- Optional fuzzy matching with glossaries. The function performs the look-up of word stems defined in Hunspell spell-check dictionaries.
- Better integration of the following resources with CafeTran search function: Google Translate, Bing Translator, Proz Term Search, TM-Town, Linguee. The search in these web resources can be performed through the CT search box directly now.
- Fixed the Linguee web resource connection issue that made CafeTran crash.

The optional fuzzy matching did not change anything in the way the matching engine works. If CT does not get the match in the usual way, it falls back to fuzzy matching by comparing word stems. This feature can be turned off in Edit > Options > Glossary tab > Look up word stems box.

## 2016 Ichiro Update 2 (20160310)

The Ichiro update 2 has the following improvements and changes:

- Numbers which do not have a decimal separator are excluded from localized formatting.
- Fixed the look of the “QA - Check all” panel on Linux with dark GTK themes.
- Fixed the occasional freeze on Mac OS X when the user connected his/her laptop to a monitor.
- The status bar with icons for docked panels is kept showing when the user detaches segment windows.
- Direct access to TM-Town web interface (see Resources > Web > TM-Town.com).
- Direct access to Linguee web interface (see Resources > Web > Linguee).
- Automatic signing-in to web services (e.g. Google Translate, TM-Town) after restart of the program.
- Activate Google Translate and Bing Translator via the Resources > Web menu now. They are also displayed in the Project Dashboard in the Resources panel.

It looks like the CT crash with Linguee web resource on Mac is caused by an ad popping up at the Linguee page. The fix is in the works.

## 2016 Ichiro Update 1 (20160205)

The Ichiro update 1 has the following improvements and changes:

- maintaining the applied format during the transfer of the translated text via the system clipboard on Mac OSX.
- showing the information message when the loaded sdlxliff file is not prepared for the translation in CafeTran.
- detection of an error during the new project creation when the user sets the project location folder directly inside the source documents folder, which lead to the creation of multiply-nested folders.
- improvement of the Dashboard appearance (colors and buttons) under Linux GTK look and feel.
- more informative tooltips for the search buttons in the Search bar.

## 2016 Ichiro - 20160119

The Ichiro update improves the previous Harbinger version in the following aspects:

- localization of numbers during automatic propagation.
- access to linguee.com resources directly from CafeTran web resources interface.
- support for Crowdin xliff files.
- viewing alphabetically-sorted keyboard shortcuts in a web browser for easy reference and printing.
- simplifying the creation of new glossaries.

This 2016 version of CafeTran is the summary of all the improvements, changes and fixes made last year and in the recent preview version. All this would be impossible without your excellent feedback. Thanks a lot!

The display of synonyms in the glossary uses the html code <br> standing for the new line. Somehow, it slipped through my code checks and CT did not convert this <br> into newline. I’ve already fixed it in the last update file so it should be displayed fine now. Please download the update file again. Thanks for pointing it out!

The Ichiro version is updated with the following:

- The UTF-8 encoding header is added to the generated keyboard shortcuts html file.
- The currently-translated document can be exported individually even when in glue mode.
- Added the IATE web resource [http://iate.europa.eu](http://iate.europa.eu), English -> Polish as an example, to Resources > Web > Examples.
- Fixed an issue with the new web resource creation.

## Imported from previous ChangeLog (2013-07-01 - 2015-11-28)

The copyright on the CafeTran **ChangeLog** is shared by Michael Beijer
([Beijer.uk](http://beijer.uk/)) and Hans Lenting
([alinea.doc](http://www.niederlaendisch.nl/)) © 2013-2015.

**NOTE:**\
 CafeTran product version codes (See: *Help \> About*) consist of:\
(1) the date (in the same format as the entries below), and\
(2) a build number for that date.

e.g.: “Product Version: CafeTran Espresso **20141218**02”

Items in bold indicate important new features or important changes to existing features.

## 2016 Harbinger – 2015-11-28

1.  The new word/characters count in the Statistics function diplaying
    the speed of translation in CafeTran running session.
2.  The new option for subsegment matching called “Subsegment hits
    threshold” to reduce the display of low-quality subsegment matches.
    The default value is 3 which ensures the hits below this number are
    discarded.
3.  The machine translation panes get two new buttons to let the user
    transfer the MT translation to the target segment and repeat the
    query with the selected fragment in a more intuitive way.
4.  Localized formating of numbers can also take place when the numbers
    are inside parenthesis.
5.  The fix in the typing of accented characters in Portuguese on Mac OS
    X.

The problem with the automatic dragging in the grid was that the whole text got copied to the target segment pane when the user selected it across segments/cells. This caused some confusion. Now, I figured out how to limit the selected text to one cell/segment. So please perform the same Harbinger update again to have the previous dragging behavior back.

Hans L. reported the issue with the locked segments in SDLXLIFF files [https://cafetran.freshdesk.com/support/discussions/topics/6000022561?page=1](https://cafetran.freshdesk.com/support/discussions/topics/6000022561?page=1). It should be fixed now.

Wolfgang drew my attention to the subsegment matching during auto-assembling at CafeTranslators forum. His auto-assembling examples included several segments where their context was similar. In such a homogeneous context for subsegments in small translation memories, CafeTran may pick up a few candidates for correct target subsegments but very limited context across the segments does not let it find the most accurate pick. It may need some additional guidance to choose one BEST candidate for auto-assembling. I slightly modified the auto-assembling algorithm to better “discern” patterns in homogeneous contexts.

CafeTran Espresso 2016 Harbinger is updated with the following:

- Display of SDLXLIFF locked segments in the project segments pane.
- Searching for case-insensitive words catches all Unicode uppercase characters now (e.g. German umlauts).
- Displaying translation memory units via the right-click at the TM pane.
- Less distractive Translate and Transfer buttons in the Machine Translation panes.
- Speed optimization to subsegment matching algorithms. Longer German articles einer, einen, einem, eines are treated as stop words.

CafeTran Espresso 2016 Harbinger is being tuned for the final release soon. These are the latest changes,

- Selection of the working language pair in the Dashboard.
- More intuitive process of the creation of the new project - activation of the UI elements when they are actually needed.
- Reduction of the main interface buttons to the basic functions.
- The search bar is off by default now. It has a quick on/off access by the keyboard shortcut CTRL (Windows, Linux) or Command (Mac) + Shift + F).
- Fixed the removal of translation memories via the right-click in the Dashboard.
- Fixed the unnecessary “Save” pop-up dialog when the working memory comes from Total Recall.
- Fixed an issue with the format numbers option when the number started with “zero” digit.
- Remembering the state of the user interface after exit when there are multiple joined resources and floating panels.
- When the target language is Japanese, CafeTran displays the auto-completion panel at the top of the screen to prevent overlapping with the system auto-completion.

Please repeat the last update procedure described at the start of this threat.

The harbinger of CafeTran Espresso 2016 version is updated today (build 2015121801). The main changes are as follows:

1. Multilingual support for glossaries. The language pair is selected based on the current project language pair.
2. More intuitive grid-based display of glossary entries.
3. Search and replace for glossaries. By default, the language of the search is the source one. You can change it via the context menu.
4. Minor interface and terminology changes discussed on the forum and aimed at making CafeTran the intuitive tool.

I have updated the harbinger release of CafeTran Espresso 2016 (build 2015122001) taking into account your latest feedback as follows:

1. Added the alternative vertical display for multicolumn glossaries and narrow window layout. This option can be set by default in Edit > Options > Glossary tab and per session via the right-click at the glossary pane.
2. The new Search and Replace glossary worked only for the current session. Now, they are also stored in the glossary file.

Taking into account our recent discussions concerning the menus, I have made a few changes and uploaded the harbinger (preview) version of CafeTran 2016 (build 2016010401). If you wish to test it, please repeat the update procedure described in the first post in this forum thread.

Furthermore, I’ve added the following functionality to the auto-propagation feature:

- auto-propagation of segment with different numbers.
- auto-propagation of segments with different non-translatable fragments.

The two auto-propagation options are on by default and can be turned off in the new Auto-propagation tab (see Edit > Preferences > Auto-propagation tab).

Today I have uploaded one of the last updates before the official release of CafeTran Espresso 2016. The changes are as follows:

- Significant simplification of the menu interface. The menus with the power features can be activated/deactivated now when you need them in your workflow. See the View menu.
- The new Match bar can be floated (see the menu View > Toobars > Float Match bar). It can let translators use CafeTran resources and features while working in the other applications such MS Word, PowerPoint, Excel, etc.
- The results of auto-assembling (subsegments, terms, fuzzy matches) can be directed to the system clipboard. See the menu Edit > Preferences > Auto-assembling > Copy matches to clipboard.
- A new command in the menu Edit > Copy target segments to clipboard. When this option is activated, each target segment is copied to the system clipboard.

The update (build 2016010701) can be performed via the usual drag and drop with the same download file as described at the start of this thread.

Thank you for your feedback! It helps me refine the UI elements. The preview is available for testing with the following changes:

- Inclusive selection of the menus with advanced features.
- Renaming Pretranslation function to Preliminary memory matching.
- Project Glossary check box is back in the Project Configuration panel (for those who forget to check it in the Dashboard).

The update (build 2016010901) can be performed via the usual drag and drop with the same download file as described at the start of this thread.

## 2015 Update 12 – 2015-11-25

1.  Edition of multiple translation memories in the glue mode when selecting a folder with the translation memories.
2.  When localized formating numbers option is on, CafeTran retains the trailing zeros in the target number now.
3.  **New “Automatic update of project statistics” option** (see the menu Project \> Statistics \> Automatic update of project statistics). After turning this option on, you should also notice the second progress bar which displays the actual character-based progress in your translation.
4.  The fix in the display of Japanese fonts in the Quick term editor.

## 2015 Update 12 – 2015-11-17

1.  Joining a translation memory to another opened translation memory is back. See the Memory \> Join memory.. menu.
2.  Listing of the web resources is in the alphabetic order in the Dashboard.
3.  Nicer and clearer display of the workflow tips in the Dashboard.

## 2015 Update 11 - 2015-11-09

- **\#1.** Import of multiple documents from nested folders (subfolders).
- **\#2.** Optional filtering on a file name/extension during multiple documents import.
- **\#3.** Bilingual export columns have the correct language set for each column to be recognized by Ms Word spell checker.
- **\#4.** Auto-propagation works across multiple xliff-based projects (.xlf .sdlxliff .mqxliff) now.
- **\#5.** Conversion of TXT glossaries to TMX format can handle the synonyms both on the source and target side.
- **\#6.** Switch to OS-native file choosers for memories, glossaries and other resources selection.
- **\#7.** A new term is added to the match results for the current segment making it accessible instantly via the double SHIFT shortcut or the F2 button.

## 2015 Update 10 - Icons with Colours (2015-11-02)

- **\#1.** New coloured icons. The user can switch between colored and monochromatic icons via the menu View \> Appearance \> Monochromatic icons.
- **\#2.** Display of highlighted and colored text in the Project segments pane for the Ms Office and LibreOffice documents.
- **\#3.** Filtering on the highlighted or colored text.
- **\#4.** After the export of the target document, CafeTran gives the option to either view the translated document or open the folder containing the document.
- **\#5.** Conversion of TXT glossaries to TMX format handles the synonyms now.
- **\#6.** New arrangement of icons in context menu.

## 2015 Update 9 - Icons for High Resolution Screens (2015-10-22)

- **\#1.** New icons for high resolution screens. The user can switch between small and large icons via the menu **View \> Appearance \> Large icons**.
- **\#2.** Fixing the issue that prevented typing some diacritical marks with the SHIFT key pressed.
- **\#3.** Fixing the issue with the + character in the file name at drag and drop on Mac OSX.
- **\#4.** Adding the option to hide the highlighting of memory or glossary hits in the source segment pane separately.

## 2015 Update 8 - Introducing the Match Bar (2015-10-22)

- **\#1.** New **Match bar**. Can be hidden using **View \> Hide match bar**.
- **\#2.** **Reversed suggestion of fragments/terms in the target segment pane** – triggered by pressing Shift key twice and the first letter of the source term in the target segment pane.
- **\#3.** Transfer current tag (Alt+9 shortcut) now works on a selection the same way as mouse tag placement. Meaning, it is now possible to wrap a selection in tags with a keyboard shortcut or voice command!
- **\#4.** New option in **Appearance \> View \> Colors** menu: "Hide match colors in the source segment". This allows you to switch off all highlighting in the source pane, if you prefer a cleaner workspace where you can focus only in the text.
- **\#5.** Suppressing soft hyphens tags when importing MS Word documents.
- **\#6.** Automatic creations of alternative translations during the bilingual import of the reviewed documents to compare the reviewed version and the original version of the segment and to filter out the reviewed changes. Meaning: it should now be possible to quickly identity any segments changed (in the bilingual review tables) by your proofreader/editor.
- **2015-10-22** \#7. Minor interface changes to enable more intuitive location of the most frequently used buttons/actions both for new users and touch screen users.
- **\#8.** Improved the selection of terms in source and target segment panes (e.g. prior to adding a selected term pair to your glossary or memory). If you select a piece of text in the source pane, and then its corresponding translation in the target pane, both are highlighted simultaneously and remain highlighted.

## 2015 Update 7 (2015-10-13)

- **\#1.** Added an option to set the occurrence threshold for contextual hits in autoassembling .
- **\#2.** Automatic adjustment of spaces function takes brackets and inverted commas into account.
- **\#3.** Rearrangement of some icons in the user interface to have a more intuitive access to them.
- **\#4.** Improved error handling during the launch. CafeTran should report an error and recover from this situation by itself. Previously, the user had to reset to the default settings manually to be able to launch again properly.
- **\#5.** Larger checkbox texts in the Project Dashboard to have them legible in the high resolution screens.
- **\#6.** If the source segments can be edited, the title of the source segment pane is red.
- **\#7.** Implemented native full screen support on Mac OSX.
- **\#8.** Automatic refresh of the glossary when the source term is modified/edited in Quick Term editor.
- **\#9.** Previous change (see: ‘**2015-07-30** Glossary fields are displayed in italics to distinguish the fields from the terms better.’ below) has been removed.

## 2015 Update 6 (2015-09-18)

- **\#1.** Implementation of **"Segments patterns"** function.
- **\#2.** Improvements in the accuracy of the “Subsegment matching” engine to propose the right translation for the subsegment.
- **\#3.** More distinct (bold and larger fonts) titled borders in the Project Dashboard on Windows.
- **\#4.** The “New project” button in the Dashboard opens the file chooser to select the source document right away after the click.
- **\#5.** All the search buttons in the main interface are placed in the Search bar now to have a more intuitive and faster access to them.
- **\#6.** All sections (panes) of the main interface have **titled borders** that describe their purpose. This makes the interface more intuitive for new users.
- **\#7.** Docked panes have **titled borders** with the name of the docked resource.
- **\#8.** **Individual glossaries and translation memories can be kept out of auto-assembling** by choosing the option after the right-click at their pane.
- **\#9.** The background grid (horizontal lines in the editor) is not a default option now so you may need to re-apply your favorite theme again in the menu View \> Appearance \> Themes \>… to notice the change. If you don’t do it, your current UI settings will still show the grid. The grid can be turned on/off by clicking View \> Appearance \> Themes \> Background grid submenu.
- **\#10.** **DEFAULT THEME CHANGED**: default toolbar colours changed from orange to green. If you preferred the old default toolbar colour (as I do) to the new light green one, go to: **View \> Appearance \> Colors \> Toolbars color**, and change the RGB colour to: ’EDD5A6’.

## 2015 Previous updates

- **2015-09-01** Fixed a file drag and drop issue on Mac OS X which caused the freeze of the Project Configuration panel. The issue appeared after updating Java to 1.8.0\_60 version.
- **2015-09-01** When opening a TMX file via the **Memory \> Open memory…** menu, the memory options stored in the TMX file are correctly replaced now with user’s options selected in the TM options panel.
- **2015-08-08** Help texts connected to the tooltips of Mac OSX menus.
- **2015-08-08** QA translation consistency check for TMX translation memories.
- **2015-08-08** Import of Bitext files to the translation memory.
- **2015-07-30** Added the possibility to remove external xliff (e.g. sdlxliff) files from the project.
- **2015-07-30** Improved handling of references to chapter titles in MIF filter.
- **2015-07-30** Automatic addition of spaces after periods during Export when translating Japanese and Chinese documents.
- **2015-07-30** Mapping of CafeTran’s “Checked” status to Studio’s “Translated” status. Meaning: you can now use CT’s Checked status (segments get highlighted when confirmed) when translating SDL Studio files.
- **2015-07-30** “Checked” status can be set for TMX segments in TMX Edit mode to make filtering on the status and jumping over it possible.
- **2015-07-30** Removal of deprecated parts of TM-Town APIs.
- **2015-07-30** Display of TM-Town documents just after linking with CafeTran for the first time.
- **2015-07-30** Segmentation issue when the source document started with blank characters such as white spaces: Fixed.
- **2015-07-30** Glossary fields are displayed in italics to distinguish the fields from the terms better.
- **2015-07-30** Added help texts for menu items.
- **2015-07-30** New Tags menu (**Translation \> Tags**) to group all tag-related actions.
- **2015-07-30** Integration of the PDF viewer component with CafeTran (see the **Tools \> PDF viewer** menu).
- **2015-07-30** QA’ed units can be saved for external HTML viewing.
- **2015-07-13** Formatting of the source segment is displayed in the source segment pane.
- **2015-07-13** Terms cache is updated automatically after editing a term in the Quick Term editor, so the updated term is used correctly during Auto-assembling.
- **2015-07-13** Mouse tag placement toggle button has been added to the target segment toolbar. It enables fast transfer of formatting (e.g. bold, italics, underline) with a single mouse click or selection.
- **2015-07-13** Two new options to let users handle formatting tags: “**Hide/Show segment boundary tags**” and “**Merge adjacent tags**”. See the **Translation \> Transfer** menu.
- **2015-07-13** Filtered translation units can now be saved in the bilingual HTML file for external viewing/printing. See the **Project \> Convert project \> To HTML file…** menu item.
- **2015-07-11** New tab in Project Dashboard: “TM-Town Resources” (next to “Local Resources” tab), allowing you to now connect online TMs/TBs to your local CT project (you have to enable TM-Town in **Edit \> Options \> Web services**).
- **2015-07-11** **Automatic adjustment of spacing during drag and drop in the target segment pane.** (needs to be enabled in **Edit \> Target segment \> Adjust word spacing**).
- **2015-07-11** Auto-propagation issue in memoQ xliff files: Fixed.
- **2015-07-11** CafeTran will now display helpful text in the status bar, when hovering over icons.
- **2015-06-30** Two new icons for searching a selection in the Source segment pane
- **2015-06-30** The Funnel icon and the Export icon above the grid have switched places. Because you will be using the Funnel icon more often than the export icon (the distance with the mouse from the Target segment pane to the new location of the funnel is shorter). Ergonomics.
- **2015-06-30** Simplification of the *Project Dashboard* by elimination of a separate category for TMX glossaries there. Since CT stores TMX settings in the TMX file, there is no need to indicate what the TMX file actually holds in the UI. There is now one category for Translation Memories which can hold whatever you like (full segments and/or fragments/phrases/terms) and one for Glossaries.
- **2015-06-30** **You can now upload your TMs and glossaries to TM-Town web service.** This is interesting because then you will be able to search them both manually and automatically from CT via the Lucene search engine that TM-Town uses for searching.
- **2015-06-30** Change of some names in the *Total Recall* menus.
- **2015-06-24** Changed the encoding of exported Transit language pair files from UTF-16 to UTF-16 Little Endian.
- **2015-06-23** “Open html page for source preview…” + “Open website for source preview…” moved from **Tools \> Web browser** to **Tools**.
- **2015-06-22** You can now change the colours of toolbars in non-transparent themes. See *View* \> *Appearance* \> *Colors* \> *Toolbars color*.
- **2015-06-22** **Added an option to the Auto-assembling feature to switch the priority between glossaries and memories** (see the menu *Edit* \> *Option* \> *Auto-assembling* tab).
- **2015-06-13** When closing CafeTran, a confirmation dialogue box is displayed.
- **2015-06-13** The Web browser menu has four new items: *Open html page for source review*, *Open website for source preview*, *Google Translate* and *Bing Translator*. **It is now possible to have a synced HTML preview file of your translation projects!**
- **2015-06-13** The Web browser menu has been moved to the Tools menu.
- **2015-06-03** The Open third-party XLIFF folder icon in the Dashboard (top right) now has a checkbox to open a folder with XLIFF files.
- **2015-06-03** Automatic target language setting for exported MS Word documents
- **2015-06-01** TM settings for TMs loaded via the Dashboard now stick. TM settings are stored in the header of the TMX. be careful when editing TMXs in an external TMX editor.
- **2015-05-26** New arrangement of the Dashboard for more intuitive use.
- **2015-05-26** New layout of the GUI for more intuitive use.
- **2015-05-26** New licensing system: CafeTran now uses a license file.
- **2015-05-08** New and secret feature that still needs some testing.
- **2015-05-04** Some improvements to mqxliff handling - improved term recognition and QA spelling of tagged segments.

## CafeTran Espresso 2015

- **2015-04-22** **CafeTran Espresso 2015 was released.**
- **2015-04-22** A new company, Collaborative Translation Networks LLC, is mentioned on the new CafeTran website.
- **2015-04-22** [New CafeTran site](http://www.cafetran.com/) was launched.

## Gandalf (Released on 1 January 2014)

- **2015-03-29** Keyboard shortcut to call/update the Projects Statistics (Control+E). Note that you can make this Statistics pane floating, position it on a secondary screen and regularly update it to keep an eye on your progression. Most stimulating!
- **2015-03-29** Keyboard shortcut to repeat the last QA (Control+L)
- **2015-03-29** Popup gets in the way when you try to click into a glossary entry. Fixed.
- **2015-03-29** CafeTran can now handle memoQ and Studio comments!
- **2015-03-27** The latest version allows to convert only filtered Project segments (e.g. checked only) to TMX via the Project \> Convert Project \> To TMX Memory…
- **2015-03-20** SDL projects: locked segments are locked in CafeTran too now. Also valid for MQXLIFF?
- **2015-03-20** Statistics pane is now positioned in the tabbed pane.
- **2015-03-20** Added colourful labels to MT engines in tabbed pane, visible on first start.
- **2015-03-12** Issue when recalling segments from Total Recall to memory. Segments containing an apostrophe character caused recall to fail. CafeTran didn’t escape the character properly as it is reserved for SQL commands. Fixed.
- **2015-03-10** Fix for Tags autopropagation issue in SDLXLIFF projects. It should fix the similar issue in MQXLIFF files.
- **2015-03-09** Support for Thai language as a language for Hunspell.
- **2015-03-07** Improvements to the Total Recall pane (it is now wider and makes use of all horizontal space).
- **2015-03-07** **Support for Java 8 on Mac.** Now we can use real File Open/Save dialogue boxes! [Watch a video](http://youtu.be/Uw9SW91G6iE) (For the time being, only the file chooser in the Project Configuration dialogue box – the other file choosers will be migrated later this year.)
- **2015-03-07** **SQLite backed Total Recall system for huge TMs.**
- **2015-03-06** Good news for users of a second screen: New tab detaching feature (called Float) when right-clicking at the tab. You can now position any resources on your second screen! [Watch a video](http://youtu.be/pB_x_qk4DIY)
- **2015-02-28** The segment number in the grid is centred vertically in the cell now to locate and click it easier.
- **2015-02-28** Segment notes and Alternative Translations can be access directly from the grid via a mouse click.
- **2015-02-28** Creation date for TMX translation units is now displayed in human readable format in CafeTran’s interface.
- **2015-02-28** Added progress bar when deleting a table from the Total Recall database.5. Improved display of QA translation units in the grid.
- **2015-02-28** Implementation of the QA tasks for TMX memories in TMX edit mode: (1) Check spelling in target segments; (2) Tags check; (3) Leading and trailing spaces check; (4) Brackets check; (5) Double spaces check; (6) At tags spaces check; (7) Numbers check; (8) Empty segments check; (9) Target the same as source check; (10) End punctuation check; (11) Initial capitalization check; (12) Double words check
- **2015-02-28** Implementation of Statistics function for single documents in multi-document project (see the new menu item Project \> Statistics \> Current Document Statistics)
- **2015-02-03** Tracked down and solved an issue that could prevent reimport of translated MQXLIFF files in memoQ. Thank you, Igor!
- **2015-01-30** Further improvement to the handling of MQXLIFF projects. All EMs and CMs are now inserted during Translation \> Insert all matches.
- **2015-01-28** Improved the handling of tags inside words in MQXLIFF projects.
- **2015-01-28** Improved the QA of tags in MQXLIFF projects.
- **2015-01-21** New feature: **Tools \> Abbreviations \> Scan Project for abbreviations**. CafeTran will list abbreviation candidates in the tabbed pane. Pressing button in list of candidates adds the relevant abbr. to the Abbreviations file (see 2015-01-20.1). Any one, two or three letter string + . is a candidate for the abbrs. list. See: [http://cafetran.wikidot.com/abbreviations](http://cafetran.wikidot.com/abbreviations)
- **2015-01-20.2** **"Dynamic segmentation"**: CafeTran now auto-joins segments at any next occurrence of an abbreviation added via **Tools \> Abbreviations \> Add selection to abbreviations** (i.e., whole project is not re-segmented).
- **2015-01-20.1** New features under **Tools \> Abbreviations**. CafeTran auto-creates a simple abbreviations text file for the given source language (on Windows @ …\\CafeTran\\cafetran\\resources\\abbreviations\\abbreviations-nl\_NL.txt, on Mac @ /Applications/CafeTran.app/Contents/Resources/Java/resources/abbreviations/abbreviations-de\_DE.txt). These abbreviations lists can work independently or in tandem with the segmentation rules. New abbreviations can be added via **Tools \> Abbreviations \> Add selection to abbreviations (Ctrl+Shift+B)**. Abbreviations added to the abbr. list (via **Tools \> Abbreviations \> Add selection to abbreviations** or **Tools \> Abbreviations \> Scan Project for abbreviations** and clicking on a button) work the same as items added to the segmentation rules (with a no break instruction). That is, CafeTran will not break the text at this abbr. in the future. In contrast to single-word abbreviations (Any one, two or three letter string + . is a candidate for the abbrs. list), multi-word abbreviations won’t trigger the new automatic segment joining mechanism and will only work in the segmentation phase of a new project.
- **2015-01-18** **Generate a list with all words with unknown spelling** via *Task* \> *List words with unknown spelling*. See: [http://cafetran.wikidot.com/listing-words-with-unknown-spelling](http://cafetran.wikidot.com/listing-words-with-unknown-spelling)
- **2015-01-15** The *Project Info* dialogue box is now called *Project Configuration*. Changed the default project location on Windows to the Documents folder. Also, there is a new field called Project Folder in the Project Configuration panel where the user can see the exact folder of her Project. It is updated as you type the name of the new Project.
- **2015-01-12** CafeTran introduces: Super Simple Follow-up Project Creation: If you reuse the project folder for the new project, CafeTran notices existing ProjectTM.tmx and ProjectTerms.txt in that folder and loads them.
- **2015-01-12** Dashboard has been optimised so that from LTR all settings are made in a logical, intuitive way and the D&D area is available at the right-hand side, which is nice if CafeTran isn’t maximised, since you then can D&D easily from the Desktop. New layout, the number of the Dashboard buttons has been reduced to the absolute minimum. New button labels.
- **2015-01-06** Added two alternative buttons in the Dashboard to quickly start a project.
- **2015-01-06** The status box of the grid went to the right-hand side.
- **2015-01-05** Adding Notes and Alternative translations broken: Fixed.
- **2015-01-04** First time you press Alt+down when starting a project doesn’t work: Fixed.
- **2015-01-04** Pop-up window issue with read-only TMs (reported by Will): Fixed.
- **2015-01-03** Added an option to extract frequent word from the current segment (in real time translation) to the Task \> FW menu.
- **2015-01-03** You can change where to add FWs (TMs or glossaries) via the Task \> FW menu.
- **2015-01-03** It was impossible to switch off the new ‘Automatic insertion of MT in target segments’ (right-click in MT pane) feature without restarting CafeTran. Fixed.
- **2015-01-03** Unicode sequences like \\U200b are removed from the MT results.
- **2015-01-03** Right-click at the MT online service pane to create a TMX memory in one pass (select “Create TMX Memory”). See: [http://cafetran.wikidot.com/using-machine-translation](http://cafetran.wikidot.com/using-machine-translation)
- **2015-01-03** Right-click at the MT online service pane to toggle automatic insertion of MT results into the TL segment pane. See: [http://cafetran.wikidot.com/using-machine-translation](http://cafetran.wikidot.com/using-machine-translation)
- **2015-01-03** Frequent Words got a new option to show only unknown FW (see the menu Task). Here, only the FWs are displayed that are not present in TMs and glossaries. See: [http://cafetran.wikidot.com/extracting-frequent-words](http://cafetran.wikidot.com/extracting-frequent-words)
- **2014-12-23** Propagated status is now shown (together with the other statuses) in the box between the src/trgt boxes in the grid. Previously, it was shown as a note.
- **2014-12-23** Problem with fuzzy match word counts when running Statistics: Fixed.
- **2014-12-22** CafeTran now handles hidden individual cells in Excel: [http://cafetran.wikidot.com/translating-excel-files-with-hidden-cells-or-ranges](http://cafetran.wikidot.com/translating-excel-files-with-hidden-cells-or-ranges)
- **2014-12-22** You can now import MS Excel files into a Glossary (**Glossary \> Import MS Excel glossary…**): [http://cafetran.wikidot.com/importing-an-excel-file-into-a-glossary](http://cafetran.wikidot.com/importing-an-excel-file-into-a-glossary)
- **2014-12-22** You can now import MS Excel files into a TMX Memory (**Memory \> Import \> Import MS Excel memory…**). See: [http://cafetran.wikidot.com/importing-an-excel-file-into-a-tm](http://cafetran.wikidot.com/importing-an-excel-file-into-a-tm)
- **2014-12-22** Small changes to the display in the grid: (1) The word “propagated” no longer appears as pink highlighted text; it is now a small red “P”. (2) Grey shading to indicate a checked segment is back to covering the entire segment again (was temporarily changed to cover only the new box in between src + trgt boxes in the grid).
- **2014-12-21** Coffee cup undock icons changed to new Glossary icons. Old Coffee cup undock icons still apply for TMX termbases.
- **2014-12-19** “Library” menu renamed “Tools”.
- **2014-12-19** New (combined) “Memory & Glossary” tab in **Project Info** dialogue. Project memories (or Project Glossaries) are no longer preselected in this tab. They can now be selected in the Dashboard, at the top of the “Translation Memories” and “TMX Termbases & Glossaries” tabs.
- **2014-12-19** **Edit \> Copy source segments to clipboard** is now sticky (i.e., it survives restarts).
- **2014-12-19** **Edit \> Options \> Window** has been removed as it is no longer needed: **CafeTran now remembers all window positions on a restart!!!**
- **2014-12-19** Problem in Excel filter where CafeTran did not recognise multi-lined cells: Fixed. See: [https://groups.google.com/forum/\#!topic/cafetranslators/i4J1yA7KSXM](https://groups.google.com/forum/#!topic/cafetranslators/i4J1yA7KSXM)
- **2014-12-19** Some cool UI changes. Mainly, improvements of the grid display and some changes to the Dashboard as well.
- **2014-12-19** Resources (translation memories, TMX termbases, glossaries) that were previously selected in the Dashboard will be selected on a restart.
- **2014-12-19** Various changes to Dashboard: Start/Open buttons now at far right, to be clicked after you have set everything moving from left to right in the Dashboard.
- **2014-12-11** Removing a document from the project now deletes it from the project folder
- **2014-12-11** “Project” section moved from centre to far left in new integrated Dashboard
- **2014-12-09** Glue issue mentioned in the Google Group: Fixed.
- **2014-12-08** More improvements made to the *Dashboard* (formerly known as *Project Manager*): (1) “Termbases & Glossaries” changed to “TMX Termbases & Glossaries”; (2) Green check mark icons changed to check boxes (which now select/de-select all); (3) Book icon changed + something else in the Project section; (4) New *Translation Memory* icon + New *(TMX) Termbase* icon.
- **2014-12-08** New Glossaries icon
- **2014-12-06** Important improvements to the new integrated Project Manager.
- **2014-12-04** **Project Manager integrated into the main UI** (first preview of CafeTran 2015).
- **2014-12-04** Improvements to the OCR Word filter
- **2014-12-04** Excel import problem fixed: Fixed.
- **2014-12-01** New: **Filter \> Display current segment in context** … being shown the previous and next segment (“context”) when running a QA routine is useful when working with alternative translations, but if you’re not, they often get in the way. You can now switch this off using the aforementioned switch.
- **2014-11-28** **New Excel filter: See the *Filter options* tab in the *Project Info* dialogue box after you added an Excel document.** Here you can set which columns to translate and (optionally) where the translation should be inserted. You can also specify which column should be loaded into the Source Language column of the grid and which one into the Target language column. See: [http://cafetran.wikidot.com/translating-multilingual-excel-files](http://cafetran.wikidot.com/translating-multilingual-excel-files) and [http://cafetran.wikidot.com/translating-excel-files-with-hidden-content](http://cafetran.wikidot.com/translating-excel-files-with-hidden-content)
- **2014-11-14** All the stuff related to Text shortcuts + Non-translatable fragments has been moved into the Library menu. Text shortcuts stuff was formerly in the Edit menu. Non-translatable fragments stuff was formerly in the Translation menu.
- **2014-11-13** Improvement of the IDML filter. CafeTran now should skip the hidden layers from import. To be tested.
- **2014-11-11** **Now CafeTran can deal with those pesky internal padlocks in Studio XLIFF projects. Note that these special tags cannot be deleted in CafeTran.**
- **2014-11-04** Fix for the resetting issue: CafeTran could lose its settings in rare occasions.
- **2014-11-04** (probably much earlier, though) When performing a QA for trailing punctuation marks/spaces, corrections now are propagated. Make sure to re-filter during QA regularly, to profit from this.
- **2014-11-04** Intruding black lines in tabbed pane are now decent dark grey. (Beautiful black lines in tabbed pane are now dark grey, which messes up Michael’s formerly perfect black & white UI.) If you want to match the lines in the tabbed pane with the borders of the other panes, choose background colour Steel in the Themes. Choose Aluminium for a less distracting grey that still matches the new grey lines.
- **2014-11-04** Subsegment guessing (HITS) has been further refined. The “HITS” are coloured depending on accuracy of a guess. *Blue*: only one hit (CafeTran shows the full target segment - no guess); *Orange*: from 2 hits to 7 (7 is the default setting (set in Options) for treating the hit as the exact fragment - e.g. in Autoassembling); *Purple*: more than 7 hits (here the guess should be quite accurate).
- **2014-11-01** **New menu Task \> Transfer non-translatable segments to target.** Now it is possible to skip segments that only contain non-translatables: which, depending on your document type can be a HUGE time saver. See [Non-translatables](http://cafetran.wikidot.com/working-with-placeables).
- **2014-10-29** CafeTran can now load multiple .txt/.csv glossaries from a single folder simultaneously, just like was already possible with TMX files. CafeTran automatically sets these glossaries to read-only. As you set the path to your glossary, point to the folder with your glossaries (instead of a file).
- **2014-10-26** **CafeTran is one of the few CAT tools with a Settings Backup feature! It is now possible to export/import your settings.** (see Options panel).
- **2014-10-26** Total Recall for all tables in one go (as an option).
- **2014-10-26** It is now possible to import a folder containing multiple TMXs into a Total Recall db. CafeTran will import all files in the folder with the .tmx extension, ignoring other files.
- **2014-10-25** Spell checker issues with language-specific custom dictionaries: fixed.
- **2014-10-24** CafeTran was mistakenly automatically joining the Segments + Phrases TMXs (if selected in the **Memories** section in the Project Manager). This has been fixed so it is the two MTs (not TMs) that are now automatically joined.
- **2014-10-21** Navigating to the Start/End of non-translatables list and user.dic is now possible with keyboard shortcuts, like in almost any editor. Saving via disk button is enabled??
- **2014-10-20** New, streamlined Project Manager. TMs & TBs are now set in the Project Info dialogue box.
- **2014-10-14** Deleting existing tables from Total Recall did not remove underlying index. Fixed.
- **2014-10-10** **Revamped F2 system**: it is now **alphabetical** (and thus much more intuitive).
- **2014-10-10** TMX property (Client) wasn’t being imported into Total Recall databases. Fixed.
- **2014-10-09** **New, smarter database access system. It is called ‘Total Recall’** and it is currently based on the H2 database. The idea is to recall from Database to Memory only segments in the Project context to avoid loading all huge data to RAM. Please see the “Total Recall” menu. See also new Recall segments… and Recall phrases… submenus. See: [http://cafetran.wikidot.com/total-recall](http://cafetran.wikidot.com/total-recall)
- **2014-10-??** Something changed with SmartArt graphics handling (check!)
- **2014-10-??** Something changed re: PowerPoint handling (check!)
- **2014-10-06** Different languages now have different custom dictionaries: [http://cafetran.wikidot.com/installing-the-hunspell-spell-checker](http://cafetran.wikidot.com/installing-the-hunspell-spell-checker)
- **2014-09-29** Issue where certain TM properties would cause problems with the AA panel (prevent it from appearing) and auto-insertion (stop it from working): Fixed.
- **2014-09-29** Significant performance improvements in the H2 SQL database. New indexing system; existing tables won’t work. You need to delete the existing tables. Next, create a new table and import your data again. On an i3 laptop it takes 2-3 seconds to complete a search in 1.5 million TUs.
- **2014-09-25** Small fix so it is no longer necessary to put a backslash in front of target entries containing regexes for numbers. ‘|\\d+€ **\\t** €000’ now works instead of ’|\\d+€ **\\t** \\€000’
- **2014-09-22** You can now drag & drop a file or folder onto the Project Manager and Project name, Project location and Document fields will be filled in automatically. File type is also automatically selected based on file extensions.
- **2014-09-14** Small changes to the border line colours when transparent themes are used.
- **2014-09-14** More intuitive Project conversion menu (see *Project \> Convert Project* menu)
- **2014-09-14** Installation of spell checking dictionaries directly from CafeTran interface (see the menu *Edit \> Spell checker \> Install Dictionary*) See: [http://cafetran.wikidot.com/installing-the-hunspell-spell-checker](http://cafetran.wikidot.com/installing-the-hunspell-spell-checker)
- **2014-09-10** New update mechanism: update CafeTran via Help \> About panel \> Install update button.
- **2014-09-10** New feature: **‘Filter with context’**. When you filter something, CafeTran now displays the segment’s previous and next segment in the Grid too, to provide you with a little more context. This applies to all of the filters available from the *Filter* menu, but also to the QA routines. For example, if you press *QA \> Double spaces check*, you will now be shown all segments with a double space (like before), but each time you click into a specific segment, its previous and next segment will also be shown (i.e., its context).
- **2014-09-09** More memoq tags processed by CafeTran
- **2014-09-08** Creating an Alternative Translation (AT) for a segment blocks it from being auto-propagated. No changes will be propagated to and from this segment.
- **2014-09-06** Keyboard shortcut for 'Reload glossary' has been added (see menu for the default setting: Ctrl+Shift+L).
- **2014-09-05** New filter: *Filter \> Alternative translations*. Shows all segments that contain Alternative Translations (ATs). When you are finished with a project: temporarily de-activate ‘Auto-propagation to other segments’ + ‘Auto-propagation to current segment’ (under Translation \> Options \>) and use this filter to check that all your segments containing ATs are correct. Remember to re-activate auto-propagation when you are done!
- **2014-09-05** Alternative Translations (ATs) are now highlighted yellow in the Grid, so segments that contain ATs stand out better.
- **2014-09-04** Handling of certain tags in memoQ XLIFF improved: they don’t hinder term recognition anymore.
- **2014-09-04** New filter for OCR files called Ms Word OCR. It suppresses some unnecessary tags.
- **2014-08-25** *Term match* and *Term match font* colour have been added. Now CafeTran can show in the translation editor (source segment box) which terms from your glossary (and probably TM4terms) have been recognised. Previously it was only possible to see segments and subsegments indicated by colours.
- **2014-08-25** If only one selection is made in the *New Term* dialogue box, the other language entry is added completely. Saves one selection to make.
- **2014-08-21** Improvement of the case toggling feature (Ctrl+=): Now it is possible to toggle X.Y. at the start of a segment to x.y. or X.y.
- **2014-08-20** Further improvements to the SDLXLIFF filter (regarding empty segments and better treatment of EXT LINK tags, they now no longer hinder term recognition, nor do they cause false positives in QA spell-checking).
- **2014-08-20** New Replace & Edit function in F&R dialogue box. ‘Replace & Edit creates a special filtered workflow where on each next segment the find phrase is automatically replaced with the replace phrase. At the same time, it is editing your replacement after each next segment.’ (Igor) **This means:** First you press Find, then R&E and the first occurrence of the Find string is replaced in the filtered view. When you press the Add/Next segment button/shortcut and move to the next filtered segment, the next occurrence is replaced, etc. This way you can cycle through the filtered view. I don’t know how to skip a single occurrence in the filtered view…
- **2014-08-20** Joining segments in CafeTran projects is improved (already translated part of a segment will stay translated when joining, auto-assembling is only used for the “new”, joined part).
- **2014-08-10** Accurate extracting of terms and phrases from TMs. Settings for the TM = Fuzzy and Hits turned on. Please lower Subsegment to Auto threshold to 2 (Edit \> Options \> Memory tab). Look for HITS results in the TM tab.
- **2014-08-07** Thin grey lines added between joined resources in tabbed pane and between docked resources to improve visual clarity of the UI.
- **2014-07-28** *Appearance* and *Font* menu items have been moved to the new *View* menu too.
- **2014-07-24** Some menu names have been made more consistent with other apps/user’s expectations: *Window* is now called *View* and the old View menu has been renamed to Filter. Also the term “Pane” is now used in the View menu now (instead of “Window”).
- **2014-07-24** For third-party XLIFF projects the PM buttons now take the name of the folder instead the name of the XLIFF file. Handy for cooperation with clients that always use the same name for their XLIFF files, e.g. because of the CMS system they use.
- **2014-07-16** New Glossary switch ‘Stop automatic matching’ available via right-click in Glossary pane.
- **2014-07-16** *Project \> Statistics* works with Views and Filters too now. Previously, running Statistics on your project included ALL segments, even if you had applied a View (e.g., *View \> Unchecked segments*) prior to running it. Now, if you select *View \> Unchecked segments*, and run Statistics, only segments whose status is ‘Unchecked’ will be counted. This is very handy for proofreading, where all segments might be translated, but you would like to know how much you have left to check.
- **2014-07-16** New ‘Copy for activation’ under *Help \> About*, which copies all the info Igor needs to activate your copy of CafeTran to your clipboard.
- **2014-07-12** New keyboard shortcut: Window \> Segment windows \> Request focus in target segment window CTRL+SHIFT+F12, important for automation with AutoHotkey (Windows) or Keyboard Maestro (Mac), works in the translation editor, the Add term dialogue, Quick Term Editor and in the Find and Replace dialogue.
- **2014-07-11** *Project \> Statistics \> Total statistics* now also shows word counts in TM fuzzy matches (previously it only showed percentages).
- **2014-07-01** Keyboard shortcuts can now be disabled in E*dit \> Options \> Keyboard shortcuts*, click on a keyboard shortcut and choose, er, ‘Disable’.
- **2014-07-01** Notes are now also shown in the Grid when filtering on certain words or phrases in your project. By ‘filtering’ I mean, using one of these shortcuts: ‘Project Source Segments’ or ‘Project Target Segments’ to display all segments containing your selection in the Grid. You can also filter from the Find and Replace dialogue (Ctrl+F), by entering some text in the Find box and clicking ‘Project Source Segments’ or ‘Project Target Segments’.
- **2014-07-01** Transit files are now exported without an underscore character being inserted before the dot. See: [http://cafetran.wikidot.com/transit](http://cafetran.wikidot.com/transit)
- **2014-07-01** Regarding the target box focus issue, Igor changed F12 (cycling focus key) so that if the focus is anywhere outside the target box, F12 brings it back to the target box. This is both handy for translators that are afraid of mice (like M.Beijer) and for automation (now we have a keyboard shortcut to place the caret directly in the target language box of the translation editor, the Find and Replace dialogue, the New Term dialogue and the Quick Term Editor.
- **2014-06-30** Changes to MT search functionality: **(1)** New ’R2’ button in the pop-up search toolbar. (R1 = Resource (Web, Glossary) / R2 = MT Services) **(2)** New shortcut in the menu *Edit \> Find at cursor*: ‘MT Services’. That is, it is now even easier to select a bit of text and send it to an online MT engine.
- **2014-06-30** New **font zooming shortcuts** (for text in the Translation Editor) @ *Edit \> Font*: Zoom +/Zoom −
- **2014-06-21** Pretranslation error caused by a source segment containing only one punctuation character. Fixed
- **2014-06-20** Recent projects can now be removed from the ‘Recent projects’ section in the Project Manager by right-clicking at the project name in the PM and selecting ‘Remove’.
- **2014-06-14** Now you can pause MT by right-clicking ‘Stop automatic MT service’ in the MT pane. This can be useful for when you are reviewing your translation. This setting is sticky and will be remembered between sessions. So now you can enable MT only for the segments [where you need some inspiration or can expect good results](http://cafetran.wikidot.com/using-machine-translation).
- **2014-05-28** New ‘Translate’ context menu. Select a word in the source segment box, and then right-click in the tabbed pane over one of the MT sections and select ‘Translate’ to translate your selection with one of the activated online MT engines.
- **2014-05-28** New task: *Task \> Replace TMX internal tags with space*. This replaces the internal tags in TMX segments with spaces and clears any resulting double spaces if needed. This is basically an improved version of the old command ‘Remove internal tags’ which was/is available in the ‘Filter’ dialogue that can be accessed when opening a TMX.
- **2014-05-28** New switch: *Edit \> Options \> MT Services \> Prefer Autoassembling with Machine Translation* This sets the default shortcut for quick MT+AA transfer to the target box. You can also switch the shortcut on on the fly by right-clicking at the MT tab pane.
- **2014-05-24** There was a problem where no hits were shown in the Glossary pane and no hits were highlighted in source segment box if there were Glossary entries with empty target fields (only source given). Fixed.
- **2014-05-16** QA Brackets checks is made a bit stricter, causing less false positives
- **2014-05-13** Fix for the Autocompletion issue mentioned on the cafetranslators forum
- **2014-05-13** [Improve Auto-assembling with Machine Translation](http://cafetran.wikidot.com/the-mt-services-tab) **Déjà Vu’s ‘Deep Miner’ has finally come to CafeTran!!!**
- **2014-05-13** [Setting the QA checks that should be performed on Check all](http://cafetran.wikidot.com/performing-qa-checks)
- **2014-04-30** When you ‘Export as bilingual document with notes’ in a multi-file project, the exported file is not given the correct file name. That is, the name of the current document. Fixed. Note that this doesn’t apply if you have glued the documents and use the above export command.
- **2014-04-21** HTML project exports (via *Project \> Save Project as… \> HTML*) now have clear divisions between the individual documents contained in the HTML file.
- **2014-04-21** *Find and Replace* dialogue box now has radio buttons, where appropriate.
- **2014-04-21** *Glossary \> Sort Glossary entries by length alphabetically* was broken. Fixed.
- **2014-04-21** New task for TMX memories in the Task menu: *Task \> Remove duplicate TMX units* (where both source and target are duplicate).
- **2014-04-17** When you add a term pair to a Memory for Terms, the pane doesn’t refresh like with a text Glossary. Fixed.
- **2014-04-17** New checkbox in Find & Replace dialogue (Cmd+F/Ctrl+F): ‘Preserve case with replacement’ (under *Options* section. See [here](http://cafetran.wikidot.com/case-adaptive-and-simultaneous-find-and-replace)
- **2014-04-17** New checkbox in Find & Replace dialogue (Cmd+F/Ctrl+F): ‘Include Project Segments’ (under *Default Scope* section). See [here](http://cafetran.wikidot.com/case-adaptive-and-simultaneous-find-and-replace)
- **2014-04-12** A small update to the new Pretranslation implementation. An issue with the language code in the translation units of the generated TMX has been fixed.
- **2014-04-11** The Pretranslation feature has been changed. After running Pretranslate, the program now generates a small .tmx file (called ‘Pretranslation.tmx’) containing the translation units which where found during the Pretranslation process. You can save this file on your computer and re-import it after closing/re-opening CafeTran via *Memory \> Import \> Import Pretranslation…*
- **2014-04-11** Text in MS Word ‘SmartArt graphics’ is now imported into CafeTran. This text can be found if you rename the .docx file to .zip, unzip it, and look in the various folders here: ’(1) C:\Users\usr\Desktop\example word document.docx.zip\word\embeddings, (2) C:\Users\usr\Desktop\example word document.docx.zip\word\diagrams, (3) C:\Users\usr\Desktop\example word document.docx.zip\word\charts’. Some examples of these objects can be seen [here](http://cafetran.wdfiles.com/local--files/pre-release-version/SmartObjects.png) and [here](http://cafetran.wdfiles.com/local--files/pre-release-version/SmartObject2.png) (screenshots open in a new window).
- **2014-04-02** MQXLIFF: Locked segments are hidden, pretranslated segments have *Checked* status
- **2014-03-30** Changed F2 term display system.
- **2014-03-30** Problem where longer non-translatable fragments were not displayed when pressing F4, if their constituent parts were present as shorter fragments. Fixed. Now all NTs present in your source segment are displayed.
- **2014-03-28** [Basic formatting is displayed in all visible segments in the grid.](http://cafetran.wikidot.com/the-grid)
- **2014-03-28** Improvement of the MQXLIFF filter
- **2014-03-25** Fix for MQXLIFF and SDLXLIFF autopropagation issue
- **2014-03-25** Issue where AA would not automatically adjust the case of the first word in a target segment, fixed.
- **2014-03-15** Improvement of the way memoQ XLIFF files are handled: tags in Help & Manual projects are now treated as CafeTran tags.
- **2014-03-10** With the Jump over Checked ticked, CafeTran 'thinks' the segment is checked (confirmed) by you and jumps over it (empty or not). The update ignores this jump during QA which might be a solution to this issue. You should have Edit \> Options \> QA tab \> QA for checked matches enabled?
- **2014-02-17** Locked segments in SDLXLIFF files are now excluded. You don’t have to waste any time on them anymore and your project count will be accurate.
- **2014-02-09** New Project group in Program Manager has been moved to the bottom of the dialogue box, in order to reflect that the settings for Glossary and TMs have to be made first: [http://cafetran.wdfiles.com/local--files/your-first-cafetran-project-in-20-screenshots/New\_PM.png](http://cafetran.wdfiles.com/local--files/your-first-cafetran-project-in-20-screenshots/New_PM.png)
- **2014-02-06** Revamped F2 system.
- **2014-02-06** Glossary search results in Find and Replace dialogue are now sorted alphabetically.
- **2014-02-02** CafeTran now supports creating a Project glossary (in the PM) and will load it automatically together with the project.
- **2014-01-31** CafeTran now remembers the last folder location after you *Project \> Save as…* (HTML, TMX, Package, etc.).
- **2014-01-29** A small update to deal with the issue of too large Options panel on small screens.
- **2014-01-27** Creation ID + Creation Date are now displayed in TMX memories (hover over little TU number to see)
- **2014-01-27** CafeTran not exporting Creation IDs into TMXs created via Project \> Save as: Fixed. TMX
- **2014-01-12** CafeTran gives you a red warning the TM tab pane when the exact match differs (i.e. in case or punctuation) from the current source segment. Also, Jump over \> Exact matches should stop at such difference in exact matches.
- **2014-01-09** Bug fixed where **\^&** was being inserted into web searches, messing things up considerably.
- **2014-01-08** New feature: case-insensitive comparison with TM.
- **2014-01-08** New feature: ***QA \> Translation conformity check*** This can be used to check for changes made to a bilingual file that was exported from a CafeTran project (edited by a proofreader) and then re-imported back into CafeTran.
- **2014-01-06** New feature (occasioned by the discussion [here](https://groups.google.com/forum/?fromgroups=#!topic/cafetranslators/2JeDBtgR_n0)) which indicates that the TM exact target is different than the current target segment. See *Options \> Memory tab \> Compare with the target segment*, or right click at the TM tab pane to activate it for a particular TM.
- **2014-01-06** In TMX edit mode: in a TU, right click: *Properties \> New property*, which will call up the Property choice panel. Click on the ‘Property name’ button, and a dropdown arrow should appear in the Name box. Click the arrow and you will see a list of all of the property names in the attached memories.
- **2014-01-06** In TMX edit mode, when you do: *View \> Segment properties*, the number of filtered units is now displayed in the grid.
- **2014-01-06** If you filter on a range using the filter box (under the source segment box), by typing in something like ’3-7’, or ’10-50’ and hitting Enter, CafeTran will tell you how many segments were filtered in the grid, and will say something like ’Translation Units: 3’ in the grid.

## Aragorn (Released on June 2013)

- **2013-12-28** New shortcut in the menu *Window* \> *Focus current tab*. This means it is now possible to switch to a glossary tab when translating and scroll it without having to use your mouse to click on the glossary tab to change focus to it.
- **2013-12-28** Enhanced editing and manipulating of Properties for TMX files (setting, replacing and removing globally, displaying them in the current TMX segment - in the TMX edit mode). New features when CafeTran is in TMX edit mode: **(1)** View \> Segment properties (to filter); **(2)** Task \> Set or Remove property for TMX units (for global changes); **(3)** Click at the property of the current segment in the project grid to edit it. **(4)** Right-click at the source segment window to access a particular property of the current segment quickly. Note: click on ‘Property names’, and then click on the dropdown arrow in the ‘Name’ field … all current properties are now displayed and can be filtered on.
- **2013-12-28** CafeTran lets you extract strings using regular expression from your current project (either a TMX, XLIFF or TTX project). See *Edit \> Find… \> Extract reg. ex. results.* Enter your regular expressions, set the Find scope and click the Find button. CafeTran will show the matching strings in the tabbed pane. This feature can be used to extract pretty muchg anything that can be gotten at with a regular expression. For example, this can be used to do a (very rough!) extraction of all the non-translatables from your text before starting the job. See [Collecting non-translatables via the Find and Replace dialogue box](http://cafetran.wikidot.com/working-with-placeables). Please keep in mind that regexes are very difficult to get right. However, with a little thought they can often be put to very good use.
- **2013-12-22** Bug fixed where setting a specific field to ‘hidden’ would break term recognition in Glossaries.
- **2013-12-22** CafeTran now shows clickable properties for the current segment in the TMX edit.mode.
- **2013-12-22** Added user-definable colours for *Subsegment match font color* and for *No subsegment match font color*, which in combination with the already existing settings *Subsegment match color* and *No subsegment match color* allow more combinations of foreground and background colours, offering better legibility (e.g. white text on red background).
- **2013-12-16** Tried to fix freezing issue (words to the left/right) but it is hard to reproduce since it does not occur here at all.
- **2013-12-16** Removed duplicates from context menu list (override AA).
- **2013-12-16** Removed the trailing ; from autocomplete suggestions when Autocomplete is fed by typing in the target window.
- **2013-12-11** DST tab-delimited output replaces the tab with newline for better viewing: source and target segments are [displayed underneath each](http://cafetran.wdfiles.com/local--files/using-spotlight-to-search-tms/ghi.png) other now.
- **2013-12-11** Saving memory (Memory \> Save as..) with a .txt extension converts any TMX to TXT tab delimited (removing duplicates in the process).
- **2013-12-11** Memory \> Open memory… opens directly any tab-delimited text file for use as a Translation memory
- **2013-12-08** It was sometimes hard to differentiate between separate glossary entries in the glossary pane because consecutive entries would sometimes all have the same highlighting colour (light green). This has been fixed: there is now a thin grey line around each entry, and a black line between the source/target entries and any metadata (fields).
- **2013-12-07** **It is now possible to hide specific metadata fields in the Glossary pane.** This can be useful to keep the Glossary pane from getting too messy if you tend to enter a lot of metadata. The fields you wish to hide can now be defined by comma separated numbers. Go to: *Edit \> Options \> Glossary \> Fields to hide*, and enter a number for each field you wish to hide. Imagine your Glossary has 10 fields (\#nl-NL –– \#en-GB –– \#Context –– \#Subject –– \#Client –– \#Note –– \#Sense –– \#Usage example –– \#Source –– \#URL), and you want to display only the ‘sense’ field (and of course the source and target term). You would therefore enter: ’1,2,3,4,6,7,8’. Only the source, target, and the sense field will now be displayed in your Glossary pane.
- **2013-12-04** Working with piped system commands such: /bin/sh -c “mdfind -onlyin /path/to/my/dir/ {} | xargs grep -h —extended-regexp —ignore-case '{}'”
- **2013-12-06** Suppressing tags in WF TMs (changing to tags positions maybe next year)
- **2013-12-04** New feature: regular expressions can now be defined at the glossary level. You can now skip adding the pipe (|) in front of terms when this flag is on. Just add the following line to your .res files: ‘Regular expressions only=yes’
- **2013-12-03** Font settings for *New Term* dialogue box added.
- **2013-12-03** Adjust trailing punctuation in SDLXLIFF now fully implemented.
- **2013-12-03** *Cancel* button in font dialogues renamed to *Exit*.
- **2013-12-01** Non-breaking spaces, etc. are now visible in the *New Term* dialogue box.
- **2013-12-01** **‘Subterm entry’ now possible in New Term dialogue!** It is now also possible to add a term pair to your glossary from inside the New Term dialogue. Imagine that you are adding a long term pair to your glossary, and you notice that it itself contains another potential term (a ‘subterm’, so to speak). Just select the source and target term as you would in the Translation Editor, and it will be added to the same (selected) glossaries as the original term you opened the New Term dialogue to enter. Select 'Satz' and 'zin' in the *New Term* dialogue box, and both *Satz=zin* and *Dieser Satz=Deze zin* are added to the glossary. See screenshot [here](http://cafetran.wdfiles.com/local--files/pre-release-version/1-12-1.png).
- **2013-12-01** **Full integration with operating system searching tools.** Terminal output is displayed in the tabbed pane in CafeTran and matches are highlighted. Set: Terminal Tool option in *Edit \> Options*. The placeholder is for the Desktop Search Tool command is {}. ‘grep’ (Linux and Mac. Also available for Windows), ‘mdfind’ (Mac spotlight in terminal). ‘find’ (Windows) Examples: grep {} /path/to/my/huge/memory.tmx, mdfind -onlyin /path/to/directory {}, find “{}” “C:\\path\\to\\my\\memory.tmx” **Note:** Use fgrep -h {} /Users/Hans/Dropbox/CafeTran/Prj/test/my\_text.txt for faster searches, suppressing the file name display. See [http://cafetran.wikidot.com/using-spotlight-to-search-tms](https://web.archive.org/web/20150108071046/http://cafetran.wikidot.com/using-spotlight-to-search-tms)
- **2013-12-01** New: *QA \> Bracket check*: See screenshot [here](http://cafetran.wdfiles.com/local--files/pre-release-version/1-12-0.png).
- **2013-11-29** CafeTran has a new Glossary tab under *Edit \> Options \> Glossary* and a **new metadata popup** will appear when you hover over a blue term in the glossary pane. See screenshot [here](http://cafetran.wdfiles.com/local--files/pre-release-version/metadata-popoup.png).
- **2013-11-24** Added menu Task \> (Remove tasks on TMX files) can be performed on attached memories now. Two more tasks that can be performed now: *Remove TMX units with no letters* and *Remove filtered TMX units*.
- **2013-11-24** Added menu *Edit \> Options \> Glossary* tab options. Added item 'Sort matches' (which sorts displayed source entries alphabetically in your glossary pane) and 'Number of fields to display'.
- **2013-11-24** **You can now increase/decrease the size of the fonts in the Translation Editor with the plus/minus icons in the tabbed pane toolbar.** The buttons used to change the font size of the text in the tabbed pane.
- **2013-11-24** Previously, local files in metadata fields in text glossaries didn’t turn into clickable links if they had spaces in them. That is, 'C:\\Users\\Administrator\\Google Drive\\Text files\\Legal\\loss of dependency.pdf' wouldn’t work because it had spaces in it. This has been fixed. Local files with spaces are now clickable links, just like internet URLs.
- **2013-11-16** Work on Java 7 support for OS X Mavericks has started. [New File Open/Save dialogues](http://cafetran.wikidot.com/new-file-open-save-dialogues) etc.
- **2013-11-11** New item in the TMX Memory dialogue: ‘Pretranslate only’. This is a new TM function to deal with huge memories, which frees up all the RAM from all unused segments just after Pretranslation is over. See: ‘Pretranslate only’ [here](http://cafetran.wikidot.com/definitions).
- **2013-11-11** There was a problem where adding a slash in *Edit \> Options \> Memory \> Additional space characters (Unicode numbers)* (and have it recognized as a space; see previous item) could break CafeTran’s handling of tags since the slash is also a part of the tag. Fixed.
- **2013-11-11** Previously, a slash character (/) would prevent neighbouring term recognition. You may now treat the slash as an additional whitespace character (a word separator). To do so, enter its Unicode character ‘U+002F’ (‘SOLIDUS’) here: *Edit \> Options \> Memory \> Additional space characters (Unicode numbers)* to enable neighbouring term recognition. Note that the slash currently has to be reinserted into the target manually: [http://www.screencast.com/t/TepR3zNXFalD](http://www.screencast.com/t/TepR3zNXFalD)
- **2013-11-09** Highlighting QA double words.
- **2013-11-09** Line breaks in segmentation .srx files.
- **2013-11-09** **Improvements to fuzzy matches highlighting.** (1) CafeTran will now mark all the missing words in the source segment (with red highlighting), even if they are shorter than the fuzzy TM source segment. (2) All changes, additions and subtractions in/to your current source text, in relation to the fuzzy match source text are now shown via red highlighting. Previously, for example, CafeTran didn’t show you when a word or phrase had been added to your current source segment text that wasn’t in your fuzzy match source text. (3) Both your current source segment and the TM fuzzy source segment are now displayed in the fuzzy match. Note that changes in word order are not shown!
- **2013-11-04** Glossaries ticked in the PM are actually loaded now in a fresh Transit project.
- **2013-11-04** ‘Document notes’ are now stored in the .xlf project file.
- **2013-11-04** The cursor used to be in the target box when opening the New Term dialogue. Now it starts in the source box.
- **2013-11-04** Documents can now be removed from projects via *Project \> Remove document…*!
- **2013-11-01** **Placeables system improved.** *Next placeable* (Shift+Escape), *Previous placeable* (Alt+f Minus), and *Transfer current placeable* (Alt+O) have been removed. Previously, only the current placeable was highlighted pink, and the aforementioned shortcuts were used to insert them. Now, all placeables are highlighted pink, and can be inserted using *List placeables* (F4) (under: *Translation \> Placeables*)
- **2013-11-01** Shortcut removed: *New memory…* (Alt+Shift+N) (formerly accessible from the Memory menu)
- **2013-11-01** *Translate segment* (Alt+Enter) renamed to *Translate selected fragment* (Alt+Enter) (accessible from the Translation menu of via the shortcut)
- **2013-11-01** Brand new menu item: *Glossary* inserted between *Library* and *Memory*
- **2013-11-01** Pressing Ctrl is no longer needed to insert hits from the auto-completion list. That is, both F2 and auto-complete terms lists now use the same term insert shortcuts/system.
- **2013-11-01** New alphabetical display of glossaries in New Term dialogue feature broke their priorities. Fixed.
- **2013-11-01** Selecting a word in the source or target box and pressing Ctrl+Enter would replace all instances of the selected word in the default scope set in the Find & Replace dialogue (i.e., in all your project source segments, memory target segments, etc.) with the segment text from your current target box. Fixed.
- **2013-10-30** *Memory \> Import \> Import Pretranslation…*
- **2013-10-30** New *Translate folder* check box in Project Info dialogue
- **2013-10-30** Glossaries are now displayed alphabetically in the *New Term* dialogue. This is useful in connection with the new Alt+1, Alt+2, Alt+3, etc. shortcuts to add terms to one of your connected (selected) glossaries. Previously, they would be in any old order. Now they are displayed alphabetically, you can always use the same shortcuts to send terms to specific glossaries. Alt+1: send term to Phrases glossary. Alt+2: send term to General glossary. Alt+3: send term to project glossary, etc.
- **2013-10-30** Import of edited notes from bilingual external review file back into CafeTran.
- **2013-10-30** Revamped Project Manager, facilitating novices
- **2013-10-23** New feature: Window \> Hide search buttons (Annoyed at those buttons that pop up every time you select a term with your mouse? Switch it off!)
- **2013-10-23** New ‘Remove’ button in the .res definition editor (*Library \> Edit resource info*). The user no longer needs to navigate inside the Java package to delete the definition files (.res) for loaded TXT Glossaries.
- **2013-10-23** **Project \> Import bilingual document**
- **2013-10-23** **Project \> Export as bilingual document with notes**
- **2013-10-23** **Project \> Export as bilingual document** … CafeTran can now export a bilingual .docx file that you can send to your proofreader, who can edit it using *Track Changes* in MS Word. Once they are finished, they can send this file back to you and you can import it back into your CafeTran project and update your segments and notes. The .docx file contains 4 columns: 1. source text, 2. target text, 3. segment notes, and 4. a column used for identifying changed segments as changed in CafeTran. See: [http://cafetran.wikidot.com/collaborating-with-a-reviewer](http://cafetran.wikidot.com/collaborating-with-a-reviewer)
- **2013-10-23** It is now possible to quickly send terms to various TXT Glossaries or TMX memories with Alt+1,2,3, etc. shortcuts in the New Term dialogues. Note that these keyboard shortcut aren’t available on OS X with the *U.S. International PC* keyboard layout.
- **2013-10-23** TXT Glossaries now also have a case sensitive/insensitive switch. Please go to the forms/GlossaryAddResource and add the following: ‘Match case=’ (You can also add this line to your .res files e.g. ‘Match case=yes’ or ‘Match case=no’)
- **2013-10-23** *Window \> Segment windows \> Cycle window with tab keys* … you can now cycle between various windows in CafeTran using the tab key on your keyboard (whereas previously an actual tab character would have been inserted). Works in Source/Target box, Find & Replace dialogue, and New Term dialogues.
- **2013-10-23** Project Manager redesigned. New division into: Segments, Phrases, Terms.
- **2013-10-09** New button in Project Info dialogue box to select a folder of source files to import.
- **2013-10-08** CafeTran did not ignore the hidden text in picture (drawing) objects inside Word: Fixed.
- **2013-10-03** It is now possible to run QA on segments with status set to 'Checked'. See: *Edit \> Options \> QA tab: QA for checked segments box*
- **2013-09-30** **RAM size optimization** (mainly for huge TMs as the [EU DGT](http://ipsc.jrc.ec.europa.eu/index.php?id=197#c2739) loaded in read-only mode but it may affect text glossaries as well).
- **2013-09-23** CafeTran wiki gets sitemap and breadcrumb navigation!
- **2013-09-16** Using **regular expressions for auto-assembling** of separable verbs is possible now. See: [here](http://cafetran.wikidot.com/using-regular-expressions-for-auto-assembling-of-separable-v)
- **2013-09-14** No non-breaking spaces required in placeables.txt for excluding word groups from QA Spell-checking.
- **2013-09-13** Groups of (adjacent) words in the target segment can now be excluded from QA Spell-checking by placing them in the placeables.txt with non-breaking spaces (NBS) between the words. Examples: VertriebsNBSGmbH, VerkaufsNBSGesellschaftNBSmbH. Excluding single words via the placeables.txt was already possible. See: [here](http://cafetran.wikidot.com/using-the-placeables-list-for-excluding-word-groups-from-spe)
- **2013-09-13** Non-breaking spaces are allowed at target side in glossaries now. This can be used to create lists with units that should get a non-breaking space between digit and unit (like: 2 km, 14,4 kV, 50 MW). A specially prepared glossary 'Units.txt' will be available here. See: [here](http://cafetran.wikidot.com/automatically-inserting-non-breaking-spaces-before-units)
- **2013-09-13** Auto-completion with punctuation characters at the cursor has been fixed. In the past, you couldn’t start typing and have auto-complete work if there was no space between your cursor and the next character. For example, if you had the word 'fuel', and then a full stop: 'fuel.' If you wanted to select the word 'fuel' and delete it, and then immediately trigger auto-complete by typing a letter, this wouldn’t work because of the full stop which was up against your cursor. Fixed.
- **2013-09-10** Empty metadata fields in Glossaries are no longer displayed in the Glossary pane.
- **2013-09-09** Regular expressions now also possible in Placeables. Entries should be preceded with a pipe character (|), just like in Glossaries.
- **2013-09-09** Additions to the placeables list can now be made from the target box too.
- **2013-09-08** New Glue dialogue, real button: Glue all files virtually :).
- **2013-09-08** Various improvements to the .idml filter to catch additional character styles (bold, italics, etc.).
- **2013-09-08** Placeables for the current segment are ignored in spell checking. Note that you have to add new placeables by selecting text in the **source segment**.
- **2013-09-08** **QA terms check** (‘QA \> Terms consistency check’) **now also works against TXT Glossaries.** Previously, this was only possible for Memories for Terms (M4Ts)
- **2013-09-08** Automatic transfer of remaining tags added as an option -\> ‘Translation \> Transfer \> Automatic transfer of remaining tags’ **For example**: there are a bunch of tags in your source segment left over that you are not going to use in your target segment. CafeTran can now automatically insert them all at the end of your translation so you don’t have to insert them manually, one by one.
- **2013-09-08** Any remaining (unused) tags that were put at the end of a segment in .IDML projects were not inserted automatically from the Project memory (TMX) when pretranslating a next project. Fixed.
- **2013-09-06** **Placeables can now be stored in a text file.** You can add them with Alt+P (Add selection to placeable) and edit the list with ’Translation \> Placeables \> Edit placeables.
- **2013-09-06** **Regular expressions in source terms in TXT Glossaries!** In TXT Glossaries, it is now possible to extend the pipe character to catch very complex terms by means of a regular expression. You just need to precede your source term with the pipe character and replace the complex term with a regular expression: E.g., if you are trying to catch: ‘voor 23% gevuld’, ‘voor 100% gevuld’, ‘voor 25% gevuld’, etc., you can now enter: ‘|voor \\d+% gevuld TAB filled up to 23%’ In the regular expression ‘\\d+%’, ‘\\d’ = a shorthand character class, which matches all numbers; it is the same as (0-9), and ‘+’ = one or more of the expression. NOTE: there is no need worrying about adding a regular expression for the target side. CafeTran will automatically insert the correct number(s) there. See [here](http://cafetran.wikidot.com/using-source-side-variables).
- **2013-09-04** Allow Tab key to switch between Find and Replace field (and a key+Tab combo to insert a Tab character). Fixed. Now it is any configurable key except TAB (see the menu: ‘Window \> Segment windows \> Cycle focus…’) It works for other dialogues too. Except TAB.
- **2013-09-04** Adjust trailing punctuation character: improve handling of closing bracket ’)’. In my opinion the bracket should be kept before a period, comma, exclamation or question mark and when it stands on its own at segment end. Now it is deleted it all cases mentioned. Fixed.
- **2013-09-05** Allow copying the Statistics table (tab-delimited) via the right mouse button to the system clipboard. Fixed. It is automatically copied to system clipboard after performing the analysis.
- **2013-09-05** Gluing: When loading a non native XLIFF file that contains several files, the Glue dialogue should be shown.
- **2013-09-05** While transposing a word to the left, the cursor should remain at the start of the transposed word, so that one can repeat transposing
- **2013-09-05** ProjectTM.tmx reverted to keeping duplicates after restart of the project: Fixed.
- **2013-09-01** .idml footnotes issue (where CafeTran placed the footnote content right where the footnote number appears in the source text.): Fixed.
- **2013-09-01** \<, \>, or " characters creating incorrect line breaks in metadata fields in glossary pane: Fixed.
- **2013-08-24** The keymap buttons in Options have the key names next to action descriptions.
- **2013-08-23** Notes can include line breaks at Export with Notes.
- **2013-08-23** Font size change recognized in Word filter.
- **2013-08-23** Setting (or removing) names to table columns at table creation in External DB.
- **2013-08-23** Searching TMs posssible during Pretranslation.
- **2013-08-23** CafeTran remembers the last source language document folder.
- **2013-08-23** **Selectable metadata lists in glossaries and memories for terms.** You can now load two lists (Subject fields, Client names) from text files. See the **Edit \> Options \> Database tab** (two new buttons to load the lists). See [here](http://cafetran.wikidot.com/using-subject-field-and-client-pick-lists).
- **2013-08-19** New feature: **Contextual Priority aka Context-aware Auto-assembling (C-3A)**. See [here](http://cafetran.wikidot.com/using-context-aware-auto-assembling)
- **2013-08-18** Terminology matching based on the property fields in TMX files as it has been in tab-delimited glossaries.
- **2013-08-18** Transpose words: The two shortcuts are reversed, in order to make them more intuitive.
- **2013-08-14** Transpose words on the whole selection, too (‘Edit \> Target segment \> Transpose selection to the left/right’). See [here](http://youtu.be/W3X5Z4vRUQs).
- **2013-08-14** Case change in Quick Term Editor fields.
- **2013-08-12** Added: ‘Library \> Glossary \> Remove source=target’
- **2013-08-12** Added: ‘Library \> Glossary \> Remove duplicate entries’
- **2013-08-12** Some glossary issues: Fixed
- **2013-08-12** DOCX file in the Def field is now clickable
- **2013-08-12** Further improvements to “subsegment guessing” function to enhance accuracy.
- **2013-08-12** The word ‘Source’ is added to Word notes that include source segments.
- **2013-08-12** Checked segments are better marked in the grid.
- **2013-08-12** **Term prioritising based on term fields**.
- **2013-08-12** Showing the last new lines of the glossary when adding a new term is back
- **2013-08-10** When using pipe characters at the source side of your glossary, you don’t have to use these pipes anymore while searching for these terms via the Find and Replace dialogue.
- **2013-08-08** Two important improvements have been made to the Transit filter, concerning the way certain tags (LineFeeds, tags surrounding spaces) in Interleaf/Quicksilver projects are handled, thus improving auto-assembling results.
- **2013-07-08** New: ‘Edit \> Options \> Desktop Search Tool’ (field for command line options to trigger your desktop search tool from inside CafeTran with a shortcut)
- **2013-07-08** New: Project | Include source segments in notes; This adds the source segment text underneath your notes. Works for Ms Word and LibreOffice (Writer and Calc).
- **2013-07-28** New: ‘Document note’ item in the Notepad menu. Press it, edit the note and then click the Save icon to save the document note. This note is exported to the header of the HTML export.
- **2013-07-26** Glossary headers are now created automatically for new glossaries.
- **2013-07-25** New: ‘Translation \> Action \> Add checked segment to memory and go to next unchecked segment’ (Ctrl+Shift+Backslash)
- **2013-07-25** New: ‘Translation \> Action \> Add checked segment to memory and go to next segment’ (Ctrl+Shift+Enter)
- **2013-07-21** Saving project as HTML is improved (along with notes and segment numbers). The html file can be opened in a web browser or edited in Word or LibreOffice.
- **2013-07-19** Holding CTRL blocks automatic transfer of selected words to the target box from resource panes.
- **2013-07-19** Clickable links in glossary pane and project notes. Links open in your system browser.
- **2013-07-16** Clicking on a blue glossary term in the tabbed pane now opens the new Quick Term Editor showing all fields (which you can define in ‘Edit \> Options \> Database’ & the txt/CSV header). That is, now empty fields are also shown so you can add metadata to empty fields in terms in your glossary straight from the Quick Term Editor.
- **2013-07-16** Searching all glossaries simultaneously is now possible from the Ctrl+F dialogue, under Default scope: Resource (Web, Glossary)
- **2013-07-16** Tab-delimited CSV/TXT glossaries now have a header, which can be used to define which field names appear in the new Quick Term Editor. The header stays put even after sorting glossary alphabetically.
- **2013-07-15** Click on (blue) source term in Glossary in tabbed pane to edit it in **new Quick Term Editor!**
- **2013-07-10** It is now possible to add new terms to several (txt) glossaries at the same time (like in the Add Term dialogue for TMX memories) using the new checkboxes in the New Term dialogue.
- **2013-07-10** F2 hits are sorted alphabetically now.
- **2013-07-09** The menu ‘View \> Project notes’ displays only segments with notes. You can also search for text in the notes after applying the notes filter.
- **2013-07-08** The last location of the Find panel is remembered.
- **2013-07-08** **Export segment notes to Word documents** with: ‘Project \> Export current document with notes’
- **2013-07-04** **Source-side synonyms**
- **2013-07-01** Progress indicator in Statistics

## Arwen (Released on March 2013)

## Frodo (Released on February 2013)

## Bilbo (Released on January 2013)

## Hobbit (Released on December 2012)
