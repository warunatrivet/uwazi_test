With Uwazi, you can share data between two or more instances. This feature is experimental and has no UI access to it yet, so you need some technical skills to activate data-sync.

It is meant to solve the following scenarios:
- You have a private collection with sensitive data, but you want to make part of the data public. In this case, you need two Uwazis and configure the data sync to push from the private instance to the public one.
- Several Uwazis want to share their data into a single one with access to all or part of the information from each other.
- You need to work off-line but send the data to an on-line server when you have connectivity for backup or publishing purposes.

It has some rules and limitations:
- The current model is based in whitelisting templates and properties. By default everything is blacklisted for security reasons and only synced if explicitly configured to do so.
- The information flows only in one direction for now. So its not a bidirectional data-sync, although we have plans for implementing this model as well.
- For security reasons, the instance sharing the data will push the data into the server receiving the data. This is a drawback when what we want its keeping a local backup of the online data for, ie, offline access to the database.
- You need a credentials with write privileges in the receiving Uwazi.
- There is no duplicate control.
- IDs of entities are overwritten, so if you happen to have duplicated IDs (very low probability), new data will erase older data.
- Not everything is synced, only entities, thesauri and relationships. Pages, menus and other configs are indepedent to each Uwazi.