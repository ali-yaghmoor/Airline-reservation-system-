# Airline Reservation System

Final project for my Computer Engineering Technology program at Seneca College, Winter 2024.

The goal was to build something that actually persists between runs — most class projects just reset every time you close them, which felt pointless. This one saves reservation data to a file so it carries over between sessions.

## What it does

- Register passengers by first and last name
- See a seat map showing what's available
- See a seat map showing what's taken
- Reservations save to a file on exit and reload next run

## How to run it

Open `Final_Project/Final_Project.sln` in Visual Studio and build from there. Configured for x64 Debug by default.

On Linux you can compile directly:

```bash
gcc "Final_Project/Econo-Flight Airline Reservation Program W 2024.c" -o airline
./airline
```

Then follow the menu options.

## Notes

First time I had to deal with file I/O in C. Getting the seat data to write and read back in the right format took longer than I expected — had to be careful about how I was parsing the text file on reload so it didn't corrupt the seat state.

Built in C, Visual Studio 2022.
