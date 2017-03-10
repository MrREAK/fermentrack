

###### Can I change the temperature format on a beer I've started logging?

No. To prevent inconsistency the log format is permanently set when logging begins to the temperature format associated with the device. If you would like to change the format and restart logging, do the following:

 1. Update the temperature format in control constants to the desired format
 2. Stop logging the existing beer
 3. Start logging a new beer


###### Help - I forgot my Fermentrack login/password!

Thankfully, this is a pretty easy issue to overcome. Django provides the `manage.py` command line script which contains the `createsuperuser` command. To leverage this, do the following (assuming the standard install locations):
 
 1. Log into your Raspberry Pi via ssh and switch to the user you installed Fermentrack to (generally this can be done with the command `sudo su brewpi` assuming you installed to the `brewpi` user)
 2. Change to the user's home directory (`cd ~`)
 3. Enable the virtualenv (`source venv/bin/activate`)
 4. Change to the Fermentrack directory (`cd fermentrack`)
 5. Run the createsuperuser command (`./manage.py createsuperuser`)
 6. Follow the prompts to create a new superuser account
 7. Log into the Fermentrack admin panel and delete/modify the old account. The Fermentrack admin panel can be accessed through the `Settings` page (the gear in the upper right) and clicking the "Django Admin" button.