# Addition

## Scenario: Addition of two positive numbers
  
  Given Calculator is turned on.
  When I type in positive number and I press plus and I type in Positive number
  and I press equal
  Then I see the addition in result

## Scenario: Addition of two negative numbers
  
  Given Calculator is turned on.
  When I type in first negative number and I press plus and I type in second
  negative number and I press equal
  Then I see the addition in result
  
## Scenario: First operand is positive and second operand is negative

  Given Calculator is turned on. ( user input: 6+-7=)

  When I type in positive number and I press plus and I type in negative number
  and I press equal
  Then calculator will subtract two numbers. Output for given user input: -1
  
## Scenario: First operand is negative and second operand is positive
  
  Given Calculator is turned on. ( user input: -7+6=)

  When I type in negative number and I press plus and I type in positive number
  and I press equal
  Then calculator will add two numbers. Output for given user input: -1
  
## Scenario: plus is pressed multiple times
  
  Given Calculator is turned on.

  When I type in number and I press more than once  
  Then calculator will consider only single plus.
