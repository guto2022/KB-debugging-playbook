# UTF-8 Encoding Error

## Context
Reading environment variables from a .env file after pasting values

## Problem
The app was breaking due to an encoding issue

## Root Cause
The .env file had invisible/special characters

## Attempts
- Tried changing encoding using "Save with Encoding" in VS Code → didn't work  
- Tried changing encoding using "Reopen with Encoding" in VS Code → didn't work  
- Tried creating the .env file via terminal → didn't work  

## Solution
Rewrote the .env file manually

## Takeaway
Invisible characters can silently break applications, especially in .env files

## Tags
#bug #backend #env #encoding