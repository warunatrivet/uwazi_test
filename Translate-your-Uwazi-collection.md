This guide will help you understand how translations works on Uwazi. After this guide you will be able to translate your own content: from documents to templates, properties, thesaurus…

You can also translate the Uwazi interface with our translation system following similars steps, but we won’t tackle that in this guide. Feel free to [contact us](https://www.uwazi.io/contact-us/) if you want to translate your Uwazi interface!

![translate](http://huridocs.github.io/uwazi-assets/wiki/screenshots/translate-context.png)

## Translation methodology

Uwazi translations works with a methodology called **fallback**. A fallback refers to an alternative document if the main one is not available.

In the example below, we have an instance with three different languages: English, Spanish and French.

![translate](http://huridocs.github.io/uwazi-assets/wiki/screenshots/translate-selector.png)

If you upload a document into English, that document *fallbacks to the other languages*. That way the same document will be available in the collection regardless the language selected by the user.

![translate](http://huridocs.github.io/uwazi-assets/wiki/screenshots/translate-upload.png)

Once you have a document uploaded into the system and fallback is working properly, you are ready to upload translations to the system. If you have the document already translated in your computer, you just need to go to Uwazi, select the language you want to upload and replace the document with the new one.

![translate](http://huridocs.github.io/uwazi-assets/wiki/screenshots/translate-replace.png)

As you can imagine, this methodology has some pros and cons:
- Users will be able to interact with your collection in any language you want: the interface, templates, properties, thesaurus and filters can be translated even though your documents are just available in one language.
- Your data will be consistent between languages. All the languages will access to the same amount of documents. No more orphan languages with just a few PDFs.
- As fallback shares documents through different languages, sometimes you can find a document written in a language different from the interface you are navigating.

## Uploading translated documents

Once you have a translated document in your computer, is time to upload it to Uwazi. First thing you need to check is the fallback. Access to the document you want to translate and check both languages. If the document appears in both, the fallback is working properly. Notice that if you already translated the properties and thesaurus, they will appear translated in each document, regardless the language of the main document.

![translate](http://huridocs.github.io/uwazi-assets/wiki/screenshots/translate-fallback.png)

Now, from the language you want to upload, go to the Attachments tab. There are three buttons below the name of the document. You should click on the second one: *Reupload a document*. This will replace the current document with the translated one. The main document will remain in the original language, but both PDF will be connected. That way you can navigate between languages and see both documents.

![translate](http://huridocs.github.io/uwazi-assets/wiki/screenshots/translate-replace-button.png)

Notice than replace documents will reset the document's *Table of Contents* and *References* if exists. This is because the new document has a new content: maybe different paragraphs, different number of pages and of course a completely different  language. 

Once you confirm the upload, and after some seconds of waiting, your new document will be uploaded and ready on the new language. Remember that if you already translated the properties and thesaurus, these will be automatically translated too.

![translate](http://huridocs.github.io/uwazi-assets/wiki/screenshots/translate-translated.png)