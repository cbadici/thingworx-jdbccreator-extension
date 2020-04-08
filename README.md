# thingworx-jdbccreator-extension
[Unofficial/Not supported] Extension that allows creating Database connectors based on a JDBC driver (not included)

This extension leverages the Thingworx FileRepository template to upload a third party JDBC driver file and create an “importable” extension using the uploaded file.

To use the builder (after importing the JDBCCreator Extension):

    1. Open the JdbcCreator mashup, click the “Choose File” button and select the JDBC driver file you want to use from your local file system
    2. Click the “Upload” button and a link will be displayed below the buttons, “Download Extension File”
    3. Click this link and save the zip file. This is your extension. You can now import this into the Thingworx platform
    The imported extension will create a Thing Template with the name of the file plus “JDBCTemplate”. For example a file named “myDbFile.jar” would create a Template named “myDbFileJDBCTemplate”
    4. Create a new Thing based on this template and connect to your data source using JDBC
    5. Update the JDBC configuration fields: JDBC Driver Class Name, JDBC Connection String (available in your JDBC driver documentation) and ConnectionValidationString (A simple query that will work regardless of table names to be executed to verify return values from the database)

