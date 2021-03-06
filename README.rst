``Scrible`` Python *Console application* for taking notes
======================================================================

    New in version 0.0.3:

    - Beautiful ui with added commands such as ``sync`` for automatic 
      synchronization of notes

    New in version 0.0.2:

    - Better listing and searching options with ``--limit`` to get
      specific number of items


**Scrible** enables you create short and descriptive notes with cloud backup
*easily*:


Launching program
======================================================================

    scrible --start

.. code:: python

    """Scrible.

    Usage:
	    createnote  (<note_title>) [-m]
	    viewnote    (<note_id>) [-m]
	    deletenote  (<note_id> | -a)
	    searchnotes (<query_string>) [(--limit <items>)]
	    viewnote    (<note_id>)
	    listnotes   [(--limit <items>)]
	    next
	    export      (<filename>)
	    import      (<filename>)
	    sync 
	    scrible (-s | --start)
	    scrible (-h | --help | --version)
	Options:
	    -s, --start  Interactive Mode
	    -h, --help  Show this screen and exit.
	    -m          Starts creating note body

    """

As you can see, the commands to use are few and easy to remember.

Installation
======================================================================

From the terminal use `pip <http://pip-installer.org>`_ or easy_install::
Aftwerwards copy the database to the install directory `scribler.db`

    pip install -e git+https://github.com/jaxtreme01/Scrible#egg=scrible

Testing
======================================================================

You can run unit tests preferably by installing nosetest and run from root of the folder:

    nosetests

Usage pattern format
----------------------------------------------------------------------

**Usage pattern** depends on the command you want to execute

- View specific notes 
.. code:: python

	viewnote (<note_id>) [-m]

- Create note with just title 
.. code:: python 

	createnote  (<note_title>)

- Create note with title and body
.. code:: python 

	createnote  (<note_title>) [-m]

- Delete notes
.. code:: python 

	deletenote  (<note_id> | -a)

- Search notes
.. code:: python 

	searchnotes (<query_string>) [(--limit <items>)]

- List notes
.. code:: python 

	listnotes [(--limit <items>)]

- Import notes
.. code:: python 

	import (<filename>)

- Export notes
.. code:: python 

	export (<filename>)

- Manually sync notes

	sync 











