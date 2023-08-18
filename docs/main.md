# FiveM Basic Manual

This Manual will be updated in the future and be mantained. 

## In Game
### Open Console
The default key-bind for the console is F8

### Manage resources
For non necessary resources you can stop, start or restart them without restarting the server. 
#### Start resource:
```start resource-name```
#### Stop resource:
``stop resource-name``
#### Restart resource:
``restart resource-name``

## Server
### Add resources
Before you carelessly add resources make shure to download them from a trusted provider and dont use pirated resources.
To add a resource you need to upload the resource folder with the ``fxmanifest.lua`` to some place in the ``../server-data/resources/`` folder.
Make shure to add the resource to the server.cfg or the cfg of your choice. If the resource is not started from one cfg it will not automaticly start.
To add a resouce to a cfg you can use start or ensure.

#### Methods:
##### Start
Just tries to start the resource and then goes to the next. If the resource can not start and crashes it will just ignore that and stop the resource.
##### Ensure
When using ensure the server will wait fort he resource to start and only then continue. This can cause problems for some resources. I reccomend only using ensure for framework dependencies and core resources.

#### Edit CFG
If you want to edit the CFG you can edit the server.cfg from TxAdmin or edit every cfg by opening them with a text editor on the server.

#### Edit Database
To edit the or work at the database some basic SQL knowlage is required. You can access is without knowlage but it can cause problems.
Open PhpMyAdmin, Heidi SQL or any SQL management software. 
Use the [SQL] login data from the password.txt file.
