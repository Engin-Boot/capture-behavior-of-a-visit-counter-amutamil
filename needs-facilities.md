# Visit-counter for a Facilities Manager

Scenario: Report visitor trends during a week of operation

  Given the operating days of week and counts on each day
  When manager asks for visitors trend
  Then report number of visitors on each day and highlight max and min

Scenario: Alert when seating capacity is full

  Given total number of seating capacity
  When all seats are occupied
  Then alert seats are filled and no available seats
