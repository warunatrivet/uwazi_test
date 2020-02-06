## Image and Media fields

Uwazi supports several embedded and native media types including:
*  YouTube, 
* FaceBook, 
* SoundCloud, 
* Streamable, 
* Vidme, 
* Vimeo, 
* Wistia, 
* Twitch, 
* DailyMotion, 
* mp3, 
* mp4, 
* wave, and others. 

To use this feature, add an image or media file to your documents and entities.

![Image and media fields](https://github.com/huridocs/uwazi-assets/blob/master/wiki/screenshots/image-and-video-fields.png)

You will notice several visualizations options are supported by Uwazi. They are:

- Hide label: if checked, it won't display this field's label in library cards.
- Full width: will remove the margins to the card border, allowing for richer visuals.
- Show in cards: media will be displayed in cards.
- Style, being either "Fit" will show the entire media inside the container or "Fill" will attempt to fill the container, using it's entire width. In cards, cropping is likely to occur.

### Uploading you own media files

If you don't want to use an external service (ie. YouTube), you can upload and display the files in Uwazi directly. To do so, add your file as an attachment to an entity, copy the URL provided by Uwazi after the upload its completed and use it in a media or markdown field.

## Embedding media into rich text fields

In order to embed a media file, add a rich text field to a document or entity and use the following syntax:
```
{media}(https://player.vimeo.com/video/67430069)
```

Video embeddings are displayable and fully functional in library cards, side panel and full width view:

![](https://github.com/huridocs/uwazi-assets/raw/master/wiki/screenshots/video-embedding.png)

You can also create a time links to particular parts of the video following this syntax:
```
{media}(https://player.vimeo.com/video/67430068, {"timelinks": {
"51:30": "presentación y declaración inicial de Jorge Contesse", 
"01:03:03":"preguntas de la representación de la víctima", 
"01:19:30":"preguntas de la representación del Estado", 
"01:21:25":"preguntas de la representación de la CIDH", 
"01:27:49":"preguntas del Juez Pérez Pérez"}})
```

Which will be rendered as:

![](https://github.com/huridocs/uwazi-assets/blob/master/wiki/screenshots/Video-timelinks.png)

