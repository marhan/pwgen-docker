# pwgen-docker #
docker container with pwgen tool used for secure password generation
***
pwgen source:
https://sourceforge.net/projects/pwgen/

Container is build with option -s always used (Generate completely random passwords)
By default running container generates 10 random secure password, each 16-characters long, but you can pass any supported parameter instead.
***
## Usage: ##
1. generate ten (10) random secure passwords 16-chars long:
  docker run --rm kciepluc/pwgen

2. generate five (5) secure passwords 24-chars long:
  docker run --rm kciepluc/pwgen 24 5

3. generate single secure password 8-chars long:
  docker run --rm kciepluc/pwgen 8

4. display program options:
  docker run --rm kciepluc/pwgen --help

