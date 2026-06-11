# The Astrian Calendar

*by Giorgian Valentin Robescu*

## Purpose
A calendar for a civilization no longer tied to any single planet or star. The Astrian Calendar anchors to a historical moment (the first human launched object to achieve orbit), and derives all units above the day from powers of two.

The 24-hour day is retained. Circadian rhythms are biological, the day is kept because of physiology.

## Anchor Point
* October 4th, 1957 (the Sputnik 1 launch)
* Represented as: `00.00.0000` (Epoch 0, Tour 0, Day 0)
* The day before is: `-00.00.0001`
* Negative dates mirror the positive system exactly, decrementing from zero.

## Units
* 1 Osk = 8 days (the "week")
* 1 Ment = 32 days // 4 Osks (the "month")
* 1 Tour = 1,024 days // 32 Ments (the "year", ~2.8 Earth years)
* 1 Epoch = 32,768 days // 32 Tours (~89.7 Earth years)

## The Days of the Osk
Dero, Dwan, Dwo, Dree, Dwor, Daiv, Dix, Deven — compressed from "day zero" through "day seven".

Day 0 of any Tour is Dero. Day 8 is also Dero (first day of the next Osk). As you can see the system uses 0-indexed math.

Another thing to note is that each ment is equal in length, and is exactly 4 osks, so every day of every ment will be the same oskday.

You can get the oskday from the day-number of the ment with the formula `day % 8`. For example if it's the 11th we know it is Dree (11 % 8 = 3, or Dree).

## Date Format & Speech
* Written: `22.03.0850`
* Literal: "Epoch 22, Tour 3, Day 850" or "Epoch 22, Tour 3, Ment 26, Day 18"
* Colloquial: "22 point 3 point 850" or "Dwo, 18 ment 26, epoch 22 tour 3"

Math: 850 / 32 = Ment 26, remainder 18. Day 18 = Osk 2, Dwo.

The day this document is written (June 11th 2026) is `00.24.0511` or "Zero point 24 point 511" or "Deven, 31 ment 15, epoch 0 tour 24".

Epoch 1 will start on June 22nd 2047.

Epoch 2 will start on March 10th 2137.
