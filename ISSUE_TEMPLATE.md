
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
+ [ ] My ASDF system has sufficient system definition metadata.
    + [ ] :license
    + [ ] :author
    + [ ] :description
+ [ ] My library has a sufficient README describing its purpose.
+ [ ] My library does not depend on libraries outside Quicklisp.
+ [ ] My library does not depend on quicklisp itself.
+ [ ] There is a library with the similar feature, but the motivation in
      this library is clear (see below, not a requirement)
+ [ ] My library has an usage instruction. (not a requirement)
+ [ ] I am an author of the library. (not a requirement)

<Add a link to your repository.>

## Author guideline (remove when you create an issue)

+ Please don't describe your project simply by saying it's an interface to
  some C library. Explain what the C library is for and why someone might
  want to use it from Common Lisp, and link to any useful information about
  the C library.
+ If there is a library with the similar feature, please consider
  collaboration/coordination, rather than making an individual library.
  If this is unachievable, please describe what is different from/superior
  to those libraries. It could be speed, simpler implementation,
  compatibility to other libraries, extensibility, and not necessarily a
  new feature. See
  [Dealing with "redundant" libraries](http://blog.quicklisp.org/2015/04/dealing-with-redundant-libraries.html)

See also:

+ [Getting a library into Quicklisp](http://blog.quicklisp.org/2015/01/getting-library-into-quicklisp.html)
+ [Some problems when adding libraries to Quicklisp](http://blog.quicklisp.org/2015/01/some-problems-when-adding-libraries-to.html).

