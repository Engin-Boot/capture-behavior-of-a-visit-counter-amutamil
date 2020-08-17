# Visit-counter technical needs

Scenario: Recover across restarts of the server
that runs the visit-counter

  Given the server and external storage
  When switch Off and On the server
  Then reload the past value form external storage

Scenario: Reconcile counts if the sensor is offline for a while

  Given the count while sensor is off
  When connection established
  Then add/update  to the already present count
