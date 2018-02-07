# Opencart 3 Summernote Cleaner

Opencart 3 modification module (OCMOD) for the [Summernote](https://github.com/summernote/summernote/) that adds a button and/or paste functionality for cleaning styles from text.

Completely based on the [summernote-cleaner](https://github.com/DiemenDesign/summernote-cleaner/) plugin.


#### 1. Summernote options

You can manualy change theese options in summernote-cleaner.js before install.

```javascript
$('.summernote').summernote({
    toolbar:[
        ['cleaner',['cleaner']], // The Button
        ['style',['style']],
        ['font',['bold','italic','underline','clear']],
        ['fontname',['fontname']],
        ['color',['color']],
        ['para',['ul','ol','paragraph']],
        ['height',['height']],
        ['table',['table']],
        ['insert',['media','link','hr']],
        ['view',['fullscreen','codeview']],
        ['help',['help']]
    ],
    cleaner:{
          action: 'both', // both|button|paste 'button' only cleans via toolbar button, 'paste' only clean when pasting content, both does both options.
          newline: '<br>', // Summernote's default is to use '<p><br></p>'
          notStyle: 'position:absolute;top:0;left:0;right:0', // Position of Notification
          icon: '<i class="note-icon">[Your Button]</i>',
          keepHtml: false, // Remove all Html formats
          keepOnlyTags: ['<p>', '<br>', '<ul>', '<li>', '<b>', '<strong>','<i>', '<a>'], // If keepHtml is true, remove all tags except these
          keepClasses: false, // Remove Classes
          badTags: ['style', 'script', 'applet', 'embed', 'noframes', 'noscript', 'html'], // Remove full tags with contents
          badAttributes: ['style', 'start'], // Remove attributes from remaining tags
          limitChars: false, // 0/false|# 0/false disables option
          limitDisplay: 'both', // text|html|both
          limitStop: false // true/false
    }
});
```
#### 2. Install

- To begin, make backup, really!
- Go to your OpenCart Admin and open Extensions menu
- Open Installer
- Click the Upload button
- Find, select and upload the summernote-cleaner.ocmod.zip file
- See the "Success: You have modified extension!" message
- Go to Extensions > Modifications > [Refresh] button
- Go to Dashboard > [ Developer Settings] button -> [Refresh] button
- Check

#### 3. Uninstall

- Make backup again
- OpenCart Admin -> Extensions menu - Installer
- Find summernote-cleaner.ocmod.zip in Install History list and click [Uninstall] button
- Go to Extensions > Modifications > [Refresh] button
- Go to Dashboard > [ Developer Settings] button -> [Refresh] button
- Check

#### 4. Thanks:
- [Diemen Design](https://github.com/DiemenDesign/)

