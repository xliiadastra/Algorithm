# Q.
Description:
Introduction
The first century spans from the year 1 up to and including the year 100, The second - from the year 101 up to and including the year 200, etc.

Task :
Given a year, return the century it is in.

Input , Output Examples :
1705 --> 18

1900 --> 19

1601 --> 17

2000 --> 20

# A)
```C
int centuryFromYear(int year) 
{
  int save = 0;
  float a = 0.0f;
  save = year / 100;
  a = year - (save * 100);
  if (a > 0)
    save = save + 1;
  
  return save;
}
