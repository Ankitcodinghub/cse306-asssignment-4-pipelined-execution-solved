# cse306-asssignment-4-pipelined-execution-solved
**TO GET THIS SOLUTION VISIT:** [CSE306 Asssignment 4-Pipelined Execution Solved](https://www.ankitcodinghub.com/product/cse306-asssignment-4-pipelined-execution-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;96790&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSE306 Asssignment 4-Pipelined Execution Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
Pipelined Execution

In this assignment, you have to design an 8-bit processor that supports pipelined datapath for a subset of MIPS instruction set. In this design, each instruction is divided into five stages: instruction fetch (IF), instruction decode (ID), execution and address calculation (EX), data memory access (MEM), and write back (WB). The length of the clock cycle equals the maxi- mum time to execute any single stage. Therefore, each instruction takes up to five clock cycles to be executed. The main components of the processor are as follows: instruction memory, data memory, register file, ALU, control unit, five pipeline registers, and a forwarding unit. Ad- ditional components such as comparators, adders, mux etc can be added as required by your design.

1 DESIGN SPECIFICATION

<ul>
<li>Addressbusanddatabusaremultiplexed.</li>
<li>Eachofdataandaddresshasasizeof8-bits.</li>
<li>An8-bitALUwillberequired,hencethename8-bitMIPS.</li>
<li>Theregisterfilemustincludethefollowingtemporaryregisters:
$zero, $t0, $t1, $t2, $t3, $t4

Each temporary register has a size of 8-bits. The assembly code that will be provided to simulate your design will use only the above mentioned registers.

• Pipeline registers: There registers will be used between any two stages of the instruc- tion. A pipeline register can be a single register or a collection of registers. There is no restriction on the size of the pipeline registers.
</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
<ul>
<li>The control unit should be micro-programmed. The control signals associated with the operations should be stored in a special memory (you can use a separate ROM for this purpose) units as Control Words.</li>
<li>Theforwardingunitisusedtodetectdatahazardandgeneratecontrolbitstoallowdata forwarding.</li>
<li>Allclocksrequiredinthecircuitmustbeprovidedfromasingleclocksource.
2 INSTRUCTION SET DESCRIPTION

In this assignment, we will consider only the four R-type instructions. You may choose any opcode value for the given instructions.
</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
Instruction ID

</div>
<div class="column">
Category

</div>
<div class="column">
Type Instruction

Shft Amnt 4-bits

</div>
</div>
<div class="layoutArea">
<div class="column">
R add R sub R and

R-type Opcode Src Reg 1 Src Reg 2 Dst Reg 4-bits 4-bits 4-bits 4-bits

3 MEMORY CONSIDERATIONS

Two separate memory units should be used for instruction and data.

</div>
</div>
<div class="layoutArea">
<div class="column">
A

B

C

D Logic R or

</div>
</div>
<div class="layoutArea">
<div class="column">
Arithmetic Arithmetic Logic

</div>
</div>
<div class="layoutArea">
<div class="column">
The format of an R- type instruction is given below.

</div>
</div>
<div class="layoutArea">
<div class="column">
<ul>
<li>InstructionMemoryisaccessedthroughan8-bitaddresswhichisstoredinan8-bitPro- gram Counter (PC) register. Each access to the instruction memory provides 20-bit (in- struction) data.</li>
<li>DataMemoryisalsoaccessedthroughan8-bitaddress.
4 HANDLING HAZARDS

In this assignment, we will only consider data hazards can occur. More precisely, we consider data hazards that can be resolved by forwarding.

In particular you have to detect and resolve the following hazards by using forwarding tech- niques.

<ul>
<li>EXHazard:occurswhenthedependentinstructisintheEXstageandthepriorinstruc- tion is in MEM stage.</li>
<li>MEM Hazard: when the dependent instruction is in the EX stage and the prior instruc- tion is in WB stage.</li>
<li>Double Data Hazard: occurs when the dependent instruction is in EX stage and it de- pends on two prior instructions, one of which, is in MEM stage, and the other is in WB stage.</li>
</ul>
</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
• In the following example, inst 1 creates EX hazard for inst 2 and MEM hazard for inst 3. Moreover, inst 2 and inst 3 both create double data hazard for inst 4.

</div>
</div>
<div class="layoutArea">
<div class="column">
inst 1: inst 2: inst 3: inst 4:

</div>
<div class="column">
add $t1, $t2, $t3 sub $t4, $t1, $t2 or $t4, $t1, $t3 add $t4, $t4, $t3

</div>
</div>
<div class="layoutArea">
<div class="column">
• Notethatnostalloperationisrequiredforyourimplementation.

5 SIMULATION AND EVALUATION

To simulate your design, an assembly code consisting only 3-5 instructions will be used. Progress of your implementation will be evaluated based on the handling of the following scenarios.

<ul>
<li>Pipelined datapath only (60% marks): No data dependency exists among the instruc- tions.</li>
<li>Pipelined datapath and Ex Hazard only (60% + 15% marks): An instruction is depen- dent on its preceding instruction.</li>
<li>Pipelined datapath and MEM Hazard only (60% + 15% marks): An instruction is de- pendent on its 2nd preceding instruction.</li>
<li>Pipelined datapath, EX Hazard, and MEM Hazard (60% + 15% + 15% marks): An in- struction i is dependent on its preceding instruction. Another instruction j ̸= i is de- pendent on its 2nd preceding instruction.</li>
<li>Pipelineddatapath,EXHazard,MEMHazard,andDoubleDataHazard(60%+15%+ 15% + 10% marks): An instruction is dependent both on its preceding and 2nd preceding instructions.
6 REPORT CONTENT

Contents of the report are recommended as follows:
</li>
</ul>
<ul>
<li>Section 1: Introduction</li>
<li>Section2:CompleteBlockdiagramofpipelineddatapath.</li>
<li>Section3:Blockdiagramsandsizeofpipelineregisters</li>
<li>Section4:Mechanismandblockdiagramofforwardingunit</li>
<li>Section 5: Discussion</li>
</ul>
</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="layoutArea">
<div class="column">
&nbsp;

</div>
</div>
</div>
