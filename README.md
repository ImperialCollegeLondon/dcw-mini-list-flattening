This is a cut-down version of a single part of Duncan White's mailing list
flattener example project.  It depends on Duncan's c-tools directory,
which lives in ~/c-tools:

To build this list flattener:

1. download the c-tools to your home directory:

cd
wget http://www.doc.ic.ac.uk/~dcw/c-tools.tgz
tar xzf c-tools.tgz

2. set up this project to use the c-tools library:

bash users should do the following:

export TOOLDIR=$HOME/c-tools
export ARCH=x86_64

Whereas csh users should do:

setenv TOOLDIR $HOME/c-tools
setenv ARCH x86_64

3. build this project via:

make

4. run it's tests:

make test