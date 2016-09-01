This cordova plugin is used to pick the files from device directory.

please add your package name into FileChooser.java and FileChooserActivity.java, for example:

import com.yourAppId.R;

Usage:

  var success = function (data) {
       console.log('get your file uri here :' + data.filepath;)
       console.log('get your file mime here :' + data.mimetype;) 
  };

  var error = function (msg) {
     alert('open file error: ' + msg);
  };
  
  window.plugins.filechooser.open({}, success, error);
  
  
![image](https://github.com/wlw362034710/cordova-filechooser-/blob/master/com.cesidiodibenedetto.filechooser/screenShots/filechooser1.png)

![image](https://github.com/wlw362034710/cordova-filechooser-/blob/master/com.cesidiodibenedetto.filechooser/screenShots/filechooser2.png)

The plugin is only support for Android 4+(IOS is not supported).

PS:for ios file picker please refer to: com.jcesarmobile.filepicker

