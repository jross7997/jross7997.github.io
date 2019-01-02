---
layout: page
title: Projects
permalink: /projects/
---

* [**Hexapod Walking Robot**](https://github.com/jross7997/Hexapod-Robot-Senior-Capstone)
\- For my Engineering Senior Capstone, my team and I designed, built, and programmed a Hexapod Walking Robot that was wirelessly 
	controlled via a web app. I did most of the programming in this project and helped with assembling and troubleshooting the 
	robot.

	The robot has six legs, each with two joints. Overall it has 12 degrees of freedom. The servos are controlled with the 
	TM4C123GH6PM (previously called the Tiva-C) Microcontroller, which was programmed in C. The web app was served and processed 
	with the NodeMCU WiFi-enabled MicroController, and that was programmed with the Arduino IDE. The NodeMCU communicates to the 
	Tiva-C using a one-way UART Bridge.

	The robot could walk forwards, backwards, turn left and right, and had two different waving functions. It could be run in 
	Continuous mode, which would allow for the robot to walk continuously forever. It has a slow mode that makes it walk slower, to 
	better show off the tripod gait that it uses.

	Overall, the robot worked very well, It was robotic in it's movements, so the addition of more degrees of freedom would be a 
	great improvement. The robot also is lacking a battery, so it is tied to a Lab Bench power Supply.

	If you're interested in learning more, check out this [project report]({{ "/docs/Walking-Robot-Report.pdf" | absolute_url }}).

* [**LED Flicker Research**](https://github.com/jross7997/LED-Flicker-Research)
	\- The flickering of a light source can cause some negative psychological and physiological effects on a person, such as headaches, migranes, and decreased
	visual task performance and comfort. Currently, the best way to reliably measure flicker is either to invest in some expensive equipment, or placing an LED
	in an opaque box with a sensor opposite the source. The professor that organized this research has proposed a new method of measuring the flicker. Since the 
	current driving the LED will determine the intensity of the output, then the flicker can be predicted from the current measurement. 

	The goal of the summer research was to build a testing apparatus, develop programs to automate the collection and processing of data, and begin testing the 
	proposed method for validity. The testing apparatus that was built largely follows the opaque box description. It was a box made from 2 by 6 inch pieces of wood,
	where the inside was painted black. The box was roughly 2.25 feet (0.7 meters) long. The ends of the box had opaque pieces of cardboard in which the LED strip and
	ambient light sensors could be attached.

	A program to collect data was built using LabVIEW, it collects data both from an oscilloscope and from a DAQ device, this allows
	 for the collection of data from both the driving current to the LED driver and the output signal from the light sensor. The data processing was done in MATLAB. 
	 The average percent flicker and flicker index was taken for both the driving current data and the output signal data.

	 We ran into some issues when it came to the selection of a sensor and a driver which caused the delay on any results that would be needed for publishing.
	 It was discovered that the sensors needed to have an analog output with no capacitance on the output. If there is a digital output or any capacitance, the
	 output signal will be smoothed out, which can make the determining any flicker metrics impossible. The issue with the driver we were using is that it was 
	 seemingly designed to prevent flicker. The driver did not produce any flicker in any of our tests, more research is still required to determine the cause of this. 

* [**Brute Force Password Cracker Addition to Web of Trust**](https://github.com/jross7997/CSC333-Brute-Force-Chrome-Extension)
	\- Written as a patner project for CSC333, we decided to add an educational password cracker to the existing Web Of Trust browser exstension.
	The cracker itself is a python script being run on a local Django server. The browser will then take in a password to crack, make a call to the Django
	server and display the number of attempts it took to crack that password to the user. The addition worked as it was supposed to, but it was rushed together. 
	If I were to do this again, I would've tried to make the addition just using JavaScript and python, instead of cobbling it together with HTML, JavaScript, and Python.
	There is also a security flaw in the design, the program sends the password that is to be cracked in a query parameter instead of encrypting it and sending it in the body.
	This was the quickest way for us to send the password data to the Django Server. If you're interested in learning more about this project, check out this [project report]({{ "/docs/Term-Paper.pdf" | absolute_url }}) that features an 
	analysis of data breaches.

* [**LEG V8 Microprocessor Project and Assembler**](https://github.com/jross7997/ECE475-CPU-Project)
	\- This was a group project for ECE475: Computer Architecture. We were given the task of writing a basic 64 bit microprocessor in VHDL from scratch. We needed
	to follow a Control Unit and Data Path model and implement a subset of the LEG V8 instruction set. The processor would be designed for the NexSys 4 development board.
	The goal was to run a specific line of C code. We had to convert the given code into Assembly, and I wrote a python script that would read properly formatted
	Assembly code into binary code that the processor could understand. We could not get the processor to run the code correctly, it got itself into a infinite loop. We simply did not have enough time
	to fix this issue. We did manage to get all of the components working separately, the issues arose when trying to get the components working in a single system. If you're interested in 
	learning more, check out this [project report]({{ "/docs/Processor-Report.pdf" | absolute_url }}).

* **Shopping Cart Web Service**
	\- A collection of assignments for CSC435: Web Services. The assignment was to build a basic web service in 4 different frameworks. [Java Servlets](https://github.com/jross7997/CSC435-Shopping-Cart-Servlets), [Java Spark](https://github.com/jross7997/CSC435-Shopping-Cart-Spark),
	[Groovy on Grails](https://github.com/jross7997/CSC435-Shopping-Cart-Grails), and [Dropwizard](https://github.com/jross7997/CSC435-Shopping-Cart-Dropwizard). Each had slightly different requirements, for example, the Servelets and Spark assignments required the use of a mySql Database.
	The web service that was made was a simple shopping service. The database would populate with food items from an online API. The users could then place items from that
	database and store it in a cart, which is stored either in the session or in a separate database depending on the version. The user can add and remove items from the cart, and the cart
	would calculate the total price of all of the items. The price was determined by the nutitional value of the food, so foods with lower calorie, fat, and sodium counts cost less than food with higher counts.

* **Multi-Function Clapper Circuit**
	\- A partner project for ECE314: Microelectronic Circuits. The assignment was to design an analog circuit to do a proposed function. But, we had to propose a function
	that is not a common circuit. It was easiest for us to modify an existing idea. We decided to take a basic clapper circuit and add a second function. The two functions would
	be selected dependent on the amplitude of the clap/snap/noise that you make. So, in the case of our circuit, a louder noise would toggle on an LED and a softer noise would toggle on a Buzzer. 
	If you're interested in learning more, check out this [project report]({{ "/docs/Clapper-Report.pdf" | absolute_url }}).

* [**Autonomous Driving and Parking**](https://github.com/jross7997/ECE375-Rover-Project)
	\- Written and designed as a group project in ECE375: Microprocessor Applications. We built a small rover and programmed the HCS12 Dragon board to autonomously drive the rover
	on a predesigned track. The track has two possible paths, the short and long paths. The path is decided by the presence of a road block. If the road block is present,
	the long path was taken, if there wasn't a road block then the short path was taken. After the path was traversed, the rover had to choose one of three different
	parking spots. The first open spot that the rover found was taken. The rover would then wait in the parking spot until it was reset. The one that we made worked very well, but it was 
	a little inconsistent. This was largely due to the older equipment that we were given. The battery was the biggest issue. It would drain very quickly, and the lower the charge on the battery, 
	the worse our rover in general would perform. It worked best on a full charge. If you're interested in learning more, check out this [project report]({{ "/docs/Robot-Report.pdf" | absolute_url }}).

* [**Random Number Generation Math Game**](https://github.com/jross7997/ECE271-Random-Number-Game-Project)
	\- A group design for ECE271: Digital Systems. This was the first school project that I did. We had to use digital logic systems to program a math game.
	Two random numbers would be displayed on some seven segment displays, and within a certain time limit, the player would have to add the numbers and give an answer
	in binary on some switches. We did not completely finish the game, there were a few bugs, but the basic functionality was there. We did not have enough time to perfect the project.
	If you're interested in learning more, check out this [project report]({{ "/docs/Random-Number-Generation-Math-Game.pdf" | absolute_url }}).

