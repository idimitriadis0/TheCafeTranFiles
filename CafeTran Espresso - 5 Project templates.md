# CAFETRAN ESPRESSO - PROJECT TEMPLATES

*Updated for CafeTran Espresso 11 Poppy Seed Roll (2022)*

CafeTran Espresso's project templates feature, explained.

*Curated by [Jean Dimitriadis](https://www.proz.com/translator/2042360) (EN/EL>FR translator).*

## PROJECT TEMPLATES - A PRESENTATION

As you work on native or external projects, CafeTran remembers various settings, layouts and resources, and applies them to new projects as well.

What if you want to quickly swap between different settings, to account for different project needs (like different clients, resources and/or language pairs)?

Or what if you wish to make a backup of the current configuraton, which you can restore later, after having modified it in the meantime?

**CafeTran offers a project templates feature which conveniently stores a variety of settings in an XML file for easy reuse in the future.**  

*Note: This is different than CafeTran Preferences, which can be exported for backup or migration purposes and imported in the Preferences. Exporting Preferences also produces an XML file, which however stores more information than the project templates. One could say that CafeTran Preferences are more global, and Project templates are more project-specific.*

### What is stored in a project template

To help you assess the usefulness of using project templates, here are some of the settings that are stored in project templates:

- The resources present in the Dashboard, along with their current selection state. This includes:
    - Total Recall memories
    - TMX translation memories
    - Glossaries
    - Web and image resources
    - MT engines and other services
- The docked and joined state of tabs when a project is open (the tabs order is not saved, though, but these can easily rearranged by drag-and-drop)
- The selected language pair
- The selected Project type (Dashboard menu ≡ > Project type)
- The default project location and source file directory (for native projects only, external projects are edited directly at the original location)
- The default file format for project creation (Note: In general, CafeTran determines the file format dynamically based on the source file extension)
- Billing information (applied rate for Statistics)
- "Replace punctuation characters" and "Replace characters at source transfer" options
- Options for QA checks
- Segment skipping options (Action menu > Skip)
- Window layout

As you see, only few of these settings relate to ones found in the Preferences. Likewise, the Theme settings are not stored (though they were in the past).

*Note: To find out exactly what information is being stored in a project template, just create one in Dashboard and open the resulting XML file with a text editor. Each line which includes <code>entry key="" value=""</code> represents a setting. However, there is absolutely no need to manually edit the XML files to use the templates feature.*

## CREATING, MANAGING AND USING PROJECT TEMPLATES

Project template-related actions are accessible via the Dashboard menu button ≡.

Here are drop-down menu items related to project templates:

![Templates menu](https://i.imgur.com/rnFRSSg.png)

- **Recent project templates** = Your recently used templates will be shown here.
- **Open project templates** = Open an already saved project template. You will be asked to select which template file to open.
- **Save in project template** = Save the current state in a project template as an .xml file. You will be asked to select a location and file name. The Save dialogue filters only .xml files. 
- **Remove current project template** = Self-explanatory. But how can you tell which is that? The current project template is indicated in the upper-left section of the Dashboard, just above the Total Recall column.
- To which we can add another, not pictured above: **New Dashboard**. This command removes the current project template. After that, you can work either without any project templates, or treat it as the entry point to create a new project template from the modified Dashboard state.

### How to save the current state in a project template

If you are happy with the current configuration and wish to store it for reuse in the future, after closing your project, just select "Save in a new template" in the Dashboard menu and chose a save location and a file name in the dialog that opens.

Simple. But **here's the trick**:

We know that CafeTran trackes and saves automatically the latest settings in whichever project template is currently used.

To save the current state for future reuse, without modifying it any further, you should stop using the project template after saving it.

There are two methods to do that:
- Save a second project template (with a different name) just after saving the first one ( the "master" project template, so to speak) and continue using that.
- Apply the Dashboard menu ≡ actions "Remove current project template" or "New Dashboard" to unload the project template.

Any further modifications will not be stored in the (first) saved project template.

At any moment, you can then open(load) the saved project template to restore and reuse the saved state.

### Where to save project templates

It is up to you to organize your .xml template files as you like.

Consider creating a separate “templates” folder in *cafetran* or *cafetran/projects* folder and saving your templates there. Subdirectories are supported as well.

### Preparing to create a project template

A project template is about storing CafeTran's current state in order to reuse in the future, so you may wish to give a little thought on the configuration you want to save.

Of course, this also depends on the intended use case (see the next section for such examples).

Here are some items that you might want to consider before saving or updating a template.

- **Actions from the Dashboard:**  Some template-related settings are directly accessible via the Dashboard.
	- **Resources:**
	    - You can choose which resources will be selected by default. If you have many web resources, are working in multiple language combinations, or want to use client-specific resources, you can also remove non-relevant resources and add those that you wish to use.
	    - To remove a web resource or a TM/glossary (except the Project memory/glossary), right-click on it and select "Remove".
	    - To add a TM or glossary, use the "Add memory" and "Add glossary" buttons. You can also add TMs by drag-and-dropping the TMX file.
	    - To add previously unused web resources to the Dashboard, you need to either close the Dashboard (Dashboard menu ≡ > Close Dashboard) or open an existing project, and open the resources you wish to add (Resources > Web). You can also create new web resources from here (Resources > Add web resource). After opening the resource(s) you wish to add to the Dashboard, close the Project (Project > Close project). The opened/added resources will now be present in the Dashboard.
	- **Language pairs:** Select the default source and target languages you wish to use for the template.
	- **Rate:** You can set your rate from the Dashboard menu ≡ > Choose your rate or from the Statistics in an open project.
- **Workflow:** If you wish to create a template for a specific workflow, select the workflow in Dashboard menu ≡ > Project type before saving the template. The Dashboard reverts to the default workflow (Translate a document) when you close a project.

- **Actions from an open project:** In addition to the above actions, you can save the template after closing a project which features the desired settings (if no project has the required characteristics, you can simply create a new one).
	 - From an open project (or by closing the Dashboard), you can **add web resources** to the Dashboard (all open resources will be displayed there upon closing the project), see explanations above (Actions from the Dashboard > Resources).
	  - The layout can be set from the View menu.
	  - The **docked, joined or floating state of tabs** is also remembered when you save a template, which can be very convenient. However, note that the tabs order cannot be saved, and the different tabs may need to be rearranged on each new project. If a joined or docked resource is missing, the joined or docked resources are displayed separately in the tabbed pane. Interface elements can also be adjusted by handlebars.
	  - The default **project location** and the **source file directory** saved in the template are those of the last open/created project.
	  - **Rate** can also be set via the Statistics (Project > Statistics).

Project templates cannot be saved or opened from the main translation interface. These actions are only accessed via the Dashboard, so:

- Once you have the project state you wish to save, close the project (Project > Close project) or exit CafeTran (Project > Exit) and restart the program.
- In the Dashboard, check that all resources you wish to reuse are present, and that they are ticked.
- Dashboard menu button ≡ > Save in project template.

*Note: You can use your file manager to access the templates folder, rename you XML files and organize them in subfolders if you wish so.*

*Advanced users may tweak XML settings by editing the XML file directly, but this is not recommended. Just use CafeTran Espresso to create and save templates.*

## SOME USAGE EXAMPLES

As it can be easily understood, project templates are versatile and can be used in a number a ways. 

Here are some of the main use cases:

- **Specific clients or projects**: You may wish to create different templates for different clients, or for all jobs related to a specific project.

- **Different language pairs**: Resources are likely to be different from one language pair to another. You can create templates for each language pair, each time featuring only the relevant resources.

- **Different workflow/layout:** Different project types (Dashboard menu ≡ > Project type) require a different configuration of the UI elements, and so do some workflows. For example, you might want to save a carefully crafted layout for translating and its twin for reviewing (all MT and resources disabled, big Grid -layout 6-, focus on the text, no distraction). Or one for when you are home with your dual screen setup (where you chose to float some panel on the second screen) and one for when you are on the road, or to stay within the CafeTran metaphor, in a cafe.