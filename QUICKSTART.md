#Get Developing for Plone Really Quickly

The following instructions assume that you already have dotcloud installed and
configured and you've already checkout the stack-python-plone from github.

##Installation:

    instance=instancename
    dotcloud create $instance

Once your instance has been configured to work with dotcloud you can run
the following command:

    dotcloud push 
  
##Usage:
Visit your new Plone site in your web browser at
`http://{yourinstance}-{useraccount}.dotcloud.com/Plone` and log in.
Use the following credentials:

    username: admin
    password: admin

##Enable aliases

    source aliases
    
##Editing the buildout.cfg file

    plonecfg

##Running buildout

    plonebuild
    
#Restart the plone instance to see your changes:

    plonerestart

or

    plonerestartall
    
##Other commands

    plonestatus