This is a Drupal 7 module which creates an 'Issue links' text filter.

Please note, this code is a work in progress and not production ready.

The 'Issue links' text filter provides a modified version of the
functionality found on drupal.org project issues whereby users can
link from one project issue to another in a project issue's node or comment
body simply using the shorthand syntax [#1234] (or [#1234-2] for comments).

References to issues in the form of [#1234] (or [#1234-2] for comments)
automatically turn into links, with the title of the issue appended.
The status of the issue is shown on hover, and links are automatically
color coded to reflect the current status of the referenced issue.


Important:
----------

This is a Drupal 7 module, so only install on D7!

The module requires that you first create a content type of 'Issue'
and that 'Issue' contains a 'Status' field

The 'Status' field is a text select list, with options such as
'active', 'needs review', and 'fixed'


Installation / Setup:
---------------------

Install the module as normal

Go to Home > Administration > Configuration > Content authoring > Text formats

Either configure an existing text format to use the 'Issue links' filter
or create a new text format which uses the 'Issue links' filter

Ideally, 'Issue links' should be first in the filter processing order


Usage:
------ 

Use [#1234] in an issue node's body to output a link (e.g. '#1234: The Title Of The Node')


Created by:
-----------

Laurence Mercer
http://lhmdesign.com