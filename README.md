# pwgen-docker #
docker container with pwgen tool used for secure password generation
***
pwgen source:
https://sourceforge.net/projects/pwgen/

Container is build with option -s always used (Generate completely random passwords). 
By default running container generates ten (10) random secure password, each 16-characters long, but you can pass any supported parameter instead.
***
## Usage: ##
  
generate ten (10) random secure passwords 16-chars long:

    docker run --rm kciepluc/pwgen-docker
  
generate five (5) secure passwords 24-chars long:

    docker run --rm kciepluc/pwgen-docker 24 5
  
generate single secure password 8-chars long:

    docker run --rm kciepluc/pwgen-docker 8
  
display program options:

    docker run --rm kciepluc/pwgen-docker --help

