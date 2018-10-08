## Image and Media fields

Uwazi supports several embedded and native media types including: YouTube, FaceBook, SoundCloud, Streamable, Vidme, Vimeo, Wistia, Twitch, DailyMotion, mp3, mp4, wave, and others. This is achieved via integration with  [React-player](https://www.npmjs.com/package/react-player), supporting all features this component provides.

Add an image or media field to your documents and entities to use this feature:

![Image and media fields](https://github.com/huridocs/uwazi-assets/blob/master/wiki/screenshots/image-and-video-fields.png)

These fields support several visualization options:

- Hide label: if checked it won't display this field's label in library cards.
- Full width: will remove the margins to the card border, allowing for richer visuals.
- Show in cards: media will be displayed in cards.
- Style, being either "Fit" will show the entire media inside the container or "Fill" will attempt to fill the container, using it's entire width. In cards, cropping is likely to occur.

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

