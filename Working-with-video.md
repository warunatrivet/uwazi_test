Uwazi supports Vimeo and Youtube video embeddings via custom syntax in rich text fields.

In order to embed a video, add a rich text field to a document or entity and use the following syntax:

* For Vimeo: {vimeo}(https://player.vimeo.com/video/67430069)
* For Youtube: {youtube}(https://www.youtube.com/watch?v=VKtAhJPZS6o)

Video embeddings are displayable and fully functional in library cards, side panel and full width view:

![](https://github.com/huridocs/uwazi-assets/raw/master/wiki/screenshots/video-embedding.png)

For Vimeo embeddings, you can also create a time links to particular parts of the video following this syntax:

{vimeo}(https://player.vimeo.com/video/67430068, {"timelinks": {"51:30": "presentación y declaración inicial de Jorge Contesse", "01:03:03":"preguntas de la representación de la víctima", "01:19:30":"preguntas de la representación del Estado", "01:21:25":"preguntas de la representación de la CIDH", "01:27:49":"preguntas del Juez Pérez Pérez"}})

Which will be rendered as:

![](https://github.com/huridocs/uwazi-assets/blob/master/wiki/screenshots/Video-timelinks.png)

