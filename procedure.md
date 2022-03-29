### Make use of simulator available under Simulator tab, to understand the operation of Timer and Counter function blocks

The procedure for using simulator is as follows:
### Part 1: Understanding the operation of On Delay Timer and Off Delay Timer
1. From the panel at left side, click on IO tab and click on DI.
2. Use left click and drag the DI block at center location in the workspace.
3. Take TON block available under TIMERS tab by clicking on it. Put this block next to DI block.
4. Next to TON block, take DO block to observe On delay timer operation. Follow the procedure mentioned in step 1.
5. Connect the output of DI block to input of TON block and output of TON block to input of DO block.
6. Right click on Timer block and configure it. Enter required delay (preset value by which the output is to be delayed) in terms of milli seconds. e.g. For a delay of 1 second, require preset value is 1000.
7. When configuration is done, click on Compile tab to activate the Run tab. Run the logic now.
8. To start the Timer operation, Change the DI value. You need to toggle the input value by using right click.
9. Observe the accumulated timer value. When it becomes equal to preset value, the timer output and the Do block output is set to 1.
10. Change the DI value to 0 again and observe the output status.
11. To observe the operation of off delay timer, first click on Stop tab. Go to compile mode. You need to replace the TON block with TOFF Timer block.
12. Right click on TON block. Select and delete the block. Form panel, select TOFF block available under Timer tab.
13. Repeat steps 5 to 9.
The output of Off delay timer is set to 1 without any delay, when DI is set to 1. But when DI is changed back to 0, the timer operation starts, delay is provided and the output is changed to 0 or Off state.

### Part 2: Understanding the operation of Up and Down counter
1. To configure the counter circuit, first reload the page by clicking Clear tab.
2. Refer step 1 mentioned in part 1 to drag DI block.
3. From the panel, click on COUNTER; click on UP, to select Up Counter block. Put this block next to DI block.
4. Next to UPCTR block, take DO block to observe Up Counter operation. Follow the procedure mentioned in step 2.
5. Connect the output of DI block to input of UPCTR block and output of UPCTR block to input of DO block.
6. Rght bclick on the UPCTR block to configure. Enter required count (preset) value after which the output is to be set.
7. When configuration is done, click on complile tab to activate Run tab.
8. To understand the counter operation, Change the DI value by toggling. You need to use right click for this.
9. Observe the accumulated count value.
10. Change the DI value to 0 again and observe the output status.
11. Repeat step 8 to 10 till the accumulated value becomes equal to preset.
When accumulated value becomes equal to preset, the counter output and the Do block output is set to 1.
12. Do not forget to drag and drop Reset block available under Counter tab to restart the counter.
13. To observe the operation of down counter, go back to compile mode by pressing Stop tab. Now replace the UPCTR block with DWCTR counter block.
14. Right click on UPCTR block. Select delete and delete the block. From the panel, select DOWN block available under Counter tab.
15. Repeat steps 5 to 11.
In case of down counter, the preset value is loaded in accumulator when the simulator is taken to Run mode. On every transition of input from 0 to 1, accumulated value is decremented by 1. When accumulated value becomes equal to 0 the output of counter is set to 1.