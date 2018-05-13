If you work on a team or in collaboration with other people, Uwazi allows you to create users with specific permissions to help you update your collection of documents.

Roles
-----

Currently we support three different roles: **visitors, editors** and **admins**.

Any **visitor** to an Uwazi instance is able to:
- View all the documents, entities, properties, connections, etc in Uwazi (but cannot edit, create, or delete anything)
- User the search and filter functionalities

A user with the role of **editor** is able to:
- Do all the things that a _visitor_ can do
- Upload documents and create entities
- Delete documents and entities
- Organize the collection (as defined in the [user guide](https://github.com/huridocs/uwazi/wiki)), including: apply properties, create connections and references, create a table of contents
- Add/edit translations

A user with the role of **administrator** is able to:
- Do all the things that an _editor_ can do
- Manage settings (as defined in the [user guide](https://github.com/huridocs/uwazi/wiki))
- Configure the information architecture (as defined in the [user guide](https://github.com/huridocs/uwazi/wiki)), including: create document and entity types/templates, create dictionaries, name connections
- Configure filters
- Add and delete users

Creating users
-------------------

As you can notice, you don't need to create visitors. This is the basic role when anyone visits your collection!

But if you want to allow some people to perform specific actions into your collection, you can create Users that will allow them login the same way you login into your admin account.

To create a new user, you need to go to **Settings** and click on the **Users** section. It will appear a list with all current users inside your collection. You will be able to create new ones, edit or delete them if necessary.

![Users section](http://huridocs.github.io/uwazi-assets/wiki/screenshots/users-base.png)

A user has three fields to be completed:

- Username
- E-Mail
- Role (Editor or Admin).

We will send an email to that person with a link to set the user's password. 

Note that if you are hosting your own Uwazi, if you are accessing the instance as localhost, for instance: http://localhost:3000/settings to send the invitation, it will use that address as the instance URL.

So, if you have a proper domain, please, create the account from that url, for instance: http://yourdoumain.com/settings. This will send a 'yourdomain.com' URL.

If you are using a local IP, for an intranet installation, then use something like http://192.168.xx.yy/settings for it to send with that address.

![New user](http://huridocs.github.io/uwazi-assets/wiki/screenshots/users-new.png)