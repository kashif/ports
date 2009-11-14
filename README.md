# Geospatial MacPorts

Some updated Portfiles for geo application via MacPorts.

## Installation

Rakefile via Jeff Hodges, just cd to the ports directory and run:

    $ rake

This will generate the PortIndex, install a new MacPorts source
pointing at this directory, and set up a Git post-commit hook to
regenerate the PortIndex any time you commit Portfile changes.

Now you can `sudo port install libspatialite` to install the latest
libspatialite etc. For a list of available local ports, try `rake list`. 
To manually update the PortIndex (or to fix the Git hook, or the sources list), 
just run `rake` again.