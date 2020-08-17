# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given : the working server which stores "number of patients visited hospital during working days and holidays seperately"
  When : director asks for the count on holidays and working days 
  Then show the count

Scenario: Compute parking slots to reserve for visiting specialists

  Given
  Total number of cars capacity that the parking area can hold
  Total number of specialists
  Already occupied parking slots
  
  When : the difference between total capacity and occupied is equal to total number of specialists
  
  Then Never allow any other for parking.
