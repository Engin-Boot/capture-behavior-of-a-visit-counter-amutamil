# Visit-counter for a Facilities Manager

Scenario: Report visitor trends during a week of operation

  Given :
  Working server,
  The operating days of week and counts on each day,
  When  :
  Manager asks for visitors on specific days.
  Then  :
  Display number of visitors on each day,
  Highlight max and min visitors.

Scenario: Alert when seating capacity is full

  Given :
  Total number of seating capacity,
  Occupied seats count,
  Working server.
  When  :
  No seats available.
  Then  :
  Alert no seats.
