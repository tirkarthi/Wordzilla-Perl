Wordzilla-Perl
==============

Version v1.0 :

  Please read the Installation instructions carefully to install them. A single, ready-to-install package with dependencies included will be released soon.

Installation :

  At the moment the app supports only GNU/Linux with Perl.

  Its a Perl script that requires DBI , DBD::SQLite and preferably SQLite3 or SQLite. 

  The app requires the Database at /home/$USER/ (Replace the $USER with username or value of `echo $USER`)

Perl modules :

  Please install the Perl modules from CPAN.

Installation :

        cpan DBI
        
        cpan DBD::SQLite

  You can also use cpanm or other means to install the modules.

SQLite :

  The app and the database uses SQLite3. Its lightweight and leaves a low memory footprint.

Installation :

        sudo apt-get install sqlite3
  
  package manager (apt-get) might vary between distributions.

Database :

  Extract the Wordzilla.tar.xz file to /home/$USER/ (Replace the $USER with username or value of `echo $USER`)
  
  md5sum : c10acd233f1ee0aa6789cca544b91a6a

Add the Perl script to $PATH:

  From the location of the script add it to the path to use it like a command.
  
        echo $PATH;
  
  select a path preferably /usr/local/bin.
  
        sudo cp Wordzilla /usr/local/bin
  
wordzilla [options] word

		-help  print the help text
		-c     print the meaning and part of speech in color
		-p     takes the part of speech as the argument
		-m     takes the number of meanings to be displayed as argument
		-man   display the man page
