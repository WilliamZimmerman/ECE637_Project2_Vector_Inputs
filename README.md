## Importing
To add this symbol to your project simply add the vec_stim folder into your project directory. 
For example:
If your project is ~/ECE637/Project2 
All you need to do is cp -r /Path/to/git/directory Path/to/project/directory 

## Instantiation 
A symbol has already been created. All you need to do is add an instance of it to your test bench like so. (Remember to use bus notation)

<img width="558" height="190" alt="Screenshot 2026-11-13 at 4 03 45 PM" src="https://github.com/user-attachments/assets/3b66e86a-7144-49d8-bf43-f103f2c34e33" />

## Operation
The symbol will change input Vector A from 0-9ns, Vector B from 10-19ns and then Vector C from 20-29ns like shown in the graph below. This is mainly to help with
testing the correctness of the adder.

<img width="1062" height="567" alt="Screenshot 2026-11-13 at 4 32 48 PM" src="https://github.com/user-attachments/assets/9d16c66a-aa26-4890-b0ba-592a8cd6fd08" />

Should you want to test a under 1ghz conditions, use the vec_stim_GHZ symbol. 

## Checking
To check your values, paste the code in the CIW_CHECK files into the ciw window (The window that you launch library manager from when you first start cadence)


## IMPORTANT NOTE ON TIMING!
AT this moment, you can't measure tadd for all 3 vectors using this because certain transitions for AIN don't happen. 
