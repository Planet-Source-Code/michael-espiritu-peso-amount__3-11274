<div align="center">

## peso amount


</div>

### Description


 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[MICHAEL ESPIRITU](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/michael-espiritu.md)
**Level**          |Beginner
**User Rating**    |5.0 (10 globes from 2 users)
**Compatibility**  |C, C\+\+ \(general\), Microsoft Visual C\+\+
**Category**       |[Coding Standards](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/coding-standards__3-32.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/michael-espiritu-peso-amount__3-11274/archive/master.zip)





### Source Code

```
#include<iostream.h>
int main()
{
	float number;
	int passnumber;
	float origvalue;
	float passcent;
	int Thousand,Hundred1,Hundred2,Hundred3,Fifty,Twenty,Ten;
	int Five,One,TwentyFivecent,Tencent,Fivecent;
	cout<< "Enter Peso Amount: "<<" ";
  cin>>number;
	origvalue=number;
	passnumber=number;
  //100 thousand;
	passnumber=passnumber/1000;
	if (passnumber==0)
	{
		passnumber=number;
		Thousand=0;
	}
	else
	{
		Thousand=passnumber;
		number=number-(Thousand*1000);
		origvalue=number;
		passnumber=number;
	}
	//500 hundred
		passnumber=passnumber/500;
	if (passnumber==0)
	{
		passnumber=number;
		Hundred1=0;
	}
	else
	{
	  Hundred1=passnumber;
		number=number-(Hundred1*500);
		origvalue=number;
		passnumber=number;
	}
	//200 hundred
  passnumber=passnumber/200;
	if(passnumber==0)
	{
		passnumber=number;
	  Hundred2=0;
	}
	else
	{
		Hundred2=passnumber;
		number=number-(Hundred2*200);
		origvalue=number;
		passnumber=number;
	}
	//100 hundred
  passnumber=passnumber/100;
	if(passnumber==0)
	{
		passnumber=number;
		Hundred3=0;
	}
	else
	{
	  Hundred3=passnumber;
		number=number-(Hundred3*100);
		origvalue=number;
		passnumber=number;
	}
	//50 pesos
  passnumber=passnumber/50;
	if(passnumber==0)
	{
		passnumber=number;
		Fifty=0;
	}
	else
	{
		Fifty=passnumber;
		number=number-(Fifty*50);
		origvalue=number;
	}
	//Twenty pesos
  passnumber=passnumber/20;
	if(passnumber==0)
	{
		passnumber=number;
	  Twenty=0;
	}
	else
	{
	  Twenty=passnumber;
		number=number-(Twenty*20);
		origvalue=number;
		passnumber=number;
	}
	//TEN PESOS
  passnumber=passnumber/10;
	if(passnumber==0)
	{
		passnumber=number;
		Ten=0;
	}
	else
	{
	  Ten=passnumber;
		number=number-(Ten*10);
		origvalue=number;
		passnumber=number;
	}
	//FIVE PESOS
  passnumber=passnumber/5;
	if(passnumber==0)
	{
		passnumber=number;
	  Five=0;
	}
	else
	{
		Five=passnumber;
		number=number-(Five*5);
		origvalue=number;
		passnumber=number;
	}
	//ONE PESOS
  passnumber=passnumber/1;
	if(passnumber==0)
	{
	  One=0;
		passcent=origvalue;
	}
	else
	{
		One=passnumber;
		origvalue=origvalue-(One*1);
	}
	//25 cents
  passcent=passcent/.25;
	if(passcent<.25)
	{
		passcent=origvalue;
	  TwentyFivecent=0;
	}
	else
	{
		TwentyFivecent=passcent;
		origvalue=origvalue-(TwentyFivecent*.25);
		passcent=origvalue;
	}
	//10 cents
  passcent=passcent/.10;
	if(passcent<.10)
  {
		passcent=origvalue;
	  Tencent=0;
	}
	else
	{
	  Tencent=passcent;
		origvalue=origvalue-(Tencent*.10);
		passcent=origvalue;
	}
	//5 cents
		passcent=passcent/.05;
	if(passcent<.05)
	{
		passcent=origvalue;
		Fivecent=0;
	}
	else
	{
	  Fivecent=passcent;
	}
	cout<<"\nPeso Number of 1 thousand: "<<Thousand<<"\n";
  cout<<"\nPeso Number of 5 hundred: "<<Hundred1<<"\n";
	cout<<"\nPeso Number of 2 Hundred: "<<Hundred2<<"\n";
	cout<<"\nPeso Number of 1 Hundred: "<<Hundred3<<"\n";
	cout<<"\nPeso Number of 50 Peso: "<<Fifty<<"\n";
	cout<<"\nPeso Number of 20 Peso: "<<Twenty<<"\n";
	cout<<"\nPeso Number of 10 Peso: "<<Ten<<"\n";
	cout<<"\nPeso Number of 5 Peso: "<<Five<<"\n";
	cout<<"\nPeso Number of 1 Peso: "<<One<<"\n";
	cout<<"\nPeso Number of 25 cent: "<<TwentyFivecent<<"\n";
	cout<<"\nPeso Number of 10 cent: "<<Tencent<<"\n";
	cout<<"\nPeso Number of 5 cent: "<<Fivecent<<"\n\n\n";
	return 0;
	}
```

