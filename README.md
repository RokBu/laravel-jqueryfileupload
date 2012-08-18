## Laravel Bundle

I have upload Sample Laravel application (Laravel-FileUpload) at ## https://github.com/boparaiamrit/Laravel-FileUpload

Install Bundle using artisan and publish assets of bundle. Then set file_upload_dir, thumb_upload_dir and delete_route config
in bundle/config.

### Delete route is used to delete file. When we use route with name 'upload' we use delete route as 'upload' and when we use controllers
like home controller with upload action then we set delete_route as 'home/upload'.

# jQuery File Upload Plugin

## Features
* **Multiple file upload:**  
  Allows to select multiple files at once and upload them simultaneously.
* **Drag & Drop support:**  
  Allows to upload files by dragging them from your desktop or filemanager and dropping them on your browser window.
* **Upload progress bar:**  
  Shows a progress bar indicating the upload progress for individual files and for all uploads combined.
* **Cancelable uploads:**  
  Individual file uploads can be canceled to stop the upload progress.
* **Resumable uploads:**  
  Aborted uploads can be resumed with browsers supporting the Blob API.
* **Chunked uploads:**  
  Large files can be uploaded in smaller chunks with browsers supporting the Blob API.
* **Client-side image resizing:**  
  Images can be automatically resized on client-side with browsers supporting the required JS APIs.
* **Preview images:**  
  A preview of image files can be displayed before uploading with browsers supporting the required JS APIs.
* **No browser plugins (e.g. Adobe Flash) required:**  
  The implementation is based on open standards like HTML5 and JavaScript and requires no additional browser plugins.
* **Graceful fallback for legacy browsers:**  
  Uploads files via XMLHttpRequests if supported and uses iframes as fallback for legacy browsers.
* **HTML file upload form fallback:**  
  Shows a standard HTML file upload form if JavaScript is disabled.
* **Cross-site file uploads:**  
  Supports uploading files to a different domain with Cross-site XMLHttpRequests.
* **Multiple plugin instances:**  
  Allows to use multiple plugin instances on the same webpage.
* **Customizable and extensible:**  
  Provides an API to set individual options and define callBack methods for various upload events.
* **Multipart and file contents stream uploads:**  
  Files can be uploaded as standard "multipart/form-data" or file contents stream (HTTP PUT file upload).
* **Compatible with any server-side application platform:**  
  Works with any server-side platform (PHP, Python, Ruby on Rails, Java, Node.js, Go etc.) that supports standard HTML form file uploads.

## Requirements
* [jQuery](http://jquery.com/) v. 1.6+
* [jQuery UI widget factory](http://wiki.jqueryui.com/w/page/12138135/Widget%20factory) v. 1.8+
* [jQuery Iframe Transport plugin](https://github.com/blueimp/jQuery-File-Upload/blob/master/jquery.iframe-transport.js) (included)
* [JavaScript Templates engine](https://github.com/blueimp/JavaScript-Templates) v. 2.1.0+ (optional)
* [JavaScript Load Image function](https://github.com/blueimp/JavaScript-Load-Image) v. 1.1.6+ (optional)
* [JavaScript Canvas to Blob function](https://github.com/blueimp/JavaScript-Canvas-to-Blob) v. 2.0.0+ (optional)
* [Bootstrap CSS Toolkit](https://github.com/twitter/bootstrap/) v. 2.0+ (optional)

The jQuery UI widget factory is a requirement for the basic File Upload plugin, but very lightweight without any other dependencies.  
The jQuery Iframe Transport is required for [browsers without XHR file upload support](https://github.com/blueimp/jQuery-File-Upload/wiki/Browser-support).  
The UI version of the File Upload plugin also requires the JavaScript Templates engine as well as the JavaScript Load Image and JavaScript Canvas to Blob functions (for the image previews and resizing functionality). These dependencies are marked as optional, as the basic File Upload plugin can be used without them and the UI version of the plugin can be extended to override these dependencies with alternative solutions.

The User Interface is built with Twitter's [Bootstrap](https://github.com/twitter/bootstrap/) Toolkit. This enables a CSS based, responsive layout and fancy transition effects on modern browsers. The demo also includes the [Bootstrap Image Gallery Plugin](https://github.com/blueimp/Bootstrap-Image-Gallery). Both of these components are optional and not required.

The repository also includes the [jQuery XDomainRequest Transport plugin](https://github.com/blueimp/jQuery-File-Upload/blob/master/js/cors/jquery.xdr-transport.js), which enables Cross-domain AJAX requests (GET and POST only) in Microsoft Internet Explorer >= 8. However, the XDomainRequest object doesn't support file uploads and the plugin is only used by the [Demo](http://blueimp.github.com/jQuery-File-Upload/) for Cross-domain requests to delete uploaded files from the demo file upload service.

[Cross-domain File Uploads](https://github.com/blueimp/jQuery-File-Upload/wiki/Cross-domain-uploads) using the [Iframe Transport plugin](https://github.com/blueimp/jQuery-File-Upload/blob/master/js/jquery.iframe-transport.js) require a redirect back to the origin server to retrieve the upload results. The [example implementation](https://github.com/blueimp/jQuery-File-Upload/blob/master/js/main.js) makes use of [result.html](https://github.com/blueimp/jQuery-File-Upload/blob/master/cors/result.html) as a static redirect page for the origin server.

## Browser Support (tested versions)
* Google Chrome - 7.0+
* Apple Safari - 4.0+
* Mozilla Firefox - 3.0+
* Opera - 10.0+
* Microsoft Internet Explorer 6.0+

Drag & Drop is only supported on Google Chrome, Firefox 4.0+, Safari 5.0+ and Opera 12.0+.  
Microsoft Internet Explorer has no support for multiple file selection or upload progress.  
[Extended browser support information](https://github.com/blueimp/jQuery-File-Upload/wiki/Browser-support).

## License
Released under the [MIT license](http://www.opensource.org/licenses/MIT).
