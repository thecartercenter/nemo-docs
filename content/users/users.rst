User Management
===============

User permission levels
----------------------

ELMO has four user levels – Enumerator, Staffer, Coordinator, and
Admin. Each user level has a different set of permissions based
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
         * Fill form responses via android devices, via SMS, or ELMO online platform.
         * Edit own user information.
         * Generate reports (only from user's own submitted data).
   * - Staffer
     - Performs real-time analysis and communicates with staff deployed to the field.
     -
         * All Enumerator privileges.
         * Generate reports from data submitted by users.
         * Broadcast SMS messages to users.
   * - Coordinator
     - Designs forms/checklists, reporting structures, and manages users for a specific mission.
     -
         * All Staffer privileges.
         * Create option sets, questions, and forms for the mission.
         * Create, edit and delete users within a mission.
   * - Administrator
     - Designs standardized forms/checklists and manages processes accross several missions.
     -
         * All Coordinator privileges.
         * Create new missions.
         * Create standard option sets, standard questions, and standard forms to be shared/imported across all missions.


Create users
------------

Create, delete, edit, and manage users on the users page. Administrators
can create general users in Admin Mode and assign them to specific
missions, or they can create users for specific missions in Mission
Mode. Coordinators can only create new users in Mission Mode.

To create new users:

1. Determine whether to work in Admin Mode or Mission Mode.
2. Navigate to the users page by clicking :guilabel:`Users` on the
   main menu.
3. Click :guilabel:`Create User`.
4. Enter the new user's information.
5. Click :guilabel:`Save`.

Import users
---------------------

You can import multiple users from an XLSX spreadsheet or CSV file.

1. From the Users page, click :guilabel:`Import Users`.
2. Click one of the links to download a template CSV or XLSX spreadsheet.
3. Assemble your user data in the template.
4. Upload the spreadsheet file.
5. Click :guilabel:`Import`.

.. note::
   You can download a template spreadsheet with the correct formatting for importing users.
   |Import Users|

Manage existing users
---------------------

To edit existing user information:

1. Find the user in the list of users.
2. Click on :fa:`pencil` located on the same line.

To delete existing users:

1. To delete a single user, click :fa:`trash`.
2. To delete multiple users, check the boxes to the left of their names and click :guilabel:`Delete Multiple Users`.

Export in vCard format
----------------------

To export users information to a vCard, which is readable by most contact list applications:

1. Check the box next to the name of each user to be exported
2. Check the box to the left of their names.
3. Click on :guilabel:`Export as vCard`.

User groups
-----------

Placing users into groups makes it easier to search for users and send
broadcasts to them. To create a group of users:

1. Check the box next to each user to be placed into the group.
2. Click :guilabel:`Add Users to Group`.
3. Click :guilabel:`Create New User Group`.
4. Type the name of the group and click :guilabel:`OK`.
5. Click the name of the group.

To add users to a preexisting group, follow the same steps as above, but
skip numbers 3 and 4.

To view user groups, go to the :guilabel:`Users` page and click :guilabel:`List
User Groups`. In the list, you can click:

- :guilabel:`List Members` to view a list of all users in the group.
- :fa:`pencil` to change the name of the user group.
- :fa:`trash` to delete the user group.

.. |Import Users| image:: Import-Users.png
