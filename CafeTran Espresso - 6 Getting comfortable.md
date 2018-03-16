# CAFETRAN ESPRESSO 2018 - GETTING COMFORTABLE

*Updated for CafeTran Espresso 2018 - Akua*

Customizing CafeTran. An introduction.

*Curated by [Jean Dimitriadis](https://www.proz.com/translator/2042360) (EN-FR/EL-FR translator).*

## PART I | TAKING A TOUR

### Intro

So you’ve installed CafeTran Espresso on your computer.

Let’s take some time to get acquainted and adjust it to your liking.

Once you accept the software license, you are greeted by the Dashboard.

To take a peek at the translation interface, you can close the Dashboard (Dashbord menu button > Close Dashboard) or simply create a new project.

### New dummy project

To create a new project, on the top right, select one of your language pairs.

Next, click New, or drag and drop a text file on the Dashboard.

Enter a project name and select the folder which will contain your project(s).

OK, let’s start getting comfortable.

### Look and Feel & Large icons

First, go to Preferences (Options) > Appearance.

Depending on your computer, you might want to uncheck the **Large icons**.

From here, you can also select a global **Look and Feel** theme.

CafeTran offers three options:

- The **Metal** Look and Feel
- The **Nimbus** Look and Feel (default)
- A third Look and Feel meant to blend with your operating system:
    - **Windows**
    - **Mac OS** for OS X
    - **GTK** for Linux

Feel free to find which suits you best.

CafeTran needs to be restarted for these new settings to take effect.

Appearance can be refined further with Themes and Colors, so let’s do that next.

<!--- TODO  (we'll also see some examples of Look and Feel, Themes and window Layout in action). --->
### Themes

![View > Themes submenu](https://i.imgur.com/2Movlv0.png)

Next, go to View > Themes.

CafeTran has a range of color-based or image-based themes to choose from.

They can be customized depending on your personal preferences.

Available choices are: Dark, Bright (default), System, and Dark/Bright image background, with or without transparency.

Bright or Dark? The choice is yours.

Transparency adds yet another twist, allowing to tweak the transparency level of the chosen image or color background at will.

The System theme provides a more neutral base look.

It goes well with the Windows/Mac OS/GTK Look and Feel theme, but does nicely on the Metal and Nimbus Look and Feel as well.

<!--- TODO Here are some examples of Look and Feel & Themes: --->

### Colors

![View > Colors submenu](https://i.imgur.com/D2ZE2e8.png)

View > Colors allows you to customize colors for various interface elements.

Choosing a Look and Feel and a Theme is usually enough, but it is good to know you can also tweak the various color settings within a theme should you wish so.

Messed up and want to revert to the default theme colors? Just reset them [Set default colors].

### Dashboard theme

When you have settled with the above, you can also choose one of the two themes available for the Dashboard.

Via the Dashbord menu button, select the Coffeehouse theme and see if it suits you better than the default one.

### Font face and size

![View > Font submenu](https://i.imgur.com/HlSPRCn.png)

In View > Fonts, you can set the font face and size for various UI items.

Choose your favorite installed font in terms of on-screen readability (or OS uniformity). Try to stick to the same font for all UI options.

Depending on your screen resolution, preference and eyesight, you might need to take some time to adjust the font size for the User interface and/or some of its specific elements.

Remember, you can easily make the source and target editor segment text bigger or smaller (via the Zoom commands or buttons).

### Window layout

![View > Window layout submenu](https://i.imgur.com/fvyhk7K.png)

Let’s now focus on the Window layout.

Depending on the project/workflow type, your screen resolution or your own preference, you might want to switch between the three available layout options. Try them out instantly!

Each layout has its reversed, mirror-like variant.

Also, each pane features handles for ad-hoc adjustment.

Resources can be further docked vertically or horizontally to the various panes, joined together, or even floated (for example to a separate monitor).

Do you prefer your Source/Target segment editors horizontal instead of vertical? No problem: View > Segment editors.

This degree of layout/appearance customizability is rarely found in other CAT tools, so use it to your advantage!

*Usage example: since I work on a laptop and tend to give much space to the resources in the tabbed pane, I prefer to use the Window layout 2.*

### Translation interface and Panes

At this point, you might be asking yourself: What does each pane do? Let’s see:

![CafeTran’s translation interface](https://i.imgur.com/EOIUVW9.png)

- **The Segments Grid**: This is where all the segmented text elements from the source file(s) are shown in sequenced order (or according to the Search and Filter options).
- **The Source and Target segment editors**: The current Source and Target text boxes where you edit your translation. We’re at the heart of the action!
- **The Tabbed pane**: The tabbed pane holds various sets of resources such as Translation memories, Glossaries, MT engines and web resources. Tabs can be reordered, docked to a specific pane, joined together or floated. At nauseum.
  - **The Matchboard**: An important CafeTran feature, the Matchboard conveniently aggregates matches/results from various resources (memory segments and fragments, glossary entries, Machine Translation suggestions, etc.) in one place. Technically, it is still a Tab, so you can dock it anywhere, just like one. Ideally, it should be close to your segment editors, and visible at all times.
- **The Quick Search bar**: Found at the top, just below the Menu, it allows you to quickly query different resources and conduct various searches (these can be launched via keyboard shortcuts as well) in Project or TM Source and Target segments, glossaries, MT engines, web resources, etc. Additional search and filtering settings (and the all important Find and Replace operations) are accessible via the standard Ctrl+F (or Cmd+F) command, which brings up the (Advanced) Search window. More filtering actions can be performed via the Filter menu.

So there you have it!

### Detached windows

Now, it is good to know that CafeTran offers a detached windows mode (View > Detached windows/Attached windows).

Very handy if you use CafeTran with an external editor or a second screen.

Depending on the window layout, the panes are detached differently, so feel free to experiment.

### Toolbars

To avoid unnecessary complexity in the beginning, CafeTran hides some of its menus by default.

Depending on your needs, you might need to Show more menus.

Just go to View > and select which you wish to have displayed or hidden.

And that concludes part I.

## PART 2 | Taking it further

This was a pretty quick tour. By now, you should have a better idea of how to begin customizing CafeTran according to your image.

Below, you’ll find some additional pointers and considerations to take it further.

### TAMING THE PREFERENCES

CafeTran comes with sane default settings, so you don’t have to change much to get started.

You can adjust the Preferences to your needs over time.

To dive deeper into Preferences, see the related [Preferences](https://github.com/idimitriadis0/TheCafeTranFiles/wiki/1-Preferences#segmentation) reference document. Take your time.

Still, there are some Preferences you might wish to set up soon:

**Preferences > General > Segmentation**

Defining the segmentation rules which will be applied for a given project is an important consideration. Check out the available options. The default (Sentence) is fine for basic needs, but you may want to explore more advanced (SRX) solutions. Recommendation: Review the Suggestion section under [Segmentation](https://github.com/idimitriadis0/TheCafeTranFiles/wiki/1-Preferences#segmentation) in the “Preferences” reference document.

**Preferences > Memory > Java Memory size (MB)**

You can define the amount of RAM dynamically allocated to Java for CafeTran’s operation.

Since resources are loaded in RAM, if you have 8 GB RAM or more, you can safely push this setting higher for a more comfortable operation. Consider increasing the default value from 1024 to 2048 (or higher). In this case, also make sure you have installed the 64-bit Java version from Oracle.

**Preferences > MT services**

If you’d like to receive Machine Translation suggestions while working on your translations, you’ll probably want to set up the available [MT services](https://github.com/idimitriadis0/TheCafeTranFiles/wiki/1-Preferences#mt-services) (Google Translate, MS Translator, MyMemory and Yandex.Translate).

Some MT services can also be queried via their web interface, straight from within CafeTran. Depending on your language pairs, check out DeepL, Google Translate, Bing Translator and Youdao, in Resources > Web (or enable them from the Dashboard).

**Preferences > Web services**

Want to query the KudoZ and other ProZ terminology resources while staying in CafeTran? Enable the [ProZ.com](https://github.com/idimitriadis0/TheCafeTranFiles/wiki/1-Preferences#web-services) service (disable WIWO if you don’t want it) and sign in to your account! You’ll also be able to ask KudoZ questions. Be sure to check the [available options](https://github.com/idimitriadis0/TheCafeTranFiles/wiki/2-Menu-and-Interface#proz-tab-and-context-menu) once logged in.

**Preferences > Keyboard shortcuts**

Keyboard shortcuts speed up things greatly.   And the point of using a CAT tool is to make your work efficient (and enjoyable), right?

At one point, you should take a moment to go through the various available shortcuts. There are a lot of them! Most (if not all) are found in the Preferences > Keyboard shortcuts.

If any is not self expalanatory, you can check the [Keyboard shortcuts](https://github.com/idimitriadis0/TheCafeTranFiles/wiki/1-Preferences#keyboard-shortcuts) section of the Preferences reference file to find out what it does.

You might wish to customize some as well.

Here are a few examples (by no means prescriptions, just to give an idea):

- Since I tend use the **Default scope** much (for searching the selected web resource), I give it the Ctrl(Cmd)+Enter shortcut and switch the **Add segment to memory and go to next untranslated segment** to Ctrl+Shift+Down. Ctrl+Enter was the historical shortcut given to the Default scope in CafeTran anyway.
- To avoid splitting or merging segments accidentally, I either disable **Split segment** and **Merge segment** shortcuts or assign a non casually triggered one, such as Alt+PageUp/PageDown.

It’s up to you!

### TAMING THE INTERFACE AND MENUS

You will certainly want to learn more about CafeTran’s translation interface and menus.

Many actions are accessible via shortcuts as well. Some menus give access to additional handy options. Take some time to cycle through them.

By default, help tips are shown at the bottom left when you hover a menu or a UI element.

To dive deeper info Menus, see the reference document “[Menus and Interface](https://github.com/idimitriadis0/TheCafeTranFiles/wiki/2-Menu-and-Interface)”.

**Resources > Web**

Speaking of Menus, being able to query various Web resources from within CafeTran’s interface is a great advantage.

If you wish to use this feature, you’ll want to add and organize web resources relevant for your language combinations and subject matter. Here, you will find explanations and [suggestions on adding web resources](https://github.com/idimitriadis0/TheCafeTranFiles/wiki/2-Menu-and-Interface#addedit-resource-window).

Want to query all open web resources at once? Make sure Resources > Simultaneous web search is ticked (it is by default). Otherwise, just uncheck this option, to avoid delays and overload.

### MEMORIES AND TERMBASES/GLOSSARIES

**Translation Memories** are an important part of any CAT tool and CafeTran is no exception.

In this regard, “settings are everything” as one would say.

Places to visit:

- **Preferences > Memories** holds various settings related to TMs (see the [Memories section](https://github.com/idimitriadis0/TheCafeTranFiles/wiki/1-Preferences#memory) in the reference documentation). To save the latest changes to a read and write TM (with Save newest duplicates), either use Memory > Import segments from projects and select your TM or use Project > Export and exchange > To TMX memory with no Filters on.
- **Memory menu** (if hidden, View > Show Memory menu) with various [Memory related actions](https://github.com/idimitriadis0/TheCafeTranFiles/wiki/2-Menu-and-Interface#memory).
- **Task > TMX memory** submenu for [tasks related to TM maintenance](https://github.com/idimitriadis0/TheCafeTranFiles/wiki/2-Menu-and-Interface#task--tmx-memory-submenu).
- And, of course, the various [TM options](https://github.com/idimitriadis0/TheCafeTranFiles/wiki/3-TM-options) (and Total Recall options) available for each TM individually. There is a whole reference document dedicated to these.

**Termbases for fragments vs glossaries?**

CafeTran memories do not only store segments. They can also store fragments and be used as Termbases. Fragments or subsegments are parts of segments and phrases. They can consist of one or more terms (which in turn can consist of one or more words). In such a case, using a Memory for storing both segments and fragments (see TM options above) can be all you need. You can also set up a separate Memory meant to store fragments only.

Another way of tackling terminology is to use Glossaries. In CafeTran, Glossaries are simple tab-delimited text files for storing terms.

Both approaches have their advantages and disadvantages, fervent adepts and detractors.

You will find your own (possibly hybrid approach) on that front.

### TEMPLATES

CafeTran offers a templates feature which stores a variety of settings in template file for easy reuse in new projects.

Saving and loading templates is accessible via the Dashboard menu.

This can be very convenient, especially if you happen to work on different language pairs or wish to  quickly swap resources and (various) settings from one project to another.

If so, check out the reference document on [Project templates](https://github.com/idimitriadis0/TheCafeTranFiles/wiki/5-Project-templates).

### FILE FORMATS

CafeTran handles many file formats natively and allows you to work on external project as well. For file types not directly supported, there are (almost) always solutions. All this is covered in the [File formats](https://github.com/idimitriadis0/TheCafeTranFiles/wiki/4-File-formats) reference document.

Of special interest if you intend to work on external bilingual files and packages (SDL Trados, MemoQ, Wordfast, etc.): Read the General notes in the [External Projects](https://github.com/idimitriadis0/TheCafeTranFiles/wiki/4-File-formats#external-projects) section, as well as the section dedicated on the related CAT tool.

And that concludes part II. This should give you a good head start!

## LIST OF CHANGES

- 20180316 File creation

## Feedback

You can send me feedback via a [ProZ message](https://www.proz.com/?sp=mailsend&eid_s=2042360). Please start your subject with the name of the document: “CafeTran - Getting comfortable.
