This cordova plugin is only for android file chooser.

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