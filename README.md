
# PRE-REQUISITE

  - Should have dns entry of master , slave and arbiter server.

# VARS
  - version (mongo version , by default 3.6)
  - replSetName (replication set name)
  - slave_dns (list variable , can add mutiple slave dns) [by default  mongo-slave.internal-mongodb.com.]
  - slave_no (no of slaves in cluster , by default 1)
  - mongo_port

# HOST
  - in host file three groups are there master , slave and arbiter

# HOW TO RUN

  - by default ansible-playbook -i hosts site.yml
  - ansible-playbook -i hosts --extra-vars '{"slave_dns":["a.com","b.com","cl.com"]}' site.yml
