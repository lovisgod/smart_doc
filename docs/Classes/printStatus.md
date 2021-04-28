---
sidebar_position: 14
---

# PrintStatus

```
/**
 * This is a sum type that represents the result of a printout
 * indicating whether the print was successful or not
 *
 * - OK class indicates that print was successful
 * - Error class captures what error prevented the printout
 */
 ```


### Constructor

`PrintStatus(val message: String)`

### Properties

`class Ok(message: String)`: [PrintStatus(message)](#)

`class Error(message: String)`: [PrintStatus(message)](#)



