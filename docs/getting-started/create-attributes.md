# Create Attributes

## What is an Attribute?
Attributes are the building blocks of Docuty. The attributes describes what you can document and helps the end user understand how to use the program. Docuty is build to be fully modular and if you feel like there are attributes that you want and is not included by default, you can just create a new one of your liking.

## Creating an Attribute
Creating an attribute is an easy thing to do and most is self explanatory, but in case you need some pointer you can continue reading.

Start by clicking on "Settings" and then "Attributes" in Docuty. You should see a table of all available attributes and remember to always look through it before creating a new one to make sure that there isn't an existing attribute you can use for your case. When certain that you need to create a new on, click "New".

A pop-up will appear with a couple of fields explained here below.
- Name - This is what Docuty uses as an identifier in the background. This need to be unique for all attributes and needs to be in lower case. Alphanumeric characters, underlines (_) and dashes (-) are the only characters permitted.

- Label - This is what you will see in Docuty. This is how the end users identifies the attribute.

- Description (Optional) - Here you can write a short description about the attribute that will help others understand what it's for.

- Visible in lists - Defines if the attribute should have a column in the table listing on each categories first page.

- Visible in detailed view - Defines if the attribute should be shown on a specific items page.

- Required - If the attribute is required to be filled on each item. If you change an attribute after an item is created, the field will be required on next update.

- Store encrypted - Define if you want the value of the attribute to be encrypted. This is convenient when storing sensitive data like passwords.

- Hide input - This can be used if you want the attribute to be hidden in both tables and on specific items view page. Instead a "Copy" button will be shown in tables (which will just copy the value) and "Show content" button on the view page. This is used when you know that the data might be sensitive and don't want anybody looking over your shoulder to see the value.

- Type - Here we specify what kind of attribute this is. This is one of the most important settings in the attribute. Each type has its specific input kind and its own table in the database.
    - Text (wysiwyg) - This is used for larger amount of text like word documents, code, or alike. The input for this will be a WYSIWYG (What You See Is What You Get) editor.

    - Simple text - This is used for larger amount of text like where no format is needed. The input for this will be a plain text editor.

    -  String - This is the most common type. It's just a simple string with an normal input field. Used for things like name, password, username, telephone number, etc.

    -  Integer - Numbers, simply put. It's like string but the input field is constrained to just numbers.

    -  On/Off - Just a simple on/off or true/false attribute. The input field is a check box and can be used for values like alive/dead, enabled/disabled, virtual/physical, etc.

    -  Drop down - This is a multi options attribute where you specify the values that can be chosen. You can also specify if the user can select only one or multiple values.

    -  Image - This is used to upload an image to an entity.

    -  Date - A simple date picker. Can be used to for instance document an installation date, an end of warranty date, etc.

    -  Date range - Like the date field, but for a date range. Can be used to for instance document both a start and an end date for a support contract, or alike.