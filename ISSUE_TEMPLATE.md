
# Please add <library name>.

<Put a description of the library here.>

Checklists:

+ [ ] The license of the code is clear and allows for its redistribution.
+ [ ] My library works on more than just one implementation of Common Lisp. CCL and SBCL in x86-64, at least.
  + [ ] My library builds without warnings.
+ [ ] My library does not conflict with existing system.
  + [ ] System name.
  + [ ] Package name / nickname.
  + [ ] Does not modify the global readtable destructively.
  + [ ] Does not alter macroexpand-hook destructively.
+ [ ] My ASDF system has sufficient system definition metadata.
    + [ ] :license
    + [ ] :author
    + [ ] :description
+ [ ] My library has a sufficient README describing its purpose.
+ [ ] My library does not depend on Common Lisp libraries outside Quicklisp.
+ [ ] My library does not depend on quicklisp itself.
+ [ ] My library does not depend on non-lisp libraries outside Quicklisp,
      or they are easily installable by standard package managers (such as
      apt-get, yum). In particular, it is available on Debian8. (not a requirement)
    + [ ] The installation command below is comprehensive. (optional)
+ [ ] There is no library with the similar feature. Or, although there is a
      similar library, I have a clear motivation to make it a standalone
      library, and it is described in README (see below, not a requirement)
+ [ ] My library has an usage instruction. (not a requirement)
+ [ ] I am an author of the library. (not a requirement)

<Add a link to your repository.>

Commands for installing Non-lisp dependencies:

```sh
apt-get install <dependencies>
```

## Author guideline (remove when you create an issue)

+ Please don't describe your project simply by saying it's an interface to
  some C library. Explain what the C library is for and why someone might
  want to use it from Common Lisp, and link to any useful information about
  the C library.
+ If there is a library with the similar feature, please consider
  collaboration/coordination, rather than writing an individual library.
  If this is unachievable, please describe what is different from/superior
  to those libraries. It could be speed, simpler implementation,
  compatibility to other libraries, extensibility, and not necessarily a
  new feature. See
  [Dealing with "redundant" libraries](http://blog.quicklisp.org/2015/04/dealing-with-redundant-libraries.html)

See also:

+ [Getting a library into Quicklisp](http://blog.quicklisp.org/2015/01/getting-library-into-quicklisp.html)
+ [Some problems when adding libraries to Quicklisp](http://blog.quicklisp.org/2015/01/some-problems-when-adding-libraries-to.html).

