<!-- TOC depthFrom:1 depthTo:6 withLinks:1 updateOnSave:1 orderedList:0 -->

- [CAFETRAN ESPRESSO - PREFERENCES](#cafetran-espresso-preferences)
	- [ACCESSING PREFERENCES (OPTIONS)](#accessing-preferences-options)
	- [GENERAL](#general)
		- [User ID:](#user-id)
		- [Database connection:](#database-connection)
			- [Drop down menu:](#drop-down-menu)
			- [Database connection button:](#database-connection-button)
		- [Applications connection:](#applications-connection)
			- [Drop down menu:](#drop-down-menu)
			- [Applications connection button:](#applications-connection-button)
		- [Spell checker:](#spell-checker)
		- [Web browser:](#web-browser)
		- [External editor:](#external-editor)
		- [Desktop search tool:](#desktop-search-tool)
		- [Rate:](#rate)
			- [Rate button:](#rate-button)
		- [Segmentation:](#segmentation)
			- [Drop-down menu:](#drop-down-menu)
			- [Segmentation editor, segmentation rules:](#segmentation-editor-segmentation-rules)
			- [Segment at all tags:](#segment-at-all-tags)
		- [Text shortcuts:](#text-shortcuts)
		- [Non-translatable fragments:](#non-translatable-fragments)
		- [Characters for removal:](#characters-for-removal)
		- [Surround with characters](#surround-with-characters)
			- [Surround with characters 1:](#surround-with-characters-1)
			- [Surround with characters 2:](#surround-with-characters-2)
			- [Surround with characters 3:](#surround-with-characters-3)
		- [Project page size (units):](#project-page-size-units)
		- [Segment Timer:](#segment-timer)
		- [Segment delay (millisec):](#segment-delay-millisec)
	- [DEFINITIONS](#definitions)
		- [List of subjects… | List of clients…](#list-of-subjects-list-of-clients)
		- [Definitions column names](#definitions-column-names)
			- [Context column name:](#context-column-name)
			- [Subject column name:](#subject-column-name)
			- [Client column name:](#client-column-name)
			- [Notes column name:](#notes-column-name)
			- [Reference column name:](#reference-column-name)
			- [User’s column name: (3x)](#users-column-name-3x)
		- [Language column names:](#language-column-names)
	- [WORKFLOW](#workflow)
		- [Image translation export to:](#image-translation-export-to)
		- [Auto-save](#auto-save)
			- [Auto-save project (segments):](#auto-save-project-segments)
			- [Auto-save memory (segments):](#auto-save-memory-segments)
			- [Auto-save glossary (entries):](#auto-save-glossary-entries)
		- [Keep formatting at export via clipboard](#keep-formatting-at-export-via-clipboard)
		- [Clipboard sensitive target:](#clipboard-sensitive-target)
		- [Remove newlines at clipboard transfer:](#remove-newlines-at-clipboard-transfer)
		- [Automatic selection of whole words:](#automatic-selection-of-whole-words)
		- [Automatic memory matching:](#automatic-memory-matching)
		- [Copy source to target during segmentation](#copy-source-to-target-during-segmentation)
		- [Transfer source to empty target during translation](#transfer-source-to-empty-target-during-translation)
		- [Replace characters at source transfer:](#replace-characters-at-source-transfer)
		- [Auto-completion (start at, word length):](#auto-completion-start-at-word-length)
		- [Enable two-word hints:](#enable-two-word-hints)
	- [AUTO-ASSEMBLING](#auto-assembling)
		- [Automatic insertion of matches](#automatic-insertion-of-matches)
		- [Transfer numbers to matches](#transfer-numbers-to-matches)
		- [Transfer tags to matches](#transfer-tags-to-matches)
		- [Match case](#match-case)
		- [Fuzzy match auto-correction](#fuzzy-match-auto-correction)
		- [Automatic fragments adjustment](#automatic-fragments-adjustment)
		- [Insert target only](#insert-target-only)
		- [Format numbers](#format-numbers)
		- [Automatic case adjustment](#automatic-case-adjustment)
		- [Beginning of sentence only](#beginning-of-sentence-only)
		- [Copy matches to clipboard](#copy-matches-to-clipboard)
		- [Replace punctuation characters](#replace-punctuation-characters)
	- [AUTO-PROPAGATION](#auto-propagation)
		- [Auto-propagation to other segments](#auto-propagation-to-other-segments)
		- [Auto-propagation to current segments](#auto-propagation-to-current-segments)
		- [Auto-propagation to other documents](#auto-propagation-to-other-documents)
		- [Auto-propagation of numbers](#auto-propagation-of-numbers)
		- [Auto-propagation of non-translatable fragments](#auto-propagation-of-non-translatable-fragments)
		- [Auto-propagation forward only](#auto-propagation-forward-only)
	- [GLOSSARY](#glossary)
		- [Alternatives entries separator:](#alternatives-entries-separator)
		- [Trim](#trim)
			- [Trim new terms:](#trim-new-terms)
			- [Trim new term start:](#trim-new-term-start)
			- [Trim new term end:](#trim-new-term-end)
		- [Fields to hide:](#fields-to-hide)
		- [Prefix matching](#prefix-matching)
		- [Sort matches alphabetically](#sort-matches-alphabetically)
		- [Skip new term window (button)](#skip-new-term-window-button)
		- [Vertical display](#vertical-display)
		- [Look up word stems:](#look-up-word-stems)
		- [Terms consistency check:](#terms-consistency-check)
		- [Skip new term window (shortcut)](#skip-new-term-window-shortcut)
		- [Display longest match only](#display-longest-match-only)
	- [MEMORY](#memory)
		- [Java memory size (MB):](#java-memory-size-mb)
		- [Switch to preliminary matching threshold:](#switch-to-preliminary-matching-threshold)
		- [Subsegment hits threshold:](#subsegment-hits-threshold)
		- [Subsegment to auto threshold:](#subsegment-to-auto-threshold)
		- [Contextual subsegment to auto threshold:](#contextual-subsegment-to-auto-threshold)
		- [Subsegment to virtual threshold:](#subsegment-to-virtual-threshold)
		- [Subsegment look-up limit:](#subsegment-look-up-limit)
		- [Subsegment minimal length:](#subsegment-minimal-length)
		- [Subsegments min. length difference (%):](#subsegments-min-length-difference-)
		- [Auto-assembling insert threshold (%):](#auto-assembling-insert-threshold-)
		- [Fuzzy match insert threshold (%):](#fuzzy-match-insert-threshold-)
		- [Function words threshold (%):](#function-words-threshold-)
		- [Fuzzy match threshold (%):](#fuzzy-match-threshold-)
		- [Fuzzy match display limit:](#fuzzy-match-display-limit)
		- [Search display limit:](#search-display-limit)
		- [Additional space characters (Unicode):](#additional-space-characters-unicode)
		- [Do not match:](#do-not-match)
		- [Compare with target segment:](#compare-with-target-segment)
		- [Look up word stems:](#look-up-word-stems)
	- [MEMORY SERVER](#memory-server)
		- [Rendezvous server port:](#rendezvous-server-port)
		- [Read only](#read-only)
		- [Request dialog,](#request-dialog)
	- [QA](#qa)
		- [Terms consistency check:](#terms-consistency-check)
		- [Prefix marching (%):](#prefix-marching-)
		- [Regular expression:](#regular-expression)
		- [Whole words:](#whole-words)
		- [Match case:](#match-case)
		- [QA for checked segments:](#qa-for-checked-segments)
	- [MT SERVICES](#mt-services)
		- [Mask non-translatable fragments](#mask-non-translatable-fragments)
		- [Team auto-assembling with machine translation](#team-auto-assembling-with-machine-translation)
		- [Online MT engines](#online-mt-engines)
			- [Google Translate:](#google-translate)
			- [MS Translator:](#ms-translator)
			- [MyMemory:](#mymemory)
			- [Yandex Translate:](#yandex-translate)
		- [Offline MT engines](#offline-mt-engines)
			- [Slate Desktop:](#slate-desktop)
	- [WEB SERVICES](#web-services)
		- [ProZ.com](#prozcom)
		- [WIWO automatic pop-up dialog](#wiwo-automatic-pop-up-dialog)
		- [TM-Town](#tm-town)
	- [APPEARANCE](#appearance)
		- [Look and Feel](#look-and-feel)
		- [Large icons](#large-icons)
		- [Monochromatic icons](#monochromatic-icons)
		- [Interface language:](#interface-language)
	- [KEYBOARD SHORTCUTS](#keyboard-shortcuts)
	- [LIST OF CHANGES](#list-of-changes)
	- [Feedback](#feedback)

<!-- /TOC -->

# CAFETRAN ESPRESSO - PREFERENCES

*Updated for CafeTran Espresso 2018 - Forerunner - 20171130 (build 2017122201)*

This reference document offers a tour of CafeTran’s Preferences (Options) and describes each item’s function, providing some additional information along the way.

*Curated by [Jean Dimitriadis](https://www.proz.com/translator/2042360) (EN-FR/EL-FR translator).*

Shortened link to this document:

## ACCESSING PREFERENCES (OPTIONS)

You can access Preferences from the **Menu (Edit>Preferences [Options])** or directly from the **Dashboard** by clicking the button shown below and choosing Preferences (Options). OS X users can also use the usual Cmd + , shortcut.

![Dashboard menu button](https://i.imgur.com/GwHznze.png)

## GENERAL

![General pane](https://i.imgur.com/T1Wfget.png)

General preferences pane allows you to set various CafeTran options and features, the most important probably being the Segmentation function.

### User ID:

Blank field by default.

The username entered here will be stored as metadata in CafeTran’s XLIFF files or external bilingual files (in TMX files as well).

### Database connection:

In addition to TMX Translation Memory files, CafeTran offers an advanced Translation Memory database feature called **Total Recall** (TR). This section allows you to set the TR database information. You can then create multiple TR databases to suit your needs.

Note: These options can be left in their default values and used as is. They only need to be tweaked for more advanced database creation.

#### Drop down menu:

Choice between H2, SQLite, Hsqldb, MySQL, New Database
Default choice: SQLite

This is where you can choose the database type or create a new TR database. After selecting the database type, or if you select “New Database”, you can view and edit the Database information settings by clicking the Database connection button.

#### Database connection button:

![The Database information window](https://i.imgur.com/EAuNH8u.png)

This button opens the Database information window, which allows you to view and edit the TR database information for the chosen Database type.

Related links:
[Working with Total Recall](https://cafetran.freshdesk.com/support/solutions/folders/6000058183)

### Applications connection:

You can connect CafeTran to OpenOffice/LibreOffice’s interface and share its spell checker.

<!---TODO: Applications connection not tested yet. How?--->

#### Drop down menu:

Available applications: OpenOffice

Related links:
[Connecting to OpenOffice or LibreOffice](http://beijer.uk/cafetran-old-wiki/cafetran.wikidot.com/connecting-to-openoffice-or-libreoffice.html) (old unofficial wiki)

#### Applications connection button:

![The Applications connection window](https://i.imgur.com/JB9iiPZ.png)

Once you choose OpenOffice in the drop-down menu, you can click the Applications connection button, and then click the Class path button to specify the directory where OpenOffice/LibreOffice is installed on your computer. The field will be populated accordingly.

### Spell checker:

Drop down menu. Choice between Hunspell and OpenOffice/LibreOffice. Default: Hunspell.

If you connect OpenOffice/LibreOffice (see previous option), you can use its spell checker instead of Hunspell. The Spell check option found in the Edit menu will disappear, as CafeTran will use the already installed spell checking dictionaries.

Related links:
[Installing a Spell Checking Dictionary](https://cafetran.freshdesk.com/support/solutions/articles/6000110210-installing-a-spell-checking-dictionary) (Hunspell)

### Web browser:

Drop-down menu: Choice between CafeTran or System. Default: CafeTran

CafeTran offers a web resources feature which allows you to use and query various web resources within its tabbed panel (Some resources are already present in the default installation, but you can add many more to suit your needs. Most web pages are supported). This can be done either via **CafeTran**’s internal browser, within the open resource’s tab or via the **System**’s default browser. If the latter is selected, a new search opens the Web resource in the default external Web browser of your operating system.

<!---TODO: Explain how to conduct web searches.--->

Note: This choice can also be set individually per each web resource.

Related links:
[Searching Internet Resources](https://cafetran.freshdesk.com/support/solutions/articles/6000110245-searching-internet-resources)
[Adding a Web Resource - Based on Examples](https://cafetran.freshdesk.com/support/solutions/articles/6000110248-adding-a-web-resource-based-on-examples)
[Web Resources in the System Browser](https://cafetran.freshdesk.com/support/solutions/articles/6000110761-web-resources-in-the-system-browser-)

### External editor:

Drop-down menu: Choice between Clipboard binding , Atom, BBEdit, Bing Translator, DeepL, Google Translate, Jarte, Notepad++. Default: Clipboard binding.

The functionality of CafeTran’s target segment editor can be further extended by binding it with an external text editor. Some specialized editors offer additional functions that can enhance the editing experience. For example, a dictation application can be tuned to work best only with certain text editors. You can also use the edit box of a Machine Translation Web page as an external editor.

Related links:
[Target Segment Editors](https://cafetran.freshdesk.com/support/solutions/articles/6000162841-target-segment-editors)
[Voice Translating](https://cafetran.freshdesk.com/support/solutions/folders/6000225250)

### Desktop search tool:

Path to the executable you wish to use when querying the Desktop search tool, or terminal command to apply and output within CafeTran.

<!---TODO: Additional information needed--->

Additional checkbox: **Terminal tool**, OFF by default. Allows to output the search result of the command set above, in a separate tab.

Related links:
[Desktop Search Tool](http://beijer.uk/cafetran-old-wiki/cafetran.wikidot.com/desktop-search-tool.html) (old unofficial wiki)

<!---Alternative:
You can also search some Reference glossary/text files with the current glossary feature as follows:
1. Select “Glossary folder” in the Glossary menu.
2. Choose “Add glossary...” from the Glossary menu and select a folder with the files (no subfolders supported).
3. After the import and loading, try to do some search via the Search bar (Glossary button).--->

### Rate:

To populate this field, click on the “Rate:” button. This is useful to calculate the total project cost for source or target segments. You can base the calculation to Words, Characters or All Characters.

<!---TODO: Check what All characters does--->

#### Rate button:

![Choose your rate window](https://i.imgur.com/KyKGNOX.png)

Note: Rate can also easily be set/modified in **Statistics** (Project>Statistics>Project Statistics) from within your current project.

![Click to set your rate](https://i.imgur.com/T4MRqF6.png)

### Segmentation:

This is where you set what rules CafeTran will use to segment the document(s) you translate. This section is **only for native projects**, not for bilingual files, which are usually already segmented.

#### Drop-down menu:

Available choices: Sentence, Paragraph, Tag, Word, Document, Rules.srx. Default: Sentence.

CafeTran offers various ways to segment a document and you can add more.

Sentence, Paragraph, Tag, Word, Document segmentation rules are not editable and must be used as is.

<!---TODO: Review the first options. What Document does--->

#### Segmentation editor, segmentation rules:

If you select Rules.srx (or other srx files from the drop-down menu), “Segmentation” becomes “**Segmentation editor**” and an additional drop-down menu appears (**Segmentation rules**), allowing you to select which source language rules you wish to apply.

CafeTran supports the SRX standard and offers the possibility to edit SRX files (which are used to specify the break rules and the exception rules on a per language basis). The Default rules take precedence over any other rules.

SRX files are stored in *cafetran/rules/segmentation* folder.
This is where you will find the Rules.srx file and where you can add other srx files as well.

**Editing segmentation rules:**

<!---TODO--->

CafeTran allows you to view, edit or create segmentation rules.

Free alternatives to the CafeTran internal SRX editor include:
Maxprograms - [SRXEditor](https://www.maxprograms.com/products/srxeditor.html)
Okapi Framework - [Ratel](http://okapiframework.org/wiki/index.php?title=Ratel) (standalone or integrated into [Rainbow](http://okapiframework.org/wiki/index.php?title=Rainbow))

**A note on abbreviations:** In addition to fine-tuning segmentation through the SRX editor, you can also use CafeTran’s Abbreviations feature for segmentation purposes. Abbreviations will act as Exception rules, meaning that they will instruct CafeTran not to break the segments if it finds such abbreviations at document creation. This is found in Resources > Abbreviations. A project can also be scanned for abbreviations (You may need to remove and add the document back, since segmentation occurs only at project creation).

Segmentation can further be adjusted manually by using the **Split** and **Merge** features (again, this works only for native CT projects).

*Suggestions:
To access more already set language rules for segmentation, you may want to download and use OmegaT’s [SRX file](https://raw.githubusercontent.com/omegat-org/omegat/master/src/org/omegat/core/segmentation/defaultRules.srx).
Save the document directly from your browser and remove the .txt extension. Rename it as needed and place it in *cafetran/rules/segmentation* folder. It will be recognized after CT has been restarted.
For a Trados-like segmentation, you may want to add the colon character (:) to the OmegaT’s Default rules and change Break: [\.\?\!]+ to [\.\?\!:]+ in the beforebreak section.*

*Another option packed with even more per language rules comes from LanguageTool and its [SRX file](https://github.com/languagetool-org/languagetool/blob/master/languagetool-core/src/main/resources/org/languagetool/resource/segment.srx)*

#### Segment at all tags:

Checkbox, OFF by default

By enabling this option, you can apply an additional rule to the selected segmentation method, namely to break segments at each tag.

### Text shortcuts:

Drop-down menu: Blank by default

You can create text shortcuts to expand any given text with a defined character combination. To create a text shortcuts file that you can use across different sessions or projects, you need to first add at least one Text shortcut in Resources > Text shortcuts > Add selection to text shortcuts, then choose Resources > Text shortcuts > List text shortcuts and click the Save button. If you don’t save the shortcuts, they will be working for the current session only. Once saved, the shortcuts file will be available in this drop-down menu.

Saved Text shortcuts files are saved as txt files in *cafetran/resources/shortcuts* folder.
Multiple shortcuts files can be saved in this folder and selected from the drop-down menu.

Text shortcuts files use the following format (each line is a new shortcut):
shortcut=expanded_text

To expand a defined shortcut, you simply type the shortcut and press the Space key.

Note: External applications may offer more advanced and universal text expansion solutions (meaning they can be used across all applications in your operating system). Still, Text shortcuts can be very useful for ad hoc text expansion needs within CafeTran.

### Non-translatable fragments:

Drop-down menu: Default: nontranslatables.txt

You can define non-translatables, which will be stored in the non-translatable list.

Non-translatables appear by default with a violet color background on the source segment and can be easily inserted via the F4 keyboard shortcut.

Non-translatables are stored in *cafetran/resources/placeables* folder.
Multiple non-translatables files can be saved in this folder and selected from the drop-down menu.

The non-translatable TXT files are simple lists with one non-translatable per line.

Note: You can also use non-translatables to mask confidential terms before being submitted them for Machine Translation. See MT services preferences pane.

### Characters for removal:

Blank field by default.

The field displays the characters that are removed by the Remove defined characters function. Use the pipe character | to separate the defined characters in the list.

This makes use of Java regular expressions.

Suggested example value: ,(?=\s\D)|<[^>]+>|\s(?=\s)

### Surround with characters

The three fields provide an easy way to surround highlighted text with the defined characters. Different types of quotes, brackets or parentheses are good candidates for this feature.

Methods to use this function:

- Edit > Target segment > Surround with characters [1,2,3]
- Use defined keyboard shortcut for each option
- Select S1, S2, or S3 from the context menu (Right-click or use defined keyboard shortcut to bring the context menu)

#### Surround with characters 1:

Default value: « S »

#### Surround with characters 2:

Default value: (S)

#### Surround with characters 3:

Default value: “S”

### Project page size (units):

Default value: 50

This sets the number of translation units (segments) that are displayed in the Segments grid. You can navigate between segments with the Arrow buttons of the Segments grid.

Note: Limiting the number of displayed segments in one “page” is one of the ways to help running CT more efficiently in battery mode.

Related links: [Running CafeTran in the Battery Mode](https://cafetran.freshdesk.com/support/solutions/articles/6000113091-running-cafetran-in-the-battery-mode)e

### Segment Timer:


Checkbox.

When this is enabled, the segment timer icon is added to the target segment editor. The segment timer allows you to go through each segment after the defined segment delay (see below) without using the keyboard. To trigger this, you simply need to Move/Go to next segment. To stop the timer, either click the button or hit the Esc key.

### Segment delay (millisec):

Default value: 2000.

Define the delay in milliseconds at which CafeTran will automatically go to the next segment, when the Segment timer option is enabled (see above).

## DEFINITIONS

![Definitions pane](https://i.imgur.com/y6kxAZW.png)

Definitions pane allows you to specify some fields that can be applied to the Glossaries and Termbases (Memories for fragments) and Project configuration. It is optional in most scenarios, but useful for more information-rich terminology implementations.

### List of subjects… | List of clients…
Clicking these buttons lets you select a TXT file which contains a list a subjects or clients that you will the be able to apply as metadata to your projects, glossaries and termbases. Once the file is specified, it will be used by CT until you set another file.

*Suggestion: You can create a “Subjects-clients” folder within cafetran/resources folder, and then a separate “clients” and “subjects” text file.*

<!---Modification: could CafeTran have such a folder and such a txt file already populated?--->

### Definitions column names

Blank fields by default.

You can set column/field names for your Glossaries/Termbases (using default names such as, Context, Subject, Notes, Reference, etc.). As long as those fields/column names are left blank, they will not appear in the glossary/termbase entries you create, keeping things simple as the default behavior.

Note: If you set multiple columns for your glossary, you may want to consider choosing the Vertical display in its context menu (right click) for better readability.

The Definitions column names include the following fields:

#### Context column name:


#### Subject column name:

#### Client column name:

#### Notes column name:

#### Reference column name:

If this column name is set, the Reference field also features a button to attach a file location to serve as reference.

#### User’s column name: (3x)

Three custom column names

### Language column names:

Drop-down menus. Up to 8 different languages/variants can be set.

This section concerns only Glossaries. CafeTran supports multilingual glossaries (glossaries that feature more than two languages/language variants). Here you can set the languages columns that will be present in new glossaries.

CafeTran keeps track of all your working languages/language variants and adds them in this section.
You may need to remove unnecessary languages/variants if you use various language pairs or do not intend to keep multilingual glossaries. When creating a new glossary, there is a Definitions button that allows you to easily set the required languages. This can also done via the glossary context menu (right-click) > Edit glossary if the glossary is already created.

![Definitions button in New glossary window](https://i.imgur.com/V3mSGB8.png)

Related links:
[Multilingual Glossaries](https://cafetran.freshdesk.com/support/solutions/articles/6000113541-multilingual-glossaries)

<!---Modification: improve default behavior--->

## WORKFLOW

![Workflow pane](https://i.imgur.com/A6m7T0g.png)

This pane includes some options related to various CafeTran workflows. Workflows can be selected from the drop-menu available in the Dashboard.

### Image translation export to:

Drop-down menu.
Available choices: Ms Word, OpenOffice, Text, Default: MS Word

This option concerns the **Translate a paper document** workflow, available from the Dashboard. In this workflow, you can translate short paper documents, scanned documents or image files. The option allows you to choose the export format CafeTran will use.

Related links:
[Translation of Paper Documents](https://cafetran.freshdesk.com/support/solutions/articles/6000111789-translation-of-paper-documents)
[Translation of Scanned Images](https://cafetran.freshdesk.com/support/solutions/articles/6000111566-translation-of-scanned-images)

### Auto-save

CafeTran auto-saves project segments, memory segments and glossary entries CafeTran according to the values specified in this section.

Note: Raising the interval makes sense if you run CafeTran on a laptop computer in battery mode. Otherwise, low numbers provide a safety net in case of an unexpected application quit or computer shutdown.

#### Auto-save project (segments):

Default value: 3

#### Auto-save memory (segments):

Default value: 5

#### Auto-save glossary (entries):

Default value: 3

Related links:
[Running CafeTran in the Battery Mode](https://cafetran.freshdesk.com/support/solutions/articles/6000113091-running-cafetran-in-the-battery-mode)

### Keep formatting at export via clipboard

Checkbox: ON by default.

This option concerns the **Translate through clipboard** workflow, available from the Dashboard.

Uncheck this option if you want to have formatting tags removed upon clipboard export.

Related links:
[Formatting in Clipboard Workflow](https://cafetran.freshdesk.com/support/solutions/articles/6000110165-formatting-in-clipboard-workflow)

### Clipboard sensitive target:

Checkbox, OFF by default

Drop-down menu: Choices: Look up, Translate, Segment. Default: Look up

This option specifies the behavior in case **Edit > Clipboard sensitive** menu option is ON.

**Look up**: the clipboard contents are looked up automatically in CafeTran’s resources.
**Translate**: the clipboard contents are translated automatically with the translation memories and glossaries.
**Segment**: the clipboard contents are pasted automatically into the target segment editor (e.g. as a translation of the current segment).

Related links:
[Clipboard Sensitive](https://cafetran.freshdesk.com/support/solutions/articles/6000168359-clipboard-sensitive)

### Remove newlines at clipboard transfer:

Checkbox, OFF by default

If this option is ON, CafeTran removes the newline character from the pasted text during the transfer via clipboard.

### Automatic selection of whole words:

Checkbox, ON by default

If this option is ON, CafeTran selects whole words even if you make a partial selection in the source or target segments. The option is quite convenient as it speeds up text selection, since mouse selection does not need to be precise. Uncheck if the behavior is unwanted.

### Automatic memory matching:

Checkbox, OFF by default

If this option is ON, CafeTran performs automatic search in the translation memories. Otherwise, only manual searches are made.

### Copy source to target during segmentation

Checkbox, OFF by default

If this option is ON, CafeTran copies source segments to target segments during segmentation.

Note: To transfer source segments to all target segments during translation (after segmentation), you can also use Task > Transfer source segments to target segments.

### Transfer source to empty target during translation

Checkbox, OFF by default

If this option is ON, CafeTran copies the content of the source segment to each empty target segment you visit during the translation.

Note: To transfer source segments to all target segments, you can also use Task > Transfer source segments to target segments.

### Replace characters at source transfer:

Three available field pairs.

These field pairs allow you to set characters you wish to replace during source transfer.

### Auto-completion (start at, word length):

Checkbox, ON by default
Two fields, Default values: Start at: 3 and word length: 7 respectively.

The checkbox allows you to enable or disable Auto-completion function.

Auto-completion is a CafeTran feature that uses text from various sources (Project segments, Memories [matches, fuzzies, hits], Glossaries, MT results, etc.). As you type, CafeTran will often bring up the auto-completion menu, which allows you to quickly complete the word instead of typing it. The auto-completion function is automatically triggered if enabled, and if there is a space following the cursor. If there is a character in the right side of the cursor, you can still manually bring the auto-completion menu with the Ctrl+Down arrow (default) keyboard shortcut.

**Start at:** minimum number of typed characters to trigger the Auto-completion function.

**Word length:** minimum character length of words to be processed by the Auto-completion function.

### Enable two-word hints:

Checkbox, ON by default

This option also concerns the Auto-completion function. If the option is ON, CafeTran will offer auto-completion options for the next word as well.

## AUTO-ASSEMBLING

![Auto-assembling pane](https://i.imgur.com/26hi7OT.png)

This pane allows you to set various auto-assembling options.

Auto-assembling is a special CafeTran feature that uses and “repairs” various enabled resources to create a suggested translation.

Auto-assembling (and TM) results can be viewed in and inserted from the Matchboard or the Auto-assembling panel (F1 keyboard shortcut, unless Translate > Pop up auto-assembling panel option is enabled)

Note: To further fine-tune the suggestions you get from Auto-assembling, you can set each resource’s Priority (Low, Medium, High) or choose which resources to keep out from auto-assembling via their context menu (right-click) > Keep out of auto-assembling.

### Automatic insertion of matches

Checkbox, OFF by default

If this option is ON, CafeTran systematically inserts the auto-assembling result to the target language box.

Note: Auto-assembling insert threshold (%) option, available in the Memory pane can be used to control the automatic insertion threshold for auto-assembling.

### Transfer numbers to matches

Checkbox, ON by default

If the option is ON, CafeTran automatically inserts the numbers present in the source segment into the target suggestion, replacing those from fuzzy matches.

### Transfer tags to matches

Checkbox, ON by default

If the option is ON, CafeTran automatically transfers the surrounding tags of the source marches in the source segment to the target language segment. It functions when you transfer a target fragment/term, auto-assembling, a fuzzy match or machine translation containing the matched fragments. It is also active during the automatic insertion of the best translation result into the target segment editor.

Related links:
[Auto-tagger: Transfer Formatting Tags to Matches](https://cafetran.freshdesk.com/support/solutions/articles/6000161178-auto-tagger-transfer-formatting-tags-to-matches)

### Match case

Checkbox, OFF by default

If this option is ON, CafeTran uses case sensitive matching for the resources it uses to provide its suggestions.

### Fuzzy match auto-correction

Checkbox, ON by default

If this option is ON, CafeTran tries to repair fuzzy matches, replacing the differing fragments with other exact fragments or non-translatables.

Fuzzy match auto-correction also works if the start and/or the end of the current segment is missing in the fuzzy match, and there are matches in TM, glossary or nontranslatables for those missing parts.

Note: This also affects the Matchboard behavior.

### Automatic fragments adjustment

Checkbox, ON by default

Here’s the developer’s explanation: This functions character is dynamically picking the recently used match for a fragment/term or its synonym as the one with top priority to use in subsequent segments (both in auto-assembling and MT improvement). It can also adjust the basic form of a fragment (e.g. sunny day) to the one you actually use in the segment (e.g. sunny days) provided that change is slight - in the form of the regular noun, in this example. Then, CT will use the adjusted fragment in the subsequent segments. So let’s say CT suggests a correct virtual TM fragment (hit) by analyzing the context but your top priority glossary inserts another suggestion (e.g. basic form). If you use the virtual fragment in the current segment, CT will enhance the priority of this virtual fragment to use in the subsequent segments.

### Insert target only

Checkbox, OFF by default

If this option is ON, CafeTran only inserts untranslated fragments during auto-assembling into the target language box.

### Format numbers

Checkbox, OFF by default

If this option is ON, CafeTran formats numbers to the target language numbering system if it is
different from the source language system.

### Automatic case adjustment

Checkbox, ON by default

If this option is ON, it lets CafeTran automatically adjust the case (at least for auto-assembling results).

NOTE: You can **manually adjust** the case of a segment, fragment or selected word.
To cycle between cases, use Edit > Target segment > Change case, or the related keyboard shortcut.
To use Title case, use Edit > Target segment > Change to title case, or the related keyboard shortcut.

To let CafeTran **automatically adjust** the case while typing, you can enable Edit > Target segment > Automatic case adjustment option.

### Beginning of sentence only

Checkbox, ON by default

If this option is ON, automatic case adjustment occurs only in the beginning of a sentence.

### Copy matches to clipboard

Checkbox, OFF by default

If this option is ON, CafeTran copies the auto-assembling match to the clipboard, so that you can be paste it directly if the result is good.

### Replace punctuation characters

Three field pairs

If enabled, auto-assembling replaces the punctuation characters as set in the field pairs.

## AUTO-PROPAGATION

![Auto-propagation pane](https://i.imgur.com/s52CzJM.png)

This pane lets you enable or disable various Auto-propagation options.

Auto-propagation is the process whereby the translation from one segment is applied to other segments that have similar source content.

Note: You can disable Auto-propagation for a specific segment via right-clicking at the source segment editor and unchecking Auto-propagation checkbox (the segment is marked as “nP” in the Grid). For non-CafeTran projects, this option works for the current session only.

### Auto-propagation to other segments

Checkbox, ON by default

If this option is ON, the current segment is propagated to other identical source segments.

### Auto-propagation to current segments

Checkbox, ON by default

If this option is ON, the translation of another identical source segment in the project is propagated to the currently edited segment.

### Auto-propagation to other documents

Checkbox, ON by default

This option lets you choose if Auto-propagation works across documents in a single project (even if the documents are not glued) or only to the current document.

### Auto-propagation of numbers

Checkbox, ON by default

If this option is ON, auto-propagation works also for segments that only differ in featured numbers.

### Auto-propagation of non-translatable fragments

Checkbox, ON by default

If this option is ON, auto-propagation works also for segments that only differ in non-translatable fragments

### Auto-propagation forward only

Checkbox, ON by default

If this option is ON, backward auto-propagation is disabled.

## GLOSSARY

![Glossary pane](https://i.imgur.com/Zx4RVp0.png)

This pane features various options relevant to Glossaries (and Termbases - Memories for fragments).

Related links:
[Working with Glossaries](https://cafetran.freshdesk.com/support/solutions/folders/6000058179)

### Alternatives entries separator:

Default value: ”;”

This option lets you define the character that will be used for synonyms and alternative entries in Glossaries.

### Trim

#### Trim new terms:

Checkbox, ON by default

This option applies trim settings to new terms.

#### Trim new term start:

Blank field by default.

Here you can define characters for removal that are present at the start of the selected term.

This makes use of Java regular expressions.

Example: Use this setting to exclude chapter numbers etc. when adding terms without making selections first: \A([0-9]*[\p{Punct}]*\s*)+

#### Trim new term end:

Default value: “[\p{Punct}]*\s*\z”

Here you can define characters for removal that are present at the end of the selected term.

This makes use of Java regular expressions.

### Fields to hide:

Here you can define Fields you wish to hide from glossary columns.

Enter the number of the Glossary field(s) you want to hide, separated with a comma (,)

This allows you to only display specific fields while keeping the fields defined in Definitions.

### Prefix matching

Checkbox, OFF by default

If this option is enabled, it introduces automatic fuzziness to your glossary matches.

Note: As the “Prefix length” option is shared with TM fragments, you can adjust the prefix length in the options for the memory (e.g. after right clicking at the memory pane). You will need to reload the glossary after turning on/off the Prefix matching option.

### Sort matches alphabetically

Checkbox, OFF by default

If multiple term matches are available, they are displayed in alphabetical order with this option enabled.

### Skip new term window (button)

Checkbox, OFF by default

If enabled, this option skips the new term window when you add a new term by clicking the Add term to glossary or Add fragment to memory buttons in the target language box buttons.

### Vertical display

Checkbox, OFF by default

If enabled, this option triggers the Vertical display option for all glossaries.

NOTE: You can manually enable/disable this option per each glossary via the context menu (right click) > Vertical display.

### Look up word stems:

Checkbox. ON by default.

If enabled, CafeTran use word stemming when querying for glossary matches.

### Terms consistency check:

Checkbox. ON by default

CafeTran will enable terms consistency check for attached glossaries for this QA step (see QA pane/menu for more information).

NOTE: You can enable/disable this option per each glossary via the context menu  (right click) > Terms consistency check.

### Skip new term window (shortcut)

Checkbox, OFF by default

If enabled, this option skips the new term window when you add a new term by hitting the Add term to glossary or Add fragment to memory keyboard shortcuts.

### Display longest match only

Checkbox, OFF by default

With this option enabled, CafeTran only shows the longest glossary match in the glossary.

## MEMORY

![Memory pane](https://i.imgur.com/BgD7MJZ.png)

This pane lets you choose the assigned RAM for CafeTran and set various aspects related to Translation Memories behaviour.

Related links:
[Working with Translation Memories](https://cafetran.freshdesk.com/support/solutions/folders/6000058172)

### Java memory size (MB):

Default value: 1024

Here you can define the amount of RAM allocated to CafeTran’s operation.

Note that with very large resources, for example translation memories or glossaries 100 MB or more in size, it may be advisable to increase the amount of RAM made available to CafeTran in Java. Consider increasing the default value from 1024 to 2048, for example. Restart the program to apply the new Java memory settings.

### Switch to preliminary matching threshold:

Default value: 50,000

Here you can set the number of segments after which TMX or Total Recall memories switch from automatic to preliminary memory matching.

Developers explanation: After you load a translation memory either from TMX files or from Total Recall, CafeTran performs an automatic matching. The currently-translated segment is matched automatically against this translation memory to produce the results of matching. As your translation memory is getting bigger and bigger over time and reaches thousands of segments, the automatic matching may get slower as the current source segment is matched against that large amount of translation memory segments. To overcome this issue of huge memories, you can perform the preliminary memory matching of the whole source document so that the matches will be available instantly, without any delay. The preliminary memory matching may take a while but you do not have to wait until it completes because matches for each next source segment are available right after the segment is processed. It means that you can translate at your own human pace while the preliminary matching is taking place in the background.

Note:  Preliminary matching workflow option can also be chosen from the Memory options > Workflow integration > Preliminary memory matching.

Note 2: You can disable the switch to preliminary matching by changing the threshold to a very high value, like 2,500,000.

Related links:
[Preliminary Memory Matching](https://cafetran.freshdesk.com/support/solutions/articles/6000059860-preliminary-memory-matching)

### Subsegment hits threshold:

Default value: 3

This option is here to help reduce the display of low-quality subsegment matches (aka Hits). Hits below the set value are discarded.

Note: If it doesn’t help, increase this value even more to 4 or 5 for your source language.

### Subsegment to auto threshold:

Default value: 7

This option sets the number of hits (subsegment or fragment matches) before a subsegment is included in auto-assembling.

Note: Increase this number if you wish to further lower possibility of incorrect guesses.

### Contextual subsegment to auto threshold:

Default value: 3

CafeTran compares the current subsegment context (in the current segment) to the TM subsegment context of the hit.

This field sets the number of hits (subsegment matches) for contextual subsegments before they are included in auto-assembling.

### Subsegment to virtual threshold:

Default value: 10

This field sets the number of hits before a subsegment is treated as an exact subsegment match (aka Virtual match).

Note: Increase this number if you wish to further lower possibility of incorrect guesses.

### Subsegment look-up limit:

Default value: 1000

This field sets the maximum number of the matches found for a given subsegment, after which, CafeTran stops searching for more matches.

### Subsegment minimal length:

Default value: 4

CafeTran guesses the meaning of source subsegments only if they are equal or longer than the set minimal length in characters.

### Subsegments min. length difference (%):

Default value: 33

CafeTran guesses the meaning of a source subsegment only if the length difference between the source subsegment and guessed target subsegment is no lower than the set percentage.

### Auto-assembling insert threshold (%):

Default value: 80

This field lets you define the accuracy of the Auto-assembling translation at which CafeTran inserts it automatically into the target language box.

### Fuzzy match insert threshold (%):

Default value: 90

This field field lets you define the accuracy of the best fuzzy match at which the program inserts it automatically into the target language box.

### Function words threshold (%):

Default value: 5

CafeTran filters out frequently occurring words which do not need to be translated into the target language as single fragments. In this field you can set the default frequency of occurrence of the words in the source text above which the program treats them as function words and they are omitted by the Auto-assembling function.

### Fuzzy match threshold (%):

Default value: 33

This field sets the minimum accuracy of the fuzzy matches which are displayed by CafeTran.

### Fuzzy match display limit:

Drop-down menu: Available choices: 1, 2, 3, 4, 5, 6 Default value: 3

This option sets the maximum number of the fuzzy matches displayed by CafeTran.

### Search display limit:

Default value: 100

### Additional space characters (Unicode):

Default value U+00A0

Here you can insert additional Unicode characters that should be treated as spaces, which counts towards term recognition and auto-assembling.

### Do not match:

Default value: ,.。:;!¡?¿[]{}()"«»‘’“”„‚

CafeTran ignores the (punctuation) characters entered here while searching for matches of the source segments in Translation Memories and Glossaries.

Note: You can also add spaces and characters as Unicode code here. For example, to match segments that start with an invisible space a.k.a. zero-width space (invisible in the source segment section, but visible when copied in the search box), you can use Unicode code U+200B.

### Compare with target segment:

Checkbox, OFF by default

If enabled, CafeTran shows a comparison of the memory match with the target segment.

### Look up word stems:

Checkbox, ON by default

If enabled, CafeTran use word stemming when querying for Translation Memory matches.

## MEMORY SERVER

![Memory server pane](https://i.imgur.com/WHUmuZD.png)

CafeTran can act as a Translation Memory server, accepting online connections and queries from other CafeTran users. In such a server mode it is possible to work in a team on a translation project. Checking the box activates the server mode. Change the default server port if the default port is already taken by another program on your computer.

### Rendezvous server port:

Default value: “4242”

### Read only

Checkbox, OFF by default

Check this box if you wish to restrict access to your translation memories. If the option is selected, other users will not be able to change or add new terms to the memories on the server.

### Request dialog,

Checkbox, OFF by default

With this option enabled, every new connection to the server is signaled by the Request pop-up dialog.

Related links:
[Rendezvous Memory Server](https://cafetran.freshdesk.com/support/solutions/articles/6000163318-rendezvous-memory-server)

## QA

![QA pane](https://i.imgur.com/FNOzbmI.png)

This pane features options related to CafeTran’s QA function (see QA menu).

### Terms consistency check:

Drop-down menu. Choices: Prefix marching or Exact matching. Default: Prefix matching

Select a method to check for the consistent usage of terms during the Quality Assurance phase. When the Prefix matching method is chosen, CafeTran analyzes prefixes of the used terms. In the Exact matching method, the program checks for the usage consistency of whole terms.

### Prefix marching (%):

Drop-down menu. Choices: 10, 20, 30, 40, 50, 60, 70, 80, 90. Default: 50

The field determines the minimal length of prefixes of the words processed during terms consistency check by Prefix matching function.

### Regular expression:

Checkbox, OFF by default.

If you run a QA > Word lists check/filtering with Regular expression option ON, CafeTran will perform filtering based on the included regular expression.

### Whole words:

Checkbox, OFF by default

If you run a QA > Word lists check with Whole words option ON, CafeTran will perform case-sensitive filtering.

### Match case:

Checkbox, OFF by default

If you run a QA > Word lists check, Match case option ON, CafeTran will perform case-sensitive filtering.

### QA for checked segments:

Checkbox, OFF by default

By default, QA steps do NOT check the checked segments.

If you wish to perform QA checks in segments that are marked as “checked” in CafeTran, you need to enable this option.

Related links:
[Quality Assurance](https://cafetran.freshdesk.com/support/solutions/folders/6000058197) (category)

## MT SERVICES

![MT services pane](https://i.imgur.com/N8mGMWg.png)

This pane features option related to Machine Translation. Individual options can also be set via the MT context menu (see [CafeTran Espresso - Menu and Interface](http://xl8.link/ct-menu).

### Mask non-translatable fragments

Checkbox, OFF by default

All non-translatable fragments longer than 3 characters are masked before being submitted for Machine Translation - both via API and the Web interface. You can see the masking effect in MT tabs. The unmasked translation result is displayed in the Matchboard and after the transfer to the target segment. The masking feature does not work with the right-click “Create TMX memory” MT function.

### Team auto-assembling with machine translation

CafeTran lets you adjust MT results with its own Auto-assembling function, replacing terms and fragments with the ones that you prefer, that is, found in your translation memories and glossaries.

Related links:
[Auto-assembling with Machine Translation](https://cafetran.freshdesk.com/support/solutions/articles/6000160533-auto-assembling-with-machine-translation)

### Online MT engines

Related links:
[Machine Translation with MT Services](https://cafetran.freshdesk.com/support/solutions/articles/6000186536-machine-translation-with-mt-services)
[Machine Translation with MT Web Resources](https://cafetran.freshdesk.com/support/solutions/articles/6000186533-machine-translation-with-mt-web-resources)
[Translating Confidential Documents](https://cafetran.freshdesk.com/support/solutions/articles/6000163344-translating-confidential-documents)

**Checkbox:**

Enables the MT engine.

**Language pairs:**

Language pairs are usually picked up automatically when working on a project. They can be defined manually using the drop-down menus for source and target language.

**Automatic:**

If this option is enabled, CafeTran makes a query and displays the machine translation result automatically as the next source segment is displayed in the source language box. If the box is unchecked, you need to click the “Translate” link in the window of the chosen machine translation engine to make a query for the current source segment, or initiate a machine translation search via the Quick Search bar “Machine Tr.” button or keyboard shortcut (default: Ctrl+Shift+F9).

Note: You can stop or enable automatic MT search for each MT engine separately, via the context menu (right click) > Stop automatic MT service.

Related links:
[Machine Translation](https://cafetran.freshdesk.com/support/solutions/folders/6000058185) (Solutions category)
[Translating Confidential Documents](https://cafetran.freshdesk.com/support/solutions/articles/6000163344-translating-confidential-documents)

#### Google Translate:

Google API key: Enter your Google Translate API key

This is a paid translation API.

Link:
[https://cloud.google.com/translate/docs/getting-started](https://cloud.google.com/translate/docs/getting-started)

#### MS Translator:

Microsoft API key: Enter your MS Translator API key

Free tier offers 2M free characters per month. Paid tiers and options exist for more characters per month, if needed.

Link:
[https://www.microsoft.com/en-us/translator/getstarted.aspx](https://www.microsoft.com/en-us/translator/getstarted.aspx)

#### MyMemory:

MyMemory API parameters: Enter a valid Translated.net account email.

Free, anonymous usage is limited to 1000 words/day.
If you provide a valid email (“de” parameter), you enjoy 10,000 words/day.
There is a 500 characters limit per queried segment.

Links:
[https://mymemory.translated.net/doc/cafetran.php](https://mymemory.translated.net/doc/cafetran.php)
[https://mymemory.translated.net/doc/usagelimits.php#whitelist_note](https://mymemory.translated.net/doc/usagelimits.php#whitelist_note)

#### Yandex Translate:

Yandex API key: Enter your Yandex API key

Link:
[https://tech.yandex.com/translate/](https://tech.yandex.com/translate/)

### Offline MT engines

#### Slate Desktop:

Slate is a commercial offline MT solution.

CafeTran is compatible with its connector utility.

Related links:
[https://slate.rocks/](https://slate.rocks/)

## WEB SERVICES

![Web services pane](https://i.imgur.com/8aLSjQy.png)

This pane allows you to enable a few Web services options. Network connectivity is required to use these features.

### ProZ.com

Checkbox.

You can link your ProZ.com account to CafeTran.

This enables you to:

- Conduct KudoZ terms searches (manually or automatically) [Free ProZ account]
- File new KudoZ questions [Free ProZ account]
- Use “What I am working on” feature (See WIWO option below)  [Free ProZ account]
- Enjoy Full (not Trial) access to CafeTran [ProZ Plus account]

After the first successful login, CafeTran will connect to ProZ.com automatically at the start.

Related links:
[Signing in to ProZ.com account](https://cafetran.freshdesk.com/support/solutions/articles/6000158973-signing-in-to-proz-com-account)
[Automatic Search of ProZ.com Resources](https://cafetran.freshdesk.com/support/solutions/articles/6000175423-automatic-search-of-proz-com-resources)
[Proz.com Term Search Integration](https://cafetran.freshdesk.com/support/solutions/articles/6000118360-proz-com-term-search-integration)

### WIWO automatic pop-up dialog

Checkbox.

WIWO (What translators are working on) is a feature activated when you use ProZ.com services. For more details: [https://www.proz.com/wiwo](https://www.proz.com/wiwo)

### TM-Town

Checkbox.

TM-Town is a web service for translators helping them match with their clients. It also offers lots of translation-related tools such as Translation Memories and Glossaries Management, Documents Alignment and CAT Tool Integration. You can use CafeTran to connect to TM-Town and use some of its services.

Note: TM-Town Professional annual plan is included in ProZ.com Plus membership package.

Related links:
[Connect to TM-Town](https://cafetran.freshdesk.com/support/solutions/articles/6000115945-connect-to-tm-town)
[CafeTran Espresso Integration](https://www.tm-town.com/blog/cafetran-espresso-integration) (TM-Town)

## APPEARANCE

![Apperance pane](https://i.imgur.com/UESaXVx.png)

This pane includes a few appearance options. Many more are available in the View menu.

### Look and Feel

Radio checkbox: Choices: Metal Look and Feel, Nimbus Look and Feel, GTK (Linux)/Windows (Windows)/MacOS (OS X)
Default choice: Nimbus Look and Feel.

Related links:
[Themes](https://cafetran.freshdesk.com/support/solutions/articles/6000115530-themes)

### Large icons

Checkbox, ON by default

Note: Depending on your screen resolution, you might want to deselect this option.

### Monochromatic icons

Checkbox, OFF by default

### Interface language:

Checkbox:
English - United States (en-US), ON by Default
Polish (pl-PL)

## KEYBOARD SHORTCUTS

![Keyboard shortcuts pane](https://i.imgur.com/SkhNJpa.png)

This pane is where you can review or set most keyboard shortcuts CafeTran uses.

**Display keyboard shortcuts in web browser** allows you to open this list in a browser window (and print them to PDF for reference).

Clicking any item of the list opens a **keyboard shortcuts window,** which allows you to change the shortcut to your liking.

![Change keyboard shortcut](https://i.imgur.com/S2EZZjq.png)

Don’t be afraid to customize them to your liking.

Below, you will find the default keyboard shortcuts (in GNU/Linux and Windows, defaults, they are different for OS X), along with their explanation:

**Add checked segment to memory and go to next segment**	Ctrl+Shift+Enter

Add your translation of this segment to your translation memories, mark the segment as checked, and move on to the next segment in the source document.

Also in Action menu.

**Add checked segment to memory and go to next unchecked segment**	Ctrl+Shift+Back Slash

Add your translation of this segment to your translation memories, mark the segment as checked, and move on to the next unchecked segment pair.

Also in Action menu.

**Add fragment to memory**	Alt+M

Create a new translation memory fragment. Any highlighted portion of the source/target segments will be preset in the resulting “New fragment” dialog.

Also in Action menu.

**Add segment note**	Alt+N

Add an annotation about this segment; it will appear below the segment in the grid pane, marked with an “N”.

Also in Action menu.

**Add segment to memory and go to next segment**	Alt+Down

Add your translation of this segment to your translation memories, and move on to the next segment in the source document.

Also in action menu.

**Add segment to memory and go to next untranslated segment**	Ctrl+Shift+Down

Add your translation of this segment to your translation memories and move on to the next untranslated segment in the source document.

Also in action menu.

**Add selection to abbreviations**	Ctrl+Shift+M

Add a selected fragment of the segment to abbreviations.

Also in Resources >  Abbreviations submenu.

**Add selection to non-translatable fragments**	Alt+P

Add a selected fragment of the segment to non-translatable fragments.

Also in Resources > Non-translatable fragments submenu.

**Add selection to text shortcuts**	Ctrl+Shift+A

Add a selected fragment of the segment to text shortcuts. It will create a text shortcut for the fragment.

Also in Resources > Text shortcuts submenu.

**Add term to glossary**	Ctrl+Shift+G

Create a new glossary entry. Any highlighted portion of the source/target segments will be preset in the resulting “New term” dialog.

Also in Action menu.

**Adjust end punctuation**	Ctrl+Close Bracket

Adjust the ending punctuation of the target segment to match that of the source segment.

Also in Edit > Target segment submenu.

**All segments**	Ctrl+Shift+K

Include all segments (Remove filters).

Also in Filter menu.

**Alternative translation**	Alt+T

Also in Action menu.

**Bold**	Ctrl+B

Also in Edit > Target segment submenu and context menu (right click) in the target language box.

**Bookmark segment**	Alt+B

Bookmark the current segment. A letter “B” will appear next to the segment number in the segment grid.

Also in Action menu.

**Change case**	Ctrl+Equals

Cycles through multiple capitalization schemes for the target segment: “first upper-cased”, all lower-case, all upper-case.

Also in Edit > Target segment submenu and in button above source language box.

**Change to title case**	Ctrl+Shift+Equals

Capitalizes the first letter of each word within the target segment.

Also in Edit > Target segment submenu and in button above source language box.

**Clipboard history**	Ctrl+Shift+C

View the history of all text copied to the clipboard.

Also in Edit menu.

**Close active tab**	Ctrl+W

Close the currently-active resource tab.

Also in View menu and tabbed panel context menu (right click).

**Close all tabs**	Ctrl+Shift+W

Close all resource tabs.

Also in View menu and tabbed panel context menu (right click).

**Cycle focus between segment editors**	F12

Switch keyboard focus to the opposite of the currently-focused pane.

Also in View >Segment editors submenu.

**Default scope**	Ctrl+Enter

Search all resources for contents of selection in source segment editor.

Also in Edit > Find at cursor submenu.

**Delete to the end of segment**	Ctrl+Shift+D

Not found elsewhere.

**Desktop search tool**	Ctrl+Shift+F8

Perform a search through the Desktop search tool.

Also through the dedicated Quick search bar button (only available if DST already set).

**Documents…**	Ctrl+D

Open a dialog listing all project source documents, and choose which one to actively display within CafeTran.

Also in Project > Documents menu and the Document button in the Grid.

**Exit**	Ctrl+Q

Exit CafeTran Espresso.

Also in Project menu.

**Export current document**	Alt+End

Export a translated copy of only the document currently-active in the CafeTran interface.

Also in Project > Export and exchange  submenu.

**Find in page**	Alt+F

Perform the search for a word in the loaded web page and highlight the result.

Also in Edit menu.

**Find…**	Ctrl+F

Open the “Find and replace” dialog, which provides extensive options for searching resources and segments.

Also in Edit > Find menu.

**Focus current tab**	Ctrl+Slash

Send keyboard focus to the currently-active resource tab.

Also in View menu.

**Full screen**	F11

Switch to full screen mode. Press F11 at any time to exit, or mouse near the top of the window to show the “Exit full screen” button.

Also in View menu.

**Glossaries**	Ctrl+Shift+F10

Search glossaries for contents of current selection in the source segment editor.

Also in Edit > Find at cursor submenu and through the dedicated  Glossaries button in the Quick search bar.

**Hide segment boundary tags**	Ctrl+Alt+U

Hide starting and ending tags for the current segment.

Also in Action > Tags submenu.

**Hide source segment tags**	Ctrl+Alt+T

Hide all the tags in the current source segment.

Also in Action > Tags submenu.

**Insert auto-assembling**	Alt+4

Transfer the auto-assembling match to the target segment editor (if one exists).

Also in Translate menu.

**Insert fuzzy match 1**	Alt+1

Transfer the first fuzzy match to the target segment editor (if one exists).

Also in Translate menu.

**Insert fuzzy match 2**	Alt+2

Transfer the second fuzzy match to the target segment editor (if one exists).

Also in Translate menu.

**Insert fuzzy match 3**	Alt+3

Transfer the third fuzzy match to the target segment editor (if one exists).

Also in Translate menu.

**Insert non-breaking hyphen**	Ctrl+Shift+Minus

Insert a non-breaking hyphen special character at the current cursor position.

Also in Edit > Target segment submenu.

**Insert non-breaking space**	Ctrl+Shift+Space

 Insert a non-breaking space special character at the current cursor position.

Also in Edit > Target segment submenu.

**Insert soft return**	Shift+Enter

Insert a soft return special character at the current cursor position.

Also in Edit > Target segment submenu.

**Italic**	Ctrl+I

Also in Edit > Target segment submenu and context menu (right click) in the target language box.

**Join segments**

Merge the contents of the next source segment into the currently-selected segment. The next segment will also be eliminated.

Also in Action menu and through the dedicated button in the target language box.

**List auto-assembling and fuzzy matches**	F1

Auto-assembled matches are formed when all subsegments in the source segment have matches in your resources. Fuzzy matches may contain less than a complete match.

Also in Translate menu.

**List non-translatable fragments**	F4

List non-translatable fragments present in the current source segment.

Also in Resources > Non-translatable fragments submenu.

**List subsegment matches**	F2

Subsegment matches are any matches in your resources to a word or “chunk” of the source segment.

Also in Translate menu.

**List tags**	F3

Display a pop-up list of all tags in the source segment. Click a tag in the list or type a tag number followed by the Esc key to transfer the tag.

Also in Action > Tags menu.

**Memory source segments**	Ctrl+Shift+F4

Search memory source segments for contents of current selection in the source segment editor.

Also in Edit > Find at cursor submenu and through the dedicated TM source button in the Quick search bar.

**Memory target segments**	Ctrl+Shift+F5

Search memory target segments for contents of current selection in the source segment editor.

Also in Edit > Find at cursor submenu and through the dedicated TM source button in the Quick search bar.

**Merge adjacent tags**	Ctrl+Alt+O

Merge adjacent tags and treat them as one tag.

Also in Actions > tags submenu.

**Mouse tag placement**	Ctrl+F3

When enabled, tags can be added to the target segment simply by left-clicking where you’d like to place a tag.

Also in Action > Tags submenu and through the <> button in the target language box.

**Move to the next segment**	Alt+Right

 Move to the next segment in the source document (without modifying your translation memories).

Also in Action menu.

**Move to the previous segment**	Alt+Left

Move to the previous segment in the source document (without modifying your translation memories).

Also in Action menu.

**MT services**	Ctrl+Shift+F9

Search machine translation for contents of current selection in the source segment editor.

Also in Edit > Find at cursor menu.

**New document…**	Ctrl+Shift+N

Create a new notepad in the tabbed pane.

Also in Resources > Notepad submenu.

**New project…**	Ctrl+N

Create a new translation project. The current active project will be closed, and the Project Dashboard will be displayed.

Also in Project menu.

**Open document…**	Ctrl+Shift+O

Open a text document in the tabbed pane.

Also in Resources > Notepad submenu.

**Open image document…**	Ctrl+Shift+I

Open an image file in the tabbed pane.

Also in Resources > Notepad submenu.

**Open memory…**	Alt+Shift+O

Browse for an existing translation memory file.

Also in Memory menu.

**Open project…**	Ctrl+O

Browse for an existing translation project. The current active project will be closed upon opening a different project.

Also in Project menu.

**Preview current document**	Alt+D

Open a preview copy of the current document in an external program.

Also in Project menu.

**Print**	Ctrl+P

Print the contents of the currently-selected tab.

Also in Resources > Notepad submenu.

**Project source segments**	Ctrl+Shift+F2

Search project source segments for contents of current selection in the source segment editor.

Also in Edit > Find at cursor submenu and through the dedicated Project source button in the Quick search bar.

**Project statistics**	Ctrl+E

Display general project statistics.

Also in Project > Statistics submenu.

**Project target segments**	Ctrl+Shift+F3

 Search project target segments for contents of current selection in the source segment editor.

Also in Edit > Find at cursor submenu and through the dedicated Project target button in the Quick search bar.

**Quick search…**	Ctrl+Shift+F

Toggle the display of the Search bar to look up quickly in the project and resources.

Also in Edit menu.

**Record/list selected words**	F5

 Toggle word recording. While recording, pressing F5 will save the selected word to a list for later reference. Pressing F5 with no selection will list the saved words.

Also in Edit menu.

**Reload glossary**	Ctrl+Shift+L

Reload the currently-selected glossary from disk.

Also in Glossary menu and the Glossary context-menu (right click).

**Remove defined character to the left**	Ctrl+Shift+Comma

Remove the characters defined in Edit-> Options-> General-Characters for removal, but only to the left of the cursor.

Also in Edit > Target segment submenu.

**Remove defined characters**	Ctrl+Shift+Period

Remove the characters defined in Edit-> Options-> General-Characters for removal from the entire target segment.

Also in Edit > Target segment submenu.

**Remove from auto-completion list**	Ctrl+Shift+R

Remove the highlighted suggestion from the auto-completion drop-down list. Just navigate to the suggestion you wish to remove (using the up or down arrow keys, or via a single left click) and press Ctrl+Shift+R.

Not found elsewhere.

**Remove tags**	Ctrl+Shift+Slash

Removes all tags in the target segment.

Also in Edit > Target segment submenu.

**Repeat last QA check**	Ctrl+L

Perform the most recent QA check again. Useful to re-check after correcting issues that may have caused a prior QA check failure.

Also in QA menu.

**Replace characters at source transfer**	Alt+R

Replace characters defined in Edit> Option> Workflow tab> Replace characters at source transfer.

Also in Resources > Non-translatable fragments submenu.

**Replace with alternative spelling**	Ctrl+Space

Cycle through possible alternate spellings or replacements for the word immediately preceding the cursor.

Also in Edit menu.

**Request focus in target segment editor**	Ctrl+Shift+F12

Focus the target segment editor.

Also in View > Segment editors submenu.

**Resource**	Ctrl+Shift+F1

Also in Edit > Find at cursor submenu and through the dedicated Resources button in the Quick search bar.

**Save all memories**	Alt+Shift+S

Save all open translation memories to disk.

Also in Memory menu.

**Save project**	Ctrl+S

Save the project. Glossaries are also saved, but translation memories are saved separately; they are configured to be automatically or manually saved.

Also in Project menu.

**Select next tab**	Ctrl+Period

Select the next resource tab.

Also in View menu.

**Select previous tab**	Ctrl+Comma

Select the previous resource tab.

Also in View menu.

**Show alternative spelling**	Context Menu

 Display a list of possible alternate spellings or replacements for the word immediately surrounding or preceding the cursor.

Also in Edit menu and with right click or context menu button on red underlined word.

**Split segment**

 Split the currently-selected segment into two. The segment will be split at the current cursor location in the source segment editor above.

Also in Action menu and dedicated button in the target language box.

**Subscript**	Ctrl+Shift+B

Also in Edit > Target segment submenu and through the context menu (right click) when in the target language box.

**Suggest phrase**	Ctrl+Down

Suggest a a term or phrase at the caret position in the target segment (opens the Auto-complete menu, if available).

Also in Translate menu.

**Superscript**	Ctrl+Shift+P

Also in Edit > Target segment submenu and through the context menu (right click) when in the target language box.

**Surround with characters 1**	Ctrl+Shift+Quote

Surround the selected text with the characters defined in Edit-> Options-> General-> Surround with characters 1.

Also in Edit > Target segment submenu and through the context menu (right click) when in the target language box.

**Surround with characters 2**	Ctrl+Shift+Close Bracket

Surround the selected text with the characters defined in Edit-> Options-> General-> Surround with characters 2.

Also in Edit > Target segment submenu and through the context menu (right click) when in the target language box.

**Surround with characters 3**	Ctrl+Shift+Open Bracket

Surround the selected text with the characters defined in Edit-> Options-> General-> Surround with characters 3.

Also in Edit > Target segment submenu and through the context menu (right click) when in the target language box.

**Total Recall source segments**	Ctrl+Shift+F6

Search Total Recall source segments for contents of current selection in the source segment editor.

Also in Edit > Find at cursor submenu and through the dedicated TR source button in the Quick search bar.

**Total Recall target segments**	Ctrl+Shift+F7

Search Total Recall target segments for contents of current selection in the source segment editor.

Also in Edit > Find at cursor submenu and through the dedicated TR target button in the Quick search bar.

**Transfer current tag**	Alt+9

Transfer the current tag in the list of tags from the source segment to the target segment.

Also in Action > Tags submenu.

**Transfer Google MT**	Alt+K

Transfer Google Translate MT result to the target segment editor.

Not found elsewhere.

**Transfer Microsoft MT**	Alt+J

Transfer Microsoft Translator MT result to the target segment editor.

Not found elsewhere.

**Transfer MT from web page**	Alt+V

Transfer the result of the machine translation on the selected MT website to the target segment editor. The transfer action can also be used when editors binding is off. See also [Machine Translation with MT Web Resources](https://cafetran.freshdesk.com/support/solutions/articles/6000186533-machine-translation-with-mt-web-resources).

Also in Translate menu.

**Transfer MyMemory MT**	Alt+H

Transfer MyMemory MT result to the target segment editor.

Not found elsewhere.

**Transfer source segment**	Alt+I

Transfer the (selected) source segment editor contents directly to the target segment editor.

Also in Translate menu.

**Transfer Yandex MT**	Alt+Y

Transfer Yandex Translate MT result to the target segment editor.

Not found elsewhere.

**Translate selected fragment**	Alt+Enter

Perform a resource search for the full source segment, or for a highlighted portion.

Also in Translate menu.

**Transpose selection to the left**	Ctrl+Shift+T

Moves the current selection to before the previous word.

Also in Edit > Target segment submenu.

**Transpose selection to the right**	Ctrl+T

 Moves the current selection to past the next word.

Also in Edit > Target segment submenu.

**Underline**	Ctrl+U

Also in Edit > Target segment submenu and context menu (right click) in the target language box.

**Zoom +** (Shift+Enter)	Ctrl+Shift+U

Also in View > Font submenu.

**Zoom -** (Ctrl+Shift+Y)	Ctrl+Shift+Y

Also in View > Font submenu.

## LIST OF CHANGES

- 20171107 File creation
- 20171130 Updated for CafeTran Espresso 2018 - Forerunner - 20171130
- 20180217 Updated for CafeTran Espresso 2018 - Akua, Migrated from Classeur.io to GitHub.com

## Feedback

You can send me feedback via a [ProZ message](https://www.proz.com/?sp=mailsend&eid_s=2042360). Please start your subject with the name of the document: “CafeTran - Preferences”.
