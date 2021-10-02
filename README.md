# Designing a Potetiometric DAC

This GitHub repository documents the design of a 10 Bit Potentiometric Digital Analog Converter. Uses SkyWater SKY130 technology and the help of simulation tools like eSim and Ngspice.

## Table of Contents
- [Introduction](#introduction)
- [Pre Layout Design and Simulation](#pre-layout-design-and-simulation)
  * [The Switch](#the-switch)
  * [2-bit DAC](#2-bit-dac)
  * [3-bit DAC](#3-bit-dac)
  * [4-bit DAC](#4-bit-dac)
  * [5-bit DAC](#5-bit-dac)
  * [6-bit DAC](#6-bit-dac)
  * [7-bit DAC](#7-bit-dac)
  * [8-bit DAC](#8-bit-dac)
  * [9-bit DAC](#9-bit-dac)
  * [10-bit DAC](#10-bit-dac)
 
# Introduction
DAC stands for Digital to Analog Converter. It is a system that converts a digital signal into an analog signal. A digital to analog converter takes in digital bits as input and converts it into a corresponding analog voltage.
The basic architecture of an N-bit potentiometric DAC is shown in the figure below.

![](ScreenShots/potentiometric_dac.png)
> Fig 1. Potentiometric architecture of an n-bit DAC

# Pre Layout Design and Simulation

# Tools used:
- [eSim](https://esim.fossee.in/downloads)
- [ngspice](http://ngspice.sourceforge.net/download.html)
- [Skywater 130nm PDK](https://github.com/google/skywater-pdk)

## The Switch

![switchschematic](ScreenShots/switchcircuit.png)
> Fig.2  Schematic of the Switch circuit designed using eSim

![switch run](ScreenShots/Switch.png)
> Fig.3 Transient Analysis of the Switch circuit in pgspice 35

From the output graph for the Switch circuit we can observe that the circuit is working as intended.
-------------------------------------------------------
## 2-bit DAC

![2bitSchematic](ScreenShots/2bitcircuit.png)
> Fig.4 Circuit schematic of a 2-bit DAC designed using eSim

![Annotation 2021-09-30 214319](ScreenShots/2biit.png)
> Fig.5 Transient Analysis of the 2-bit circuit in pgspice

Here we observe that the 2-bit didigtal input has been converted into its corresponding analog output.
We 2^2 = 4 steps in the analog output.

-------------------------------------------------------
## 3-bit DAC

![3bit](ScreenShots/3bitcircuit.png)
> Fig.6 Circuit Schematic of a 3-bit DAC designed in eSim

![3bitspice](ScreenShots/3bit.png)
> Fig.7 Transient Analysis of the 2-bit circuit in pgspice


Here we get 8 steps in the analog output as the system was given 3 digital input bits.

-------------------------------------------------------
## 4-bit DAC

![schematic](ScreenShots/4bitcircuit.png)
> Fig.8 Circuit Schematic of a 4-bit DAC designed in eSim 

![cktlevelsim](ScreenShots/4bit.png)
> Fig.9 Transient Analysis of the 2-bit circuit in pgspice

Here we get 16 steps in the analog output as the system was given 4 digital input bits.

-------------------------------------------------------
## 5-bit DAC

![schematic](ScreenShots/5bitcircuit.png)
> Fig.10 Circuit Schematic of a 5-bit DAC designed in eSim

![sim](ScreenShots/5bit.png)
> Fig.11 Transient Analysis of the 2-bit circuit in pgspice

Here we get 32 steps in the analog output as the system was given 5 digital input bits.

-------------------------------------------------------
## 6-bit DAC

![schematic](ScreenShots/6bitcircuit.png)
> Fig.12 Circuit Schematic of a 6-bit DAC designed in eSim

![sim](ScreenShots/6bit.png)
> Fig.13 Transient Analysis of the 2-bit circuit in pgspice

Here we get 64 steps in the analog output as the system was given 6 digital input bits.

-------------------------------------------------------
## 7-bit DAC

![schematic](ScreenShots/7bitcircuit.png)
> Fig.14 Circuit Schematic of a 7-bit DAC designed in eSim

![sim](ScreenShots/7bit.png)
> Fig.15 Transient Analysis of the 2-bit circuit in pgspice

Here we get 128 steps in the analog output as the system was given 7 digital input bits.

-------------------------------------------------------
## 8-bit DAC

![schematic](ScreenShots/8bitcircuit.png)
> Fig.16 Circuit Schematic of a 8-bit DAC designed in eSim

![sim](ScreenShots/8bit.png)
> Fig.17 Transient Analysis of the 2-bit circuit in pgspice

Here we get 256 steps in the analog output as the system was given 8 digital input bits.

-------------------------------------------------------
## 9-bit DAC

![schematic](ScreenShots/9bitcircuit.png)
> Fig.18 Circuit Schematic of a 9-bit DAC designed in eSim

![sim](ScreenShots/9bit.png)
> Fig.19 Transient Analysis of the 2-bit circuit in pgspice

Here we get 512 steps in the analog output as the system was given 9 digital input bits.

-------------------------------------------------------
## 10-bit DAC

![schematic](ScreenShots/10bitcircuit.png)
> Fig.20 Circuit Schematic of a 10-bit DAC designed in eSim

![sim](ScreenShots/9bit.png)
> Fig.21 Transient Analysis of the 2-bit circuit in pgspice

Here we get 1024 steps in the analog output as the system was given 10 digital input bits.

-------------------------------------------------------
