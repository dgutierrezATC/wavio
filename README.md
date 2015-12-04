wavio
=====

`wavio` is a Python module that defines two functions:

* `wavio.read` reads a WAV file and returns an object that holds the sampling
  rate, sample width (in bytes), and a numpy array containing the data.
* `wavio.write` writes a numpy array to a WAV file, optionally using a
  specified sample width.

The module uses the `wave` module in Python's standard library, so it has the
same limitations as that module.  In particular, it does not support compressed
WAV files, and it does not handle floating point WAV files.  (When floating
point data is passed to `wavio.write` it it converted to integers before being
written to the WAV file.)  The functions can read and write 8-, 16-, 24- and
32-bit integer WAV files.

`wavio` has been tested with Python versions 2.7, 3.4 and 3.5.

`wavio` depends on numpy (http://www.numpy.org).  It has been tested with versions
1.8.1, 1.9.0 and 1.10.1, and will likely work with older versions.

-----

_Author_:     Warren Weckesser  <br />
_Repository_: https://github.com/WarrenWeckesser/wavio  <br />
_License_:    BSD 2-clause (http://opensource.org/licenses/BSD-2-Clause)  <br />
