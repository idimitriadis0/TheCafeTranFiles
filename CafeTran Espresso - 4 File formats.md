# CAFETRAN ESPRESSO - FILE FORMATS

*Updated for CafeTran Espresso 11 Poppy Seed Roll (2022)*

This document: (1) covers natively supported file formats in CafeTran, (2) provides compatibility information for external bilingual projects (files and packages), and (3) discusses solutions to handle not yet supported file types.

## 1. SUPPORTED FILE FORMATS AND WORKFLOWS

Be it office suite documents, web, DTP, AutoCAD or localization file types, CafeTran supports natively a variety of different file formats with its default “**Translate document**” workflow.

It also offers a “**Multiple document folder**” option that allows you to translate and filter multiple files and file types within a folder (which may include nested folders).

With its “**Translate external projects**” workflow, CafeTran lets you further leverage its advantages as well as your own resources by handling a host of bilingual files and packages that originate from other CAT tools, all without leaving your favorite program.

This wide compatibility with external bilingual files may come in handy if you wish to prepare files on a different CAT tool which handles **file types not yet supported by CafeTran** or offers **additional filter options** for already supported formats, so that you can widen your net even more while still performing the bulk of the translation in CafeTran.

Finally, additional workflows make it possible to translate images and scanned/paper documents (“**Translate Paper document**”), work with PDFs and source document edited directly at the application designed for this document type (**Translate through Clipboard**), edit and perform maintenance tasks on TMX memories (**Edit Translation Memory**) or quickly align short documents to produce reference TMs (**Align two documents**).

## File formats overview

