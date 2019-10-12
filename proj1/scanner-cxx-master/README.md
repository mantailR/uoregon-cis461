# scanner-cxx
C++ (bison, re-flex) version of project 1, scanner (aka lexer)

Author: Tai Lin

# to build
make image (build docker image and product a lexer in bin folder)

docker run -it proj1

in docker: bin/lexer samples/filename.qk(you can test any sample in samples)

if you don't want to use docker:

instead of using make image, just type make in command line.

then test the scanner as in docker container.

# some points to improve
currently double quoted string is implemented by regular expressions, may change
to patterns and states later, which is more clear and easy to understand.

the error report doesn't show the location of the error, may use another error
function with location parameter after I understand how location works.

there was a externally visible file name fix, I didn't know how it works and be
producted, I will fix it after asking professor.
