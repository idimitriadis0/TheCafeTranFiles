<!-- TOC depthFrom:1 depthTo:6 withLinks:1 updateOnSave:1 orderedList:0 -->

- [CAFETRAN ESPRESSO - PROJECT TEMPLATES](#cafetran-espresso-project-templates)
	- [TEMPLATES - A PRESENTATION](#templates-a-presentation)
	- [CREATING, MANAGING AND USING TEMPLATES](#creating-managing-and-using-templates)
	- [SOME USAGE EXAMPLES](#some-usage-examples)
	- [LIST OF CHANGES](#list-of-changes)
	- [Feedback](#feedback)

<!-- /TOC -->

# CAFETRAN ESPRESSO - PROJECT TEMPLATES

*Updated for CafeTran Espresso 2018*

An explanation of the project templates feature in CafeTran Espresso 2018.

*Curated by [Jean Dimitriadis](https://www.proz.com/translator/2042360) (EN/EL>FR translator).*

<!--- *Shortened link to this document:* --->

## TEMPLATES - A PRESENTATION

When you reopen a project from the Dashboard or the Project menu, CafeTran remembers various settings and resources used before, so that you can quickly pick up from where you left.

What if you want to apply these settings to future jobs, or quickly swap between different settings, to account for different project needs?

Since Yeddi Update 9 (May 2017), CafeTran offers a templates feature which conveniently stores a variety of settings in an XML template file for easy reuse in new projects.

In their current form, project templates store information such as:

- The resources present in the Dashboard, along with their current selection state. This includes:
    - Total Recall memories
    - TMX translation memories
    - Glossaries
    - Web and image resources
    - MT engines and other services
- The docked and joined state of tabs when a project is open (the tabs order is NOT saved, though)
- The selected language pair
- The selected workflow
- The default project location and source file directory (for native projects only)
- The default file format for project creation (Note: In general, CafeTran determines the file format dynamically based on the source file extension)
- Appearance settings such as:
    - The theme and dashboard theme
    - The windows layout
    - Various color settings (found in View > Colors)
- Billing information (applied rate for Statistics)
- "Replace punctuation characters" and "Replace characters at source transfer" options

To find out exactly what information is being stored in a project template, just create a project template in the Dashboard and open the resulting XML file with a text editor. Each line which includes <code>entry key="" value=""</code> represents a setting. There is no need to manually edit the XML files to use the templates feature.

## CREATING, MANAGING AND USING TEMPLATES

Template-related actions are accessible via the Dashboard menu button:

![Dashboard menu button](https://i.imgur.com/E2keydI.png)

The two dropdown menu items related to templates are:

![Templates menu](https://i.imgur.com/sDnZ6OX.png)

- **Open project templates** = Open an already saved project template. You will be asked to select which template file to open.
- **Save project template** = Save a project template as an .xml file. You will be asked to select a location (and file name). The Save dialogue filters only .xml files. You can save changes to an existing project template by saving it under the same file name.

It is up to you to organize your .xml template files as you like.

Consider creating a separate “templates” folder in *cafetran* or *cafetran/projects* folder and saving your templates there. Subdirectories are supported as well.

So, what are the required actions before saving a new template?

Since project templates store content accessible through the Dashboard, as well as settings related to an existing, open project, depending on the use case, you need to perform some steps from the Dashboard and some from an open project before saving or updating a template.

- **Actions from the Dashboard:**  Many template-related settings are directly accessible via the Dashboard, which acts as a template editor.

  - **Resources:**
    - You can choose which resources will be selected by default. If you have many web resources, are working in multiple language combinations, or want to use client-specific resources, you can also remove non-relevant resources and add those that you wish to use.
    - To remove a web resource or a TM/glossary (except the Project memory/glossary), right-click on it and select "Remove from the Dashboard".
    - To add a TM or glossary, use the "Add memory" and "Add glossary" buttons. You can also add TMs by drag-and-dropping the TMX file.
    - To add web resources, you need to either close the Dashboard (Dashboard menu > Close Dashboard) or open an existing project, and open the resources you wish to add (Resources > Web). You can also create new web resources from here (Resources > Add web resource). After opening the resource(s) you wish to add to the Dashboard, close the Project (Project > Close project). The opened/added resources will now be present in the Dashboard.

  - **Language pairs:** Select the default source and target languages you wish to use for the template.

  - **Rate:** You can set your rate from the Dashboard menu (Dashboard > Choose your rate) or from the Statistics in an open project

  - **Workflow:** If you wish to create a template for a specific workflow, select the workflow in Dashboard menu > Project type before saving the template. The Dashboard reverts to the default workflow (Translate a document) when you close a project.

- **Actions from an open project:** In addition to the above actions, you can save the template after closing a project which features the desired settings (if no project has the required characteristics, you can simply create an dummy one). Note: To save all related settings, it is preferable to Quit CafeTran, reopen the program, then save the Template.

  - From an open project (or by closing the Dashboard), you can **add web resources** to the Dashboard (all open resources will be displayed there upon closing the project), see explanations above (Actions from the Dashboard > Resources).

  - Appearance settings (such as **theme, window layout and colors**) can be set from the View menu.

  - The **docked, joined or floating state of tabs** is also remembered when you save a template, which can be very convenient. However, note that the tabs order cannot be saved, and the different tabs may need to be rearranged on each new project. If a joined or docked resource is missing, the joined or docked resources are displayed separately in the tabbed pane.

  - The default **project location** and the **source file directory** saved in the template are those of the last open/created project.

  - **Rate** can also be set via the Statistics (Project > Statistics).


So, in short:

**To save the project settings in Templates**:
  - Open a project with the resources you'd like to use and set the translation interface as you wish to reuse it.
  - Quit CafeTran and reopen the program.
  - In the Dashboard, check that all resources you wish to reuse are present, and that they are ticked.
  - Dashboard menu button > Save project template.

**To update an existing Template**:
- Dashboard menu button > Project templates > select the one you wish to load.
- Open a project, Quit CafeTran and save the template with the same file name.

You can use your file manager to access the templates folder, rename you XML files and organize them in subfolders if you wish so.

Advanced users may tweak XML settings by editing the XML file directly, but this is not recommended. Just use CafeTran Espresso to create and save templates.

## SOME USAGE EXAMPLES

As it can be easily understood, templates are versatile and can be used in a number a ways. Here are some usage examples (these can be combined, of course):

- **Different language pairs**: Resources are likely to be different from one language pair to another. You can create templates for each language pair, each time featuring only the relevant resources.
- **Specific clients/projects/file formats**: You may wish to create different templates for different clients, or for all jobs related to a specific project.
- **Different resources**: You may simply wish to have different resources selected or present per each template, for various reasons. In this case, all actions can be carried out from within the Dashboard. Simply tick or add the desired resources and save the template.
- **Remember layout and tab states**: If you tend to join, dock or float specific resources/tabs, or use different layout or layout/theme/color adjustments, you can easily save these and make new project boot faster.

<!--- Note for same client projects: In this case (although not necessarily recommended), you can even create one CT project and then just add/remove documents keeping the same project resources. This solution will work for CafeTran projects. --->

## LIST OF CHANGES

- 20180307 File creation
- 20180621 Updated for CafeTran Espresso 2018 - Akua Update 10

## Feedback

You can send me feedback via a [ProZ message](https://www.proz.com/?sp=mailsend&eid_s=2042360). Please start your subject with the name of the document: “CafeTran - Templates.
