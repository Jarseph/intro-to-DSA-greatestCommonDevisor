# intro-to-DSA-greatestCommonDevisor

function gcd1
  // accepts a - a non-negative integer
  //         b - a non-negative integer

  if a is equal to 0 then the GCD of a and b is b, so return b
  if b is equal to 0 then the GCD of a and b is a, so return a
  while b is not 0 do
    let r be the remainder of dividing a by b
    set a to equal b
    set b to equal r
  return a
  
  
  function gcd2
  // accepts a - a non-negative integer
  //         b - a non-negative integer

  if a is equal to 0 then the GCD of a and b is b, so return b
  if b is equal to 0 then the GCD of a and b is a, so return a

  initialize an array named divA with the value [1, a]
  initialize an array named divB with the value [1, b]
  initialize an empty array named common

  for i = 2 to a - 1 do
    if a can be divided by i without a remainder then
      add i to the array divA

  for i = 2 to b - 1 do
    if b can be divided by i without a remainder then
      add i to the array divB

  for each number n in the array divA do:
    if n is in the array divB then
       add n to the array common

  initialize a variable named largest to the smallest possible number
  for each number n in commmon do:
    if n is greater than largest then
      assign largest the value n

  return largest
  
  
