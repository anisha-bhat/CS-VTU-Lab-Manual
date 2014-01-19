## Aim: To check given input is a palindrome or not, comment with suitable message.

## Theory
> what is a palindrome?
    any word/number read same both ends , is said to be a palindrome.
ex. MALAYALAM, 10101.

 the main 

  
## Algorithm:
1. Start.
2. take input, initialise respectively.
3. assign given input to a variable, reverse and assign to another variable .
4. compare above two variables, 
       on true display succesful message
   otherwise suitable message.
     
5. Stop.


## Code: 
   
    #include<stdio.h> 
    #include<stdlib.h>

  int main(void)   
{
   int iNum, iRev=0, iTemp,iRem;
    printf("\n**************************************************************************");
    printf("\n*\tPROGRAM TO CHECK WHETHER AN INTEGER IS A PALINDROME OR NOT\t *\n");
    printf("**************************************************************************");

    printf("\nEnter a number\n");
    scanf("%d",&iNum);

      iTemp = iNum;

       while(iNum!=0)
       {
                iRem = iNum % 10;  //taking remainder digit ex. let iNUM=101
                                    //  iREm= 101 % 10 =1;
                iRev = iRev * 10 + iRem;  // to reverse iNUM, ex.  iRev= o*10+1= 1.

                iNum = iNum/10;  //for next digit place  iNum= 101/10= 10.1 (since int only 10)
        }
        printf("\nReverse is %d",iRev);

        if(iRev == iTemp)
                printf("\nNumber %d is a palindrome\n",iTemp);
        else
                printf("\nNumber %d is not a palindrome\n",iTemp);

        return 0; 

}
## Output:
*Commands for execution:-*

* Open terminal for compilation .
* Change directory to the file location in the terminal.
* compilation command:Run gcc *filename.c* in terminal.
* for display output:If no errors, run ./a.out

*Screenshots:-*

![ScreenShot of Output](9.png)
