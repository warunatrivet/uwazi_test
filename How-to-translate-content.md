## Which content can you translate?

All the content inside Uwazi can be translated to any language you want. There are different ways to translate content (depend on what you want to have translated) but basically they are divided in two main groups:

### Uwazi Interface

The Uwazi Interface (also called "System") contains all translations for every component you see in the application: buttons, alerts, messages... 

As an open source tool, we aim collaboration and personalization on those translations. Inside `Settings > Translation`, you will find all the languages available on your collection. If you want a language that is not already available, [ask our developers team](https://www.uwazi.io/contact/) to add it. Once all the languages are setup, you will be able to add your own translations or modify the default ones to fit your own criteria.

For more information you can review our [guide to translate the interface](https://github.com/huridocs/uwazi/wiki/Translate-the-interface).

### Your content

Every document you upload, entity you create, property or thesauri you add is also translatable.

Sometimes you will need to translate them from `Settings > Translation`, other times it will be as easy as changing the language and modify the content there.

Check our [guide to translate documents](https://github.com/huridocs/uwazi/wiki/Upload-translated-documents) and our [guide to translate metadata and filters](https://github.com/huridocs/uwazi/wiki/Translate-document-metadata-and-filters) for more information.

![translate](http://huridocs.github.io/uwazi-assets/wiki/screenshots/translate-context.png)

## Our translation methodology

The Uwazi translation system works with a methodology called **fallback**. A fallback refers to an alternative document if the main (or intended) one is not available.

In the example below, we have an instance with three different languages: English, Spanish and French.

![translate](http://huridocs.github.io/uwazi-assets/wiki/screenshots/translate-selector.png)

When you upload a document in English, that document serves as the *fallback for the other languages*. This is because a Spanish nor French translation of this document is available. In this way, the same document will be available in the collection regardless the language selected by the user.

![translate](http://huridocs.github.io/uwazi-assets/wiki/screenshots/translate-upload.png)

If a translation of a document is available, the administrator can add that translation on that same document under its corresponding language, and the two documents will be linked. 

![translate](http://huridocs.github.io/uwazi-assets/wiki/screenshots/translate-replace.png)

As you can imagine, this methodology has some pros and cons.
Pros:
- Users will be able to interact with your collection in any language you want: the interface, templates, properties, thesaurus and filters can be translated even though your documents are just available in one language.
- Your data will be consistent between languages. All the languages will points to the same documents. No more orphan languages with just a few PDFs.

Con:
- Because the fallback approach shares documents through different languages, users may find a document written in a language different from the interface you are navigating.

# Additional notes
* But we currently do not support right-to-left rendering for Arabic and other right-to-left languages. 
* As from version 1.4 (November 2018), you can add languages yourself - see https://github.com/huridocs/uwazi/wiki/Manage-languages
* When languages are enabled, you will see the language abbreviation in the top right corner of the site.