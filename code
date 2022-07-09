#include <iostream>
using namespace std;

int main()
{
	unsigned int x,z=0,idade,sexo,sintoma,dias,ajuda,teste,resultado,sexM=0,idadeM=0,SinAjud=0,asint=0;
	float mediaDia,porcentIdoso,mediaIdade,somaDias=0,idoso=0,idosoAjuda=0;
	
	
	
	cout<<"Quantos participantes?:"<<endl;
	cin>>x;
	while (z<x){
	cout<<"Qual � a idade?:"<<endl;
	cin>>idade;
	cout<<"Sexo da pessoa (1- Masculino 2- Feminino)"<<endl;
	cin>>sexo;
	cout<<"Teve sintomas do CoronaVirus? (1- Sim 2-N�o)"<<endl;
	cin>>sintoma;
	if (sintoma == 1){
	   cout<<"por quantos dias teve sintoma?:"<<endl;
	   cin>>dias;
	   somaDias = somaDias + dias;
	   cout<<"precisou procurar ajuda m�dica?: (1- Emerg�ncia, 2- Consulta M�dica, 3- N�o)"<<endl;
	   cin>>ajuda;
	}   
	cout<<"Realizou algum teste de covid?: (1- Sim 2- N�o)"<<endl;
	cin>>teste;
	if (teste==1){
		cout<<"qual foi o resultado? (1- Positivo 2- Negativo)"<<endl;
		cin>>resultado;
	}
	    
	if (sintoma==1 && ajuda==3){  //sintomas sem ajuda >
		SinAjud = SinAjud +1;
	}    
    if (idade > 65)  { //sobre maior de 65 
		idoso = idoso +1;
	}
	if (idade > 65 && ajuda==1){ //sobre maior de 65 que buscaaram ajuda
		idosoAjuda = idosoAjuda +1;
	}
	if (sintoma == 2 && resultado ==1){ //assintomaticos
		asint = asint +1;
	}
	if (sexo == 2 && sintoma ==1 && resultado ==2){ //mulheres com sintoma e negativo
		idadeM = idadeM + idade;
		sexM = sexM + 1;}
	
	z++;
}
    mediaDia = somaDias/x;
    if (idoso>=1 && idoso >=1){
    porcentIdoso = idosoAjuda/idoso;}
    if (idadeM>=1 && sexM >=1){
    mediaIdade = idadeM/sexM;}
    
    cout<<"x--------x--------x---------x---------x--------x--------x-------x-------x"<<endl;
	cout<<"Quantos sem sintomas que o exame deu positivo? resp = "<<asint<<endl;
	cout<<"Percentual de 65+ que procuraram emergencia -> "<<porcentIdoso<<" (1 equivale a 100%)"<<endl;
	cout<<"Media de duracao dos sintomas de covid -> "<<mediaDia<<endl;
	cout<<"Quantos tiveram sintomas e nao procuraram ajuda? resp = "<<SinAjud<<endl;
	cout<<"Media de idade das mulheres com sintoma e resultado negativo -> "<<mediaIdade<<endl;
	
	return 0;
}
