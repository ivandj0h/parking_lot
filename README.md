# The Parking Lot

## About The Problem

The Parking lot that can hold up to 'n' cars at any given point in time. Each slot is
given a number starting at 1 increasing with increasing distance from the entry point
in steps of one. I want to create an automated ticketing system that allows my
customers to use my parking lot without human intervention.

When a car enters my parking lot, I want to have a ticket issued to the driver. The
ticket issuing process includes us documenting the registration number (number
plate) and the colour of the car and allocating an available parking slot to the car
before actually handing over a ticket to the driver (we assume that our customers are
nice enough to always park in the slots allocated to them). The customer should be
allocated a parking slot which is nearest to the entry. At the exit the customer returns
the ticket which then marks the slot they were using as being available.
Due to government regulation, the system should provide me with the ability to findout:

- Registration numbers of all cars of a particular colour.
- Slot number in which a car with a given registration number is parked.
- Slot numbers of all slots where a car of a particular colour is parked.

## Getting Started

[![Build Status](https://travis-ci.org/iolufemi/Express-REST-API-Generator.svg?branch=dev)](https://travis-ci.org/iolufemi/Express-REST-API-Generator) [![codecov](https://codecov.io/gh/iolufemi/Express-REST-API-Generator/branch/master/graph/badge.svg)](https://codecov.io/gh/iolufemi/Express-REST-API-Generator) [![Documentation Status](https://readthedocs.org/projects/api-template/badge/?version=latest)](http://api-template.readthedocs.io/en/latest/?badge=latest)
![Test Status](https://github.com/bchew/dynamodump/actions/workflows/test.yml/badge.svg)
![Code Style](https://img.shields.io/badge/code%20style-black-black)

To Run this Program, what you've to do are :

- clone this Repository <br />
  `git clone https://github.com/ivandi1980/parking_lot.git`
- Install all dependencies (testing dependent packages) <br />
  `npm install`
- Run the main program <br />
  `node index.js`
- Run all tests cases <br />
  `npm test test/run.testcases.js`

## Input-Output Examples

- Input (contents of file):<br />

  - create_parking_lot 6
    - park KA-01-HH-1234 White
    - park KA-01-HH-9999 White
    - park KA-01-BB-0001 Black
    - park KA-01-HH-7777 Red
    - park KA-01-HH-2701 Blue
    - park KA-01-HH-3141 Black
  - leave 4
  - status
    - park KA-01-P-333 White
    - park DL-12-AA-9999 White
    - registration_numbers_for_cars_with_colour White
    - slot_numbers_for_cars_with_colour White
    - slot_number_for_registration_number
    - KA-01-HH-3141
    - slot_number_for_registration_number MH-04-AY-1111

- Output (to STDOUT):<br />
  - Created a parking lot with 6 slots
    - Allocated slot number: 1
    - Allocated slot number: 2
    - Allocated slot number: 3
    - Allocated slot number: 4
    - Allocated slot number: 5
    - Allocated slot number: 6
  - Slot number 4 is free
  - Slot No. Registration No Colour
    1. KA-01-HH-1234 White
    2. KA-01-HH-9999 White
    3. KA-01-BB-0001 Black
    4. KA-01-HH-2701 Blue
    5. KA-01-HH-3141 Black
  - Allocated slot number: 4
  - Sorry, parking lot is full
  - KA-01-HH-1234, KA-01-HH-9999, KA-01-P-333
  - 1, 2, 4, 6
  - Not found

## The Stack

The Stack that i use for this Project is `Javascript`, the reason is because i love `Javascript` very much and i am confortable to working with it.

## The Dependencies

I don't use many dependencies for this Project, i just use 2 dependencies such are :

1. <a href="https://mochajs.org/">Mocha</a>
2. <a href="https://www.chaijs.com/">Chai</a>

Those two dependencies are used to do testing, just it, nothing more.

## Credit

<a href="https://linkedin.com/in/ivandjoh" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="ivandjoh" height="15" width="20" /></a>
<a href="https://instagram.com/ivandjoh" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/instagram.svg" alt="ivandjoh" height="15" width="20" /></a>
