---
title: Code
---

## Overview
Here is my code for the microcontroller. What my code does is send a clock signal to the shift register, it then reads the bits of the shift register. If it reads that the shift register detected a button pressed, it sends out the unlock signal.

```
#include "mcc_generated_files/system/system.h"

/*
    Main application
*/

int main(void)
{
    uint8_t my_data=0;
    uint8_t value=0;
    uint8_t ii=0;
    SYSTEM_Initialize();
   
    // If using interrupts in PIC18 High/Low Priority Mode you need to enable the Global High and Low Interrupts
    // If using interrupts in PIC Mid-Range Compatibility Mode you need to enable the Global Interrupts
    // Use the following macros to:

    // Enable the Global Interrupts
    //INTERRUPT_GlobalInterruptEnable();

    // Disable the Global Interrupts
    //INTERRUPT_GlobalInterruptDisable();

    my_data = 0b11110000; //data stored as 8bit
    value = 0b11110000;

    while(1)
    {
        //test code that didn't work
        /*IO_RC3_SetHigh();
        //LATCbits.LATC4=(my_data>>ii)&(0b00000001); //shifts data out on RC4
        my_data=(LATCbits.LATC4>>1)&(0b00000001); //maybe reads RC4 and shifts data 1
        ii++;
        if (ii>7) ii=0;
        __delay_ms(500);
        IO_RC3_SetLow();
        __delay_ms(500);
        */
       

        // Load parallel data into shift register
       
       
        IO_RF6_SetHigh();    // return high
        __delay_ms(100);
        IO_RF6_SetLow();     // PL low ? load

        value = 0;
        // Read 8 bits
        for (uint8_t i = 0; i < 8; i++)
        {
            // Pulse clock
           
           

            // Shift in MSB-first
            value <<= 1;
            if (PORTFbits.RF4)
            {
                value |= 1;
            }
            //value &= PORTFbits.RF4;   // read Q7 output
           
           
            IO_RF5_SetHigh();
            __delay_ms(100);

            IO_RF5_SetLow();
            __delay_ms(100);
           
           
        }
        printf("Buttons: 0x%02X\r\n", value);
        if ((value & 0b00000001)!=0)

        {
            IO_RB2_SetHigh();
            __delay_ms(20);
        }
        else
        {
            IO_RB2_SetLow();
            __delay_ms(20);
        }
        __delay_ms(20);
    }    
}
```
