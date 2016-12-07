# docker-mytop

MySQL *mytop* based on Alpine.
Removed all unneeded content to keep it lightweight.

## Usage

Pull the image and connect to a host running a database!

Just run mytop:

    docker run --rm -it srcoder/mytop

Link a .mytop file:

    docker run --rm -itv /path/to/.mytop:/root/.mytop srcoder/mytop

Link another container:

    docker run --rm -it --link databasecontainer:db srcoder/mytop -h db

## Common options

- `-h` host[:port]
- `-P` port
- `-S` socket
- `-u` user
- `-p` password
- `-d` database
- `-s` delay

Find the other options: http://jeremy.zawodny.com/mysql/mytop/mytop.html

## Authors

- [Jeroen Boersma](https://github.com/JeroenBoersma)

## License

MIT

