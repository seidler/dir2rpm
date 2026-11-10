
Makes an RPM package from an installation folder.

Typical usage with config-make-make_install :
Configure, if wished with --prefix. Run 
make DESTDIR=/tmp/tempdir

Then run dir2rpm with the temporary directory
dir2rpm programm version /tmp/tempdir

rm -rf /tmp/tempdir

Some makefiles do not support the DESTDIR variable. 
(php e.g. uses INSTALL_ROOT )