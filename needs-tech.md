# Visit-counter technical needs

Scenario: Recover across restarts of the server
that runs the visit-counter

  Given :
  Working server, External storage.
  
  When  :
  server is switch Off.
  Then  :
  store the "Visitor count" in external storage.
  
  When  :
  server is switch On.
  Then  :
  Load the "Visitor count" from external storage.

Scenario: Reconcile counts if the sensor is offline for a while

  Given :
  Sensor, Working server, Local storage.
  
  When  :
  connection lost.
  Then  :
  Reset local storage to "zero"
  Increase count in local storage from zero.
  
  When  :
  Server reconnects.
  Then  :
  Update count in server from local storage.
