compiler the cpp program command
```
# cd cpp
# g++ -fpic -I/root/jdk1.8.0_131/include -I/root/jdk1.8.0_131/include/linux -c HelloJNI.cpp
# g++ -o libhello.so -shared HelloJNI.o
```

confirm the shared library command
```
# nm libhello.so
```

Set environment variable
```
# export LD_LIBRARY_PATH=/root/java-native-example/cpp
```

