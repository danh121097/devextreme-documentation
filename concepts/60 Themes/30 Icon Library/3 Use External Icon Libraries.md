DevExtreme UI widgets support external icon libraries ([Font Awesome](https://fortawesome.github.io/Font-Awesome), [GLYPHICONS](https://glyphicons.com) and [ionicons](https://ionicons.com)).

To use an icon library, add a link to the appropriate style sheet.

    <!--HTML-->
    <!--Font Awesome-->
    <link rel="stylesheet" type="text/css" href="/css/font-awesome.css" />

    <!--GLYPHICONS-->
    <link rel="stylesheet" type="text/css" href="/css/glyphicons.css" />

    <!--ionicons-->
    <link rel="stylesheet" type="text/css" href="/css/ionicons.min.css" />

[note]Referenced style sheet should contain a valid link to an icon font file.

To display an icon from an external library within a UI widget, pass the icon's css selector to the [widget](/concepts/60%20Themes/30%20Icon%20Library/0%20Use%20Icons%20for%20Widgets.md '/Documentation/Guide/Themes/Icon_Library/#Use_Icons_for_Widgets')'s or [command](/concepts/60%20Themes/30%20Icon%20Library/1%20Use%20Icons%20for%20Commands.md '/Documentation/Guide/Themes/Icon_Library/#Use_Icons_for_Commands')'s **icon** option, or to an item object's **icon** field if you need to display an icon for a collection widget item.

    <!--JavaScript-->
    //Font Awesome
    var buttonOptions = {
        ...
        icon: 'fa fa-home'
    }

    //GLYPHICONS
    var buttonOptions = {
        ...
        icon: 'glyphicon glyphicon-home'
    }

    //ionicons
    var buttonOptions = {
        ...
        icon: 'ion ion-home'
    }

[note]

For Font Awesome version 5, add the following CSS to ensure icons are rendered properly:

    <!--CSS-->
    .dx-icon.fa {
        width: auto;
        height: auto;
    }

[/note]