## Addition

# Scenario: Addition of two positive numbers
  
  Given Calculator is turned on.

  When I type in "positive number"
      and I press "plus"
      and I press "Positive number"
      and I press "equal"
  
  Then I see the "added number" in result

# Scenario: Addition of two negative numbers
  
  Given Calculator is turned on.

  When I type in "negative number"
      and I press "plus"
      and I press "nagative number"
      and I press "equal"
  
  Then I see the "added number" in result
  
# Scenario: Addition of numbers is "out of range"
  
  Given Calculator is turned on.

  When I type in "number"
      and I press "plus"
      and I press "number"
      and I press "equal"
  
  Then I see the "Positive or negative infinite" in result
  
# Scenario: plus is pressed multiple times
  
  Given Calculator is turned on.

  When I type in "number"
      and I press "plus"
      and I press "plus"
      and I press "plus"
  
  Then I see the "only one plus sign" in result
