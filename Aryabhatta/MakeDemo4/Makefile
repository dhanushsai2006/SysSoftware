all:
	gcc -c foo/src/foo.c -o foo/obj/foo.o -Ifoo/include
	ar rcs foo/lib/libfoo.a foo/obj/foo.o #it create libfoo.a
	gcc -c bar/src/bar.c -o bar/obj/bar.o -Ibar/include
	ar rcs bar/lib/libbar.a bar/obj/bar.o #it create libbar.a
	gcc driver.c -Ifoo/include -Ibar/include -L./foo/lib -L./bar/lib -lfoo -lbar
clean:
	rm -f a.out


