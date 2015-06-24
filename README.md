# crow-vm

A development environment for NYC City Record Online.

# Prerequisite

  1. Install [vagrant](https://www.vagrantup.com/) 
  2. Install [ansible](http://docs.ansible.com/intro_installation.html)
  3. set _nyc_app_id_ & _nyc_app_key_ in roles/parser-address/defaults/main.yml
  4. vagrant box add ubuntu/trusty64
  5. Add the following line to your hosts file:
      ```
      127.0.0.1   crownyc-ubuntu-trusty64
      ```
  6. Download glassfish-4.1.zip & move it to roles/glassfish4/files

      ```
      wget http://download.java.net/glassfish/4.1/release/glassfish-4.1.zip
      mv glassfish-4.1.zip roles/glassfish4/files
      ```

# Provision

```
vagrant up
```

# Test
4. if you can see [this demo site](http://crownyc.ubuntu.trusty64:8080/hello), it probably worked.

# Use your box

```
vagrant ssh
```

