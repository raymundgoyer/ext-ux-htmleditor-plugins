# MOVED TO GITHUB #

https://github.com/VinylFox/ExtJS.ux.HtmlEditor.Plugins

This code repository will no longer receive updates, please visit Github for most recent version.

# Ext.ux.form.HtmlEditor.Plugins #
![http://www.vinylfox.com/wp-content/uploads/2009/06/htmleditor-plugin-set.png](http://www.vinylfox.com/wp-content/uploads/2009/06/htmleditor-plugin-set.png)

This is a set of plugins for the ExtJS HtmlEditor that add more advanced HTML editing capabilities. Learn more about these plugins on my [blog post about them](http://www.vinylfox.com/plugin-set-for-additional-extjs-htmleditor-buttons/).

Currently, these are the plugins that have been created for this set:

  * WordPaste
  * Divider
  * Table
  * HR
  * IndentOutdent
  * SubSuperScript
  * RemoveFormat
  * MidasCommand
  * SpecialCharacters

## Example Usage ##

```
{
	xtype: 'htmleditor',
	...,
	plugins: [
		new Ext.ux.form.HtmlEditor.Word(),  
		new Ext.ux.form.HtmlEditor.Divider(),  
		new Ext.ux.form.HtmlEditor.Table(),  
		new Ext.ux.form.HtmlEditor.HR(),  
		new Ext.ux.form.HtmlEditor.IndentOutdent(),  
		new Ext.ux.form.HtmlEditor.SubSuperScript(),  
		new Ext.ux.form.HtmlEditor.RemoveFormat() 
	],
	...
}
```

## Button Icons ##

The icons used for each of the buttons is not provided as part of this plugin, they must be acquired separately. An example of the CSS needed for each buttons icon is provided in the [styles.css](http://code.google.com/p/ext-ux-htmleditor-plugins/source/browse/trunk/src/styles.css) file located in the src folder. Here is an example style for the table button icon.

```
.x-edit-table {background: url(../images/table.png) 0 0 no-repeat !important;}
```

The style name is generated from the midas command name which can be found in the _cmd_ property of the plugin. In the case of non midas commands, the _onRender_ handler of the plugin has a reference to the _iconCls_ name used.

For nice icon sets, check out the following sites.
  * http://www.famfamfam.com/
  * http://code.google.com/p/fugue-icons/
  * http://www.everaldo.com/crystal/