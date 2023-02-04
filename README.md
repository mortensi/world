# Redis port of the world database

This is a port of the popular "world" database for Redis. I have converted the database available at the MySQL website ([Setting Up the world Database](https://dev.mysql.com/doc/world-setup/en/))

As reported in the source database, the world database is Copyright Statistics Finland, http://www.stat.fi/worldinfigures. 

## Usage

1. Download the [`world.txt`](https://raw.githubusercontent.com/mortensi/world/main/world.txt) file
2. Import into Redis with `cat world.txt | redis-cli`

## Notes

* All the entities are stored as Redis Hashes
* The database presents three entities: `city`, `country`, `countrylanguage`
* `city`'s unique key is an autoincrement integer, e.g. `city:653`
* `country`'s unique key is the country code, e.g. `country:esp`
* `countrylanguage`'s unique key is an autoincrement integer, e.g. `countrylanguage:6`
