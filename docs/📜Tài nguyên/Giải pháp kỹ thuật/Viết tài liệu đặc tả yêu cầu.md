---
share: true
created: 2023-09-05T16:17
updated: 2025-04-22T20:34
---
Tuy [Hình ảnh một phần mềm được xây dựng bằng lý tính từ lý thuyết là một ảo tưởng](../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/C%C3%B4ng%20ngh%E1%BB%87%20th%C3%B4ng%20tin/K%E1%BB%B9%20thu%E1%BA%ADt%20ph%E1%BA%A7n%20m%E1%BB%81m/Ki%E1%BA%BFn%20tr%C3%BAc/H%C3%ACnh%20%E1%BA%A3nh%20m%E1%BB%99t%20ph%E1%BA%A7n%20m%E1%BB%81m%20%C4%91%C6%B0%E1%BB%A3c%20x%C3%A2y%20d%E1%BB%B1ng%20b%E1%BA%B1ng%20l%C3%BD%20t%C3%ADnh%20t%E1%BB%AB%20l%C3%BD%20thuy%E1%BA%BFt%20l%C3%A0%20m%E1%BB%99t%20%E1%BA%A3o%20t%C6%B0%E1%BB%9Fng.md), nhưng [Việc giả bộ là phần mềm được xây dựng bằng lý tính là có ích](../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/C%C3%B4ng%20ngh%E1%BB%87%20th%C3%B4ng%20tin/K%E1%BB%B9%20thu%E1%BA%ADt%20ph%E1%BA%A7n%20m%E1%BB%81m/Ki%E1%BA%BFn%20tr%C3%BAc/Vi%E1%BB%87c%20gi%E1%BA%A3%20b%E1%BB%99%20l%C3%A0%20ph%E1%BA%A7n%20m%E1%BB%81m%20%C4%91%C6%B0%E1%BB%A3c%20x%C3%A2y%20d%E1%BB%B1ng%20b%E1%BA%B1ng%20l%C3%BD%20t%C3%ADnh%20l%C3%A0%20c%C3%B3%20%C3%ADch.md)

## Computer Specification
A specification of the machines on which the software must run. The machine need not be hardware-for some software this section might simply be a pointer to a language reference manual.

## Input/Output Interfaces
A specification of the interfaces that the software must use in order to communicate with the outside world.

## Specification of Output Values
For each output, a specification of its value in terms of the state and history of the system's environment.

## Timing Constraints
For each output, how often, or how quickly, the software is required to recompute it. 

## Accuracy Constraints
For each output, how accurate it is required to be.

## Likely Changes
If the system is required to be easy to change, the requirements should contain a definition of the areas that are considered likely to change. You cannot design a system so that everything is equally easy to change. Programmers should not have to decide which changes are most likely.

## Undesired Event Handling
The requirements should also contain a discussion ,of what the system should do when, because of undesired events, it cannot fulfill its full requirements. Most requirements documents ignore those situations; they leave the decision about what to do in the event of partial failures to the programmer.