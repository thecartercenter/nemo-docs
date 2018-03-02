Questions
=========

Create a question
-----------------

To create a question:

1. Click on :guilabel:`Questions` in the menu bar.
2. Click on :guilabel:`Create New Question`.

.. image:: create-question.png
  :alt: create question

:guilabel:`Code`
   A unique name for the question. Observers will not see this box.

:guilabel:`Type`
  Type of the question, more details can be found in :ref:`question-types` section.

:guilabel:`Title`
  Title of the question.

:guilabel:`Hint`
  Further instructions for the question. more details can be found in :ref:`hints` section.

:guilabel:`Is Key Question`
  Answers to key questions help summarize responses and appear in the response listing. If this box is marked, a column showing these answers will be added in the Responses tab.

:guilabel:`Tags`
  Add :ref:`tags` to this question.

.. _question-types:

Types of questions
------------------

+------------+---------------------------------------------------------------+
| Text       | Text designed with a shorter character limit, specifically    |
|            | used for SMS                                                  |
+------------+---------------------------------------------------------------+
| Long Text  | Text designed for paragraphs rather than simple               |
|            | phrases/sentences                                             |
+------------+---------------------------------------------------------------+
| Integer    | This is a numeric answer that must be a whole number without  |
|            | decimals                                                      |
+------------+---------------------------------------------------------------+
| Decimal    | This is numeric answer that allows for decimals               |
+------------+---------------------------------------------------------------+
| Location   | This question may be answered with a GPS coordinate derived   |
|            | from the user’s device (e.g. tablet with GPS)                 |
+------------+---------------------------------------------------------------+
| Select One | Only one answer may be selected from a multiple choice Option |
|            | Set                                                           |
+------------+---------------------------------------------------------------+
| Select     | Multiple answers may be selected from a multiple choice       |
| Multiple   | Option Set                                                    |
+------------+---------------------------------------------------------------+
| Date/Time  | Enter both the date and the time                              |
+------------+---------------------------------------------------------------+
| Date       | Enter the date                                                |
+------------+---------------------------------------------------------------+
| Time       | Enter the time                                                |
+------------+---------------------------------------------------------------+
| Image      | Take a picture or choose a jpg orpngimage                     |
+------------+---------------------------------------------------------------+
| Annotated  | Take or choose a picture and annotate it                      |
| Image      |                                                               |
+------------+---------------------------------------------------------------+
| Signature  | Sign with a finger                                            |
+------------+---------------------------------------------------------------+
| Sketch     | Sketch an image with a finger                                 |
+------------+---------------------------------------------------------------+
| Audio      | Record or choose a sound                                      |
+------------+---------------------------------------------------------------+
| Video      | Record or choose a video                                      |
+------------+---------------------------------------------------------------+

.. _hints:

Hints
-----

Hints are optional help texts used to provide additional instructions on the question.

- On ELMO desktop, hint can be seen when clicking on :guilabel:`i` icon on the right of the question.
- On ODK Collect (ELMO Android app), the hint will be shown below the question as follows:

.. image:: hint-android.png
  :alt: hint Android 

Language translations
---------------------

Question titles and hints can be translated into any language that has
been set for the mission. To add a language to a mission, go to :guilabel:`Settings` menu and edit :guilabel:`Preferred Languages`.

.. image:: preferred-languages-enfr.png
   :alt: preferred languages


When editing a question. Title and Hint will show up for selected languages:

.. image:: title-hint-enfr.png
   :alt: title hint

.. note::

  To view the translation, change the language by clicking :guilabel:`Change Language` in the footer. For example, the French translation of an English question will appear once French is selected.

.. _tags:

Tags
----

Tags are an easy way to organize information around a common keyword or
theme. In ELMO, questions may be tagged with keywords or descriptors,
which may be used to find all of the questions with the same tag. Tags
are also used in Reports to help sort information assigned to questions.

.. figure:: tags.png
   :alt: tags


To tag questions:

1. Open or create the question you wish to tag.
2. Type in the :guilabel:`Tags` box and click :guilabel:`Enter` to add a tag.

.. note::

  - You can add multiple tags.
  - To delete a tag, click on the :guilabel:`X` next to the tag.

3. Click :guilabel:`Save` after adding tags to save your changes.


Display logic
-------------

By default all questions are shown in the form. Display logic controls which question to show depending on conditions.

To edit display logic:

1. Click :guilabel:`Forms` menu.
2. Select a form from the list and click :guilabel:`Edit` icon.
3. Click on the :guilabel:`Question` you want to edit.
4. Click on the display logic dropdown and choose between three options:

  - Always display this question.
  - Display this question if all of these conditions are met.
  - Display this question if any of these conditions are met.

.. image :: display-logic.png
  :alt: Display logic


.. note::

  - Click on :guilabel:`+ Add Condition` if you want to add another condition for the same question.
  - Check :guilabel:`hidden` box if you want to hide this question from the form.
  - Check :guilabel:`required` box to make this question required. Form cannot be submitted if not answered, unless an override code is provided.



Skip Logic
----------

On ODK Collect (ELMO Android app), by default when you swipe left or click on next button you will be redirected to the following question in the form. With the skip logic you can go to any question on the form if conditions are met.

To edit skip logic:

1. Click :guilabel:`Forms` menu.
2. Select a form from the list and click :guilabel:`Edit` icon.
3. Click on the :guilabel:`Question` you want to edit.
4. Click on skip logic dropdown and select :guilabel:`After this question, skip ...`.
5. Choose the destination and conditions to be met.

.. image :: skip-logic.png
  :alt: Skip logic
