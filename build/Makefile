all: build


GITVERSION= "no-version"

CXXFLAGS+= -std=gnu++0x -DGITVERSION=\"$(GITVERSION)\"
CXXFLAGS+= -Wno-format -Wno-pointer-arith -I ../

CXXFLAGS+=   -march=native -DHASHSEED1=0x74b0dc51 -DHASHSEED2=0x19495cff -O3 -D VALUELENGTH=12


HEADERS= ./lib/*.h

build: *.cc

run: build
	./build overall.txt /home/yy/gitothello/Othello/src/shortbin/ .Kmer.bin.short
