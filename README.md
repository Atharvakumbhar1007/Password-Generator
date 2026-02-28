# Password Generator Web Application

A modern and responsive Password Generator built using HTML, CSS, and JavaScript. This application allows users to generate secure and customizable passwords with a real-time strength indicator and theme switching functionality.

## Overview

This project demonstrates core JavaScript concepts including DOM manipulation, event handling, random number generation, array operations, and theme management using CSS variables.

Users can generate strong passwords by selecting different character options and adjusting the desired password length.

## Features

Generate secure random passwords

Adjustable password length using slider

Include uppercase letters (A–Z)

Include lowercase letters (a–z)

Include numbers (0–9)

Include special characters

Password strength indicator (Weak, Medium, Strong)

Copy password to clipboard

Dark mode and light mode toggle

Automatic system theme detection

Responsive user interface

## Technologies Used

HTML5

CSS3 (CSS Variables for theme management)

JavaScript (Vanilla JS)

Clipboard API

DOM Manipulation

## How the Password Generation Works

User selects desired character types.

Selected generation functions are stored in an array.

At least one character from each selected type is added to ensure validity.

Remaining characters are generated randomly.

The final password is shuffled using the Fisher-Yates algorithm.

Password strength is calculated based on selected criteria.

## Password Strength Logic

### Strong:

Uppercase and lowercase letters included

At least one number or symbol

Password length greater than or equal to 8

### Medium:

Letters combined with number or symbol

Password length greater than 6

### Weak:

Does not satisfy the above conditions

## Theme Implementation

The application detects system theme preference using:

window.matchMedia("prefers-color-scheme: dark")

CSS variables are dynamically updated to switch between dark and light modes.

Clipboard Functionality

The generated password can be copied using the modern Clipboard API:

navigator.clipboard.writeText(password)

A temporary confirmation message is displayed after copying.

## Key JavaScript Concepts Demonstrated

DOM Selection and Traversal

Event Listeners

Random Number Generation

String and Array Manipulation

Fisher-Yates Shuffle Algorithm

Conditional Logic

CSS Variable Manipulation

System Theme Detection

Possible Future Improvements

## Password entropy calculation

Password history tracking

Export password as file

Strength percentage meter

Animated UI transitions
