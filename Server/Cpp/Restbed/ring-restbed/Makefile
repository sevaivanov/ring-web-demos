.PHONY: clean

UNAME := $(shell uname)

ifeq ($(UNAME), Darwin) 
    LIB_EXT := .dylib
else
    LIB_EXT := .so
endif

simple:
	g++ -o dring.out main.cpp ringrestbed.cpp -std=c++11 \
		-lrestbed -lcrypto -lpthread -lssl \
		-I/usr/include/dring #/usr/lib/libring.a

clean:
	rm -rf *$(LIB_EXT) *.out

