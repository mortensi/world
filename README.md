# Redis port of the world database

This is a port of the popular "world" database for Redis. I have converted the database available at the MySQL website ([Setting Up the world Database](https://dev.mysql.com/doc/world-setup/en/))

As reported in the source database, the world database is Copyright Statistics Finland, http://www.stat.fi/worldinfigures. 

## Usage

1. Download the `world.txt` file
2. Import into Redis with `cat world.txt | redis-cli`
