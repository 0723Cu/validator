
3 March 2016.
This release fixes the checker behavior such that no error is incorrectly
emitted any longer for `minlength` attributes on `input[type=text]` and
`input[type=password]`/, and no error is incorrectly emitted any longer for
`integrity` attributes containing multiple values. Also added in this
release is a new error for the case where a `<time>` element and children
but no `datetime` attribute. The CSP-checking behavior was also improved.

More: https://github.com/validator/validator/blob/master/CHANGELOG.md#1633

The files in this release provide a portable standalone version of the Nu Html
Checker in two different forms: as a Java jar file, and as a Java war file.

Use the jar file either for batch checking of HTML documents from the command
line and from other scripts/apps, as documented at http://validator.github.io,
or as a self-contained service for browser-based checking of HTML documents over
the Web—similar to http://html5.validator.nu/ and http://validator.w3.org/nu/.

Use the war file to deploy the Nu Html Checker through a servlet container such
as Tomcat, as documented at https://validator.github.io/validator/#servlet.
