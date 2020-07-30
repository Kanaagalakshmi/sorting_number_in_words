//input 10
//output
/*
ZER0
ONE
TWO
THREE
FOUR
FIVE
SIX
SEVEN
EIGHT
NINE
TEN*/
#include<stdio.h>
#include<malloc.h>
#include<stdlib.h>
#include<string.h>
const char * numtowords(int num,char []);
int main ()
{
  int num;
  char * *wordlist=0;
  char numinwords[10];
  printf ("ENTER THE NUM:");
  scanf ("%d",&num);
 wordlist=(char**)malloc((num+1)*sizeof(char *));
  
  for(int i=750000000;i<=num;i++,printf("\n")){
     printf("%s",numtowords(i,numinwords));
     /*numtowords(i,numinwords);
      wordlist[i]=(char*)malloc((sizeof(numinwords))*sizeof(char));
      strcpy(wordlist[i],numinwords);
      printf("%s",wordlist[i]);
    */
      
  }
  
}

const char * numtowords(int num,char numinword[]){
     char word_tens[10][10]={"","","TWENTY ","THIRTY ","FORTY ","FIFTY ","SIXTY ","SEVENTY ","EIGHTY ","NINETY "};
  char word_tenth[10][11]={"","ELEVEN ","TWELVE ","THIRTEEN ","FOURTEEN ","FIFTEEN ","SIXTEEN ","SEVENTEEN ","EIGHTEEN ","NINETEEN "};
 char word_ones[11][7]={"","ONE ","TWO ","THREE ","FOUR ","FIVE ","SIX ","SEVEN ","EIGHT ","NINE ","TEN "
  }    ;
  char powerwords[4][10]={"HUNDRED ","THOUSAND ","LAKH ","CRORE "};
      int thnum,num1,lknum,cnum=0;
      char numsinword[100]="";
      //1-99
      if (num<=10){
        strcpy(numinword,word_ones[num]);
      }
      else if (num>10&&num<=19){
         strcpy(numinword,word_tenth[num%10]);
        }
      else if(num>19&&num<100){
          if(num%10==0){
              strcpy(numinword,word_tens[num/10]);
          }
          else{
              strcat(numsinword,word_tens[num/10]);
              strcat(numsinword,word_ones[num%10]);
              strcpy(numinword,numsinword);
              
          }
      }
      //end 1-99
      //100-999
      else if(num>=100&&num<1000){
          int h=num/100;
          strcat(numsinword,word_ones[h]);
          strcat(numsinword,powerwords[0]);
          if((num%100)!=0)strcat(numsinword,"AND ");
          int num1=num%100;
          if (num1<=10){
        strcat(numsinword,word_ones[num1]);
        strcpy(numinword,numsinword);
              
      }
      else if (num1>10&&num1<=19){
         strcat(numsinword,word_tenth[num1%10]);
         strcpy(numinword,numsinword);
              
        }
      else if(num1>19&&num1<100){
          if(num1%10==0){
              strcat(numsinword,word_tens[num1/10]);
              strcpy(numinword,numsinword);
          }
          else{
              strcat(numsinword,word_tens[num1/10]);
              strcat(numsinword,word_ones[num1%10]);
              strcpy(numinword,numsinword);
              
          }
      }
      
      
      }
      //end 100-999
      //********************************************************//
      //********************************************************//
      
      //THOUSAND STARTS
      else if(num>=1000&&num<99999){
          thnum=num/1000;
          if (thnum<=10){
        strcat(numsinword,word_ones[thnum]);
        strcpy(numinword,numsinword);
              
      }
      else if (thnum>10&&thnum<=19){
         strcat(numsinword,word_tenth[thnum%10]);
         strcpy(numinword,numsinword);
              
        }
      else if(thnum>19&&thnum<100){
          if(thnum%10==0){
              strcat(numsinword,word_tens[thnum/10]);
              strcpy(numinword,numsinword);
          }
          else{
              strcat(numsinword,word_tens[thnum/10]);
              strcat(numsinword,word_ones[thnum%10]);
              strcpy(numinword,numsinword);
              
          }
          
      }
     char th[10]="";
     // strcpy(numsinword,"");
  strcat(th,powerwords[1]);
  strcat(numsinword,th);
  if((num%1000)<=100&&(num%1000!=0)||(num%100)==0&&(num%1000)!=0)strcat(numsinword,"AND ");
     // strcpy(numinword,numsinword);
      num=num%1000;
      //1-99
      if (num<=10){
          
       // strcat(numsinword,th);
          
        strcat(numsinword,word_ones[num]);
        strcpy(numinword,numsinword);
      }
      else if (num>10&&num<=19){
         // strcat(numsinword,th);
       
         strcat(numsinword,word_tenth[num%10]);
         strcpy(numinword,numsinword);
        }
      else if(num>19&&num<100){
          if(num%10==0){
           //    strcat(numsinword,th);
       
              strcat(numsinword,word_tens[num/10]);
              strcpy(numinword,numsinword);
          }
          else{
        //strcat(numsinword,th);
       
              strcat(numsinword,word_tens[num/10]);
              strcat(numsinword,word_ones[num%10]);
              strcpy(numinword,numsinword);
              
          }
      }
     
      //end 1-99
      //N THOUSAND AND N HUNDREDS
      //100-999
      else if(num>=100&&num<1000){
          int h=num/100;
          strcat(numsinword,word_ones[h]);
          strcat(numsinword,powerwords[0]);
          if((num%100)!=0)strcat(numsinword,"AND ");
          int num1=num%100;
          if (num1<=10){
        strcat(numsinword,word_ones[num1]);
        strcpy(numinword,numsinword);
              
      }
      else if (num1>10&&num1<=19){
         strcat(numsinword,word_tenth[num1%10]);
         strcpy(numinword,numsinword);
              
        }
      else if(num1>19&&num1<100){
          if(num1%10==0){
              strcat(numsinword,word_tens[num1/10]);
              strcpy(numinword,numsinword);
          }
          else{
              strcat(numsinword,word_tens[num1/10]);
              strcat(numsinword,word_ones[num1%10]);
              strcpy(numinword,numsinword);
              
          }
      }
      
      
      }
      //end 100-999
      
      
          
      }
      //THOUSAND ENDS
      //*****************************************************************
      //*****************************************************************
      /* &&&&&&&&&&&&&&&&& */
      
      //LAKHS
      else if(num>=100000&&num<9999999){
          lknum=num/100000;
          if (lknum<=10){
        strcat(numsinword,word_ones[lknum]);
        strcpy(numinword,numsinword);
              
      }
      else if (lknum>10&&lknum<=19){
         strcat(numsinword,word_tenth[lknum%10]);
         strcpy(numinword,numsinword);
              
        }
      else if(lknum>19&&lknum<100){
          if(lknum%10==0){
              strcat(numsinword,word_tens[lknum/10]);
              strcpy(numinword,numsinword);
          }
          else{
              strcat(numsinword,word_tens[lknum/10]);
              strcat(numsinword,word_ones[lknum%10]);
              strcpy(numinword,numsinword);
              
          }
          
      }
     char lk[10]="";
     // strcpy(numsinword,"");
  strcat(lk,powerwords[2]);
  strcat(numsinword,lk);
  //if((num%1000)<=100&&(num%1000!=0)||(num%100)==0&&(num%1000)!=0||(num%100000)<=1000&&(num%100000)!=0)strcat(numsinword,"AND ");
    if(num%1000==0&&num%100==0&&num%100000<1000&&num%100000!=0)strcat(numsinword,"AND ");
    if(num%100000!=0&&num%1000<100)strcat(numsinword,"AND ");
     // strcpy(numinword,numsinword);
      num=num%100000;
      //1-99
      if (num<=10){
          
       // strcat(numsinword,th);
          
        strcat(numsinword,word_ones[num]);
        strcpy(numinword,numsinword);
      }
      else if (num>10&&num<=19){
         // strcat(numsinword,th);
       
         strcat(numsinword,word_tenth[num%10]);
         strcpy(numinword,numsinword);
        }
      else if(num>19&&num<100){
          if(num%10==0){
           //    strcat(numsinword,th);
       
              strcat(numsinword,word_tens[num/10]);
              strcpy(numinword,numsinword);
          }
          else{
        //strcat(numsinword,th);
       
              strcat(numsinword,word_tens[num/10]);
              strcat(numsinword,word_ones[num%10]);
              strcpy(numinword,numsinword);
              
          }
      }
      else if(num>=1000&&num<99999){
          thnum=num/1000;
          if (thnum<=10){
        strcat(numsinword,word_ones[thnum]);
        strcpy(numinword,numsinword);
              
      }
      else if (thnum>10&&thnum<=19){
         strcat(numsinword,word_tenth[thnum%10]);
         strcpy(numinword,numsinword);
              
        }
      else if(thnum>19&&thnum<100){
          if(thnum%10==0){
              strcat(numsinword,word_tens[thnum/10]);
              strcpy(numinword,numsinword);
          }
          else{
              strcat(numsinword,word_tens[thnum/10]);
              strcat(numsinword,word_ones[thnum%10]);
              strcpy(numinword,numsinword);
              
          }
          
      }
     char th[10]="";
     // strcpy(numsinword,"");
  strcat(th,powerwords[1]);
  strcat(numsinword,th);
  if((num%1000)<=100&&(num%1000!=0)||(num%100)==0&&(num%1000)!=0)strcat(numsinword,"AND ");
     // strcpy(numinword,numsinword);
      num=num%1000;
      //1-99
      if (num<=10){
          
       // strcat(numsinword,th);
          
        strcat(numsinword,word_ones[num]);
        strcpy(numinword,numsinword);
      }
      else if (num>10&&num<=19){
         // strcat(numsinword,th);
       
         strcat(numsinword,word_tenth[num%10]);
         strcpy(numinword,numsinword);
        }
      else if(num>19&&num<100){
          if(num%10==0){
           //    strcat(numsinword,th);
       
              strcat(numsinword,word_tens[num/10]);
              strcpy(numinword,numsinword);
          }
          else{
        //strcat(numsinword,th);
       
              strcat(numsinword,word_tens[num/10]);
              strcat(numsinword,word_ones[num%10]);
              strcpy(numinword,numsinword);
              
          }
      }
     
      //end 1-99
      //N THOUSAND AND N HUNDREDS
      //100-999
      else if(num>=100&&num<1000){
          int h=num/100;
          strcat(numsinword,word_ones[h]);
          strcat(numsinword,powerwords[0]);
          if((num%100)!=0)strcat(numsinword,"AND ");
          int num1=num%100;
          if (num1<=10){
        strcat(numsinword,word_ones[num1]);
        strcpy(numinword,numsinword);
              
      }
      else if (num1>10&&num1<=19){
         strcat(numsinword,word_tenth[num1%10]);
         strcpy(numinword,numsinword);
              
        }
      else if(num1>19&&num1<100){
          if(num1%10==0){
              strcat(numsinword,word_tens[num1/10]);
              strcpy(numinword,numsinword);
          }
          else{
              strcat(numsinword,word_tens[num1/10]);
              strcat(numsinword,word_ones[num1%10]);
              strcpy(numinword,numsinword);
              
          }
      }
      
      
      }
      //end 100-999
      
      
          
      }
      
     
      //end 1-99
      //END LAKHS
      
      /* &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&& */
      
      /* ################################### */
      
      //CRORE STARTS
      
      }
      else if(num>=10000000&&num<999999999){
          cnum=num/10000000;
          if (cnum<=10){
        strcat(numsinword,word_ones[cnum]);
        strcpy(numinword,numsinword);
       // printf("%s",numinword);
              
      }
      else if (cnum>10&&cnum<=19){
         strcat(numsinword,word_tenth[cnum%10]);
         strcpy(numinword,numsinword);
              
        }
      else if(cnum>19&&cnum<100){
          if(cnum%10==0){
              strcat(numsinword,word_tens[cnum/10]);
              strcpy(numinword,numsinword);
          }
          else{
              strcat(numsinword,word_tens[cnum/10]);
              strcat(numsinword,word_ones[cnum%10]);
              strcpy(numinword,numsinword);
              
          }
          
      }
     char cr[10]="";
     // strcpy(numsinword,"");
  strcat(cr,powerwords[3]);
  
  strcat(numsinword,cr);
  // printf("%s",numsinword);
       
  //if((num%1000)<=100&&(num%1000!=0)||(num%100)==0&&(num%1000)!=0||(num%100000)<=1000&&(num%100000)!=0)strcat(numsinword,"AND ");
    if(num%10000000!=0&&num%100000==0&&num%1000==0||num%10000000<1000&&num%10000000!=0)strcat(numsinword,"AND ");
     //if(num%100==0)strcat(numsinword,"AND ");
     // strcpy(numinword,numsinword);
      num=num%10000000;
     
     //NO OF CRORES ET THE REMAINING LAKHS THOUSANDS AND HUNDREDS 
     // else 
      if(num>=100000&&num<9999999){
          lknum=num/100000;
          if (lknum<=10){
        strcat(numsinword,word_ones[lknum]);
        strcpy(numinword,numsinword);
        //printf("%s",numinword);
              
      }
      else if (lknum>10&&lknum<=19){
         strcat(numsinword,word_tenth[lknum%10]);
         strcpy(numinword,numsinword);
        //printf("%s",numinword);
              
        }
      else if(lknum>19&&lknum<100){
          if(lknum%10==0){
              strcat(numsinword,word_tens[lknum/10]);
              strcpy(numinword,numsinword);
       // printf("%s",numinword);
       
          }
          else{
              strcat(numsinword,word_tens[lknum/10]);
              strcat(numsinword,word_ones[lknum%10]);
              strcpy(numinword,numsinword);
       // printf("%s",numinword);
              
          }
          
      }
     char lk[10]="";
     // strcpy(numsinword,"");
  strcat(lk,powerwords[2]);
  strcat(numsinword,lk);
  // printf("%s",numinword);
       
  //if((num%1000)<=100&&(num%1000!=0)||(num%100)==0&&(num%1000)!=0||(num%100000)<=1000&&(num%100000)!=0)strcat(numsinword,"AND ");
    if(num%1000==0&&num%100==0&&num%100000<1000&&num%100000!=0)strcat(numsinword,"AND ");
    if(num%100000!=0&&num%1000<100)strcat(numsinword,"AND ");
   }  // strcpy(numinword,numsinword);
      if(num>=100000&&num<=9999999){
      num=num%100000;
      //1-99
      if (num<=10){
          
       // strcat(numsinword,th);
          
        strcat(numsinword,word_ones[num]);
        strcpy(numinword,numsinword);
      // printf("%s",numinword);
       
          
      }
      else if (num>10&&num<=19){
         // strcat(numsinword,th);
       
         strcat(numsinword,word_tenth[num%10]);
         strcpy(numinword,numsinword);
        }
      else if(num>19&&num<100){
          if(num%10==0){
           //    strcat(numsinword,th);
       
              strcat(numsinword,word_tens[num/10]);
              strcpy(numinword,numsinword);
          }
          else{
        //strcat(numsinword,th);
       
              strcat(numsinword,word_tens[num/10]);
              strcat(numsinword,word_ones[num%10]);
              strcpy(numinword,numsinword);
              
          }
      }}//}
      else if(num>=1000&&num<99999){
          thnum=num/1000;
          if (thnum<=10){
        strcat(numsinword,word_ones[thnum]);
        strcpy(numinword,numsinword);
              
      }
      else if (thnum>10&&thnum<=19){
         strcat(numsinword,word_tenth[thnum%10]);
         strcpy(numinword,numsinword);
              
        }
      else if(thnum>19&&thnum<100){
          if(thnum%10==0){
              strcat(numsinword,word_tens[thnum/10]);
              strcpy(numinword,numsinword);
          }
          else{
              strcat(numsinword,word_tens[thnum/10]);
              strcat(numsinword,word_ones[thnum%10]);
              strcpy(numinword,numsinword);
              
          }
          
      }
     char th[10]="";
     // strcpy(numsinword,"");
  strcat(th,powerwords[1]);
  strcat(numsinword,th);
  if((num%1000)<=100&&(num%1000!=0)||(num%100)==0&&(num%1000)!=0)strcat(numsinword,"AND ");
  }   // strcpy(numinword,numsinword);
      num=num%1000;
      //1-99
      if (num<=10){
          
       // strcat(numsinword,th);
          
        strcat(numsinword,word_ones[num]);
        strcpy(numinword,numsinword);
      }
      else if (num>10&&num<=19){
         // strcat(numsinword,th);
       
         strcat(numsinword,word_tenth[num%10]);
         strcpy(numinword,numsinword);
        }
      else if(num>19&&num<100){
          if(num%10==0){
           //    strcat(numsinword,th);
       
              strcat(numsinword,word_tens[num/10]);
              strcpy(numinword,numsinword);
          }
          else{
        //strcat(numsinword,th);
       
              strcat(numsinword,word_tens[num/10]);
              strcat(numsinword,word_ones[num%10]);
              strcpy(numinword,numsinword);
              
          }
      }
     
      //end 1-99
      //N THOUSAND AND N HUNDREDS
      //100-999
      else if(num>=100&&num<1000){
          int h=num/100;
          strcat(numsinword,word_ones[h]);
          strcat(numsinword,powerwords[0]);
          if((num%100)!=0)strcat(numsinword,"AND ");
          int num1=num%100;
          if (num1<=10){
        strcat(numsinword,word_ones[num1]);
        strcpy(numinword,numsinword);
              
      }
      else if (num1>10&&num1<=19){
         strcat(numsinword,word_tenth[num1%10]);
         strcpy(numinword,numsinword);
              
        }
      else if(num1>19&&num1<100){
          if(num1%10==0){
              strcat(numsinword,word_tens[num1/10]);
              strcpy(numinword,numsinword);
          }
          else{
              strcat(numsinword,word_tens[num1/10]);
              strcat(numsinword,word_ones[num1%10]);
              strcpy(numinword,numsinword);
              
          }
      }
      
      
      }
      //end 100-999
      
      
          
      
      
     
      //end 1-99
      
      //CRORE ENDS
      
      /* ################################### */
     // printf("&&&%s&&&&\n",numinword);
      return numinword;

          
      }}







