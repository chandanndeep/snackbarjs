# SnackbarJS

SnackbarJS is a lightweight and jQuery powered plugin made to work in Bootstrap style, just like the Bootstrap tooltips work.

Include it with:

    <head>
        <link href=snackbar.min.css rel=stylesheet>
    </head>
    <body>
        ...
        <script src=snackbar.min.js></script>
    </body>

Use it is easy as write:

    <span data-toggle=snackbar data-content="This is my awesome snackbar!">Click me</span>

or

    $.snackbar({content: "This is my awesome snackbar!"});

## Options

There are some options to customize SnackbarJS look and beahvior:

    var options =  {
        content: "Some text", // text of the snackbar
        style: "toast", // add a custom class to your snackbar
        timeout: 100 // time in milliseconds after the snackbar autohides, 0 is disabled
    }

    $.snackbar(options);

**Tip**: SnackbarJS returns always a jQuery element which corresponds to the snackbar DOM element, you can use it to get the ID of it, or do any kind of stuff with it.

## Interact with snackbars

Once you have created a snackbar you can show, hide or toggle it with:

    $("#snackbarid").snackbar("show");
    $("#snackbarid").snackbar("hide");
    $("#snackbarid").snackbar("toggle");
    
`#snackbarid` can be both the button with the data-toggle=snackbar attribute or the snackbar element.  
Call it on a not-existing snackbar will create it before the specificed action.

## Demo

To see SnackbarJS in action visit [the demo page](http://fezvrasta.github.io/snackbarjs/).
