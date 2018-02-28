.. HTML line break definition
.. |br| raw:: html

   <br />

User Management
===============

User permission levels
----------------------

ELMO has four kinds of user levels – observer, staffer, coordinator, and
administrator. Each user level has a different set of permissions based
on the functions they are expected to perform during ELMO missions.

.. list-table::
   :header-rows: 1
   :widths: auto
   :align: left

   * - Role
     - Responsibility
     - Privileges
   * - Enumerator
     - Collects and submits data from the field.
     - 
         * Fill form responses via android |br| devices, via SMS, or ELMO online |br| platform.
         * Edit own user information.
         * Generate reports (only from user's |br| own submitted data).
   * - Staffer
     - Performs real-time analysis and |br| communicates with staff deployed |br| to the field.
     - Observer privileges plus:
         * Generate reports from data |br| submitted by users.
         * Broadcast SMS messages to users.
   * - Coordinator
     - Designs forms/checklists, reporting |br| structures, and manages users for a |br| specific mission.
     - Staffer privileges plus:
         * Create option sets, questions, |br| and forms for the mission.
         * Create, edit and delete users |br| within a mission.
   * - Administrator
     - Designs standardized forms/checklists |br| and manages processes accross |br| several missions.
     - Coordinator privileges plus:
         * Create new missions.
         * Create standard option sets, |br| standard questions, and standard |br| forms to be shared/imported |br| across all missions.


Create users
------------

Create, delete, edit, and manage users on the users page. Administrators
can create general users in Admin Mode and assign them to specific
missions, or they can create users for specific missions in Mission
Mode. Coordinators can only create new users in Mission Mode.

To create new users:

1. Determine whether to work in Admin Mode or Mission Mode.
2. Navigate to the users page by clicking the :guilabel:`Users` menu on the
   main menu.
3. Click :guilabel:`Create User`.

   |New-user|

4. Enter the new user informations on the **Create User** page.

.. note::
  User’s phone number must include country code.

5. Click **Save.**

Create multiple users
---------------------

1. Click :guilabel:`Create Multiple Users`.
2. Upload a spreadsheet with information for the new users.
3. Click Import.

.. note::
   Click **Spreadsheet template** to download an example spreadsheet with the correct formatting for uploading multiple users.
   |Create Multiple Users|


Manage existing users
---------------------

To edit existing user information:

   1. Find the user in the list of users.
   2. Click on the :guilabel:`Pencil icon` located on the same line.
   3. Click :guilabel:`Save`.

To delete existing users:

   - To delete a single user, click the :guilabel:`Trashcan icon`.
   - To delete multiple users, check the box to the left of their names and click :guilabel:`Delete Multiple Users`.

To send an email or SMS broadcast to users:

   1. Check the boxes next to each user to contact.
   2. Click :guilabel:`Send Broadcast`. This redirects to a page where you can define the medium, subject, and content of the broadcast.

Export vCard
------------

To export users information to a vCard, which is readable in Microsoft Outlook:

1. Find each user whose vCard will be exported.
2. Check the box to the left of their names.
3. Click on :guilabel:`Export as vCard`.

User groups
-----------

Placing users into groups makes it easier to search for users and send
broadcasts to them. To create a group of users:

1. Add multiple users to a mission.
2. Click the :guilabel:`Users` tab.
3. Check the box next to each user to be placed into the group.
4. Click :guilabel:`Add Users to Group`.
5. Click :guilabel:`Create New User Group`.
6. Type the name of the group and click :guilabel:`OK`.
7. Click the name of the group.

To add users to a preexisting group, follow the same steps as above, but
skip numbers 5 and 6.

To view user groups, go to the :guilabel:`Users` tab and click :guilabel:`List
User Groups`. In the list, you can click:

- :guilabel:`List Members` to view a list of all users in the group.
- :guilabel:`Pencil icon` to change the name of the user group.
- :guilabel:`Trashcan icon` to delete the user group.

.. |New-user| image:: New-user.png
.. |Create Multiple Users| image:: Create-Multiple-Users.png
