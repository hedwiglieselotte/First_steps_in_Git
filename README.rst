~~~~~~~~~~~~~~~~~~
First_steps_in_Git
~~~~~~~~~~~~~~~~~~

This is a repository for git beginners to practise the git workflow

.. contents::


Getting started
===============

To check if Git is already installed type the following in your terminal:

.. code:: bash

    git --version



Installation:
*************

* Linux/Unix: `<https://git-scm.com/download/linux>`_

* Windows: `<https://git-scm.com/download/win>`_

* Mac OS X: `<https://git-scm.com/download/mac>`_



Update your git configuration
******************************

Set global name and email:

.. code:: bash

    git config --global user.name "Your Name"

    git config --global user.email@example.com


See your configuration
**********************

.. code:: bash

    git config --list



Task
====


1. Write your name to the file "List_of_attendees.txt" on the existing branch "features/write_attendees“

**Solution:**

	* Checkout the features/write_attendees branch
		.. code:: bash
	
			git checkout features/write_attendees

	* Add "Your Name" to "List_of_attendees.txt"

	* Stage your changes
		.. code:: bash

			git add List_of_attendees.txt

	* Commit your changes
		.. code:: bash

			git commit -m "Add Your_Name to the list of attendees"

	* Push your changes
		.. code:: bash
			git push


2. Create a new branch from main and add a directory named like you. It should contain a text file with a brief introduction of your person

**Solution:**

	* Create the new branch features/Your_Name_attendees
		.. code:: bash

			git checkout -b features/Your_Name_attendees

	* Create a directory named like you and add "Introduction_Your_Name.txt" which contains a brief introduction of your person

	
	* Stage your changes
		.. code:: bash

			git add Introduction_Your_Name.txt

	* Commit your change 
		.. code:: bash

			git commit -m "Add short introduction of Your_Name to Attendees repository"

	* Push your changes 
		.. code:: bash

			git push --set-upstream origin features/Your_Name_attendees

	* Create a PR at github 



License
=======

MIT License

Copyright (c) 2020 oemof developing group

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.


.. |badge_coverage| image:: https://coveralls.io/repos/github/oemof-heat/DHNx/badge.svg?branch=dev&service=github
    :target: https://coveralls.io/github/oemof-heat/DHNx?branch=dev
    :alt: Test coverage

.. |badge_travis| image:: https://api.travis-ci.org/oemof/DHNx.svg?branch=dev
    :target: https://travis-ci.org/oemof/DHNx
    :alt: Build status

.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4147049.svg
   :target: https://doi.org/10.5281/zenodo.4147049

.. |readthedocs| image:: https://readthedocs.org/projects/dhnx/badge/?version=latest
    :target: https://dhnx.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
