Wordzilla-Perl
==============

Version v0.1 :

  Please read the Installation instructions carefully to install them. A single, ready-to-install package with dependencies included will be released soon.

Installation :

  At the moment the app supports only Linux with Perl.

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
  
  package manager (apt-get) might vary between the Operating Systems.

Database :

  Extract the Wordzilla.tar.xz file to /home/$USER/ (Replace the $USER with username or value of `echo $USER`)
  
  md5sum : c10acd233f1ee0aa6789cca544b91a6a

Add the Perl script to $PATH:

  From the location of the script add it to the path to use it like a command.
  
        echo $PATH;
  
  select a path preferably /usr/local/bin.
  
        sudo cp Wordzilla /usr/local/bin
  
How to use the app :

  If you have added the script to your path then execute the command as follows
  
        Wordzilla <your_word> <enter>
  
  Replace <your_word> with the word whose meaning is to be found and press enter.
  
  You can also enter the command as 'Wordzilla' without input. It asks the word as the input.
  
  It gives the part of speech followed by meaning. The entry for effective is as follows
  
        Wordzilla effective <enter>
      
        effective has 4 meanings.
      
        Adjective 
        Having the power to produce a required effect or effects.
      
        View all meanings ( Y / N ) : 
  
  It shows the first meaning and asks you whether to show the later meanings if present. 
  
  If you press Y or y, it shows all the meanings.
  
  If you press N or n, it exits the app.
  
  You can also change the location of the database to search within the Perl script.
