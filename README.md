# 7_segment_display
My first personal project. I would like be able, with a breadboard and wires, to display 10 numbers (0 -> 9) when I push some buttons. These will then be incremented by 1 each time with another button. 

## Table de vérité 

| A = 8 | B = 4 | C = 2 | D = 1 | Décimal | a | b | c | d | e | f | g |
| --- | --- | --- | --- | :---: | --- | --- | --- | --- | --- | --- |--- |
| 0 | 0 | 0 | 0 | 0 | 1 | 1 | 1 | 1 | 1 | 1 | 0 | 
| 0 | 0 | 0 | 1 | 1 | 0 | 1 | 1 | 0 | 0 | 0 | 0 | 
| 0 | 0 | 1 | 0 | 2 | 1 | 1 | 0 | 1 | 1 | 0 | 1 |
| 0 | 0 | 1 | 1 | 3 | 1 | 1 | 1 | 1 | 0 | 0 | 1 | 
| 0 | 1 | 0 | 0 | 4 | 0 | 1 | 1 | 0 | 0 | 1 | 1 |
| 0 | 1 | 0 | 1 | 5 | 1 | 0 | 1 | 1 | 0 | 1 | 1 |
| 0 | 1 | 1 | 0 | 6 | 1 | 0 | 1 | 1 | 1 | 1 | 1 |
| 0 | 1 | 1 | 1 | 7 | 1 | 1 | 1 | 0 | 0 | 0 | 0 |
| 1 | 0 | 0 | 0 | 8 | 1 | 1 | 1 | 1 | 1 | 1 | 1 |
| 1 | 0 | 0 | 1 | 9 | 1 | 1 | 1 | 1 | 0 | 1 | 1 |
| 1 | 0 | 1 | 0 | 10 | X | X | X | X | X | X | X |
| 1 | 0 | 1 | 1 | 11 | X | X | X | X | X | X | X |
| 1 | 1 | 0 | 0 | 12 | X | X | X | X | X | X | X |
| 1 | 1 | 0 | 1 | 13 | X | X | X | X | X | X | X |
| 1 | 1 | 1 | 0 | 14 | X | X | X | X | X | X | X |
| 1 | 1 | 1 | 1 | 15 | X | X | X | X | X | X | X |

### As a reminder, these are the logic gates tables 
![The gates](fatimaalame/7_segment_display/logic_gates.png)

source: https://www.bragitoff.com/2015/10/digital-logic-ics-with-symbols-and-truth-tables/

a =  A OR C OR (B AND D) OR (NOT B AND NOT D)
b = NOT B OR (NOT C AND NOT D) OR (C AND D)
