# GPS ↔ Gregorian Calendar Converter #

### Project Overview

This project is a lightweight Python utility designed to convert dates between the GPS calendar system and the Gregorian calendar, and vice versa. The tool supports interactive user input and provides accurate conversion using the official GPS epoch reference.

### Background

- GPS Time started on January 6, 1980, known as the GPS Epoch

- GPS time is represented using:

      GPS Week Number
      Day of Week (Sunday = 0 to Saturday = 6)


### Features

- Convert GPS Week + Day Number → Gregorian Date

- Convert Gregorian Date → GPS Week + Day Number

- Interactive command-line interface

- Input validation and error handling

- Uses standard Python libraries

### Methodology
*1. GPS to Gregorian Conversion*

- Uses the official GPS Epoch:
  **1980-01-06**

- Adds:

    Number of weeks × 7 days
    Day-of-week offset

*2. Gregorian to GPS Conversion*

- Computes day difference from GPS Epoch

- Calculates:

    GPS Week Number
    GPS Day Number (Sunday = 0)

### Technologies & Libraries Used
**Programming Language**
- Python

**Standard Libraries**
- datetime
- timedelta
