# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given : The server is working and count stored in server.
  When  : Director asks for "Count on holidays" and "Working days".
  Then  : Display the "Count on holidays" and "Working days".

Scenario: Compute parking slots to reserve for visiting specialists

  Given :
  Working server,
  Total capacity of the parking area,
  Total number of specialists,
  Already occupied parking slots.
  When  :
  Director asks "compute parking slots".
  Then  :
  Display the "Parking slots available".
