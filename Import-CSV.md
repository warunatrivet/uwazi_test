## Migration of databases to Uwazi using CVS files

One should take account of the following:

    1. Use CSV (comma separated values) file rather than XLS or XLSX (Excel) files – CSV files are easier to parse
    2. Migration works with matching names – therefore, one should create a structure in Uwazi with the same field names as the column headers in the CSV file. For field names one can use either lower case or capitals. It is always possible to rename fields in Uwazi after import.
    3. It is useful (or even necessary) to create a list of templates/formats that are to be migrated, mentioning type of field and name of field in Uwazi
    4. The order of the columns is not important, data will be imported in the correct column in Uwazi
    5. The “title” is required and serves to identify a record. It does not have to be unique.
    6. The “date added” is filled automatically with information during the import into Uwazi.
    7. The names of columns should not contain empty spaces, one should use two underscore symbols __ as separator. For example first__name
    8. The pipe symbol | is to be used as separator in a field with multiple values.
    9. For links to external documents, use the convention [Name](link), for example [HURIDOCS Micro-thesauri](https://www.huridocs.org/resource/micro-thesauri/)
    10. It is possible to import different CVS files into the same template.
    11. If the various columns in the CVS file are to be migrated to different templates in Uwazi one should split the CVS file so that the data for each template are separate.
    12. After an import has been done, editing of records should take place within Uwazi. A feature to update a set of imported records is under development.
    13. If the source data is in different languages, these languages should be set up beforehand in Uwazi.
    14. Attachments can be imported as a ZIP file of PDFs. There should be a CSV file with the title of the record to which the attachment is to be linked and the name of the file.
    15. A feature that is not yet supported is multiple dates within one field.

Related issues:

    1. A feature under development is export of structure and export of all data.
    2. Another feature is under development for importing only thesauri. This will also allow to import terminology lists in different languages.
    3. HURIDOCS has developed 48 micro-thesauri for the documentation of human rights violations. They are available in several languages as CSV files, see https://www.huridocs.org/resource/micro-thesauri/
    4. Different fields in Uwazi can be linked to the same thesaurus.
    5. For exceptional situations occurring in particular instances we seek to make “work arounds” rather than new features which take more time.