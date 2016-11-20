How to set up ssh alias and ssh keygen
=======================================

Change ``USERNAME``, ``SERVER``, ``SERVER-NAME`` and ``PORT``


On server::

  cd .ssh
  ssh-keygen -t rsa  
  cat id_rsa.pub >> authorized_keys
  chmod 600 authorized_keys
  rm id_rsa.pub 

On client::
  
  cd ~/.ssh 
  scp -P PORT USERNAME@SERVER:.ssh/id_rsa SERVER-NAME.rsa 
  chmod 600 SERVER-NAME.rsa 


Add this to ``~/.ssh/config``::

  Host SERVER 
       HostName SERVER
       Port PORT 
       User USERNAME 
       IdentityFile ~/.ssh/SERVER-NAME.rsa 
