# SAP UI5 Demo UI Using XML

SAPUI5 supports multiple view types (XML, HTML, JavaScript). We choose XML as this produces the most readable code and will force us to separate the view declaration from the controller logic. 

We create a new view folder in our app and a new file for our XML view inside the app folder. The root node of the XML structure is the view. Here, we reference the default namespace sap.m where the majority of our UI assets are located. We define an additional sap.ui.core.mvc namespace with alias mvc, where the SAPUI5 views and all other Model-View-Controller (MVC) assets are located.

```
<mvc:View
   xmlns="sap.m"
   xmlns:mvc="sap.ui.core.mvc">
   <Text text="Hello World"/>
</mvc:View>
```

### Code Explaination:

- `<mvc:View>`: This is the root element of an XML view. It represents a view in the Model-View-Controller (MVC) architecture. The `mvc` prefix is associated with the `sap.ui.core.mvc` namespace, which is where the View class is defined.

- `xmlns="sap.m"`: This defines the default namespace for the XML document. In this case, it's set to `sap.m`, which means that you can use controls from the `sap.m` library (like Button, Input, etc.) directly without having to prefix them.

- `xmlns:mvc="sap.ui.core.mvc"`: This defines an additional namespace for the XML document. The `mvc` prefix is associated with the `sap.ui.core.mvc` namespace. This allows you to use classes from this namespace in your XML view.

So, this code is essentially setting up an empty SAPUI5 XML view that can use controls from the `sap.m` library and classes from the `sap.ui.core.mvc` namespace. You would typically add more controls inside the `<mvc:View>` tags to create your user interface.
