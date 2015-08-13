# ABOUT QUICKLISP-PROJECTS

quicklisp-projects has metadata for Common Lisp projects tracked by
Quicklisp. Each subdirectory is named after a project, and a project's
subdirectory has a source.txt file describing how to get the project's
files. Other metadata files will be added in the future.

The qlc-meta directory is special, and has files related to creating
and updating Quicklisp data.



## TO ADD A PROJECT TO QUICKLISP

For background info, see [Getting a library into
Quicklisp](http://blog.quicklisp.org/2015/01/getting-library-into-quicklisp.html)
and [Some problems when adding libraries to
Quicklisp](http://blog.quicklisp.org/2015/01/some-problems-when-adding-libraries-to.html).

Please do *not* open a pull request.

Please open a github issue here:

  https://github.com/quicklisp/quicklisp-projects/issues

In the issue, please provide a brief description of what your project
is for and where to fetch its sources.

Your project should include some form of README describing the project
and its purpose.

The system definition(s) for the project should include :DESCRIPTION,
:AUTHOR, and :LICENSE options.


Personal pet peeve: Please don't describe your project simply by
saying it's an interface to some C library. Explain what the C library
is for and why someone might want to use it from Common Lisp, and link
to any useful information about the C library.
