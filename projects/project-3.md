---
layout: project
type: project
image: images/legLiteMain.png
title: LegLite Simulated CPU
permalink: projects/legLite
# All dates must be YYYY-MM-DD format!
date: 2018-12-15
labels:
  - SystemVerilog
  - Vivado
  - CPU Architecture
  - Digital Logic
summary: A basic simulated CPU developed for EE361L final project.
---

For this project, the goal was to simulate a computer CPU capable of processing instructions formatted in a simplified LEGv8 instruction set. To do this, we used SystemVerilog to design various components such as an ALU, registers, and multiplexers and organize them in such a way that allows instructions to be interpreted.

Of the team, I was responsible for organizing and linking together the coded components. This would be like wiring the components together on a physical board.

Below is an example of a written module: the 4-1 MUX. This would take in 4 inputs and determine which one to push to the output.

<hr>
<pre>
// 4:1 Multiplexer
module MUX4(
	result,  // 16 bit output
	indata0, // Input 0
	indata1, // Input 1
	indata2, // Input 2
	indata3, // Input 3
	select   // 2-bit select input
	);	

output [15:0] result;
input [15:0] indata0, indata1, indata2, indata3;
input [1:0] select;

reg [15:0] result;

always @(indata0 or indata1 or indata2 or indata3 or select)
	case(select)
	0: result = indata0;
	1: result = indata1;
	2: result = indata2;
	3: result = indata3;
	endcase

endmodule
</pre>
<hr>
<hr>

<pre>
You open your eyes, and you are greeted by an unfamiliar ceiling.
Startled, you get to your feet and quickly scan your surroundings. It's
dark except for the stream of light coming from a crack on the only boarded
window in the room. You try to peek through the crack, but you cannot see
anything. You wonder where you are and who could have possibly brought you here.

<--------------------help------------------------>
Enter quit or one of the following commands -
Weld light look walk pickup inventory help h ?
<------------------------------------------------>

look
The room is a picture of decay with only a faded number identifying it as room-4. The bed you were
 lying on is stained with what looks like dried blood. Could it be your blood? No - it is not. The
 only way out of the room aside from the door to the corridor is a window that is boarded shut. It
 looks like it has been like that for decades. There is a door going west from here. You see a candle
 on the floor. You see a match on the floor.

pickup candle
- you are now carrying the candle -

pickup match
- you are now carrying the match -

light match candle

The candle is now lit. It illuminates everything in the room.

walk west
The corridor is lit with the candle. It is so long that you cannot see to the end. You notice that
 there are words written on the wall. There is a door going east from here. There is a way going north
 from here. There is a door going south from here.
</pre>

<hr>
