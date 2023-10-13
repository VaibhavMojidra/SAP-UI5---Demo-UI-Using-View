# SAP UI5 Demo UI Using View

SAPUI5 supports multiple view types (XML, HTML, JavaScript). We choose XML as this produces the most readable code and will force us to separate the view declaration from the controller logic. 

We create a new view folder in our app and a new file for our XML view inside the app folder. The root node of the XML structure is the view. Here, we reference the default namespace sap.m where the majority of our UI assets are located. We define an additional sap.ui.core.mvc namespace with alias mvc, where the SAPUI5 views and all other Model-View-Controller (MVC) assets are located.

```<mvc:View
   xmlns="sap.m"
   xmlns:mvc="sap.ui.core.mvc">
   <Text text="Hello World"/>
</mvc:View>```