# ui5\_async\_load

> Test loading ui5 asynchronously by specifying the preload=async bootstrap attribute

This app shows an example of loading UI5 with the preload=async attribute. This causes the loading of libraries to occur asynchronously. However the core must still load synchronously first. Performance testing has shown that this is marginally faster than the standard bootstrap, but not worth bothering about unless you want to display a spinner/splash screen, etc.
The difference between this method and the dynamic boostrap insertion method is that the UI5 core must load before the spinner will be shown. So if you want all the load time occupied by a spinner then use the dynamic technique, otherwise if you don't mind a lag before the spinner shows then this oneis pretty simple.

Page load times - a comparison: https://docs.google.com/spreadsheet/ccc?key=0AophLm-khFuodGJTNV9MQ0t2c05fU1phdGh3LVVJTWc&usp=sharing

Generated by Yeoman: generator-openui5.
