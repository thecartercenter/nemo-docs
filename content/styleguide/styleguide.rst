*************************
Documentation Style Guide
*************************

.. _spelling-and-grammar:

Spelling and grammar
=======================

.. _american-spelling:

American spelling and grammar
-----------------------------

Whenever U.S. English and British (or other) English spelling or usage disagree, standard U.S. spelling and usage is preferred.

.. rubric:: Wrong

.. code-block:: rst

  The colour of the button is grey.

.. rubric:: Right

.. code-block:: rst

  The color of the button is gray.
  
.. _quote-marks:
    
Quote marks
--------------

 - Quote marks should generally be avoided if possible.
 - *Smart* quotes (also known as *curly quotes* or *directional quotes*) are not permitted in source files.
 
.. _avoid-quotes:
 
Avoid quote marks
~~~~~~~~~~~~~~~~~~~~~

Quote marks are used in prose writing to indicate verbatim text. This is rarely useful in technical writing, as verbatim text usually requires a more specific semantic markup.

.. rubric:: Wrong

.. code-block:: rst

  Click the button that says, "Save."
  
.. rubric:: Right

.. code-block:: rst

  Click :guilabel:`Save`.
  
.. rubric:: Wrong

.. code-block:: rst

  You may see an error message that says, "Something went wrong."
  
.. rubric:: Right

.. code-block:: rst

  You may get an error: ``Something went wrong.``

  
.. _straight-quote:
  
Straight quotes
~~~~~~~~~~~~~~~~~~

Any time that you *do* need to use quotation marks, use straight (or *plain*) quotes. Sphinx and Docutils will output the typographically correct quote style.

.. _click:

Click instructions
------------------

When giving user interface click instructions always use **Click** rather than **Click on**.

.. rubric:: Wrong

.. code-block:: rst

  Click on :guilabel:`Create user`.
  
.. rubric:: Right

.. code-block:: rst

  Click :guilabel:`Create user`.


.. _serial-comma:

Serial comma
-----------------

In a comma-delineated list of items, the penultimate item should be followed by a comma.

.. rubric:: Wrong

.. code-block:: rst

  Apples, oranges and pears.
  
.. rubric:: Right

.. code-block:: rst

  Apples, oranges, and pears.
  
A bulleted list is often more clear than an inline list.

.. rubric:: Correct

.. code-block:: rst

  You will need to be familiar with git, GitHub, and Python.
  
.. rubric:: Possibly Better

.. code-block:: rst

  You will need to be familiar with:
  
  - git
  - GitHub
  - Python
  
There's no hard rule about which to use in any situation. Use your judgement: try it both ways and see which is more clear.


.. _ordered-vs-unordered:

Ordered and unordered lists
-----------------------------

An order list is numbered. It should be used when the order of the list is essential. For example, when enumerating a series of steps in a procedure.

.. rubric:: Wrong

.. code-block:: rst

  - First we do this.
  - And then we do this.
  - And the we do this.
  
.. rubric:: Right

.. code-block:: rst

  1. Do this.
  2. Do this.
  3. Do this.
  
An unordered list is bulleted. It should be used for a collection of items in which order is not essential.

.. rubric:: Wrong

.. code-block:: rst

  1. apples
  2. oranges
  3. bananas
  
.. rubric:: Right

.. code-block:: rst

  - apples
  - oranges
  - bananas

.. _avoid-latin:

Avoid Latin
-------------

Several Latin abbreviations are common in written English:

.. startignore

 - etc.
 - i.e.
 - e.g.
 - viz.
 - c.f.
 - n.b.

.. endignore
 
At best, these present a minor barrier to understanding. This is often made worse by unintentional misuse.

Avoid Latin abbreviations.

.. rubric:: Wrong

.. code-block:: rst

  If you are writing about a specific process (e.g., installing an application)...
  
.. rubric:: Right

.. code-block:: rst

  If you are writing about a specific process (for example, installing an application)...

.. startignore

.. _etc:
  
Etc.
~~~~~~~~

*Et cetera* (or *etc.*) deserves a special mention.

*Et cetera* means "and all the rest," and is often used to indicate that there is more that could or should be said, but which is being omitted.

Writers often use *etc.* to gloss over details of the subject which they are not fully aware of. If you find yourself tempted use *etc.*, ask yourself if you really understand the thing you are writing about.


.. _avoid-unneeded-words:

Avoid unneeded words
-----------------------

.. _adverbs:

Adverbs
~~~~~~~~~~~

Adverbs often contribute nothing. Common offenders include:

 - simply
 - easily
 - just
 - very
 - really
 - basically

.. rubric:: Wrong

.. code-block:: rst

  To open the file, simply click the button.
  
.. rubric:: Right

