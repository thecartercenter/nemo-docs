Questions
=========

Create a question
-----------------

To create a question:

1. Click :guilabel:`Questions` in the menu bar.
2. Click :guilabel:`Create New Question`.

.. image:: create-question.png
  :alt: create question

:guilabel:`Code`
   A unique name for the question.

:guilabel:`Type`
  Type of the question. More details can be found in :ref:`question-types` section.

:guilabel:`Title`
  Title of the question.

:guilabel:`Hint`
  Further instructions for the question. More details can be found in :ref:`hints` section.

:guilabel:`Is Key Question`
  Answers to key questions help summarize responses and appear in the response listing. If this box is marked, a column showing these answers will be added in the Responses tab.

:guilabel:`Tags`
  Add :ref:`tags` to this question.

.. _question-types:

Types of questions
------------------

.. list-table::
   :widths: auto
   :header-rows: 1

   * - Type
     - Description
   * - Text
     - Short text that shows in a single line of input.
   * - Long Text
     - Long text that shows in multiple lines of input.
   * - Integer
     - Numeric answer that must be a whole number without decimals.
   * - Decimal
     - Numeric answer that allows for decimals.
   * - Location
     - GPS location of the user.
   * - Select One
     - Only one answer can be selected from a multiple choice option set.
   * - Select Multiple
     - Multiple answers can be selected from a multiple choice option set.
   * - Date/Time
     - Enter both date and time.
   * - Date
     - Date only field.
   * - Time
     - Time only field.
   * - Image
     - The image should be at most 5MB. Accepted formats are: jpg, png.
   * - Annotated Image
     - The image should be at most 5MB. Accepted formats are: jpg, png. You can add markup to the image.
   * - Signature
     - Sign with a finger in ODK Collect or upload a signature image in NEMO/ELMO.
   * - Sketch
     - Sketch an image with a finger.
   * - Barcode
     - Scan a barcode with ODK Collect.
   * - Audio
     - Record or select a sound from your device. File size should be at most 10MB. Accepted formats are: mp3, ogg, webm, wav.
   * - Video
     - Record or select a video from your device. File size should be at most 10MB. Accepted formats are: 3gp, mp4, webm, mpg, wmv, avi.


.. _hints:

Hints
-----

Hints are optional help texts used to provide additional instructions on the question.

- On NEMO/ELMO desktop, click :fa:`info-circle` on the right of the question to see the hint.
- On ODK Collect (NEMO/ELMO Android app), the hint will be shown below the question as follows:

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
theme. In NEMO/ELMO, questions may be tagged with keywords or descriptors,
which may be used to find all of the questions with the same tag. Tags
are also used in Reports to help sort information assigned to questions.

To tag questions:

1. Open or create the question you wish to tag.
2. Type in the :guilabel:`Tags` box and click :guilabel:`Enter` to add a tag.

.. note::

  - You can add multiple tags.
  - To delete a tag, click :fa:`times` next to the tag.

3. Click :guilabel:`Save` after adding tags to save your changes.


Metadata type
-------------

Metadata type is a special value that can be pre-filled into a question. If chosen the question will be automatically hidden and not required, and any conditions will be removed.
For now the Metadata is only available for Date/Time question type.

1. Create a new Date/Time question.
2. Click the :guilabel:`Metadata Type` dropdown.
3. Select the Metadata you want to record.

.. note::

  - Form Start Time: will record the time Enumerator started the form.
  - From End Time: will record the time Enumerator ended the form.


Advanced options
----------------
The following features are only available for questions that are added to form.

Display logic
^^^^^^^^^^^^^
By default all questions are shown in the form. Display logic controls which question to show depending on conditions.

.. image :: display-logic.png
  :alt: Display logic


To edit display logic:

1. Click :guilabel:`Forms` menu.
2. Click :fa:`pencil` next to the form you want to edit.
3. Click on the :guilabel:`Question` you want to edit.
4. Click on the display logic dropdown :fa:`caret-down` and choose between three options:

  - Always display this question.
  - Display this question if all of these conditions are met.
  - Display this question if any of these conditions are met.




.. note::

  - Click :guilabel:`+ Add Condition` if you want to add another condition for the same question.


Skip logic
^^^^^^^^^^

On ODK Collect (NEMO/ELMO Android app), by default when you swipe left or click :fa:`arrow-right` you will be redirected to the following question in the form. With the skip logic you can go to any question on the form if conditions are met.

To edit skip logic:

1. Click :guilabel:`Forms` menu.
2. Select a form from the list and click :fa:`pencil`.
3. Click on the :guilabel:`Question` you want to edit.
4. Click on skip logic dropdown :fa:`caret-down` and select :guilabel:`After this question, skip ...`.
5. Choose the destination and conditions to be met.

.. image :: skip-logic.png
  :alt: Skip logic


Constraints
^^^^^^^^^^^

Constraints are conditions that must be met in order for an answer to be accepted. This feature is only available on the mobile app **ODK Collect**.

To edit constraints:

1. Click :guilabel:`Forms` menu.
2. Select a form from the list and click :fa:`pencil`.
3. Click on the :guilabel:`Question` you want to edit.
4. Click on constraints dropdown :fa:`caret-down` and select :guilabel:`Only accept an answer if ...`.
5. Select the conditions and rules to be met.

.. image :: constraints.png
  :alt: Constraints

.. note::
  - Constraints can only be added on previous questions.
  - When editing an Integer question type you can also add a constraint about the :guilabel:`Minimum` and :guilabel:`Maximum` value.


Default answer
^^^^^^^^^^^^^^

Text entered here will be pre-filled in the answer space (for ODK Collect only). You can enter a ``$QuestionCode`` to include the value of a previous question, and ``$!RepeatNum``
to include the number of the current item in a repeat group.

For example, entering ID: ``$Household-$!RepeatNum`` would pre-fill the answer with ID: 176-2 for the second person in household 176,
assuming you have a question with code 'Household'. You can also enter an XPath expression by wrapping it with calc():
``calc($VillageNum + 100 / 2)``

Required, hidden, and disabled options
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: required-hidden-disabled.png
   :alt: Required

- *Required*: Check :guilabel:`Required?` box to make this question required. Form cannot be submitted if not answered, unless an override code is provided.
- *Hidden*: (ODK Collect Only) Check :guilabel:`Hidden?` to hide question on the form but still collect default answer.
- *Disabled*: Check :guilabel:`Disabled?` to hide the question and not collect anything.
