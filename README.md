# autonomus
#pragma config(Motor,  port1,            ,             tmotorVex393_HBridge, openLoop)
#pragma config(Motor,  port2,            ,             tmotorVex393_MC29, openLoop)
#pragma config(Motor,  port3,            ,             tmotorVex393_MC29, openLoop, reversed)
#pragma config(Motor,  port4,            ,             tmotorVex393_MC29, openLoop, reversed)
#pragma config(Motor,  port5,           RBMotor,       tmotorVex393_MC29, openLoop)
#pragma config(Motor,  port6,           LSciLift,      tmotorVex393_MC29, openLoop)
#pragma config(Motor,  port7,           RSciLift,      tmotorVex393_MC29, openLoop, reversed)
#pragma config(Motor,  port8,           Lclaw,         tmotorVex393_MC29, openLoop, reversed)
#pragma config(Motor,  port9,           Rclaw,         tmotorVex393_MC29, openLoop, reversed)
#pragma config(Motor,  port10,           ,             tmotorVex393_HBridge, openLoop, reversed)
//*!!Code automatically generated by 'ROBOTC' configuration wizard               !!*//

task main()
{
	motor(port2) = -127; // move backward
	motor(port3) = -127;
	motor(port4) = -127;
	motor(port1) = -127;
	wait10Msec(17);
	motor(port2) = 0; // stop wheels
	motor(port3) = 0;
	motor(port4) = 0;
	motor(port1) = 0;
	motor(port10) = 127; // put claw down
	motor(port7) = 127;
	wait10Msec(100);
	motor(port10) = 0;
	motor(port7) = -50;
	motor(port10) = -50; // raise claw
	wait10Msec(23);
	motor(port10) = -13;
	motor(port7) = -13;
	motor(port2) = 127; // move forward
	motor(port3) = 127;
	motor(port4) = 127;
	motor(port1) = 127;
	wait10Msec(195);
	motor(port2) = -80; // move back
	motor(port3) = -80;
	motor(port4) = -127;
	motor(port1) = -127;
	motor(port10) = 30; // slow down claw
	motor(port7) = 30;
	wait10Msec(100);
	motor(port2) = 0; // stop all
	motor(port3) = 0;
	motor(port4) = 0;
	motor(port1) = 0;
	motor(port10) = 0;
	motor(port7) = 0;
	motor(port1) = -100; // turn to cap 1
	motor(port2) = -100;
	motor(port3) = 100;
	motor(port4) = 100;
	wait10Msec(50);
	motor(port2) = 0; // stop wheels
	motor(port3) = 0;
	motor(port4) = 0;
	motor(port1) = 0;
	motor(port2) = 127; // move toward cap 1
	motor(port3) = 127;
	motor(port4) = 127;
	motor(port1) = 127;
	wait10Msec(18);
	motor(port2) = 0; // stop
	motor(port3) = 0;
	motor(port4) = 0;
	motor(port1) = 0;
	motor(port10) = -80; // flip cap
	motor(port7) = -80;
	wait10Msec(28);
	motor(port1) = -100; // turn to cap 2
	motor(port2) = -100;
	motor(port3) = 100;
	motor(port4) = 100;
	motor(port10) = 0; // stop claw
	motor(port7) = 0;
	wait10Msec(40);
	motor(port2) = 127; // move toward cap 2
	motor(port3) = 127;
	motor(port4) = 127;
	motor(port1) = 127;
	wait10Msec(135);
	motor(port1) = 100; // turn to cap
	motor(port2) = 100;
	motor(port3) = -100;
	motor(port4) = -100;
	wait10Msec(55);
	motor(port1) = 0; // turn to hit cap
	motor(port2) = 0;
	motor(port3) = 0;
	motor(port4) = 0;
	motor(port7) = -50;
	motor(port10) = -50;
	motor(port1) = -100; // turn to platform
	motor(port2) = -100;
	motor(port3) = 100;
	motor(port4) = 100;
	wait10Msec(85);
	motor(port7) = -17; //keep claw up
	motor(port10) = -17;
	motor(port1) = 0; // stop motors
	motor(port2) = 0;
	motor(port3) = 0;
	motor(port4) = 0;
	motor(port2) = 127; // move toward platform
	motor(port3) = 127;
	motor(port4) = 127;
	motor(port1) = 127;
	wait10Msec(150);
	motor(port1) = 0; // turn to platform
	motor(port2) = 0;
	motor(port3) = 0;
	motor(port4) = 0;






}
