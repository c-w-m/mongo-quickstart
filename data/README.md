# Directions to restore this data into MongoDB

To restore any of these databases to MongoDB, you'll need to uncompress them and then run this command:

```shell
$ source .tox/dev36/bin/activate
(dev36) $ cd data
(dev36) $ unzip pypi_db.unzip  # creates unzip directory (pypi)
(dev36) $ mongorestore --drop --db pypi ~/.../data/pypi  # use full path to unzip directory
```