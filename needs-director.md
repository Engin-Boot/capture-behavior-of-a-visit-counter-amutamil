# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given number of patients visited hospital during working days and holidays
  When director asks for the count
  Then show the count

Scenario: Compute parking slots to reserve for visiting specialists

  Given
  Total number of cars capacity that the parking area can hold
  Total number of specialists
  Already occupied Parking slots
  
  When
  Total capacity - Occupied == Total number of specialists.
  
  Then
  Never allow any other for parking.