.. code-block:: rst

  To open the file, click the button.
  
.. rubric:: Wrong

.. code-block:: rst

  You can easily edit the form by...
  
.. rubric:: Right

.. code-block:: rst

  To edit the form...
  
.. _filler-phrases:  
  
Filler words and phrases
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Many words and phrases provide no direct meaning. They are often inserted to make a sentence seem more formal, or to simulate a perceived style of business communication. These should be removed.

Common filler phrases and words include:

- to the extent that
- for all intents and purposes
- when all is said and done
- from the perspective of
- point in time

This list is not exhaustive. These "canned phrases" are pervasive in technical writing. Remove them whenever they occur.

.. endignore

.. _semicolons:

Semicolons
-------------

Semicolons are used to separate two independent clauses which could stand as individual sentences but which the writer feels would benefit by close proximity.

Semicolons can almost always be replaced with periods (full stops). This rarely diminishes correctness and often improves readability.

.. rubric:: Correct

.. code-block:: rst

  These "canned phrases" are pervasive in technical writing; remove them whenever they occur.
  
.. rubric:: Better

.. code-block:: rst

  These "canned phrases" are pervasive in technical writing. Remove them whenever they occur.

.. _pronouns:
    
Pronouns
----------

.. _third-person-pronouns:

Third-person personal pronouns
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. startignore

Third-person personal pronouns are:

- he/him/his
- she/her/her(s)
- they/them/their(s) 

.. note:: 

  While some people consider *they/them/their* to be non-standard (or "incorrect") as third-person singular, it has gained wide use as a gender-neutral or gender-ambiguous alternative to *he* or *she*.

There are two issues with personal pronouns:

- gender bias
- clarity

To avoid gender bias, the third person gender-neutral *they/then/their(s)* is preferred over *he* or *she* pronouns when writing about abstract individuals.

.. endignore

.. rubric:: Wrong

.. code-block:: rst

  The enumerator uses his device.
  
.. rubric:: Right

.. code-block:: rst

  The enumerator uses their device.


Unfortunately, *they/them/their* is not a perfect solution. Since it is conventionally used as a plural pronoun, it can cause confusion.

Therefore, avoid the use of personal pronouns whenever possible. They are often out of place in technical writing anyway. Rewriting passages to avoid personal pronouns often makes the writing more clear.

.. rubric:: Correct

.. code-block:: rst

  When using Collect, first the enumerator opens the app on their device. Then they complete the survey.
  
.. rubric:: Better

.. code-block:: rst

  To use Collect:
  
  - open the app
  - complete the survey

.. _same:  
  
"Same"
~~~~~~~~~

*Same*, when used as an impersonal pronoun, is non-standard in Modern American English. It should be avoided.

.. rubric:: Wrong

.. code-block:: rst

  NEMO is a data collection tool. The same can be used for...
  
.. rubric:: Right

.. code-block:: rst

  NEMO is a data collection tool. It can be used for...

.. rubric:: Right

.. code-block:: rst
  
  NEMO is a data collection tool that is used to...
  

.. _titles-style-guide:  
  
Titles 
------------

.. _title-casing:

Title case and sentence case
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Document titles should be in ``Title Case`` -- that is, all meaningful words are to be capitalized.

Section titles should use ``Sentence case`` -- that is, only the first word should be capitalized, along with any proper nouns or other words usually capitalized in a sentence.

.. _title-verb-forms:

Verb forms
-----------

If a document or section describes a procedure that someone might do, use a verb ending in *-ing*. (That is, a `gerund <https://en.wikipedia.org/wiki/Gerund>`_.) Do not use the "How to..." construction.

.. rubric:: Wrong

.. code-block:: rst

  How to install NEMO
  --------------------------
    
.. rubric:: Right

.. code-block:: rst

  Installing NEMO
  ----------------------
    
If section title is a directive to do something (for example, as a step in a procedure), use an imperative. 

.. code-block:: rst

  Installing NEMO
  ------------------------
  
  Download NEMO
  ~~~~~~~~~~~~~~~~~~~~~~

  Section content here.

  
.. _section-label-style-guide:  
  
Section labels
~~~~~~~~~~~~~~~~

Section titles should almost always be preceded by labels.

The only exception is very short subsections that repeat --- like the **Right** and **Wrong** titles in this document.

In these cases, you may want to use the :rst:dir:`rubric` directive.
    
.. _other-title-considerations:
      
Other titling considerations
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

- Do not put step numbers in section titles.
- Readers skim. Section titles should be clear and provide information.



.. note:: 

  This document is a derivative of the original `ODK style guide <https://docs.opendatakit.org/docs-style-guide/>`_ licensed under a Creative Commons Attribution 4.0 International License.

.. endignore