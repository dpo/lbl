===================================
LBL: C wrapper around MA27 and MA57
===================================

:Author: D. Orban <dominique.orban@gerad.ca>

Installing LBL
==============

1. Place the source files for MA27 and MA57 in some directory. You will need
   fd15d.f ma27ad.f mc21d.f mc34d.f mc47d.f mc59d.f mc64d.f mc71d.f ma57d.f.
   See http://www.hsl.rl.ac.uk/hsl2007

2. Edit and customize make.inc

3. Type ``make all``.

You can clean out temporary files with ``make clean`` and sanitize everything
with ``make purge``.


Testing LBL
===========

Type ``make example``. Change to the `example` directory and type
``./example``.

The expected output is::

   Input matrix:
   1  1  2.000000
   1  2  3.000000
   2  3  4.000000
   2  5  6.000000
   3  3  1.000000
   3  4  5.000000
   5  5  1.000000
   Input right-hand side:
   8.000000 45.000000 31.000000 15.000000 17.000000 
   Solution:
   1.000000 2.000000 3.000000 4.000000 5.000000

Enjoy!
