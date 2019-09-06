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
