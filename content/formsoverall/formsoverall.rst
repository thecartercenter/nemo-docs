.. HTML line break definition
.. |br| raw:: html

   <br />

Forms
=====

Forms menu
----------

The **Forms** menu lists all the available forms for a mission. These are the components:

.. image:: forms-tab.png
  :alt: Forms tab


:guilabel:`Create New Form` Click to :ref:`create-general-form`. |br|
:guilabel:`SMS Test Console` Click to test form submission via SMS. |br|
:guilabel:`Import Standard Forms` Click to :ref:`import-standard-forms` to the mission. These forms can be edited within the mission.

For every form in the list, action icons are in the right and works as follows:

.. image:: forms-tab-inset.png
   :alt: forms tab inset


:fa:`pencil` Click to edit the form. |br|
:fa:`trash` Click to delete the form. This can only be done for forms that are unpublished. |br|
:fa:`arrow-up` Click to publish the form. |br|
:fa:`arrow-down` Click to unpublish the form. |br|
:fa:`copy` Click to create an identical copy of the form. |br|
:fa:`print` Click to print the form. |br|
:fa:`comment` Click to see the SMS guide of the form. |br|

.. _create-general-form:

Create a general form
-----------------------

**To create a new Form**:

1. Click :guilabel:`Forms` menu.
2. Click :guilabel:`Create New Form`.
3. Type a name for the form in the text box.

.. note::

  By clicking on :guilabel:`More Settings` you can:

  - Set a **Default Response Name** for the form.
  - Check the :guilabel:`Allow Incomplete` box to allow forms to be submitted without required questions filled in.
  - Check the :guilabel:`SMSable` box if you want to be able to receive responses to the form via SMS. For more information check :ref:`smsable`.


**To add questions to the Form**:

1. Click :guilabel:`+ Add Questions`.

  - Select from existing questions in the question bank.
  - Or create a new question to add to the Form (see :doc:`../formsquestions/formsquestions` section below for detailed instructions).

2. Click :guilabel:`Save` when finished editing.


Create a standard form
------------------------

Forms, questions, and option sets created in **Admin Mode** can be reused in multiple missions. If the Admin Mode link does not appear on the screen, permission is not granted to create standard forms.

1. Click :guilabel:`Admin Mode`.
2. Click :guilabel:`Forms` menu.
3. Click :guilabel:`Create New Form`.
4. Type a name for the form in the text box.
5. Click :guilabel:`Save`.

    .. image:: create-standard-form.png
      :alt: Create standard form 

6. Click :guilabel:`+ Add Questions` to add questions to the form.
7. To create a group of questions, click :guilabel:`Add Group`.
8. Click :guilabel:`Save`.

.. image:: standard-form-add-questions.png
  :alt: Standard form add questions


.. _import-standard-forms:

Import standard forms
------------------------

To import a Standard Form:

1. Click :guilabel:`Forms` menu.
2. Click :guilabel:`Import Standard Forms`.
3. Check the boxes next to the forms you want to import.
4. Click :guilabel:`Import`.

.. image:: import-standard-forms.png
  :alt: Import standard forms


Create groups and grids
-------------------------

Groups
~~~~~~

Grouping questions by context makes it easier for users to fill forms. Groups cannot be placed within questions or other groups.

**To create a group**:

1. Create or edit an existing form.
2. Create or add questions to the form.
3. Create at least one group.

  a. Click :guilabel:`Add Group`.
  b. Give the group a unique name.
  c. If needed, check the box 'Repeatable?'.
  d. Choose the Display Logic.

    - Always display this group.
    - Display this group if all of these conditions are met.
    - Display this group if any of these conditions are met.
   
  f. Click :guilabel:`Save`.

4. Click and drag the questions in the desired order of appearance.
5. Click and drag groups in the desired order of appearance.
6. Drag questions intended for groups to the right so that they appear indented in relation to the group.
7. Click :guilabel:`Save` to save the form, or click :guilabel:`Save and Publish` if the form is ready to be used.

.. image:: drag-and-drop.gif
   :alt: Drag and drop

Grids
~~~~~

Groups can be used to create grids, an example of which is shown below.

.. figure:: Screenshot_2016-03-15-10-23-18.png
   :alt: Screenshot\_2016-03-15-10-23-18

.. note::

  Grids can only be created under certain conditions:

  - Questions must be in the same group.
  - Questions must be of **Select One** type.
  - Questions must have the same option set.

**To create a grid**:

1. Create or edit an existing form.
2. Create or edit an existing group.
3. Place **Select One** questions with the same option set in the group.
4. Click :guilabel:`Save` to save the form, or click :guilabel:`Save and Publish` if the form is ready to be used.


Publish a form
-----------------

Once a form has been created, it must be published before users can submit responses. To publish a form:

1. Click :guilabel:`Forms` menu.
2. On the right side of the page, click :fa:`arrow-up` located on the same line as the form to publish. If the arrow is down :fa:`arrow-down` the form is already published.

.. image:: publish-forms.png
   :alt: publish forms

Print form
--------------

To print a hardcopy of a form:

1. Click :guilabel:`Forms` menu.
2. Select a form from the list.
3. Click :guilabel:`Print Form`.
