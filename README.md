# QuickFakeTest
Simple test for fake storage devices (usb stick, pen drive, memory card, ...)

## Introduction
I've tried few different software to check how much memory there was on my fake usb pen drive, and they all failed or were so slow that I've interrupted them.
I guess it's because they tried to check the whole capacity (2TB).

## This script
This bash script writes 1GB test files. Each time, after having written a new file, it checks the previous files.
When that starts to fail, the script exits.
Just count how many files (minus one) and it should be approximately the capacity of your storage device.