![CafeTran Espresso - Supported file formats](https://i.imgur.com/WmHwk4T.png)

**CT uses a native filter for external formats marked with an asterisk.*

*Note: The external projects compatibility list does not reflect an official statement.*

## CafeTran’s own file formats

CafeTran embraces easy formats and open standards for its own internal operations. It uses:

 - **Projects**: industry standard **XLIFF** (XML Localization Interchange File Format) files
 - **Translation Memories** and fragment bases: **TMX** (Translation Memory Exchange) files
- **Segmentation rules**: **SRX** (Segmentation Rules Exchange) file format
 - **Glossaries**: simple **tab-delimited TXT** files

It also features a powerful **TMX editor** and can import **TBX** (TermBase Exchange) glossaries, among many other resource types.

CafeTran can export any native project to a compressed **CTP package** Project > Export and exchange > To Package. This zipped file contains the project’s XLIFF, the source files, the TMX and glossary files, as well as any other document contained in the project folder (exported target files, bilingual review documents, etc.) for easy sharing.

Last but not least, CafeTran offers an excellent **Export bilingual document (.docx)** (with or without notes) feature for native projects, which allows you to review the translation in a DOCX file and import the changes and additional notes back into CafeTran. External projects can also benefit from the same feature (minus the import functionality), and all projects can be Exported to HTML (along with other formats), which produces a bilingual table with notes in an HTML file that can be viewed in MS Word or OpenOffice/LibreOffice Writer.

## CafeTran’s File type filters

![File type filters](https://i.imgur.com/nEzYovO.png)

Here is the list of native file type filters CafeTran offers when creating a new project (“Translate document”):

 - Text (.txt)
 - LibreOffice (.odt/ods/odp/odg)
 - MS Word (.docx/xml)
 - MS Word OCR (.docx/xml)
 - MS Excel (.xlsx)
 - MS PowerPoint (.pptx)
  - iWork (.pages/key/numbers)
  - XML
  - HTML
  - XML/HTML with tags
 - AbiWord (.abw)
 - MS Word Uncleaned (.docx/xml)
 - LibreOffice Uncleaned (.odt)
 - AutoCAD (.dfx)
 - InDesign (.inx)
 - InDesign (.idml)
 - FrameMaker (.mif)
 - Subtitles (.srt)
 - Subtitles (.itt)
 - Java Properties (.properties)
 - Windows .NET Resources (.resx)
 - Mac String Resources (.strings)
 - String resource header (.loc)
 - DTP Tagged Text
 - Tagged MS Excel (.xlsx)
 - Transit XML File
 - Vector image (.svg)
 - Image (.jpg/gif/bmp/png) or Paper

## File types in detail

Supported file types are discussed in more detail in this section. Additional information will be added later on, as needed.

### Microsoft Office

Only files from MS Office 2003 and later (.docx, .xlsx, .pptx) are natively supported by CafeTran.

For .doc, .xls and .ppt formats, check the Unsupported formats section below.

Password-protected files are not imported. You need to remove the protection before importing them into CafeTran.

#### MS Word (.docx)

Notes:

- MS Word files containing macros **.docm** are also handled via this filter (although the file type might need to be selected manually).
- Hidden content is not imported into CafeTran, which can be an effective solution for filtering out content that you don't wish to translate. Just remember to unmask hidden content when done. You can also use the TransTools Word add-in to [Hide/Unhide Text](https://www.translatortools.net/docs/transtools/hide-unhide).
- CafeTran filters out of the deleted text in Ms Word source documents with the track changes enabled.

#### MS Word OCR (.docx/xml)

CafeTran offers a special filter to handle MS Word documents after OCR, which clears the source text of unnecessary formatting tags.

Note: You can also use this filter anytime the MS Word document produces many unnecessary tags.

Alternatives for tag cleaning:
[CodeZapper](http://asap-traduction.com/CodeZapper) (MS Word add-in)
[TransTools- Tag Cleaner](http://www.translatortools.net/word-doccleaner.html#TagCleaner) (MS Word add-in). Tag Cleaner is part of the [TransTools](http://www.translatortools.net/about.html) suite featuring many useful utilities for preparing different Microsoft Office documents.

Related links:
[Handling Tag Soup](https://cafetran.freshdesk.com/support/solutions/articles/6000160720-handling-tag-soup)
[Word Documents After Optical Character Recognition](https://cafetran.freshdesk.com/support/solutions/articles/6000112413-word-documents-after-optical-character-recognition)

#### MS Word Uncleaned (.docx/xml)

Use this filter for Trados RTF/DOC Uncleaned documents (converted to DOCX). Uncleaned documents from other tools should work as well, please report if otherwise.

#### MS Excel (.xlsx)

Notes:

- MS Excel files containing macros **.xlsm** are also handled via this filter (although the file type might need to be selected manually).


![Excel file filter options](https://i.imgur.com/bX9Qhep.png)
- When you choose the **Excel filter**, you have access to the following Filter options:

   - **Import source column**: allows you to specify from which column(s) to import source text
    - **Import target column**: allows you to specify from which column(s) you wish to import content in the translated segments. Empty cells are also imported, so not all cells need to have content. Note: If you define two Excel columns for import separately (in two Import fields of the filter), the second column is to be imported for the review of the existing translation. If you specify two import columns separately, leave the export column empty.
    - **Import notes column:** allows you to define a column that will be imported in the form of Notes in CafeTran.
    - **Export column**: allows you to specify to which column(s) you want to export your translation.
    - **No segmentation in cells**: If enabled, this option treats each cell as a segment, overriding any segmentation settings.
 - If no Filter option is set, CafeTran loads the entire Excel content, and translation will replace the source text. Likewise, if no export column is set, translation will replace the source text.
- CafeTran imports only visible (not hidden) columns, rows or sheets. Hiding these in Excel before starting a project allows you to filter out content that you don't wish to translate.
- [Custom formatting](https://github.com/idimitriadis0/TheCafeTranFiles/wiki/2-Menu-and-Interface#edit--target-segment-submenu) (including bold, italics, underline, subscript and superscript) is supported in Excel projects.
- Suggestion: If you use Filter options, export a file preview (Project > Preview current document) early on to make sure the content is exported as expected.

#### Tagged MS Excel (.xlsx)

The Tagged MS Excel filter is designed for handling certain GUI resource file types using XML/HTML code, where strings are surrounded by tags.

Note: The final file should be checked against any missing parts in code, as some HTML codes can be interpreted or deleted.

#### MS PowerPoint (.pptx)

### LibreOffice

#### Writer (.odt)

Notes: CafeTran filters out of the deleted text in LibreOffice source documents with the track changes enabled.

#### LibreOffice Uncleaned (.odt)

Use this filter for Trados RTF/DOC Uncleaned documents (converted to ODT). Uncleaned documents from other tools should work as well, please report if otherwise.

#### Calc (.ods)

#### Impress (.odp)

#### Draw (.odg)

### AbiWord (.abw)

### Apple iWork

To translate Apple iWork documents, you need to save them in the older Pages/Numbers/Keynote ’09 file format:

Upon creating a CafeTran project using the iWork filter, you will get a dialog. Just choose the *index.xml* file and press OK to load the segments.

Related links:
[Open older iWork files in newer versions of Pages, Numbers, and Keynote](https://support.apple.com/en-us/HT203997)

#### iWork Pages (.pages)

[Import and export different file formats with Pages](https://support.apple.com/en-us/HT202227)

#### iWork Numbers (.numbers)

[Import and export different file formats with Numbers](https://support.apple.com/en-us/HT205391)

#### iWork Keynote (.key)

[Import and export different file formats with Keynote](https://support.apple.com/en-us/HT202220)

### Web localization/XML files

#### XML

Suggestions:

- Enabling Preferences > Segment at all tags along with your segmentation rules might be a good solution for some XML files.
- Since this file type does not yet support filter options, if the text to be translated is not displayed or filtered in CafeTran, you might need to use an external tool (such as Memsource, memoQ, Okapi Framework, etc.) to prepare the XML file (see tools in Solutions section).

#### HTML

This filter also handles XHTML files.

Notes:

- CafeTran does not recognize the alt tag.
- With CafeTran's internal segmentation rules, links and their attributes are editable.

Suggestions:

- Since this file type does not yet support filter options, if the text to be translated is not displayed or filtered in CafeTran, you might need to use an external tool (such as Memsource, memoQ, Okapi Framework, etc.) to prepare the HTML file.

#### XML/HTML with tags

Choose this filter to include the text inside the XML/HTML tags to the displayed segments.

#### Transit XML File

See PPF and Transit XML files under External projects section.

#### Tagged MS Excel (.xlsx)

The Tagged MS Excel filter is designed for handling certain GUI resource file types using XML/HTML code, where strings are surrounded by tags.

Note: Final file should be checked against any missing parts in code, as some HTML codes can be interpreted or deleted.

### DTP

#### InDesign (.inx)

InDesign Interchange (INX) is an older format, primarily used for saving documents back to a previous version of InDesign (CS3).

Note: For handling Adobe InDesign **INDD** files directly, see the Unsupported formats section.

#### InDesign (.idml)

The Adobe InDesign Markup Language (IDML) format replaces the Interchange (INX) format used for saving backwards in previous versions.

While INDD represents the extension given to all InDesign files created in the standard way in any version of the design software, IDML (InDesign Markup) is an XML format which allows users of different versions of InDesign to open up the file without a problem.

Typically, IDML files are smaller than INDD files, since non-embedded images aren’t included. IDML is the standard format for translating InDesign files.

Note: For handling Adobe InDesign **INDD** files directly, see the Unsupported formats section.

#### FrameMaker (.mif)

Adobe FrameMaker is an authoring and publishing solution for XML and Maker Interchange Format (MIF) is the markup language Adobe FrameMaker uses for technical document.

#### DTP Tagged Text

CafeTran handles Quark Express DTP Tagged Text files.

<!--- TODO --->

#### Vector image (.svg)

Scalable Vector Graphics (SVG) is an open standard XML-based vector image format for two-dimensional graphics with support for interactivity and animation.

SVG images and their behaviors are defined in XML text files. They can be produced by Inkscape [free and open source software], Adobe Illustrator, Adobe Flash Professional, or CorelDRAW, and rendered to common raster image formats such as PNG using the same software.

NOTE: Since Adobe Illustrator can import and export SVG files, an SVG filter can help handle Adobe Illustrator files (*.ai or *.eps) as well as DWG or CAD files, exported to SVG by Adobe Illustrator. For handling AI files using the SVG file filter, see the Unsupported formats section.

### AutoCAD

AutoCAD, developed by Autodesk, Inc. and first released in December 1982, is a software application for computer-aided design (CAD) and drafting that supports both 2D and 3D formats.

#### AutoCAD (.dxf)

A DXF (Drawing eXchange Format) file is a type of drawing interchange file used to transfer data between various applications. It is either a binary or an ASCII representation of a drawing file, often used to share drawing data between other CAD programs.

In AutoCAD, you can convert a DXF file to DWG format by opening the file and saving it in DWG format. You can then work with the resulting drawing file as you would with any other drawing file.

[Exporting a DXF file](https://knowledge.autodesk.com/support/autocad-lt/learn-explore/caas/CloudHelp/cloudhelp/2018/ENU/AutoCAD-LT/files/GUID-5EA0F1DC-EA92-4ADB-9BDF-C352DF3AFC5F-htm.html) in AutoCAD.

Be sure to visit the Filter options tab in the New document creation dialog, in order to check which of the available layers you wish to filter.

![AutoCAD file filter options](https://i.imgur.com/QvjN420.png)

NOTE: For handling the binary **DWG** files, see the Unsupported formats section.

### Software localization

CafeTran provides some filters that allow you to localize various mobile and desktop software applications.

#### Java Properties (.properties)

Java Properties files are simple text files that are used in Java applications.

You can localize these within CafeTran with the help of this file filter.

#### Windows .NET Resources (.resx)

The file filter for NET XML Resource Template (.resx) files can be used for localizing .NET and Windows Phone applications.

#### Mac String Resources (.strings)

The Mac String Resources filter can be used to localize iOS or OS X applications.

The ’/* comments */’ in .stringd are displayed as Notes in CafeTran.

#### Android (and other) XML files (.xml)

The XML filter can be used to localize Android applications, among other content (since XML can have various applications).

#### String resource header (.loc)

String resource header files are used for localization of programs written in C or C++ language.

### Subtitles

Subtitling offline or online software is often used not only to create, edit, and time code, but also to translate subtitles, including SubRip files, because it integrates video and audio context and offers various features specific to subtitling.

For those wishing to translate subtitling files in CafeTran Espresso, the developer has recently added support for SRT and ITT files. The program can also open videos (Resources > Open movie) and offers access to YouTube as a Web resource (Resources > Web > YouTube).

Note: Split and Join segments actions are disabled during the translation of subtitles, to avoid any resulting timing issues.

#### Subtitles (.srt)

SubRip Text files.

#### Subtitles (.itt)

iTunes Timed Text files.

### Paper document workflow

#### Image (.jpg/gif/bmp/png)

Images and scanned documents can be translated with the help of the “Translate Paper document” workflow.

For an OCR approach to images, see the PDF > OCR section in Unsupported formats.

Related links:
[Translation of Scanned Images](https://cafetran.freshdesk.com/support/solutions/articles/6000111566-translation-of-scanned-images)
[Translation of Paper Documents](https://cafetran.freshdesk.com/support/solutions/articles/6000111789-translation-of-paper-documents)

## 2. EXTERNAL PROJECTS

Intercompatibility (both in and out) is an important CafeTran Espresso feature. “Translate external project” workflow lets you handle a host of bilingual files and packages that originate from other CAT tools, all without leaving your favorite program. This section offers details on different external bilingual project types.

### GENERAL NOTES ON BILINGUAL XLIFF FILES

“Translate external project” workflow presents some differences when compared to the native “Translate document” workflow. Here are some of these differences you may want to consider:

- **Export target file format**. For external projects, CafeTran does not export to the original target language document file format. Instead, it Finalizes the edited bilingual file(s). To final target file export is generally done by the client who created the translation project in their tool (or, in some cases, by the translator, if they use the same tool). This is a general limitation and is not inherent to CafeTran.
- **Export target file Preview**. For the same reason as above, CafeTran does not export a target file Preview for external projects.
- **Segmentation**. For external projects, CafeTran does not handle the segmentation phase as this takes place at the bilingual file creation. If you open an unsegmented file, CafeTran will show a warning message. Ask for properly prepared (segmented) files.
- **Split/Join** segments. CafeTran only supports **virtual joining of segments** in external projects. The feature allows to join segments in segments’ editor and rearrange their contents comfortably. As soon as the joined segments leave the editor, their number is the same as before joining but their respective text contents is changed (rearranged), hence the virtual aspect of this feature. Make sure you keep the added tags intact.
- **Project creation**. For native projects, CafeTran creates a Project folder, copies the source documents and generates a segmented native XLIFF, which it opens for translation. For external projects, **CafeTran edits the external bilingual files directly at their own directory location**. Make sure you have a copy if needed.
- **Project memory/Project glossary**. If Project memory and/or Project glossary are checked in the Dashboard when opening an external project, the ProjectTM.tmx and ProjectTerms.txt files are conveniently created and placed at the same working folder.
- **Packages**. Supported packages (.sdlppx, .mqxlz) are expanded and edited at the working folder location. To reopen an already expanded package, just drag and drop the package file once again. You can export a package (or return package) via Project > Export and exchange > To Package.
- The Export button becomes a **Finalize button** in CafeTran’s segments grid. This sets the Checked status (corresponds to Translated in Trados/Confirmed in memoQ) to all target segments and saves the project. Generally, this step should be performed prior to delivering the files. Note: If you need to keep a different status for some segments than the translated status, DON'T use the Finalize button. Instead, filter the segments you want to set as Translated, and apply the Task > Set translated status for target segments.
- **QA > Tags check** must be performed prior to finalizing the project, to ensure no tag issues are present in the delivered files. It is also recommended to run the **QA > At tags spaces check**.
- **TM match marks**. The translation memory match values are not stored in non-CafeTran project. They are available for the current session only, unless the projects provide their own values.
- **Segment statuses**. CafeTran attempts to map its own additional segment statuses (Checked, Approved, Locked) to the statuses applied by the external tool. More information can be found in each tool’s section below.
- **Segment Notes (Comments)**. CafeTran generally maps its Notes feature to the Comments supported by external tools. More information can be found in each tool’s section below.
- **Extra formating tags** (bold, italics, underline) cannot be added, contrarily to native projects. Additional formatting will need to be conducted at final document export.
- **Export bilingual DOCX for review**. You can export bilingual DOCX files (with or without notes) for external review via Project > Export & Exchange menu. However, importing the changes directly back into CafeTran via Projects > Export & Exchange > Import bilingual file is reserved to native projects.
- **Auto-propagation** is supported (also across multiple files, if they are virtually glued together). However, the P and nP marks for auto-propagation and no propagation of individual segments are displayed **for the current session only**.
- Related links:
[Project File Formats Created in Other Tools](https://cafetran.freshdesk.com/support/solutions/articles/6000166523-project-file-formats-created-in-other-tools)

### Trados Studio

Trados Studio files and packages are very well supported in CafeTran.

CafeTran Espresso can also import SDLTM translation memories and SDLTB termbases, which are converted into the TMX format.

In addition to the general notes above, please consider the following **known limitations**:

- Tags at the start of the source segment cannot be moved around in the target segment.
- Trados Comments are shown as Notes in CT and CT Notes are imported as Comments in Trados Studio (but do not get the levels FYI, Warning, and Error). In CT, segments with Notes/Comments have a leading and an ending tag. This is normal.
- Alternative translations work for the current session only in Studio projects. If they interfere with Trados, you can try removing them via Task > Remove alternative translations in CafeTran.

**Supported features**:

CafeTran is capable of displaying basic formatting (bold, underline and italic) in the Grid for Word-based sdlxliff files.

**Segment status**:

In the screenshot below, you see how the various [Trados statuses](https://docs.rws.com/813470/575898/trados-studio-2021-sr2/segment-status-column) (also [here](https://docs.rws.com/813470/344740/trados-studio-2021-sr2/translation-statuses)) mentioned in the green Notes are displayed in CafeTran.

![Trados statuses in CafeTran Espresso](https://i.imgur.com/DoI5PFX.png)

- "Translated" segments in Trados get the "Checked" status in CafeTran (gray background in segments, plus simple gray background in segment number) and vice versa. This is the status segments get when you press the Finalize button in CafeTran.
- "Translation approved" segments in Trados appear as "Approved" in CafeTran (gray segment background, plus gray segment number background with green frame).
- "Translation rejected" segments in Trados appear as "Rejected" in CafeTran (no segment background, plus gray segment number background with red frame).
- "Signed-off" segments in Trados do not have a specific status in CafeTran.
- "Sign-off rejected" segments do not have a specific status in CafeTran.
- "Locked"/"Complete Sign-off" (marked with PM and a lock in Trados) have the Locked status in CafeTran.
- Context Matches (CM) and 100% matches have the 100% match status in CafeTran.
- Fuzzy matches in Trados have the same match mark in CafeTran (but this is not so the other way around).
- You have the option to omit setting the Translated status for target segments during the export to .sdlrpx packages and apply a statuses to filtered segments.

Note: If you mark Studio segments as Locked in CafeTran, this status is active for the current CT session only. The CafeTran status does not interfere with the locked segment status (Complete sign-off) that is set in Studio by the project manager.

**Track changes:**

Trados review jobs that rely on **Track changes** feature should be able to be performed in CafeTran.
 This feature is available via the Edit >  Track Changes > Manage menu. See the Changes tab after activation.  There, you can Accept and Reject changes to the current target segment. CafeTran does also map Translator Approved and Translator Rejected Trados statuses.
- Filtering on tracked changes can be done via the Filter menu.
- Accepting or rejecting all tracked changes in one task is done via the Task menu.

**Known Workarounds:**

- If Trados files that have been Finalized in CafeTran do not get the Translated status back in Studio (they show as untranslated in the statistics, although their segments have the “translated” icon), just run Batch Tasks > Translation Count on the project to get the Translated status to 100%. This information can be shared with the PM if needed, as it requires virtually no effort.

#### SDLXLIFF

SDLXLIFF is the Trados version of the bilingual XLIFF format. Please refer to the above general notes on bilingual XLIFF files and read more specific details concerning Trados files in CafeTran.

#### SDLPPX

- **Opening SDLPPX packages**
When you drag and drop an SDLPPX package on CafeTran’s Dashboard, the program unpacks it automatically and loads the included SDLXLIFF files, and imports any attached SDLTM translation memory and SDLTB termbase (including multiple SDLTM or SDLTB files) in the form of a (read-only) TMX memory.

You need to check the unpacked package to see if it contains any additional material that could be useful to you (reference material, project analysis, etc.).

- **Exporting SDLPPX packages**
After you finish the translation of SDLPPX package, finalize it and export it back to package via Project > Export > To package. Then, you have two options for the export: Project package or Return package.

The translated return package (SDLRPX) should be opened in Trados Studio which created the normal (SDLPPX) package. If you did not create this project yourself, export to as a normal project package (SDLPPX) to review it in your installation of Trados Studio.

#### SDLTM translation memories

CafeTran handles SDLTM translation memories, which are imported as <u>read-only</u> TMX files in CafeTran. The process is very quick and painless.

You can do so manually via Memory > Import > Import SDLTM memory or simply Memory > Open memory.

SDLTM files present in Trados packages (SDLPPX) are automatically imported as a TMX in CafeTran when you open a package. The TM options dialog is shown, allowing you to fine-tune their options or apply additional filtering. All SDLTM files present in the package are joined together during the import. To open them separately, use the manual process above.

In the SDLTB section below, you can find external utilities that also handle SDLTM conversion.

#### SDLTB termbases

CafeTran handles SDLTB terminology files, which are imported as TMX termbases into CafeTran.

You can do so manually via Memory > Import > Import SDLTB termbase.

SDLTB files present in Trados packages (SDLPPX) are automatically imported as a TMX in CafeTran when you open a package. The TM options dialog is shown, allowing you to fine-tune their options or apply additional filtering. All SDLTB files present in the package are joined together during the import. To open them separately, use the manual process above.

If you prefer to convert the imported SDLTB termbase to the glossary format, proceed as follows: After importing the SDLTB, select the glossary in which you wish to import the converted entries, then go to Memory > Export > Export segments to glossary. You will be asked to select the memory you wish to export from in the next dialog.

**External SDLTM and SDLTB conversion utilities**

Although their use is now redundant, since CafeTran already handles SDLTM and SDLTB files on its own, here are some additional utilities that offer SDLTM and SDLTB conversion capabilities outside CafeTran:

- Van Nellen’s [Trados Studio Resource Converter](https://closedtags.com/trados-studio-resource-converter/) is a free cross-platform Java app that offers conversion from both SDLTM and SDLTB files.

![Trados Studio Resource Converter](https://i.imgur.com/hbnHVoS.png)

 Steps to convert a SDLTB in Trados Studio Resource Converter:
 - Click on “Convert SDLTB” button.
 - Navigate to the file’s directory and select the SDLTB file.
 - Select “Tab-separated TXT” in the “Please select the output type” dialog.
 - Select “Separated by a pipe (|)” in the “Please select how synonyms should be presented” dialog.

- [WfConverter](http://wordfast.fi/blog/cat-tools/2012/11/03/convert-sdltm-and-sdltb-without-studio-and-multiterm/) by Jean-Philippe Odent.
- [Glossary Converter](http://www.cerebus.de/glossaryconverter/index.html), available as an Trados plugin and as a standalone Windows program. It can serve to convert term bases from and to SDLTB.
- [XBench](https://www.xbench.net/) QA and Terminology Management tool version 3.x (paid, yearly licencing plan) can open SDLTB files and convert them to either TMX or tab -delimited TXT format.

#### TRADOS UNCLEAN RTF/DOC

These older Trados files should be handled with the MS Word Unclean file filter, once you save them as DOCX files.

If you own a Trados licence, you can also use the [SDLXLIFF to Legacy Converter](http://appstore.sdl.com/language/app/sdlxliff-to-legacy-converter/134/) to deal with those using a round trip.

#### TRADOS WORKBENCH - TTX

TRADOStag files (TTX) are bilingual files used in Trados TagEditor, part of SDL’s legacy tool called Trados Translator’s Workbench.

These files need to be pre-segmented (Tools > Translate > Segment unknown sentences in Trados) before you can translate them in CafeTran.

The process is described in detail in this [article.](http://www.necco.ca/dv/trados.htm#Segmenting_Trados_Files)

#### TRADOS WORKBENCH - RTF

Trados Workbench unclean RTF files should be handled with the MS Word Unclean file filter, once you save them as DOCX files. These should have been pre-segmented first in Trados Workbench.

<!--- #### WORLDSERVER PACKAGES - WSXZ / GroupshareTODO --->

#### IMPORTING CAFETRAN’S TMX TO STUDIO

You can import CafeTran’s and other TMX translation memories to Trados Studio using the Import wizard. Imported data contains translation units with their associated fields.

In order to import data into a translation memory, the translation memory must already exist and be displayed in the navigation pane.

To display this wizard for the active translation memory, select File > Import from the menu bar in the Translation Memories view.

Related links:
[Overview: Importing and Exporting Translation Memory Data](http://producthelp.sdl.com/sdl%20trados%20studio/client_en/TM_View/TM_Data/Importing_Exporting_TM_Data/O_ImExpTM.htm),
[Overview: Import Wizard](http://producthelp.sdl.com/sdl%20trados%20studio/client_en/Ref/H-N/Import_Wizard.htm)

#### CONVERTING CAFETRAN GLOSSARIES TO SDLTB

[Glossary Converter](http://www.cerebus.de/glossaryconverter/index.html), available as an Trados plugin and as a standalone Windows program can be used to convert CafeTran glossaries into SDLTB term bases. It needs to be set up correctly before the conversion. Instructions to follow.

<!--- TODO LATER --->

### memoQ

memoQ’s MQXLIFF and MQXLZ files are well supported in CafeTran, although MQOUT packages require additional care.

**Segment status:**

- Edited and/or Pre-translated segments in memoQ appear as Translated in CafeTran.
- (Translator) Confirmed segments in memoQ are marked as Checked in CafeTran. Finalizing in CafeTran will set the status of all segments to Translator Confirmed in MemoQ.
- Warning: 100% segments in memoQ are invisible in CafeTran. Have the original file and/or a bilingual RTF table at hand for context.
- Warning: Locked segments in memoQ are invisible in CafeTran. Have the original file and/or a bilingual RTF table at hand for context.

<!--- TODO LATER **Known workarounds:** --->

#### MQXLIFF

MQXLIFF is a memoQ-flavored XLIFF file format. It is well handled by CafeTran (please refer to the above general notes on bilingual XLIFF files and read more specific details concerning memoQ).

Notes: 

- CafeTran now displays the match percentage for the target segments included in .mqxliff translation projects.
- Context notes are shown in as Notes in the Grid in MQXLIFF projects.

#### MQXLZ

MQXLZ are memoQ’s zip packages containing MQXLIFF files. MQXLZ files are unpacked for translation and zipped back by CafeTran via Project > Export and exchange > To Package (without overwriting the original [unpacked] .mqxlz package file).

#### MQOUT

MQOUT are memoQ’s project packages.

There are several ways to receive MQOUT packages. By e-mail or another electronic mean, in memoQ via Project > Check Out Online Project, or on a web browser, via WebTrans.

NOTE: As described below, handling MQOUT requires some additional steps, which may represent a hassle. If possible, ask to receive MQXLZ (or MQXLIFF) files and TM/TB separately, and to simply send back the translated MQXLZ or MQXLIFF files.

*The following is based on a memoQ Package Guide. *

A memoQ handoff (.mqout) package is a zip in disguise. Unzipping it reveals at least three subfolders:

 - Translation documents = Contains the documents to be translated, in a zipped XLIFF format (MQXLZ) which includes the MQXLIFF files. You do not need to unpack the MQXLZ file, CafeTran does it for you. Just drag and drop it on the Dashboard.
- TM = Contains the translation memories used in the project in TMX format, which can be imported and opened in CafeTran.
- TB = Contains the term bases used in the project, in CSV format. These require a small preparation before being able to import them in CafeTran.

 How to handle MQOUT packages:

- Unpack the contents of the .mqout file. Depending on your software, you may need to rename .mqout to .zip for that.
- Drag and drop the MQXLZ file (containing the MQXLIFF files) in CafeTran’s Dashboard, to start working on the project.
- Open the TMX files in CafeTran. Optionally set them as read-only, just for reference.
- Add the converted CSV term base as a CafeTran glossary (tab-delimited .txt file).
- Translate the project in CafeTran. Run QA.
- Save the translation with the Finalize button.
- Export .mqxlz package via Project > Export and exchange > To Package (without overwriting the original [unpacked] .mqxlz package file).
- You now need to create the handback file (.mqback), containing only the translated files, no TM or TB. This is described below.

Packing up the translated XLIFF files in a memoQ Handback (MQBACK) package:

 - When you have finished translating the XLIFF files, be sure to save them in a new, empty folder. Preferably, name this folder ProjectName.YourName. Then follow these steps:
    - In the original handoff package that you unpacked in Section 2.2, there is a file called HandoffPackageInfo.xml. Copy this file to the new folder, and rename the second copy to DeliveryPackageInfo.xml.
    - Open the new DeliveryPackageInfo.xml file in a plain text editor such as Notepad.
    - Delete almost all lines from the file, but do not delete the lines going from <?xml version="1.0"?> to the closing tag of HandoffPackageInfo.
    - In the file, change <HandoffPackageInfo to <HandoffDeliveryPackageInfo. Change <UserName to <User.
    - Save the file.
    - Create a zip file from the contents of this folder. (It should now contain the translated MQXLIFF files and the DeliveryPackageInfo.xml file.)
    - Compress the folder to a .zip. Rename the .zip file so that it is called Project-Name.YourName.mqback.
    - Send the file to your project manager. The project manager will be able to update the master project the same way as he/she would when he/she received a handback package directly from memoQ.

#### memoQ online projects

Information taken from the old wiki [old wiki](https://web.archive.org/web/20151018135237/http://cafetran.wikidot.com/translating-memoq-files):
- When handling online projects, many aspects depend on the export/import rights the PM assigns to you on the server settings.
- In some cases server files cannot be exported or cannot be re-imported. There is a simple trick to export and re-import server files: Simply click on Create view on the Document tab in memoQ. This view can be exported and re-imported.
- Please bear in mind that in most cases TMs and/or TBs cannot be exported from memoQ server projects. And the PM won't see any progress until you re-import your file.
- Note that memoQ translator free (the edition you get after your trial version ends) cannot be used in memoQ online projects, although it can be used for accepting jobs from a memoQ server.

<!--- TODO LATER check this section --->

#### memoQ bilingual RTF files

MQXLIFF, and MQXLZ files are the recommended way to receive memoQ projects in CafeTran. Please ask for one of these formats instead.

If you must translate bilingual RTF files exported  from memoQ in CafeTran, here is a suggested workflow ([see the original discussion](https://cafetran.freshdesk.com/support/discussions/topics/6000021149/page/2?url_locale=)):

- Convert RTF to DOCX (or ODT)
- Copy SL column in a second DOCX
- Import the second DOCX into CT
- Tell CT to copy source to target
- Export as bilingual document
- Paste target language into the second column of the exported document
- Import in CT
- QA
- Export finished translation
- Convert DOCX to RTF

Also see the RTF entry in Unsupported formats section below.

#### memoQ Translation Memories

memoQ Translation memories can be exported to TMX from a memoQ installation. TMX can also be used to import TMs into memoQ.

TMs included in MQOUT packages are already in the TMX format.

#### memoQ Term Bases

To prepare Term Bases exported via memoQ or received as CSV via a MQOUT package:

- Open the CSV file with a spreadsheet program (MS Excel, LibreOffice Calc, etc.).
- Look for the two columns that match your source and target language and copy them to a new worksheet, arranging them in that correct order (source terms - target terms).
- You can then copy-paste the two columns into a plain .txt file with UTF-8 encoding and open the file as a glossary in CafeTran (the first line of each column should include the language beginning with a #. Example: #en-US, #en-GB or #fr-FR, to match the language pair you are working on).

### Wordfast Pro

WFP 3 files are well supported in CafeTran, while WFP 4/5 currently less so.

#### WFP 3 - TXML

TXML is the bilingual file format used by Wordfast Pro 3.

It is supported by CafeTran, as part of the “Translate external project” workflow.

Notes:

- CafeTran supports comments in .txml files.
- CafeTran displays the match score information for the target segments included om .txml translation projects.

#### WFP 6 - TXLF

 Wordfast Pro 6 uses the TXLF bilingual file format.

This file format is handled by CafeTran, as part of the “Translate external project” workflow, with the following limitations.

TXLF notes are mapped as CafeTran notes.

**Segment status, known limitations:**

- Segments with confirmed/Unconfirmed and Locked status all show as simply Translated in CafeTran.
- Finalizing the TXLF file in CafeTran does not change the status in WFP 6.

#### WFP 6 - GLP

Wordfast Pro 5 zipped packages have the .glp file extension.

They are not handled directly by CafeTran and need to be expanded.

Translate the TXLF files contained in the folder bearing the same title.

#### RTF/DOC/DOCX Bilingual Review

These Wordfast Pro exported files are usually meant to be used for external review or for exchange with Wordfast Classic or for external review in MS Word. Whenever possible, ask for a TXML/TXLF file instead.

You may want to try CafeTran’s MS Word Uncleaned file filter if you wish to translate these files. If you do so, please report back.

Related links:
[Wordfast Pro 3 - Bilingual Export](https://wordfast.com/WFP3/PM_Using_PM_plug-in/Bilingual_review.htm),

[Wordfast Pro 6 - Biligual Export](https://www.wordfast.com/WFP/6.6/t3159441.html)

#### Wordfast TXT TMs

Memory > Import tab delimited memory menu option allows you to import segments from a Wordfast tab-delimited memory file to the selected translation memory in CafeTran.

Note: Wordfast Pro can also export its memory to the TMX format that CafeTran can open or import directly.

Related links:
[Exchanging TMX TMs with Non-Wordfast Users](https://www.wordfast.net/w/index.php/Exchanging_TMX_TMs_with_Non-Wordfast_Users)

#### Wordfast Glossaries

Wordfast Pro can export Glossaries as tab-delimited TXT files or TBX files. Both file formats are handled by CafeTran. Tab-delimited TXT might need some preparation, but is otherwise used as CafeTran’s native Glossary format. TBX can be imported via TMX in Memory > Import TBX terminology.

### Déjà Vu

[Atril’s Déjà Vu](https://atril.com/) CAT tool offers the [External View](https://atrilsolutions.zendesk.com/hc/en-us/articles/205447771-External-View-files) (EV), a format specifically created for the purposes of proofing and outsourcing translation work and one of the first implementations of bilingual review files.

Déjà Vu X3 Professional can export External View files to RTF and XLIFF. Proofed or outsourced files can then be imported back into Déjà Vu.

CafeTran can handle External View files, with some limitations, although it cannot be used to translate Satellite files and Pack & Go packages, as explained below.

Related links:
[Déjà Vu - External View](https://atrilsolutions.zendesk.com/hc/en-us/sections/201606291-External-View) (Contains seemingly outdated information about XLIFF availability in Déjà Vu X3 Professional, as opposed to Déjà Vu X3 Workgroup edition).

**Known limitations:**

- Déjà Vu Comments are not mapped to CafeTran's Notes.
- Déjà Vu segment statuses are not differentiated in CafeTran and CafeTran does not change their status back in Déjà Vu, even after the Finalize button is clicked (see below). You will need to change the segment status to Translated in Déjà Vu.

**Segment status:**

- Segments marked as Translated, Proofread, Approved, Pending, Do not send (or simply Edited, with no status) all appear as simply translated in CafeTran.
- Warning: Locked segments in Déjà Vu are invisible in CafeTran (there is also an option to Suppress Locked segments, etc. when exporting an External View file). Have the original file and/or a bilingual RTF table at hand for context.
- Segments with 100% matches are not marked as such in CafeTran.
- Finalizing segments in CafeTran does not set a specific status in Déjà Vu. Segments are shown as Edited (no status). Furthermore, previous status (Translated, Proofread, Approved, Pending, Do not send, 100% match) is kept, even if the segments have been edited in CafeTran. You will need to change the segment status to Translated in Déjà Vu.

**Known workarounds:**

- According to this [old wiki article](https://web.archive.org/web/20151018135232/http://cafetran.wikidot.com/translating-deja-vu-files), you can update comments to show CafeTran’s Notes in Déjà Vu by using an SQL command in Déjà Vu.
- According to the same article, If a project contains more than one file, check Project > Documents in CafeTran and glue all files as needed. By default the last file is selected.

#### External View XLF

CafeTran handles External View XLIFF files (and their tags), with the segment status limitations explained above.

#### External View bilingual RTF tables

RTF files are mostly meant for users without a translation tool. XLIFF is the preferred format for users of another translation tool. Please ask for a XLIFF file instead.

#### Déjà Vu Satellite files (.dvsat)

After a Déjà Vu X3 Workgroup project has been created and the external files have been imported, it is possible to generate satellite work files. The free version of Déjà Vu (after the Déjà Vu Professional 30-day trial ends) can be used to view and work on satellite projects sent by translation firms).

A satellite file contains only one source and one target language (as opposed to a full project file, which typically consists of the source language plus a number of target languages) with all the information needed by the translator. This information can exclude the formatting and image code, thus significantly reducing the file size and making it easier to transmit.

A satellite file contains a number of automatic restrictions. It is not possible to delete files, split/join rows, edit the source, or lock/unlock rows.

If the security options for the originating project file are enabled, users of the satellite files will have to log in with a user name and password. This will give them access to a predefined security level, which in turn will either permit or prohibit the overwriting of translation entered by other users or the project owner.

Once the translation of a satellite is finished, it can be sent back to the project owner who can import it into its parent project file.

Note: As per the above, DVSAT files can only be handled from within Déjà Vu. Ask your client whether they can send you XLIFF External View files instead.

Related links:
[Déjà Vu - Documentation - User manual](https://atrilsolutions.zendesk.com/hc/en-us/categories/200891162-Tutorials-and-Documentation)

#### Déjà Vu Pack & Go packages (.dvpng)

Pack & Go packages are highly compressed exports from project files that are ideal for the transmission of Déjà Vu X3 Professional data. The Pack & Go feature is available as a standalone feature for the transfer of complete projects, or as part of the satellite creation for the transfer of even smaller bilingual satellite projects.

Opening a Pack & Go package with Déjà Vu X2 or Déjà Vu X3 will start the Pack & Go Wizard, which will allow you to define where you want to have your new project stored. When the translation of the project is finished, you can once again export it into the Pack & Go format to transmit it back to the project owner.

Note: As per the above, DVPNG files can only be handled from within Déjà Vu. Ask your client whether they can send you XLIFF External View files instead.

[Déjà Vu - Documentation - User manual](https://atrilsolutions.zendesk.com/hc/en-us/categories/200891162-Tutorials-and-Documentation)

#### Déjà Vu TMs (.dvmdb)

Déjà Vu uses DBMDB access database files for its native TMs and can import or export TMX files (which can be used by CafeTran), among other formats.

If you don't have access to a Déjà Vu installation, you can open DBMDB database files in Excel after renaming them from .dbmdb to .mdb. XBench can also help convert these files.

Related links:
[Déjà Vu - How To Export A Translation Memory To TMX](https://atrilsolutions.zendesk.com/hc/en-us/articles/115004332365-How-to-export-a-Translation-Memory-to-TMX)
[Déjà Vu - How To Use A TMX File In Déjà Vu](https://atrilsolutions.zendesk.com/hc/en-us/articles/205379992-How-to-use-a-TMX-file-in-D%C3%A9j%C3%A0-Vu)

#### Déjà Vu TBs (.dvtdb)

Déjà Vu uses DVTDB access database files for its native TBs and can import or export tab-delimited TXT glossary files (which can be used by CafeTran), among other formats.

If you don't have access to a Déjà Vu installation, you can open DVTDB database files in Excel after renaming them from .dvtdb to .mdb.  XBench can also help convert these files.

Related links:
[Déjà Vu - How To Export A TB To CSV Format](https://atrilsolutions.zendesk.com/hc/en-us/articles/205456621-How-to-export-a-TB-to-CSV-format)
[Déjà Vu - How To Import A TXT Or CSV File Into A TB](https://atrilsolutions.zendesk.com/hc/en-us/articles/205382392-How-to-import-a-TXT-or-CSV-file-into-a-TB)

### STAR Transit NXT Professional+

CafeTran offers a native Transit XML file filter for handling [STAR Transit NXT](https://www.star-group.net/en/products/translation-localization.html) translation projects.

#### PPF AND TRANSIT XML files

*The following procedure has been copied verbatim from CafeTran’s Knowledge base, see link below. *

PPF packages are translation projects created by Transit CAT tool. They are zipped files which need to be unpacked before the translation in CafeTran. Follow these steps to prepare and translate a PPF package:

 1. Rename the received .ppf package to the .zip package and unzip it to a folder.
 2. Create a separate working folder outside the unpacked package.
 3. Locate the source language files in the unpacked package. They end with the three-letter language code for your source language.
 4. Copy the source language files to the working folder you created in step 2.
 5. Run CafeTran and create a new project choosing a single source language file in the working folder or the whole working folder with several files. If you choose a folder instead of a single file, please select “Multiple document project” option in the Dashboard menu ≡.
 6. Choose Transit XML filter from the “File of type” list in the Project Configuration dialog and click the OK button.
 7. Translate the project and perform QA > Tags check making sure that tags are correct.
 8. Export the translation and go to CafeTran project’s folder where the exported file(s) are located.
 9. Change the three-letter source language code in the name of exported file(s) to the three-letter language code of your target language.
 10. Copy the translated file(s) with the three-letter target language code to the unzipped PPF package folder.
 11. Zip back the folder and change the name (extension) of the zipped package from .zip back to .ppf.
 12. Send the translated .ppf package to your client.

Note: You can find three-letter language codes for your language pair here.

 If PPF package contains *.TXE terminology files to use in the translation, please perform the following:

 1. Choose Memory > Import TBX terminology… from CafeTran’s menu.
 2. Navigate to the folder with the *.TXE terminology file and choose it.
 3. In Memory options, make sure “Fragments memory” option is selected.
 4. Click the OK button to import *.TXE terminology to CafeTran memory.

Related links:
[Translation of PPF packages](https://cafetran.freshdesk.com/support/solutions/articles/6000186095-translation-of-ppf-packages)

#### Transit TermStar terminology files - TXE

To import a TXE terminology file in CafeTran:

 1. Choose Memory > Import TBX terminology… from CafeTran’s menu.
 2. Navigate to the folder with the *.TXE terminology file and choose it.
 3. In Memory options, make sure “Fragments memory” option is selected.
 4. Click the OK button to import *.TXE terminology to CafeTran memory.

#### Transit XV packages - PXF

The older version, Transit XV used the PXF extension for packages. You should be able to ask for a PPF file instead, in the unlikely event you receive a PXF package.

### Memsource

CafeTran can handle MXLIFF files that you download from your own [Memsource](https://www.memsource.com/) translator account or those you are allowed to download from an account enabled by a translation agency on a project basis (some clients/accounts seem to disable the download feature).

MXLIFF notes are mapped as CafeTran notes.

**Translation status:**

- Checked segments in CafeTran appear as Confirmed in Memsource and vice versa.

#### MXLIFF

Follow these steps to translate MXLIFF files in CafeTran:

 1. Download the MXLIFF files from the Memsource online account (Go to the project’s dashboard, check the files you wish to download and click on the Download button).
 2. Create a working folder and copy the bilingual MXLIFF files.
 3. Translate the files in CafeTran and perform QA > Tags check making sure that tags are correct.
 4. Run Task > Set checked status for target segments. CafeTran’s “Checked” status is mapped to Memsource’s “Confirm” status.
 5. Launch Memsource Editor and connect with the same Memsource credentials (click [here](https://www.memsource.com/download/) to download and install it on your computer), and open one MXLIFF file at a time.
 6. (Recommended) Run Memsource’s QA checks and/or run bilingual file export/import operation as needed.
 7. Upload the MXLIFF file to the Memsource server via Document > Upload to server in Memsource Editor. Repeat for each file.
 8. Finalize the project in Memsource Editor for Web.

This last step generally requires the following actions:
 - Check that all files are 100% confirmed.
 - if you need to upload files to a server upon project completion, use Download > Completed file.
 - Click on Edit and change the Status to “Completed by Linguist”.

Note: Access to Memsource’s Translation Memories (TM) and Termbases (TB) can only be achieved via Memsource Cloud or Memsource Editor, unless you are allowed to download them. In that case, TMs can be downloaded as TMX or XLSX and TBs as TBX or XLSX.

**Handling Memsource tags:**

Tags used in Memource MXLIFF files appear to be some internal markings unrelated to the XLIFF format itself, but rather to the source document being translated. They are displayed in the form of {1> <1} or {1} and are not recognized as tags in CafeTran by default.

To convert the sequence of {1> and <1} characters into CafeTran's nontranslatables and hide it, you can add the following regular expression to your glossary of non-translatable fragments (Resources > Non-translatable fragments > Add selection to non-translatable fragments):

     |\{.?+>|<.?+\}^

If you skip the last ^ character, they will not hidden.

Then, you will be able to easily place these tags with the F3 keyboard shortcut for inserting tags.

Related resources, for your reference:
[Memsource Editor](https://help.memsource.com/hc/en-us/sections/360003807219-Memsource-Editor)

### SMARTCAT

[Smartcat](https://www.smartcat.ai/)'s online CAT tool supports [exporting and importing back translated XLIFFs](https://help.smartcat.ai/hc/en-us/articles/360000240072-Export-XLIFF-from-Smartcat). Exported Smartcat XLIFFs can then be translated in CafeTran and uploaded back into Smartcat. When you hit Finalize and choose to set the Translated status in CafeTran, all segments are marked as Confirmed in Smartcat, which means the final translated document can be directly exported from the online interface.

### CROWDIN

Crowdin is an online localization project management platfom and translation tool for developers and website owners.

#### Crowdin's XLIFFs

XLIFF files downloaded from Crowdin are properly handled using CafeTran’s “Translate external project” workflow.

Crowdin’s Context information is displayed as CafeTran Notes.

Note: Access to Crowdin’s Translation Memories (TM) and Termbases (TB) can only be achieved via Crowdin.

### XTM Cloud

[XTM Cloud](https://xtm.cloud/) is an online Translation Management Software.

XLIFF files downloaded from XTM Cloud are properly handled (including tags) by CafeTran’s “Translate external project” workflow. They can be imported back into XTM Cloud by a Project Manager.

If TIPP packages containing multiple XLIFF files are used, ask for a Multi-XLIFF file instead (a single XLIFF file which basically joins all the XLIFF files inside), so that you can translate and upload translation for all files at once.

Note: Access to XTM Translation Memories (TM) and Termbases (TB) can only be achieved via XTM Cloud.

### XLIFF 2.0

XLIFF 2 is being developed by the OASIS XLIFF TC. The latest published version of XLIFF 2 can be found [here](http://docs.oasis-open.org/xliff/xliff-core/v2.0/xliff-core-v2.0.html).

CafeTran uses an experimental filter for XLIFF 2.0 files. Report any issues to the developer.

Note: [Okapi XLIFF Toolkit](https://bitbucket.org/okapiframework/xliff-toolkit) is a library that implements a set of Java components to create, read and manipulate XLIFF 2 documents. It can be used to validate a XLIFF 2.0 file (which can also be done online via this [XLIFF Manager](https://www.maxprograms.com/products/xliffmanager.html).

### Interoperability Now! TIPP and XLIFF:DOC

The TIPP package format (along with the XLIFF:DOC bilingual XML files it contains) is part of the Interoperability Now! initiative. It aspires to make it easier to pass projects and assignment packages among different translation tools. TIPP also has the objective to make resources and other settings interoperable among tools.

TIPP zipped packages cannot be simply unzipped, translated and zipped back.

However, XLIFF:doc files can be edited in CafeTran, so you can ask for those instead.

See the Unsupported section for more details.

Related links:
[Interoperability Now! project](https://code.google.com/archive/p/interoperability-now/)

## 3. UNSUPPORTED FORMATS

You may come across translation projects which require handling various yet unsupported formats. This section lists and discusses different such formats (the list is bound to expand as needs arise) along with possible ways to deal with them. The next section (Solutions) catalogs various tools you can use to prepare unsupported file formats and export them back to their original format after translating them in CafeTran, so be sure to check it as well.

### PDF

PDF (Portable Document Format) represents a difficult format to deal with. You should ask your client for the editable file that generated the PDF file instead. If this is not possible, different strategies and solutions exist for editable and non-editable PDF documents, some of which are presented below.

- **CafeTran Espresso**

CafeTran does not offer OCR, but can handle editable PDFs with its **Translate through Clipboard** workflow (either exporting to MS Word, OO/LO Writer or directly pasting the translation into a dedicated PDF editor) and short non-editable (scanned) PDFs with its **Translate paper document** workflow.

Related links:
[Basic Clipboard Workflow](https://cafetran.freshdesk.com/support/solutions/articles/6000108822-basic-clipboard-workflow)
[Translation of PDF Documents](https://cafetran.freshdesk.com/support/solutions/articles/6000109979-translation-of-pdf-documents)
[Translation of Paper Documents](https://cafetran.freshdesk.com/support/solutions/articles/6000111789-translation-of-paper-documents)

- **OCR**

Especially for scanned (non-editable) PDFs and images, an obvious solution is to use an OCR program to scan the file and prepare an editable form of the source document (generally in MS Word or OpenOffice/LibreOffice format) that you then translate in CafeTran.

Note: OCR conversion, source file preparation and final layout editing require additional time and are generally billed as an extra service.

Because scanned PDF documents are routinely sent in for translation, obtaining an efficient OCR solution can often be a worthy investment. [ABBYY FineReader](https://www.abbyy.com/finereader/) (Windows, Mac) is the most popular choice (and, in latest versions, also integrates the PDF editing capabilities of PDF Transformer+), but it’s not the only one. Other offline paid solutions include [Adobe Acrobat Pro DC](https://acrobat.adobe.com/us/en/acrobat/pricing.html?promoid=DZTH12D8&mv=other) (Windows, Mac, OCR, PDF editor, OCR, PDF to Word, Word, Excel or PowerPoint to PDF), [Kofax OmniPage](https://www.kofax.com/products/omnipage) (Windows), [Readiris](http://www.irislink.com/EN-US/c1462/Readiris-16-for-Windows---OCR-Software.aspx) (Windows, Mac) and [Wondershare PDFelement](https://pdf.wondershare.com/pdfelement/) (Windows, Mac, PDF editor, OCR, PDF to Word).

Free offline OCR solutions which make use of Tesseract, an open source OCR engine (which produces accurate results, but is less efficient with complex layouts), include: [FreeOCR](http://www.paperfile.net/download.html) (Windows), [gImageReader](https://github.com/manisandro/gImageReader) (GNU/Linux, Windows, also create searchable PDFs), [VietOCR](http://vietocr.sourceforge.net) (Windows, Mac, GNU/Linux).

Online solutions: [Convertio](https://convertio.co/ocr/) (10 page free trial, API available, prepaid and API packages available, multiple languages supported, excellent results), [PDFCandy](https://pdfcandy.com/pdf-ocr.html), [Free Online OCR](https://www.onlineocr.net/) (max. size 15 MB, good OCR recognition for basic layouts, uses Tesseract), [TM-Town](https://www.tm-town.com/blog/uploader-and-alignment-redux) (online, uses Tesseract).

On the CAT tools front, [MateCat](https://matecat.com) (online) and [Wordfast Anywhere](https://www.freetm.com/anywhere.html) (online) offer PDF OCR conversion. [Trados Studio](http://www.sdl.com/software-and-services/translation-software/sdl-trados-studio/) also offers OCR, powered by Solid Documents Technology, or via the IRIS PDF OCR plugin (powered by Readiris).

Inceni’s [TransPDF](https://transpdf.iceni.com/) (free or pay as you go) online service tackles the PDF problem in a different way, via conversion to XLIFF and back, offering an OCR feature paid with credits along the way (see below for more details).

Note: Many PDF editors and OCR solutions also offer the possibility to run OCR on the PDF itself, in order to make it editable and/or searchable. Making the PDF editable allows you to further edit or convert the document. Making it searchable is interesting if you wish to use the scanned PDF for reference purposes.

**Handling OCR tags**

CafeTran offers a special filter to handle MS Word documents after OCR, which clears the source text of unnecessary formatting tags.

Alternatives for tag cleaning:
[CodeZapper](http://asap-traduction.com/CodeZapper) (MS Word add-in)
[TransTools- Tag Cleaner](http://www.translatortools.net/word-doccleaner.html#TagCleaner) (MS Word add-in). Tag Cleaner is part of the [TransTools](http://www.translatortools.net/about.html) suite featuring many useful utilities for preparing various types of Microsoft Office documents.

- **EDITABLE PDF TO TEXT CONVERSION**

While OCR can be used on editable PDFs, there are generally other effective methods for converting this type of PDF to text (DOCX, etc.).

Typically, the resulting file still needs source preparation before translation, or at least some final layout editing after file export.

**Offline tools** with PDF conversion capabilities include: [WPS PDF to Word Converter](https://www.wps.com/pdf-to-word) (paid, free for 5 page documents, Windows, tested with excellent results), [Foxit's PhantomPDF](https://www.foxitsoftware.com/pdf-editor/) (paid, Windows, Mac, PDF editor, PDF to Word), [Adobe Acrobat Pro DC](https://acrobat.adobe.com/us/en/acrobat/pricing.html?promoid=DZTH12D8&mv=other) (paid, Windows, Mac, PDF editor, OCR, PDF to Word, Word, Excel, or PowerPoint to PDF), [Wondershare PDFelement](https://pdf.wondershare.com/pdfelement/) (paid, Windows, Mac, PDF editor, OCR, PDF to Word), [PDF Architect](https://www.pdfforge.org/pdfarchitect/personal) (paid, Windows, PDF editor, OCR, PDF to Word), [Solid Converter](http://www.soliddocuments.com/pdf/-to-word-converter/304/1) (paid, Windows and Mac), [Nitro](https://www.gonitro.com/home-1#) (paid, Windows, PDF editor, PDF to Word), [PDFSam](https://pdfsam.org/) (paid for PDF to word, OCR and other stuff on Windows / free cross-platform utility for basic editing tasks, such as splitting and merging PDFs), [Ableword](http://www.ableword.net/pdftoword.html) (free, Windows, Word and PDF editor, PDF to Word), and [Sejda Desktop](https://www.sejda.com/desktop) (free/paid, Windows, Mac, GNU/Linux, PDF editor, PDF to Word, Word to PDF, also online version).
[Microsoft Word](https://support.office.com/en-us/article/Edit-PDF-content-in-Word-b2d1d729-6b79-499a-bcdb-233379c2f63a) (2013 and later, on Windows) also offers the ability to turn a PDF into an editable document. [LibreOffice](https://libreoffice.org/) does this as well, but text appears within text boxes, which only makes it usable for PDF editing, not document preparation.
For simple text extraction, you can also use the free [Adobe Reader](https://get.adobe.com/reader/otherversions/) and other PDF readers.

**Online tools**:

[CleverPDF](https://www.cleverpdf.com/pdf-to-word), [Foxit PDF to Word converter](https://www.foxitsoftware.com/pdf-to-word-converter/), [EasyPDF PDF to Word](https://www.easepdf.com/pdf-to-word/) and [CloudConvert](https://cloudconvert.com/) all produce very good results (CloudConvert has the added bonus that it also handles a host of different file conversion types and offers an API. It is also used by MateCat).

Other online converters include: [PDFCandy PDF to Word](https://pdfcandy.com/result/27f78ac486f64003.html), [Smallpdf](https://smallpdf.com/) (PDF to word is based on Solid Documents, other PDF related actions and conversions are supported), [Convertio](https://convertio.co/), [Zamzar](http://www.zamzar.com/) (many different conversion types), [PDFtoWord](https://www.pdftoword.com/) (also offline as Nitro).

For command line enthusiasts, programs such as pdftotext, pdfreflow (pdftohtml), Calibre’s e-book-convert, pdf2htmlEX, pdfbox can be added to the mix for PDF text extraction.

On the CAT tools front, [MateCat](https://matecat.com) (online) and [Wordfast Anywhere](https://www.freetm.com/anywhere.html) (online) offer PDF conversion. [Smartcat](https://smartcat.ai/) (a CAT tool developped by ABBYY) also offers paid OCR packages, while [Trados Studio](http://www.sdl.com/software-and-services/translation-software/sdl-trados-studio/) can handle editable PDFs directly.

Inceni’s [TransPDF](https://transpdf.iceni.com/) (free or pay as you go) online service tackles the PDF problem in a different way, via conversion to XLIFF and back (see below for more details).

- **PDF TO XLIFF TO PDF - INCENI INFIX & TRANSPDF**

If you need to translate a PDF document with tricky layout that you need to replicate and deliver back into PDF (not DOCX) format, the following solution can be very efficient.

**Iceni Infix** is a PDF editor (with a monthly subscription or one-off payment) that offers the possibility to export text strings from editable PDFs as XLIFF files, then import them back and perform final adjustments. Infix 7 now uses a online TransPDF service or an offline legacy solution (with some drawbacks).

Related links:
Infix 7 - [Translating PDF](https://www.iceni.com/help/Infix/7/en/TranslatingPDF.html)
Infix - [Pricing](https://www.iceni.com/infix.htm#pricing)

**TransPDF** is on online (free/pay as you go) service that aims to end the frustration of translating PDFs by converting them to good quality XLIFF for use with your own translation tools.

Simply upload your PDF to TransPDF and translate the XLIFF you get back using your own CAT tool (connectors exist for Trados, Memsource and memoQ). Upload your translated XLIFF and you will get a fully-formatted, translated PDF. Any post-editing can be done for free using Infix 7 PDF editor. This solution can also perform OCR (paid through credits) on scanned PDFs.

Note: By default, text is segmented per paragraph, although some tools, such as Trados and Memsource, apply additional segmentation, which makes the resulting XLIFF far more usable. I would recommend performing a round trip via one of these two tools to take advantage of the improved segmentation. You can also try to resegment the XLIFF file from paragraph to sentence via the Okapi Framework.

On the plus side, the original layout is preserved and should only require limited PDF editing (although in language pairs with high expansion rate, keeping the same layout can be troublesome), greatly reducing the time needed for layout finalization/DTP work.

On the down side, the service has some price attached to it which, although quite low, represents an additional cost. Furthermore, even with the improved segmentation if you go for a roundrip through Trados or Memsource, the file might present a few less than optimal segmentation situations that you cannot fix as you would in a native CafeTran project.

Still, TransPDF represents an interesting option you should try.

Note: ProZ.com members get a [25% discount](https://go.proz.com/transpdf-credit-purchase) when buying credits. ProZ.com Plus members also receive 10 credits per month, as part of their [Plus package](http://www.proz.com/about-plus-package).

Related links:
TransPDF - [Home page](https://www.iceni.com/transpdf.htm),
TransPDF - [Pricing](https://www.iceni.com/transpdf.htm#pricing),
TransPDF - [Help and support](https://transpdf.iceni.com/support/),
TransPDF - [PDF Translation, Step-by-step](https://transpdf.iceni.com/segments/xl_help),
TransPDF - [Using MemoQ for PDF translation](https://docs.memoq.com/current/en/Places/transpdf-account.html),
TransPDF - [Using Memsource for PDF translation](https://transpdf.iceni.com/guide/memsource)

- **EXTRACT PDF TABLES - TABULA**

If you want to extract tables from editable PDFs (not only for translation, but also for terminology files), [Tabula](https://tabula.technology) (Windows, MacOS, GNU/Linux) is a great open source and free solution. Output is exported to CSV or Microsoft Excel file formats.

- **PDF EDITING**

PDF editing solutions are also useful to keep around for various tasks, including CafeTran’s “Translate through Clipboard” workflow.

[Adobe Acrobat Pro DC](https://acrobat.adobe.com/us/en/acrobat/pricing.html?promoid=DZTH12D8&mv=other) (Windows, Mac), [Nitro Pro](https://www.gonitro.com/download), [Kofax Omnipage](https://www.kofax.com/Products/omnipage/standardl) (Windows, PDF editor, PDF to Word), [Foxit Phantom PDF](https://www.foxitsoftware.com/pdf-editor/) (Windows, PDF editor, PDF to Word), [Wondershare PDFelement](https://pdf.wondershare.com/pdfelement/) (paid, Windows, Mac, PDF editor, OCR, PDF to Word), [PDF Architect](http://www.pdfforge.org/pdfarchitect/download) (paid, Windows, PDF editor, OCR, PDF to Word), [Soda PDF](https://www.sodapdf.com/) (Windows, online, PDF editor, PDF to Word), [iSkysoft PDF Editor](https://pdf.iskysoft.com/) (paid, Windows, Mac), [FlexiPDF](http://www.softmaker.de/flexipdf) (paid, Windows, PDF Editor, doc to PDF converter) and [Master PDF Editor](https://code-industry.net/masterpdfeditor/) (free with watermarking/paid, Windows, Mac, and GNU/Linux // Linux free edition is 100% usable without PDF watermarking) are some of the available options. [ABBYY FineReader](https://www.abbyy.com/finereader/) (Windows, Mac), mostly known for OCR, now also integrates the PDF editing capabilities of PDF Transformer+.

On the (mostly) free front: [Sejda Desktop](https://www.sejda.com/desktop) (free/paid, Windows, Mac, GNU/Linux, PDF editor, PDF to Word, Word to PDF, also free/paid online version) [AbleWord](http://www.ableword.net/) (free, Windows, Word and PDF editor), [PDF-XChange Editor](https://www.tracker-software.com/product/pdf-xchange-editor) (Windows, Free and Plus versions available), [LibreOffice](https://libreoffice.org/) Writer or Draw (free, Windows, Mac, GNU/Linux, text appears within text boxes), Inkscape (free, Windows, Mac, GNU/Linux, SVG editor, can also serve to edit PDFs - each page separately - and translate images).

Online PDF editors: [Sejda PDF Editor](https://www.sejda.com/pdf-editor), [PDFCandy](https://pdfcandy.com/edit-pdf.html).

- **CONVERT TO PDF**

Sometimes, you may need to deliver documents to PDF format as well.

Office suite applications ([Microsoft Office](https://products.office.com/) [Windows, Mac, online], [OpenOffice](https://www.openoffice.org)/[LibreOffice](https://libreoffice.org/) [cross-platform], [WPS Office](https://www.wps.com/) [Windows, GNU/Linux], [SoftMaker Office](http://www.softmaker.com/en/softmaker-office) [cross-platform], [Google Docs](https://docs.google.com) [online]) and many software applications can export a document they handle directly to PDF.

Most PDF editing tools mentioned above should also handle document to PDF conversion, such as [Adobe Acrobat Pro DC](https://acrobat.adobe.com/us/en/acrobat/pricing.html?promoid=DZTH12D8&mv=other) (Windows, Mac), [Nuance Power PDF](https://www.nuance.com/print-capture-and-pdf-solutions/pdf-and-document-conversion/power-pdf-converter.html) (Windows), [Foxit Phantom PDF](https://www.foxitsoftware.com/pdf-editor/) (Windows), [Wondershare PDFelement](https://pdf.wondershare.com/pdfelement/) (Windows, Mac), [PDF Architect](https://www.pdfforge.org/pdfarchitect/personal) (Windows), [Soda PDF](https://www.sodapdf.com/) (Windows, Mac) and [iSkysoft PDF Editor](https://pdf.iskysoft.com/) (Windows, Mac), [FlexiPDF](http://www.softmaker.de/flexipdf) (Windows, PDF Editor, Word to PDF converter).
There are also apps like [PrimoPDF by Nitro](http://www.primopdf.com/) (Windows, free), [Icecream PDF converter](https://icecreamapps.com/PDF-Converter/) (Windows, free/paid).

Online: [Soda Word to PDF](https://www.sodapdf.com/word-to-pdf/), [PDFCandy](https://pdfcandy.com/), [Smallpdf](https://smallpdf.com/), as well as general (batch) file converters such as: [Zamzar](http://www.zamzar.com/), [CloudConvert](https://cloudconvert.com/), [Convertio](https://convertio.co/).

### DOC / XLS / PPT

Microsoft Office 1997–2003 files (.doc, .xls, .ppt) are not directly supported in CafeTran.

You can either convert these files to DOCX, XLSX, PPTX before translating them in CafeTran or, if compatibility/presentation issues might arise, use a round trip solution (MateCat, Wordfast Pro 3 & 6, Okapi Framework, Memsource, Trados Studio, memoQ, etc.). Check the Solutions section below.

### RTF

Short for Rich Text Format, RTF is a text file format with only some additional basic formatting.

You will need to convert RTF to DOCX or ODT before translating it in CafeTran. After export, you can convert it back to RTF using MS Word or OpenOffice/LibreOffice. Conversion should be lossless.

CAT tools that allow you to handle RTF via a round trip: MateCat, Smartcat, Wordfast Pro 3, Trados, MemoQ.

#### Bilingual RTF/DOC files / Multi-column RTF tables

RTF (or DOC) is being sometimes used as a bilingual document format by a number of CAT tools, such as: some versions of Trados (“External Review”), Wordfast Pro (“Bilingual Review"), Déjà Vu ("External View") and memoQ (“Two-column RTF” or Multi-column RTF tables).

In general, you will be better off asking for a bilingual XLIFF-flavored file.

Otherwise, please note additional file preparation and handling might be needed before proceeding to the translation in CafeTran.

#### Multi-column RTF tables

Multi-column RTF tables are Rich Text Format documents that contain one or more memoQ documents.

![Anatomy of an RTF table](https://i.imgur.com/xfEL77Q.png)

They are also used in Déjà Vu External View.

Related links:
[memoQ - Multi-column RTF tables](http://memoq.helpmax.net/en/explanations/exchanging-documents-with-other-tools/multi-column-rtf-tables/)

### PUB (Microsoft Publisher)

Microsoft Publisher is an entry-level desktop publishing application from Microsoft, differing from Microsoft Word in that the emphasis is placed on page layout and design rather than text composition and proofing.

This format is tricky to handle as it has few export options, Few CAT tools support it.

[Fluency](https://www.westernstandard.com/Fluency/freelancers.aspx) CAT tool (paid, Windows and OS X, offers a free 15-day trial) is able to handle .pub files and even export to xliff (File > Export Fluency XLIFF file), allowing you to work in CafeTran.

If you own the right edition of MS Publisher (It is part of the Microsoft Office suite), you can also use “Translate through Clipboard” workflow (explained above) to translate in CafeTran and paste the results in MS Publisher.

Finally, this interesting article @ [Multifarious](https://multifarious.filkin.com/2016/01/11/ms-publisher/) discusses a different solution for MS Publisher files.

### VDX (Microsoft Visio)

Microsoft Visio is a diagramming and vector graphics application that is part of the Microsoft Office family.

If you have Microsoft Visio, you can use [TransTools For Visio](https://www.translatortools.net/products/transtools/visio-translation) that allows you to extract translatable text from Visio drawings (all formats supported by Microsoft Visio) and to merge translations back into the original Visio drawings.

CAT tools that allow you to handle Visio files via a round trip: Wordfast Pro 3, Okapi Framework, MemoQ, Déjà Vu.

### INDD (InDesign)

If you need to handle .indd instead of .idml files, [Language Terminal](https://www.languageterminal.com/)’s free InDesign online converter allows you to work with InDesign in any CAT tool. Registration required.

Steps:

 1. In Language terminal, drag and drop the INDD file in the InDesign conversion section.
 2. Select source and target language, then press convert.
 3. Once the conversion is completed, click on the file name to download a ZIP file.
 4. Extracting the ZIP file produces an MQXLZ (memoQ ZIP) file and a reference PDF.
 5. Change the MQXLZ extension to zip and unzip the file.
 6. Translate the extracted MQXLIFF file in CafeTran.
 7. When done, add the translated and finalized MQXLIFF file to Language Terminal.
 8. The MQXLIFF file will be converted to a translated INDD file.

[Video](https://www.youtube.com/watch?v=Z4GrkPtowpI&feature=youtu.be) tutorial.

### AI (ILLUSTRATOR)

Adobe Illustrator Artwork (AI) is a proprietary file format developed by Adobe Systems for representing single-page vector-based drawings in either the EPS or PDF formats. The .ai filename extension is used by Adobe Illustrator. The AI file format was originally a native format called PGF.

While AI files are not directly supported in CafeTran, since Adobe Illustrator can import and export SVG files, you can use CafeTran's SVG filter to handle Adobe Illustrator files (*.ai or *.eps).

To save the AI file as an SVG, you need to use a compatible application. There are several options:

Paid options:

- Purchase the Sysfilter pack or a monthly/annual Sysfilter subscription for Illustrator [here](https://polmannshop.com/online/en/search?controller=search&orderby=position&orderway=desc&search_query=sysfilter&submit_search=). Generates XLIFF files for import/export.
- Get a monthly subscription to Adobe Illustrator itself ([here](https://www.adobe.com/creativecloud/plans.html)). Use that to save as .SVG.

Free option: Use the free/libre software [Inkscape](https://inkscape.org/). For more information, review the related documentation for [Inkscape for Adobe Illustrator users](https://inkscape.org/learn/faq/#inkscape-edits-svg-file-which-was-originally-created-adobe-illustrator-are-lost-when-importing-back-ai) and an [additional explanation/workaround](https://inkscape.org/learn/faq/#inkscape-edits-svg-file-which-was-originally-created-adobe-illustrator-are-lost-when-importing-back-ai).

Adobe Illustrator instructions:

- Before you export your document, you need to change the text from single line text boxes to full paragraph text boxes in Illustrator. This ensures correct segmentation.

- To prevent too many tags and ensure correct segmentation, use the following Illustrator export settings (make sure you do not use "Preserve Illustrator Editing Capabilities"):

  ![Adobe Illustrator - Export to SVG options](https://i.imgur.com/xZA2GiX.png)

- Saving the document as SVG separates out the images. Therefore, save the SVG to its own  separate folder.

- Import the SVG into CafeTran. After the translation, export the file back into the original folder so that the images can be linked correctly.

### DWG (AutoCAD)

Generally, prior to translation, the AutoCAD DWG proprietary binary format needs to be converted into DXF, an exchange plain text format, which is handled by CafeTran (see Supported filters section above).

Ideally, this should be done by the client in AutoCAD. Various (often expensive) software solutions also offer DWG to DFX conversion.

If the DWG is exported as an SVG file (in Adobe Illustrator), if can be translated using the SVG file filter.

Free conversion solutions include: [ODA File Converter](https://www.opendesign.com/guestfiles/oda_file_converter) (free, cross-platform)

Free DWG/DFX viewers include: [DraftSight](https://www.3ds.com/products-services/draftsight-cad-software/free-download/) (Windows, OS X, GNU/Linux)

### PO

GNU Gettext Portable Object (.po) format used in localization is not yet directly supported by CafeTran.

Tools that allow you to handle PO files via a round trip: MateCat, Wordfast Pro 3, Okapi Framework, Memsource, Swordfish, Heartsome, Trados Studio, memoQ.

### JSON

JavaScript Object Notation (JSON) files are not directly supported by CafeTran.

CAT tools that allow you to handle JSON files via a round trip: MateCat, Wordfast Pro, memoQ, Swordfish, Trados Studio (via an Open Exchange application). Okapi Framework can also help prepare files for translation and then back to the original format.

### EPUB / MOBI / AZW / e-book

*Report any issues as described in the Feedback section of this document*

#### EPUB

EPUB (or ePub, short for electronic publication) is an e-book file format with the extension .epub that can be downloaded and read on devices like smartphones, tablets, computers, or e-readers.

An EPUB file is a ZIP archive that contains, in effect, a website—including HTML files, images, CSS style sheets, and other assets. It also contains metadata. EPUB 3 is the latest version. By using HTML5, publications can contain video, audio, and interactivity, just like websites in web browsers.

So, while the EPUB format itself is not directly handled by CafeTran, since the text to translate is contained in HTML files, one method of translating EPUBs is be the following:

1. Extract the EPUB to a folder: rename the EPUB to ZIP and extract as usual. Alternatively, [7-Zip](http://www.7-zip.org/download.html) file archiver (among others) can uncompress EPUBs directly. Another method: Convert the ePub to ZIP via [Calibre](https://calibre-ebook.com/) e-book management application.
3. Translate the subfolder (typically called “text”) containing the .html files in CafeTran (enable the “Multiple documents project” option in the Dashboard menu ≡).
4. Rebuild the .ePub file. This may include the following steps:
    - Replace the .html files in the “text folder” with the translated ones.
    - Regenerate/Edit the TOC.NCX (Table of Contents) file. TOC generation and Editing can be done via the [Sigil](https://sigil-ebook.com/get/) free E-book editor, as described [here](https://www.epubble.com/let-sigil-make-the-ncx-file/). Editing can also be done with [Calibre](https://calibre-ebook.com/download)’s e-book editor (accessible via the “Edit book” button or context menu action).
    - ZIP the file and rename it to EPUB.
    - View it in Calibre and run additional validation checks (see below).

Additional validation checks can be done in Sigil (via its FlightCrew ePub validation plugin). You should also run a validation test in [EpubCheck](http://validator.idpf.org/) (online/offline) or the GUI version [Pagina ePub checker](https://www.pagina.gmbh/produkte/epub-checker/). EpubCheck is an open source tool that validates EPUB books, so that you can make sure that your book complies with the EPUB format’s specifications. This may be a requirement for some publishing platforms. Final checks can of course be conducted by the author or the publisher.

More details on the external tools mentioned:

- [Calibre](https://calibre-ebook.com/) is a complete cross-platform e-book management suite. It lets you manage and access your digital library, view and edit e-books, convert them from one format to another, and much more. You can read its [user manual](https://manual.calibre-ebook.com/).
- [Sigil](https://sigil-ebook.com/) is an excellent cross-platform E-book editor.

MEMSOURCE ROUND TRIP METHOD

Since [Memsource](http://memsource.com/) handles EPUBs directly, you can use it to import the EPUB file, export the bilingual MXLIFF, translate it in CafeTran, upload the MXLIFF file in Memsource and finalize the translation. This is described in detail in the External projects > Memsource Cloud section of this document.

CALIBRE CONVERSION METHOD

You can convert any e-book to DOCX or RTF (and other formats) with Calibre, translate it and convert it back (to any format). This method is nice for producing a usable text file, but the back-conversion is likely to produce problems. If you need to deliver an EPUB file (and not a DOCX or other text type), you’re better off using the methods described above.

#### MOBI / AZW / AZW3

The **Mobipocket** e-book format (.mobi) is based on the Open e-book standard using XHTML and can include JavaScript and frames. It also supports native SQL queries to be used with embedded databases. Mobipocket can be read in Amazon Kindle ad well as other e-Book devices and readers.

The **Amazon Kindle’s AZW** format is basically just the Mobipocket format with some non standard variations. The Kindle format is available on a variety of platforms, such as through the Kindle app for the various mobile device platforms.

Older Kindle e-readers use the proprietary format, **AZW**. It is based on the Mobipocket standard, with a slightly different serial number scheme (it uses an asterisk instead of a dollar sign) and its own DRM formatting.

Since, Amazon.com has released Kindle Format 8, also known as .**AZW3**. The .azw3 file format supports a subset of HTML5 and CSS3 features, with some additional non-standard features; the new data is stored within a container which can also be used to store a Mobi content document, allowing limited backwards compatibility.

Translating MOBI / AZW3 E-books would require the following additional steps, with regards to the EPUB translation process described above:

1. Preparation: Convert the azw/mobi file to an ePub file with Kindleunpack or Calibre (import the book in Calibre, then Convert books > EPUB).
3. Finalization: Convert the updated .ePub file to an .azw3 file. You can do so via Calibre or online converters (such as Zamzar and CloudConvert).

https://www.mobileread.com/forums/showthread.php?t=243216

#### IBOOKS

The .ibooks format is created with the (discontinued) iBooks Author E-book layout software and Pages application from Apple Inc.. This proprietary format is based on the EPUB standard, with some differences in the CSS tags used in an ibooks format file, thus making it incompatible with the EPUB specification

An option to handle iBooks would be to use [Pages](https://support.apple.com/en-us/HT211136) (MacOS only) to export from IBOOKS to EPUB format, perform the EPUB translation as described above, then create a new iBooks Author file and import the translated .ePub into it for finalizing and publishing (since iBooks Author only opens iBooks Author projects, .ibooks).

Related links:
Apple - [Pages official support page](https://support.apple.com/pages)

### TIPP (Packages)

The TIPP package format is part of the Interoperability Now! initiative and contains **XLIFF:doc** documents. It aspires to make it easier to pass projects and assignment packages among different translation tools. TIPP also has the objective to make resources and other settings interoperable among tools.

TIPP zipped packages cannot be simply unzipped, translated and zipped back. You should ask for or use the included XLIFF:doc files instead.

memoQ has full support for TIPP packages and XLIFF:doc documents, so you also can use it for handling these packages.

Related links:
[Interoperability Now! project](https://code.google.com/archive/p/interoperability-now/)

## 4. SOLUTIONS

Since CafeTran offers a wide compatibility with external bilingual files, you can take advantage of this to prepare files (into a format CafeTran can accept) using a different software tool which handles **file types not yet supported by CafeTran** or offers **additional filter options** for already supported formats, then export the files back to their original format using the same tool once you’ve completed the translation in CafeTran (what we will call a “round trip”).

Note: Working on External projects presents some differences and/or limitations when compared to the native “Translate document” workflow in CafeTran. These differences and limitations are discussed in detail in the General notes of the External projects section above.

**CafeTran Espresso - Clipboard workflow**

Before reviewing external options, it’s good to know that CafeTran offers a Clipboard workflow which is not limited to any file format and can be used in various translation scenarios, allowing you to work in collaboration with many different software programs.

In the context we discuss here, these scenarios might include:

- translating content from dedicated software programs/editors that use file formats which aren’t supported by CafeTran, while still viewing the content in full context;
- translating content from CAT tools that don’t support appropriate exchange formats;
- translating content which can be copied but not modified, as is the case for many non-scanned PDF files.

In this workflow, View > Detached windows can help you arrange your screen to include both CafeTran and an external program, even without using two displays.

Related links:
[Basic Clipboard Workflow](https://cafetran.freshdesk.com/solution/articles/6000108822-basic-workflow).

### XLIFF Manager

*Recommended*

[XLIFF Manager](https://maxprograms.com/products/xliffmanager.html) is a cross-platform open source graphical user interface for [OpenXLIFF Filters](https://www.maxprograms.com/products/openxliff.html) (an open source set of filters for creating, merging and validating XLIFF 1.2 and 2.0 files) written in JavaScript.

With XLIFF Manager you can:

- Create XLIFF 1.2 and 2.0 files that can be translated in any modern CAT tool for a variety of file types.
- Convert your translated XLIFF files to original format with a couple of clicks.
- Validate XLIFF files created by any tool. Validation is supported for XLIFF 1.0, 1.1, 1.2 and 2.0.
- Produce an HTML file with word counts and segment status statistics from an XLIFF document.
- The XLIFF files generated by OpenXLIFF Filters don't use proprietary markup and are fully compatible with most CAT tools.

Supported file formats:

- Adobe InDesign Interchange (INX)
- Adobe InDesign IDML CS4, CS5, CS6 & CC
- HTML
- Microsoft Office (2007 and newer)
- Microsoft Visio XML Drawings (2007 and newer)
- MIF (Maker Interchange Format OpenOffice/LibreOffice/StarOffic
- Plain Text
- SDLXLIFF (Trados Studio)
- TXML (GlobalLink/Wordfast PRO)
- WPML XLIFF (WordPress Multilingual Plugin)
- XML Formats
- XML (Generic)
- DITA 1.0, 1.1, 1.2 and 1.3
- DocBook 3.x, 4.x and 5.x
- SVG
- Word 2003 ML
- XHTML
- JavaScript
- Java Properties
- PO (Portable Objects)
- RC (Windows C/C++ Resources)
- ResX (Windows .NET Resources)
- TS (Qt Linguist translation source)

### Okapi Framework - Rainbow

*Offline, cross-platform, free and open source*

*This solution is for more advanced users.*

The Okapi Framework is a cross-platform and free open-source set of components and applications that offer extensive support for localizing and translating documentation and software.

Rainbow is an Okapi application which allows you to launch different utilities to help you perform various localization-related tasks. Like other Okapi applications, it uses the components called “filters” that take input files in a given native format and extract its translatable content into common resources that the Okapi tools can manipulate and modify. You can create and execute [Pipelines](http://okapiframework.org/wiki/index.php?title=How_to_Create_a_Pipeline_in_Rainbow), a series of [Steps](http://okapiframework.org/wiki/index.php?title=Steps) that produce a given outcome. For example, you can create a Pipeline that uses [Rainbow Translation Kit Creation Step](http://okapiframework.org/wiki/index.php?title=Rainbow_Translation_Kit_Creation_Step) to create a (XLIFF or other type of) translation package from a set of input documents, translate the XLIFF, and use [Rainbow Translation Kit Merging Step](http://okapiframework.org/wiki/index.php?title=Rainbow_Translation_Kit_Merging_Step) to merge the files of the package back into their original format.

[Filters](http://okapiframework.org/wiki/index.php?title=Filters#Filter_Config_Examples) are the configurable components that convert input documents from their native file format into a common internal set of resources that all Okapi components use. The extracted content can be re-written into the original file format. When using the steps, the extraction is done by the [Raw Document to Filter Events Step](http://okapiframework.org/wiki/index.php?title=Raw_Document_to_Filter_Events_Step) and the rewriting by the [Filter Events to Raw Document Step](http://okapiframework.org/wiki/index.php?title=Filter_Events_to_Raw_Document_Step).

Related links:
[Okapi Framework - Filters](http://okapiframework.org/wiki/index.php?title=Filters) (to get an idea of supported file types)
[Okapi Framework - Knowledge Base](http://okapiframework.org/wiki/index.php?title=Knowledge_Base)

Note: Open source MateCat filters mentioned above are partly built using Okapi filters.

### MateCat

MateCat is a free online CAT tool* which handles no less than 70 different formats and offers an excellent and easy way to translate file types for which CafeTran does not yet offer native support, acting as an additional file filter.

MateCat round trip procedure:

1. (Optional) Create a MateCat account or login with your Google credentials, for easier access and management of your projects.
2. Create a project in [MateCat](https://www.matecat.com/) by giving it a name, selecting the language pair (and the subject if desired) and uploading the files.
3. Once you click Analyze, you will see a breakdown of the word count. You can access the job itself by clicking Translate in the bottom right, then Open job.
4. On the Translation Editor page, click the arrow next to the Preview button in the top-right corner of the screen and select the option Export XLIFF from the drop-down menu to download the translatable XLIFF file, which you can save on your PC. The XLIFF will be pre-translated with suggestions from your private TMs, the public TM and machine translation.
5. Translate and Finalize the XLIFF file in CafeTran. (You may need to use Project > Documents to view/glue all documents, some text sections of each file being held in separate .xml documents within the XLIFF itself.)
6. Use this [MateCat tool](https://www.matecat.com/utils/xliff-to-target) to convert the translated XLIFF back into the original file format (DOCX, if OCR or PDF conversion is used). Just drag and drop, the download will start!

Additional notes:

- Added bonus: the XLIFF will be pre-translated with suggestions from your private TMs (you can import them prior to or at project creation), the public MyMemory TM and machine translation (Google/Microsoft translate/DeepL). Other MT options are also available.
- If you wish so, you can disable MT (Settings > Machine Translation), although public MyMemory TM matches will still appear in the XLIFF file you download and target segments with no matches will be populated with source text. To start with a clean slate, you can use Task > Remove target segments in CafeTran. This will also set the progress statistics to 0%.
- Highly recommended steps if you intend to perform at least part of the translation in MateCat: Create a private TM resource:
    - In the Project creation page, click on Settings (Alternatively, in the TM and glossary field, expand the drop-down menu and select Create resource).
     - Click on + New resource button in the opened dialog. Give the TM an optional name. Hit Confirm.
     You will see that “MyMemory: Collaborative translation memory” resource is Enabled for Lookup, but not set to be Updated anymore. That way, translated segments will only be stored in your private resources.
 - Be sure to check MateCat’s Privacy policy to confirm this solution is appropriate for you. If you prefer offline solutions, you’ll be better off using other options, such as the Wordfast Pro 3 demo version or, if you feel comfortable, Okapi Framework (see below).
 - The same goes if you wish to configure additional filter options, since MateCat does not seem to offer any for its supported file formats.

 Related links:
[MateCat - online support documentation](https://www.matecat.com/support/)
[MateCat - Translating offline](https://www.matecat.com/support/translating-projects/translating-offline/)
[MateCat - Philosophy and Terms of service](https://www.matecat.com/terms/) (includes Privacy policy)

#### MateCat file formats

Below you will find the full list of supported file formats in MateCat (in bold, those not natively supported by CafeTran): Microsoft Office (DOCX, XLSX, PPTX, **DOC**, **DOT**, DOCM, **DOTX**, **DOTM**, **XLS**, **XLT**, XLSM, **XLTX**, **XLTM**, **PPT**, **PPS**, **PPTM**, **PPSX**, **PPSM**, **POT**, **POTM**), OpenOffice (ODT, **OTT**, ODS, **OTS**, ODP, OTP), Web (HTM, HTML, XHTML, **CSV**, **TSV**, XML, **DTD**, **JSON**, **YAML**, **YML**) Localization (SDLXLIFF, XLIFF, XLF, **PO**, TTX, TXML, Android XML), Desktop publishing (MIF, IDML, **ICML**, **DITA**), Others (TXT, PROPERTIES, RESX, STRINGS, SRT, **WIX**), OCR [via Nuance OCR SDK] (BMP, GIF, PNG, JPEG, TIFF, Scanned PDFs). Others (**RTF**, Regular PDFs [converted to DOCX via CloudConvert]).

Note: CafeTran does not offer OCR, but can handle image translation (except for TIFFs) via the “Translate paper document” workflow, editable PDFs with its Clipboard workflow and short non-editable PDFs with its Paper document workflow.

Related links:
List of [MateCat - Supported file formats and languages](https://www.matecat.com/support/introducing-matecat/supported-browser-languages-formats/)
List of [MateCat filters - Supported file formats](https://github.com/matecat/MateCat-Filters/wiki/Supported-file-formats)

**Note:
 An open source version of Matecat’s client-server web application can also be installed and used offline, although the list of supported file types does not include those requiring commercial licenses for its filters.*

### Smartcat

*Free, online*

[Smartcat](https://www.smartcat.ai/) supports [exporting and importing back translated XLIFF files](https://help.smartcat.ai/hc/en-us/articles/360000240072-Export-XLIFF-from-Smartcat), handles various additonal file types and offers **filter options**. This makes it excellent for roundtrip scenarios. See also their [best practices](https://help.smartcat.ai/hc/en-us/articles/115003578451-XLIFF-export-Best-practices) document.

Additional supported [file formats](https://help.smartcat.ai/hc/en-us/articles/360006979511-File-formats-supported-in-Smartcat) include: DOC, XLS, PPT, POT/POTX, RTF, PHP, PO, MIF, DITA XML, HELP+MANUAL XML, CSV, TSV, DTD, JSON, TJSON, YML, INC, various image formats, powered by OCR (JPG/JPEG, TIF/TIFF, BMP, PNG, GIF, DJVU/DJV, DCX, PCX, JP2, JPC, JFIF, JB2), WSXZ packages.

Related links:
[Smartcat Help Center](https://help.smartcat.com/hc/en-us/categories/360002572820-Freelancers)

### Memsource

*Online/offline, cross-platform, Personal Edition or Freelancer edition*

Memsource free Personal Edition account offers max. 2 files for translation (10 MB each). Old files will need to be deleted before adding new ones. Memsource paid Freelancer Edition (monthly subscription) offers unlimited file use.

Related links:
[Memsource Cloud - Translator editions](https://www.memsource.com/pricing/#translators)

Memsource handles a wide range of file types and offers various **file filters**.

Additional supported file filters include: Multilingual MS Excel, Multilingual XML, Adobe Photoshop - PSD, JSON, CSV, YAML, DITA (dita, .ditamap), DocBook, PO Gettext, PHP, Markdown (.md, .markdown), Quark Tag, CATKEYS, EPUB, INI, LANG, PLIST, RC, SUB, TS, WIKI, YAML, TAG, XTG.

### Wordfast Pro 3

*Offline, cross-platform, free trial version, no time limit*

You can use the cross-platform legacy Wordfast Pro 3 to perform a round trip for different file types.

While WFP demo version has a cap on the size of resources (TMs and glossaries) that can be imported, it can import a source document of any size.

WFP roudtrip procedure:

1. Import the source document into WFP and save it.
2. Open the WFP work file (.txml) in CT and translate it.
3. Open the WFP work file in WFP and choose “Save Translated File.”

Additional supported file formats include:

 - Adobe InCopy ICML, PO, RTF, DOC, XLS, PPT, ASP, JPS, SRT, VDX (Microsoft Visio)

Also, some file formats already supported by CafeTran can offer additional filter options in WFP (in Edit > Preferences > Formats), such as the ability to choose whether to include slide notes, hidden slides etc. in PowerPoint presentations.

Related links:
Download [Wordfast Pro 3](https://www.wordfast.com/products/wordfast_pro_3)

### Wordfast Pro 6

*Offline, cross-platform, free trial version, no time limit*

If you own a Wordfast Pro 6 license, you can use this CAT tool to create projects which support additional file formats or filter options, and perform the translation in CafeTran, since CT handles TXLF files.

You can use the cross-platform Wordfast Pro 6 to perform a round trip for different file types. While WFP demo version has a cap on the size of resources (TMs and glossaries) that can be imported, it can import a source document of any size.

[Supported file formats | Download](http://www.wordfast.com/products/products_wordfast_pro_5) (Specifications tab)

### Swordfish

*Offline, cross-platform, 30-day trial/open source and free to build*

Additional supported file filters include: DocBook 3.x, 4.x and 5.x, JavaScript, PHP Arrays, PO (Portable Objects), RC (Windows C/C++ Resources), TS (Qt Linguist translation source), DITA. Swordfish integrates the OpenXLIFF filters, which can be accessed standalone via XLIFF Manager.

Related links:
Download [Swordfish](https://www.maxprograms.com/products/swordfish.html).

### Heartsome

*Offline, cross-flatform, free and open source*

Additional supported file filters include: DITA, PO, RC.

Related links:
[Heartsome Translation Studio 8.0](https://github.com/heartsome/translationstudio8)

### Online/Offline file converters

As mentioned in the Unsupported formats subsection when considering options for handling PDFs, various online or offline file converters might help you perform a conversion from an unsupported file type to another which CafeTran supports.

Not all conversions are lossless though, and caution/testing is required.

- **Online**

Hundreds of online file converters exist, here are few good ones:
[CloudConvert](https://cloudconvert.com/), [Zamzar](http://www.zamzar.com/), [Convertio](https://convertio.co/).

- **Offline**

These generally depend on the type of file conversion you need to make, it is difficult to make a specific recommendation. Using specialized software is in general more appropriate offline. For example, converting a DOC to DOCX is just a matter of using MS Word, OpenOffice/LibreOffice, WPS Office, etc.

### Trados Studio

*Paid, offline | Windows only*

If you own an Trados Studio license, you can use this CAT tool to create projects which support additional file formats or filter options, and perform the translation in CafeTran, since CT handles SDLXLIFF files.

An Trados license also helps perform operations such as Document Preview, Bilingual document import/export and, of course, Export translated files function and importing TMX to SDLTM, that can’t be done on Trados files in CafeTran.

Trados supports additional plugins that further enhance its features, some of them adding support for additional file formats.

Related links:
[Supported file types](http://producthelp.sdl.com/sdl_trados_studio_2015/client_en/FileTypes/Supported-File-Types.html) in Trados Studio.
[Additional information](http://producthelp.sdl.com/sdl%20trados%20studio/client_en/File_Types/Preparing_Different_Files_Types_for_Translation.htm) on supported file types.

### memoQ

*Paid, offline | Windows only*

If you own a memoQ license, you can use this CAT tool to create projects which support additional file formats or filter options, and perform the translation in CafeTran, since CT handles MQXLIFF files.

memoQ offers a 45-day free trial version of [memoQ translator pro](https://www.memoq.com/en/memoq-translator-pro) edition. The trial is valid for new customers only and can be later activated if you purchase a full license. You also need to download this version if you are working for customers using a [memoQ server](https://www.memoq.com/en/memoq-server).

[memoQ translator free](https://www.memoq.com/en/memoq-translator-free) is the basic software your trial version turns into at the end of the trial period if you choose not to purchase a license. It has only very basic translation memory and term base functionality and does not help you in large projects (only one document can be translated at a time, so not a great solution for free round trips after the trial period ends). It’s still suitable for personal use on small translation projects though. It is not possible to use memoQ translator free in memoQ online projects (although, as stated above, it is used for accepting jobs from memoQ server).

[Supported file formats](https://www.memoq.com/en/languages-and-file-formats) in memoQ

### Déjà Vu

*Paid, offline | Windows only*

If you own a Déjà Vu license, you can use this CAT tool to create projects which support additional file formats or filter options, and perform the translation in CafeTran, since CT handles Déjà Vu External View XLIFF files.

Related links:
[Déjà Vu - Supported File Formats](https://atrilsolutions.zendesk.com/hc/en-us/articles/205383202-Supported-File-Formats)
[Déjà Vu - Supported Formats And How To Use Them](https://atrilsolutions.zendesk.com/hc/en-us/sections/201686442-Supported-formats-and-how-to-use-them)