Administrator can configure the available languages in settings > languages:

![](https://github.com/huridocs/uwazi-assets/blob/master/wiki/screenshots/manage-languages.png)

## Some notes on the Uwazi language model

When a user uploads a document or creates an entity, a copy of this information will be added to the other available languages. In order to have that piece of information translated, users must switch languages and update the information in the other languages. If the translation is not provided, the information will be displayed in the language it was uploaded regardless of the language the user is working on.

Example. Imagine we have an Uwazi instance with two languages, Arabic and English. While working in Arabic, an administrator uploads a document written in Arabic. An exact copy of this document will appear when switching to English. Admins need to edit this information and provide the English version, if available. If not, this acts as a "fallback" so users navigating in English will see that document in Arabic. Now if the admin uploads a document in English while working in English, a copy of the document (in English) will appear in the Arabic version of the site.

Some metadata is automatically synced across languages: thesauri based properties (select and multi-select), relationships, date based properties, geolocation and numeric. These properties can be automatically translated, so they just get synced when edited.

Table of contents is also synced as long as we are using the same source document (since it depends on the contents of the documents). So if an admin uploaded a document in English and got copied to the Arabic version, and we never uploaded the Arabic document, creating table of contents entries will also create them in the Arabic version since its the same text (yes, in English). The moment we upload the Arabic document, the table of contents won't be synced anymore.

Text references, media and text fields (text and rich text), are not synced across languages on edition. But they are synced along with the rest of properties on creation: when initially uploading a document or creating an entity, all the metadata added before hitting save for the first time will be copied to the other languages. Further editions won't update the not synchronizable fields.