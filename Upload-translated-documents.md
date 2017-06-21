In Uwazi, _editors_ can add translated documents to existing documents in Uwazi. This page explains what needs to be in place in order to add translated documents to Uwazi, and a typical workflow for adding these documents. 

# Requirements
In order to add translated documents to an existing document, you need to have more than one language enabled on your Uwazi instance. To request languages, contact the Uwazi team.

# Uwazi's translation system
* You can translate Uwazi into any language (but we currently do not support right-to-left rendering). 
* When languages are enabled, you will see the language abbreviation in the top right corner of the site. 
* When the _admin_ or _editor_ uploads a document, that document will be attached to the language that is enabled during the upload process. For example, if a document is in English, the user must upload that document when the instance is set to _EN_. 
* When the user selects a language, they will continue to see all of the available information in Uwazi, but if any of that content is available in the selected language they will see that instead of the default language. This includes the user interface, document/entity properties, and the documents themselves. 

# Workflow: How to add translated documents
1. Switch the website's language to the language of the translated document you are adding. For example, if you are adding a French translation of a document in Uwazi, make sure you have selected _FR_ as the interface language in the top right corner. 
2. Open the document for which you want to add a translated document to. 
3. Go to the attachments tab. 
4. Replace the current document with the translated document.


***

## Uploading translated documents

Once you have a translated document in your computer, is time to upload it to Uwazi. First thing you need to check is the fallback. Access to the document you want to translate and check both languages. If the document appears in both, the fallback is working properly. Notice that if you already translated the properties and thesaurus, they will appear translated in each document, regardless the language of the main document.

![translate](http://huridocs.github.io/uwazi-assets/wiki/screenshots/translate-fallback.png)

Now, from the language you want to upload, go to the Attachments tab. There are three buttons below the name of the document. You should click on the second one: *Reupload a document*. This will replace the current document with the translated one. The main document will remain in the original language, but both PDF will be connected. That way you can navigate between languages and see both documents.

![translate](http://huridocs.github.io/uwazi-assets/wiki/screenshots/translate-replace-button.png)

Notice than replace documents will reset the document's *Table of Contents* and *References* if exists. This is because the new document has a new content: maybe different paragraphs, different number of pages and of course a completely different  language. 

Once you confirm the upload, and after some seconds of waiting, your new document will be uploaded and ready on the new language. Remember that if you already translated the properties and thesaurus, these will be automatically translated too.

![translate](http://huridocs.github.io/uwazi-assets/wiki/screenshots/translate-translated.png)
