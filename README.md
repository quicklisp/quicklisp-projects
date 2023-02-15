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
is for and where to fetch its sources in one of the [supported source formats](#supported-sources).

Your project should include some form of README describing the project
and its purpose.

The system definition(s) for the project should include :DESCRIPTION,
:AUTHOR, and :LICENSE options.


Personal pet peeve: Please don't describe your project simply by
saying it's an interface to some C library. Explain what the C library
is for and why someone might want to use it from Common Lisp, and link
to any useful information about the C library.

## Supported Sources

Quicklisp is able to pull code from several kinds of sources. Please see an examples of each provided below.

### branched-git

Points to a specific branch in a Git repo.

*Example:* `branched-git https://gitlab.common-lisp.net/antik/antik.git master`

### darcs

*Example:* `darcs http://dwim.hu/live/hu.dwim.perec/`

### ediware-http

Historical source pointing to software by prolific lisper Edi Weitz. Points to projects hosted in the GitHub profile <https://github.com/edicl/>.

*Example:* `ediware-http chunga`

### http/https/single-file

Points to a single file available at a URL.

This file is expected to be in one of the formats, with accompanying file extension:

* .lisp - Uncompressed single-file lisp source
* .lsp - Uncompressed single-file lisp source
* .tar - Uncompressed tarball
* .tar.gz - Compressed tarball
* .tgz - Compressed tarball
* .zip - ZIP archive

*Example:* `https https://common-lisp.net/project/adw-charting/adw-charting.tar.gz`
*Example:* `single-file http://www.tfeb.org/programs/lisp/memoize.lisp`

### kmr-git

Points to a git repo hosted on <http://git.kpe.io/>.

*Example:* `kmr-git cl-base64`

### latest-github-release

Points to the latest available release on a GitHub project.

*Example:* `latest-github-release https://github.com/Lisp-Stat/array-operations.git`

### latest-github-tag

Points to the latest available tag on a GitHub project.

*Example:* `latest-github-tag https://github.com/sheepduke/chameleon.git`

### latest-gitlab-release

Points to the latest available release in a GitLab repo.

*Example* `latest-gitlab-release https://gitlab.com/daewok/adopt-subcommands.git`

### mercurial 

*Example:* `mercurial https://hg.stevelosh.com/adopt`

### git

*Example:* `git https://gitlab.common-lisp.net/alexandria/alexandria.git`

### svn

*Example:* `svn https://svn.common-lisp.net/cl-monad-macros/trunk`

### tagged-git

*Example:* `tagged-git https://github.com/borodust/bodge-blobs-support.git stable`
