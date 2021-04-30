# Sigil stylesheets
QT Stylesheets for Sigil ePub editor (https://sigil-ebook.com/)
*version 1.1*

About
-------
These Qt themes (stylesheet) are specially developed for **Sigil** (https://sigil-ebook.com/) and deeply based on themes developed for **FreeCAD** (https://www.freecadweb.org/) by the same developer.
They might work with other software that uses Qt styling.

Dark style with dark editor example:
![Dark-Emerald and Dark Editor stylesheet](/examples/dark_emerald_and_dark_editor.jpg?raw=true "Dark-Emerald stylesheet")

Darker style with dark editor example:
![Dark-Blue and Dark Editor stylesheet](examples/darker_blue_and_dark_editor.jpg?raw=true "Dark-Blue stylesheet")

Light style with light editor example:
![Light-Emerald and Light Editor stylesheet](/examples/light_emerald_and_light_editor.jpg?raw=true "Light-Emerald stylesheet")

You can find a screenshot of all 24 stylesheet variants under [the /examples/ folder](/examples/).


Installation
------
1. Choose a style you like from `/qt_stylesheets/` folder (for instance dark-blue and dark editor) and copy the *.qss* file. Paste it into in the Sigil Preferences folder, which is accesible via `Sigil > Preferences > Open Preferences location`. Note that, by the time being, just one stylesheet can be loaded and there is no option inside Sigil to choose a stylesheet, so you must rename the *.qss* file to the following exact filename: **qt_styles.qss**

2. Place the `/images_dark-light/` folder into the **Preferences folder** (the same one where you just placed qt_styles.qss). The images won't load unless you edit the qt_styles.qss file with a text editor and **change the images URL path to a full path**, that is, you should find the string `qss:` and replace it by `YOUR_USER_PATH/` so that you end up with something like:
    - **OSX** = /Users/[YOUR_USER_NAME]/Library/Application Support/sigil-ebook/sigil/images_dark-light/
    - **WINDOWS** = C:/Users/[YOUR_USER_NAME]/AppData/Local/sigil-ebook/sigil/images_dark-light/
    - **LINUX** = /home/[YOUR_USER_NAME]/.local/share/sigil-ebook/sigil/images_dark-light/

3. You will need to manually edit **Code View colors** (`Preferences > Appearance > Code View > Colors`) in order to match the stylesheet code editor background with some other colors that can only be set there. Alternatively you can use a set of colors that I provide here: go to **Sigil Preferences folder**, (`Sigil > Preferences > Open Preferences location`) and edit the file **sigil.ini** with a text editor. Go to `[user_preferences]` section and change the following lines:

    - if you have chosen a stylesheet with a dark editor:

    ```code_view_css_comment_color=@Variant(\0\0\0\x43\x1\xff\xff\x65xn#\x80\0\0\0)
    code_view_css_property_color=@Variant(\0\0\0\x43\x1\xff\xff\xc8\xaf\xd2z\xe6\x66\0\0)
    code_view_css_quote_color=@Variant(\0\0\0\x43\x1\xff\xff\xa7\xd1\xe6\x66\x7f\n\0\0)
    code_view_css_selector_color=@Variant(\0\0\0\x43\x1\xff\xff\xc7\xbb\x63\xef\xe6\x66\0\0)
    code_view_css_value_color=@Variant(\0\0\0\x43\x1\xff\xff\xe6\x66\xa0$b\b\0\0)
    code_view_font_family_standard=Courier New
    code_view_font_size=18
    code_view_highlight_open_close_tags=true
    code_view_line_highlight_color="@Variant(\0\0\0\x43\x1\xff\xff.\xb2\x33\x9c=p\0\0)"
    code_view_line_number_background_color=@Variant(\0\0\0\x43\x1\xff\xff&\xda+\x2\x33Q\0\0)
    code_view_line_number_foreground_color=@Variant(\0\0\0\x43\x1\xff\xffGLM\x9eZ@\0\0)
    code_view_spelling_underline_color=@Variant(\0\0\0\x43\x1\xff\xff\xff\xff\0\0\0\0\0\0)
    code_view_xhtml_attribute_name_color=@Variant(\0\0\0\x43\x1\xff\xff\xe6\x66\x9f\xf9\x61\xfe\0\0)
    code_view_xhtml_attribute_value_color=@Variant(\0\0\0\x43\x1\xff\xff\x95\x80\xcc\xccp\xa4\0\0)
    code_view_xhtml_css_color=@Variant(\0\0\0\x43\x1\xff\xff\xc8r\xd2n\xe6\x66\0\0)
    code_view_xhtml_css_comment_color=@Variant(\0\0\0\x43\x1\xff\xff\x65\x1en\x14\x80\0\0\0)
    code_view_xhtml_doctype_color=@Variant(\0\0\0\x43\x1\xff\xff\xc8r\xd2n\xe6\x66\0\0)
    code_view_xhtml_entity_color=@Variant(\0\0\0\x43\x1\xff\xff\xe6\x66\xa0[c\x12\0\0)
    code_view_xhtml_html_color=@Variant(\0\0\0\x43\x1\xff\xff\xcc\xccO\\\\\x92\0\0)
    code_view_xhtml_html_comment_color=@Variant(\0\0\0\x43\x1\xff\xff\x65\x1en\x14\x80\0\0\0)
    ```

    - if you have chosen a stylesheet with a light editor:

    ```code_view_css_comment_color=@Variant(\0\0\0\x43\x1\xff\xff\xa0\xa0\xa0\xa0\xaa\xaa\0\0)
    code_view_css_property_color=@Variant(\0\0\0\x43\x1\xff\xff\x32\x32\x32\x32<<\0\0)
    code_view_css_quote_color=@Variant(\0\0\0\x43\x1\xff\xff\x64\x64\xa0\xa0ZZ\0\0)
    code_view_css_selector_color=@Variant(\0\0\0\x43\x1\xff\xff\xa0\xa0<<\xa0\xa0\0\0)
    code_view_css_value_color=@Variant(\0\0\0\x43\x1\xff\xff\xaf\xafnn((\0\0)
    code_view_font_family_standard=Courier New
    code_view_font_size=18
    code_view_highlight_open_close_tags=true
    code_view_line_highlight_color=@Variant(\0\0\0\x43\x1\xff\xff\xe8\xe8\xe8\xe8\xe8\xe8\0\0)
    code_view_line_number_background_color=@Variant(\0\0\0\x43\x1\xff\xff\xdc\xdc\xdc\xdc\xdc\xdc\0\0)
    code_view_line_number_foreground_color=@Variant(\0\0\0\x43\x1\xff\xff\xaa\xaa\xaa\xaa\xb4\xb4\0\0)
    code_view_spelling_underline_color=@Variant(\0\0\0\x43\x1\xff\xff\xff\xff\0\0\0\0\0\0)
    code_view_xhtml_attribute_name_color=@Variant(\0\0\0\x43\x1\xff\xff\xaf\xafnn((\0\0)
    code_view_xhtml_attribute_value_color=@Variant(\0\0\0\x43\x1\xff\xff\x64\x64\xa0\xa0ZZ\0\0)
    code_view_xhtml_css_color=@Variant(\0\0\0\x43\x1\xff\xff\x32\x32\x32\x32<<\0\0)
    code_view_xhtml_css_comment_color=@Variant(\0\0\0\x43\x1\xff\xff\xa0\xa0\xa0\xa0\xaa\xaa\0\0)
    code_view_xhtml_doctype_color=@Variant(\0\0\0\x43\x1\xff\xff\x32\x32\x32\x32<<\0\0)
    code_view_xhtml_entity_color=@Variant(\0\0\0\x43\x1\xff\xff\xaf\xafnn((\0\0)
    code_view_xhtml_html_color=@Variant(\0\0\0\x43\x1\xff\xff\xcd\x41)a9\xc4\0\0)
    code_view_xhtml_html_comment_color=@Variant(\0\0\0\x43\x1\xff\xff\x65\x1en\x14\x80\0\0\0)
    ```


From there you can tweak the colors from the Sigil Preferences user interface at your will.

Known bugs and TO DOs
------
- you can just select one stylesheet. It would be nice to have a preference entry to select between a list of *.qss* files
- you should set a full path for images (icons) to be drawn in Sigil. It would be nice that a "Preferences folder location" variable is set so that the stylesheet just writes *qss:* and Sigil changes it on the fly.
- inside `Tools > Add cover...` window there is a splitter that shows zoomed, it seems to be something hardcoded.
- as Sigil already lets user setup some colors inside `Preferences > Appearance`, it's kind of messy because you need to "syncronize" colors from the stylesheet with those color Preferences in order to get a final nice theme. It would be desiderable that all "Code editor" colors can be accesible by `Preferences > Appearance` and another Preference entry let user choose between a list of UI styles (.qss files).

Customization
------
If you would like to change the overall look/style of the theme, open the .qss file with a text editor and you will find a table with all the colors used. You will just need to "find and replace" the old colors for your new ones.


License
------
Copyright (c) 2021 Pablo Gil Fernández.

![Attribution-ShareAlike 4.0 International](http://i.creativecommons.org/l/by-sa/3.0/88x31.png)
This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/).
