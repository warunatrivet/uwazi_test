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