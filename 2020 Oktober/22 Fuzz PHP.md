https://github.com/php/php-src

Resource:

https://www.tripwire.com/state-of-security/vert/fuzzing-php-for-fun-and-profit/

https://sean.heelan.io/2017/08/12/fuzzing-phps-unserialize-function/

Compiling PHP with AFL

depedencies
```
sudo apt install libbison-dev re2c libxml2-dev libsqlite3-dev
```

```
./buildconf --force
CC=afl-clang-fast CXX=afl-clang-fast++ ./configure
AFL_USE_ASAN=1 make
```

next:

https://blog.jmpesp.org/2020/01/fuzzing-php-with-domato.html

