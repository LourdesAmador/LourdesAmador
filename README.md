#include <stdio.h>
#include <windows.h>
#include <stdlib.h>

int cat;
int lvl;
int peli;
int ktant;	//Variables
int anime;
int pais;
int animal;
int series;
int pts=0;
int seg=11;

int main() {
	
	system("Title Trivia Divertida");
	system("Color f");						//Modificacion de menù
	system("cls");
	system("Color 70");
	
	printf("\t\t------------------------------------------------------------\n");
	printf("\t\tIntrucciones: Elija cualquiera categoria que desees jugar!!\n");
	printf("\t\tcon diferentes tipos de niveles..¡RETA A TUS AMIGOS!\n");
	printf("\t\tEl que tenga mas puntos gana!\n");
	printf("\t\t------------------------------------------------------------\n");
	
	
	printf("\n\t\tElija una categoria:\n");
	printf("\n\t\t1) Peliculas\n");
	printf("\t\t2) Cantantes\n");
	printf("\t\t3) Dibujos animados\n");
	printf("\t\t4) Paises\n");		                     //Categorias
	printf("\t\t5) Animales\n");
	printf("\t\t6) Series\n");
	printf("\t\t7) Salir del juego\n");
	scanf("%d",&cat);
	system("cls");
	switch(cat)
	{
	case 1: printf("\n\t\t    Trivia de peliculas\n");
	printf("\n\t\tEscoge el nivel de dificultad\n");
	printf("\n\t\t1) Facil\n");							//Niveles de dificultad
	printf("\t\t2) Intermedio\n");
	printf("\t\t3) Dificil\n");
	scanf("%d",&lvl);
	system("cls");
	switch(lvl)
	{
		
	case 1: printf("\n\t\t¿Cómo se llamaba el búho mascota de Harry Potter?\n");
	printf("\n\t\t1) Errol\n");
	printf("\t\t2) Hedwig\n");
	printf("\t\t3) Crookshanks\n");									//Pregunta Facil
	printf("\t\t4) Scabbers\n");
	printf("\n\t---------------------------------------------------------------------------\n");
	printf("\t\tTienes 10 segundos para contesar, piensa bien tu respuesta!!\n");
	printf("\t---------------------------------------------------------------------------\n");
	while(seg>=0){
		seg--;
		if(seg==-1){
			seg=seg+12;
			break;
			
			
			
		}
		printf("[%ds]\t",seg);
		Sleep(0500);
	}
	printf("\n\t---------------------------------------------------------------------------\n");
	printf("\n\t\t\t\tTu respuesta es: ");
	scanf("%d",&peli);
	switch(peli) 
	{
	case 1: printf("\n\t\t\t\t\t********************\n");
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t* INCORRECTO -2pts *\n");
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t********************\n");
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	case 2:printf("\n\t\t\t\t**********************************\n");
	printf("\t\t\t\t*                                *");
	printf("\n\t\t\t\t* CORRECTO, FELICIDADES !! +3pts *\n");                  // PELICULAS (case NIVEL FACIL)
	printf("\t\t\t\t*                                *");
	printf("\n\t\t\t\t**********************************\n");
	pts=pts+3;
	system("Color 2");
	system("pause");
	main();
	break;
	
	case 3: printf("\n\t\t\t\t\t********************\n");
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t* INCORRECTO -2pts *\n");
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t********************\n");
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	case 4: printf("\n\t\t\t\t\t********************\n");
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t* INCORRECTO -2pts *\n");
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t********************\n");
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	default: printf("\n\t\t\t\t\t*****************\n");
	printf("\t\t\t\t\t*               *");
	printf("\n\t\t\t\t\t*   ERROR 404   *\n");
	printf("\t\t\t\t\t*               *");
	printf("\n\t\t\t\t\t*****************\n");
	system("pause");
	main();
	}
	break;
	case 2: printf("\n\t\t¿Cuál fue el símbolo de Katniss Everdeen en Los juegos del hambre?\n");
	printf("\n\t\t1) Sinsajo \n");
	printf("\t\t2) Aguila\n");
	printf("\t\t3) Cisne \n");																//PELICULA NIVEL INTERMEDIO
	printf("\t\t4) Leona\n");
	printf("\n\t---------------------------------------------------------------------------\n");
	printf("\t\tTienes 10 segundos para contesar, piensa bien tu respuesta!!\n");
	printf("\t---------------------------------------------------------------------------\n");
	while(seg>=0){
		seg--;
		if(seg==-1){
			seg=seg+12;
			break;
			
			
			
		}
		printf("[%ds]\t",seg);
		Sleep(0500);
	}
	printf("\n\t---------------------------------------------------------------------------\n");
	printf("\n\t\t\t\t\tTu respuesta es: ");
	scanf("%d",&peli);
	switch(peli) 
	{
	case 1: printf("\n\t\t\t\t**********************************\n");
	printf("\t\t\t\t*                                *");
	printf("\n\t\t\t\t* CORRECTO, FELICIDADES !! +3pts *\n");                 
	printf("\t\t\t\t*                                *");
	printf("\n\t\t\t\t**********************************\n");
	pts=pts+3;
	system("Color 2");
	system("pause");
	main(); 
	break;
	
	case 2: printf("\n\t\t\t\t\t********************\n");
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t* INCORRECTO -2pts *\n");                             	//CATEGORIA PELICULAS (case nivel intermedio)
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t********************\n");			
	pts=pts-2;
	system("Color 4");
	system("pause");
	main();
	break;
	
	case 3:printf("\n\t\t\t\t\t********************\n");
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t********************\n");	
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	case 4: printf("\n\t\t\t\t\t********************\n");
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t********************\n");	
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	default: printf("\n\t\t\t\t\t*****************\n");
	printf("\t\t\t\t\t*               *");
	printf("\n\t\t\t\t\t*   ERROR 404   *\n");
	printf("\t\t\t\t\t*               *");
	printf("\n\t\t\t\t\t*****************\n");
	system("pause");
	main();
	}
	break;
	
	case 3: printf("\n\t\t¿Cuál fue la primera película animada de largometraje que se lanzó?\n");
	printf("\n\t\t1) Pocahontas  \n");
	printf("\t\t2) Blanca Nieves y los siete enanitos\n");
	printf("\t\t3) Cisne \n");																//PELICULA NIVEL dificil
	printf("\t\t4) Leona\n");
	printf("\n\t\t----------------------------------------------------------------------\n");
	printf("\t\tTienes 10 segundos para contesar, piensa bien tu respuesta!!\n");
	printf("\t\t----------------------------------------------------------------------\n");
	while(seg>=0){
		seg--;
		if(seg==-1){
			seg=seg+12;
			break;
			
			
			
		}
		printf("[%ds]\t",seg);
		Sleep(0500);
	}
	printf("\n\t\t----------------------------------------------------------------------\n");
	printf("\n\t\t\t\t\tTu respuesta es: ");
	scanf("%d",&peli);
	switch(peli) 
	{
	case 1: printf("\n\t\t\t\t\t********************\n");
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t********************\n");
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	case 2: printf("\n\t\t\t\t**********************************\n");
	printf("\t\t\t\t*                                *");
	printf("\n\t\t\t\t* CORRECTO, FELICIDADES !! +3pts *\n");                 
	printf("\t\t\t\t*                                *");
	printf("\n\t\t\t\t**********************************\n");				
	pts=pts+3;
	system("Color 2");
	system("pause");
	main();
	break;
	
	case 3: printf("\n\t\t\t\t\t********************\n");
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t********************\n");
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	case 4: printf("\n\t\t\t\t\t********************\n");
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t********************\n");
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	default:printf("\n\t\t\t\t\t*****************\n");
	printf("\t\t\t\t\t*               *");
	printf("\n\t\t\t\t\t*   ERROR 404   *\n");
	printf("\t\t\t\t\t*               *");
	printf("\n\t\t\t\t\t*****************\n");
	system("pause");
	main();
	}
	break;
	
	default: printf("\n\t\t\t\t*****************\n");
	printf("\t\t\t\t*               *");
	printf("\n\t\t\t\t*   ERROR 404   *\n");
	printf("\t\t\t\t*               *");
	printf("\n\t\t\t\t*****************\n");
	system("Color 74");
	system("pause");
	main();
	}
	break;
	
	
	case 2:printf("\n\t\t     Trivia de Cantantes\n");
	printf("\n\t\tEscoge el nivel de dificultad\n");
	printf("\n\t\t       1) Facil\n");							                           //Niveles de dificultad
	printf("\t\t       2) Intermedio\n");
	printf("\t\t       3) Dificil\n");
	scanf("%d",&lvl);
	system("cls");
	switch(lvl)
		
	{
		
	case 1: printf("\n\t\t¿Que genero musical canta el cantante Bad Bunny?\n");
	printf("\n\t\t1) Pop\n");
	printf("\t\t2) Reggaeton\n");
	printf("\t\t3) Electronica\n");									//Pregunta Facil
	printf("\t\t4) Jazz\n");
	printf("\n\t----------------------------------------------------------------\n");	
	printf("\tTienes 10 segundos para contesar, piensa bien tu respuesta!!\n");
	printf("\t----------------------------------------------------------------\n");
	while(seg>=0){
		seg--;
		if(seg==-1){
			seg=seg+12;
			break;
			
			
			
		}
		printf("[%ds]\t",seg);
		Sleep(0500);
	}
	printf("\n\t----------------------------------------------------------------\n");
	printf("\n\t\t\t\tTu respuesta es: ");
	scanf("%d",&ktant);
	switch(ktant) 
	{
	case 1: printf("\n\t\t\t\t********************\n");
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t********************\n");
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	case 2: printf("\n\t\t\t**********************************\n");
	printf("\t\t\t*                                *");
	printf("\n\t\t\t* CORRECTO, FELICIDADES !! +3pts *\n");                       // CANTANTES (case NIVEL FACIL)
	printf("\t\t\t*                                *");
	printf("\n\t\t\t**********************************\n");				
	pts=pts+3;
	system("Color 2");
	system("pause");
	main();
	break;
	
	case 3: printf("\n\t\t\t\t********************\n");
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t********************\n");
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	case 4: printf("\n\t\t\t\t********************\n");
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t********************\n");
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	default: printf("\n\t\t\t\t*****************\n");                         
	printf("\t\t\t\t*               *");
	printf("\n\t\t\t\t*   ERROR 404   *\n");
	printf("\t\t\t\t*               *");
	printf("\n\t\t\t\t*****************\n");
	system("pause");
	main();
	}
	break;
	
	case 2: printf("\n\t\t¿Como se llama el cantante que canta la cancion: Abrazame muy fuerte?\n");
	printf("\n\t\t\t\t\t1) Marco Antonio Solis\n");
	printf("\t\t\t\t\t2) Luis Perales\n");
	printf("\t\t\t\t\t3) Juan Gabriel\n");									//Pregunta intermedia
	printf("\t\t\t\t\t4) Victorio Vergara\n");
	printf("\t\t----------------------------------------------------------------------\n");
	printf("\t\tTienes 10 segundos para contesar, piensa bien tu respuesta!!\n");
	printf("\t\t----------------------------------------------------------------------\n");
	while(seg>=0){
		seg--;
		if(seg==-1){
			seg=seg+12;
			break;
			
			
			
		}
		printf("[%ds]\t",seg);
		Sleep(0500);
	}
	printf("\n\t\t----------------------------------------------------------------------\n");
	printf("\n\t\t\t\t\tTu respuesta es: ");
	scanf("%d",&ktant);
	switch(ktant) 
	{
	case 1: printf("\n\t\t\t\t\t********************\n");
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t********************\n");
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	case 2:printf("\n\t\t\t\t\t********************\n");
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t********************\n");			
	pts=pts-2;
	system("Color 4");
	system("pause");
	main();
	break;
	
	case 3: printf("\n\t\t\t\t**********************************\n");
	printf("\t\t\t\t*                                *");
	printf("\n\t\t\t\t* CORRECTO, FELICIDADES !! +3pts *\n");                 
	printf("\t\t\t\t*                                *");
	printf("\n\t\t\t\t**********************************\n");	
	pts=pts+3;
	system("Color 2");
	system("pause");
	main(); 
	break;
	
	case 4: printf("\n\t\t\t\t\t********************\n");
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t********************\n");
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	default: printf("\n\t\t\t\t\t*****************\n");
	printf("\t\t\t\t\t*               *");
	printf("\n\t\t\t\t\t*   ERROR 404   *\n");
	printf("\t\t\t\t\t*               *");
	printf("\n\t\t\t\t\t*****************\n");
	system("pause");
	main();
	}
	break;
	
	case 3: printf("\n\t\t¿En que año y, a  que edad, murio el cantante panameño mejor conocido como: Danger man ?\n");
	printf("\n\t\t1) 1999, 38 años\n");
	printf("\t\t2) 2004, 37 años\n");
	printf("\t\t3) 2010, 40 años\n");									          //Pregunta dificil
	printf("\t\t4) 2008, 35 años \n");
	printf("\n\t\t\t----------------------------------------------------------------------\n");
	printf("\t\t\tTienes 10 segundos para contesar, piensa bien tu respuesta!!\n");
	printf("\t\t\t----------------------------------------------------------------------\n");
	while(seg>=0){
		seg--;
		if(seg==-1){
			seg=seg+12;
			break;
		
		
		
		}
	printf("[%ds]\t",seg);
	Sleep(0500);
	}
	printf("\n\t\t\t----------------------------------------------------------------------\n");
	printf("\n\t\t\t\t\tTu respuesta es: ");
	scanf("%d",&ktant);
	switch(ktant) 
	{
	case 1: printf("\n\t\t\t\t\t\t********************\n");
	printf("\t\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t\t********************\n");
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	case 2: printf("\n\t\t\t\t\t\t********************\n");
	printf("\t\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t\t********************\n");		// CANTANTE (case NIVEL DIFICIL)
	pts=pts-2;
	system("Color 4");
	system("pause");
	main();
	break;
	
	case 3: printf("\n\t\t\t\t\t**********************************\n");
	printf("\t\t\t\t\t*                                *");
	printf("\n\t\t\t\t\t* CORRECTO, FELICIDADES !! +3pts *\n");                 
	printf("\t\t\t\t\t*                                *");
	printf("\n\t\t\t\t\t**********************************\n");	
	pts=pts-2;
	system("Color 2");
	system("pause");
	main(); 
	break;
	
	case 4: printf("\n\t\t\t\t\t\t********************\n");
	printf("\t\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t\t********************\n");
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	default: printf("\n\t\t\t\t\t\t*****************\n");
	printf("\t\t\t\t\t\t*               *");
	printf("\n\t\t\t\t\t\t*   ERROR 404   *\n");
	printf("\t\t\t\t\t\t*               *");
	printf("\n\t\t\t\t\t\t*****************\n");
	system("pause");
	main();
	}
	break;
	
	default: printf("\n\t\t\t\t*****************\n");
	printf("\t\t\t\t*               *");
	printf("\n\t\t\t\t*   ERROR 404   *\n");
	printf("\t\t\t\t*               *");
	printf("\n\t\t\t\t*****************\n");
	system("Color 74");
	system("pause");
	main();
	}
	break;
	
	case 3:printf("\n\t\t Trivia de Dibujos Animados\n");
	printf("\n\t\tEscoge el nivel de dificultad\n");
	printf("\n\t\t1) Facil\n");							//Niveles de dificultad
	printf("\t\t2) Intermedio\n");
	printf("\t\t3) Dificil\n");
	scanf("%d",&lvl);
	system("cls");
	switch(lvl)
	{
		
	case 1: printf("\n\t\tCual fue el primer dibujo animado creado por Walt Disney?\n");
	printf("\n\t\t1) Mickey Mouse\n");
	printf("\t\t2) Pluto\n");
	printf("\t\t3) Minnie Mouse\n");									//Pregunta Facil
	printf("\t\t4) El pato Donald\n");
	printf("\n\t\t------------------------------------------------------------\n");
	printf("\t\tTienes 10 segundos para contesar, piensa bien tu respuesta!!\n");
	printf("\t\t------------------------------------------------------------\n");
	while(seg>=0){
		seg--;
		if(seg==-1){
			seg=seg+12;
			break;
			
			
			
		}
		printf("[%ds]\t",seg);
		Sleep(0500);
	}
	printf("\n\t\t------------------------------------------------------------\n");
	printf("\n\t\t\t\tTu respuesta es: ");
	scanf("%d",&anime);
	switch(anime) 
	{
	case 1: printf("\n\t\t\t**********************************\n");
	printf("\t\t\t*                                *");
	printf("\n\t\t\t* CORRECTO, FELICIDADES !! +3pts *\n");                 
	printf("\t\t\t*                                *");
	printf("\n\t\t\t**********************************\n");	
	pts=pts+3;
	system("Color 2");
	system("pause");
	main(); 
	break;
	
	case 2: printf("\n\t\t\t\t********************\n");
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t********************\n");		// DIBUJOS ANIMADO (case NIVEL FACIL)
	pts=pts-2;
	system("Color 4");
	system("pause");
	main();
	break;
	
	case 3: printf("\n\t\t\t\t********************\n");
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t********************\n");	
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	case 4: printf("\n\t\t\t\t********************\n");
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t********************\n");	
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	default: printf("\n\t\t\t\t*****************\n");
	printf("\t\t\t\t*               *");
	printf("\n\t\t\t\t*   ERROR 404   *\n");
	printf("\t\t\t\t*               *");
	printf("\n\t\t\t\t*****************\n");
	system("pause");
	main();
	}
	break;
	
	case 2: printf("\n\t\t\tComo se llamaba la camioneta de Scooby Doo?\n");
	printf("\n\t\t1) Furgoneta Misteriosa\n");
	printf("\t\t2) Equipo Scooby\n");
	printf("\t\t3) Maquina Misteriosa\n");
	printf("\t\t4) Caza Misterios\n");
	printf("\n\t\t------------------------------------------------------------\n");
	printf("\t\tTienes 10 segundos para contesar, piensa bien tu respuesta!!\n");
	printf("\t\t------------------------------------------------------------\n");
	while(seg>=0){
		seg--;
		if(seg==-1){
			seg=seg+12;
			break;
			
			
			
		}
		printf("[%ds]\t",seg);
		Sleep(0500);
	}
	printf("\n\t\t------------------------------------------------------------\n");
	printf("\n\t\t\t\tTu respuesta es: ");
	scanf("%d",&anime);
	switch(anime) 
	{
	case 1: printf("\n\t\t\t\t********************\n");
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t********************\n");	
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	case 2: printf("\n\t\t\t\t********************\n");
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t********************\n");						// DIBULOS ANIMADO (case NIVEL FACIL)
	pts=pts-2;
	system("Color 4");
	system("pause");
	main();
	break;
	
	case 3: printf("\n\t\t\t\t**********************************\n");
	printf("\t\t\t\t*                                *");
	printf("\n\t\t\t\t* CORRECTO, FELICIDADES !! +3pts *\n");                 
	printf("\t\t\t\t*                                *");
	printf("\n\t\t\t\t**********************************\n");	
	pts=pts+3;
	system("Color 2");
	system("pause");
	main(); 
	break;
	
	case 4: printf("\n\t\t\t\t********************\n");
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t********************\n");	
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	default: printf("\n\t\t\t\t\t*****************\n");
	printf("\t\t\t\t\t*               *");
	printf("\n\t\t\t\t\t*   ERROR 404   *\n");
	printf("\t\t\t\t\t*               *");
	printf("\n\t\t\t\t\t*****************\n");
	system("pause");
	main();
	}
	break;
	
	case 3: printf("\n\t\t\t¿Como se llama el carpintero que creo a Pinocho?\n");
	printf("\n\t\t1) Mario\n");
	printf("\t\t2) Adolfo\n");
	printf("\t\t3) krilin\n");									//Pregunta Facil
	printf("\t\t4) Geppetto\n");
	printf("\n\t\t------------------------------------------------------------\n");
	printf("\t\tTienes 10 segundos para contesar, piensa bien tu respuesta!!\n");
	printf("\t\t------------------------------------------------------------\n");
	while(seg>=0){
		seg--;
		if(seg==-1){
			seg=seg+12;
			break;
			
			
			
		}
		printf("[%ds]\t",seg);
		Sleep(0500);
	}
	printf("\n\t\t------------------------------------------------------------\n");
	printf("\n\t\t\t\tTu respuesta es: ");
	scanf("%d",&anime);
	switch(anime) 
	{
	case 1: printf("\n\t\t\t\t\t********************\n");
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t********************\n");	
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	case 2: printf("\n\t\t\t\t\t********************\n");
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t********************\n");			// DIBUJOS ANIMADO (case NIVEL FACIL)
	pts=pts-2;
	system("Color 4");
	system("pause");
	main();
	break;
	
	case 3: printf("\n\t\t\t\t\t********************\n");
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t********************\n");	
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	case 4: printf("\n\t\t\t\t**********************************\n");
	printf("\t\t\t\t*                                *");
	printf("\n\t\t\t\t* CORRECTO, FELICIDADES !! +3pts *\n");                 
	printf("\t\t\t\t*                                *");
	printf("\n\t\t\t\t**********************************\n");
	pts=pts+3;
	system("Color 2");
	system("pause");
	main(); 
	break;
	
	default: printf("\n\t\t\t\t\t*****************\n");
	printf("\t\t\t\t\t*               *");
	printf("\n\t\t\t\t\t*   ERROR 404   *\n");
	printf("\t\t\t\t\t*               *");
	printf("\n\t\t\t\t\t*****************\n");
	system("pause");
	main();
	}
	break;
	
	default: printf("\n\t\t\t\t*****************\n");
	printf("\t\t\t\t*               *");
	printf("\n\t\t\t\t*   ERROR 404   *\n");
	printf("\t\t\t\t*               *");
	printf("\n\t\t\t\t*****************\n");
	system("Color 74");
	system("pause");
	main();
	}
	break;
	
	case 4: printf("\n\t\tTrivia de Paises!\n");
	printf("\n\t\tEscoge el nivel de dificultad\n");
	printf("\n\t\t1) Facil\n");							//Niveles de dificultad
	printf("\t\t2) Intermedio\n");
	printf("\t\t3) Dificil\n");
	scanf("%d",&lvl);
	system("cls");
	switch(lvl)
	{
		
	case 1: printf("\n\t\tEn qué pais puedes visitar Machu Picchu?\n");
	printf("\n\t\t1) Brazil\n");
	printf("\t\t2) Mexico\n");
	printf("\t\t3) Chile\n");									//Pregunta Facil
	printf("\t\t4) Perú\n");
	printf("\n\t\t------------------------------------------------------------\n");
	printf("\t\tTienes 10 segundos para contesar, piensa bien tu respuesta!!\n");
	printf("\t\t------------------------------------------------------------\n");
	while(seg>=0){
		seg--;
		if(seg==-1){
			seg=seg+12;
			break;
			
			
			
		}
		printf("[%ds]\t",seg);
		Sleep(0500);
	}
	printf("\n\t\t------------------------------------------------------------\n");
	printf("\n\t\t\t\tTu respuesta es: ");
	scanf("%d",&pais);
	switch(pais) 
	{
	case 1: printf("\n\t\t\t\t********************\n");
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t********************\n");		
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	case 2: printf("\n\t\t\t\t********************\n");
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t********************\n");		// PAIS (case NIVEL FACIL)
	pts=pts-2;
	system("Color 4");
	system("pause");
	main();
	break;
	
	case 3: printf("\n\t\t\t\t********************\n");
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t********************\n");	
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	case 4: printf("\n\t\t\t**********************************\n");
	printf("\t\t\t*                                *");
	printf("\n\t\t\t* CORRECTO, FELICIDADES !! +3pts *\n");                 
	printf("\t\t\t*                                *");
	printf("\n\t\t\t**********************************\n");	
	pts=pts+3;
	system("Color 2");
	system("pause");
	main(); 
	break;
	
	default: printf("\n\t\t\t\t*****************\n");
	printf("\t\t\t\t*               *");
	printf("\n\t\t\t\t*   ERROR 404   *\n");
	printf("\t\t\t\t*               *");
	printf("\n\t\t\t\t*****************\n");
	system("pause");
	main();
	}
	break;
	
	case 2: printf("\n\t\t\t\tCual es la capital de Canadá?\n");
	printf("\n\t\t\t\t1) toronto\n");
	printf("\t\t\t\t2) ottawa\n");
	printf("\t\t\t\t3) quebec\n");
	printf("\t\t\t\t4) montreal\n");
	printf("\n\t\t------------------------------------------------------------\n");
	printf("\t\tTienes 10 segundos para contesar, piensa bien tu respuesta!!\n");
	printf("\t\t------------------------------------------------------------\n");
	while(seg>=0){
		seg--;
		if(seg==-1){
			seg=seg+12;
			break;
			
			
			
		}
		printf("[%ds]\t",seg);
		Sleep(0500);
	}
	printf("\n\t\t------------------------------------------------------------\n");
	printf("\n\t\t\t\tTu respuesta es: ");
	scanf("%d",&pais);
	switch(pais) 
	{
	case 1: printf("\n\t\t\t\t********************\n");
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t********************\n");	
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	case 2: printf("\n\t\t\t\t**********************************\n");
	printf("\t\t\t\t*                                *");
	printf("\n\t\t\t\t* CORRECTO, FELICIDADES !! +3pts *\n");                 
	printf("\t\t\t\t*                                *");
	printf("\n\t\t\t\t**********************************\n");	
	pts=pts+3;
	system("Color 2");
	system("pause");
	main();
	break;
	
	case 3: printf("\n\t\t\t\t********************\n");
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t********************\n");	
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	case 4: printf("\n\t\t\t\t********************\n");
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t********************\n");	
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	default: printf("\n\t\t\t\t\t*****************\n");
	printf("\t\t\t\t\t*               *");
	printf("\n\t\t\t\t\t*   ERROR 404   *\n");
	printf("\t\t\t\t\t*               *");
	printf("\n\t\t\t\t\t*****************\n");
	system("pause");
	main();
	}
	break;
	
	case 3: printf("\n\t¿Que pais cuenta con el glaciar más joven y con la colonia de murciélago más grande del mundo?\n");
	printf("\n\t1) Canadá\n");
	printf("\t2) Túnez\n");
	printf("\t3) Islandia\n");									//Pregunta Dificil
	printf("\t4) Estados Unidos\n");
	printf("\n\t\t------------------------------------------------------------\n");
	printf("\t\tTienes 10 segundos para contesar, piensa bien tu respuesta!!\n");
	printf("\t\t------------------------------------------------------------\n");
	while(seg>=0){
		seg--;
		if(seg==-1){
			seg=seg+12;
			break;
			
			
			
		}
		printf("[%ds]\t",seg);
		Sleep(0500);
	}
	printf("\n\t\t------------------------------------------------------------\n");
	printf("\n\t\t\t\tTu respuesta es: ");
	scanf("%d",&pais);
	switch(pais) 
	{
	case 1: printf("\n\t\t\t\t\t********************\n");
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t********************\n");	
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	case 2: printf("\n\t\t\t\t\t********************\n");
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t********************\n");			// PELICULAS (case NIVEL FACIL)
	pts=pts-2;
	system("Color 4");
	system("pause");
	main();
	break;
	
	case 3: printf("\n\t\t\t\t\t********************\n");
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t********************\n");	
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	case 4: printf("\n\t\t\t\t**********************************\n");
	printf("\t\t\t\t*                                *");
	printf("\n\t\t\t\t* CORRECTO, FELICIDADES !! +3pts *\n");                 
	printf("\t\t\t\t*                                *");
	printf("\n\t\t\t\t**********************************\n");
	pts=pts+3;
	system("Color 2");
	system("pause");
	main(); 
	break;
	
	default: printf("\n\t\t\t\t\t*****************\n");
	printf("\t\t\t\t\t*               *");
	printf("\n\t\t\t\t\t*   ERROR 404   *\n");
	printf("\t\t\t\t\t*               *");
	printf("\n\t\t\t\t\t*****************\n");
	system("pause");
	main();
	}
	break;
	
	default: printf("\n\t\t\t\t*****************\n");
	printf("\t\t\t\t*               *");
	printf("\n\t\t\t\t*   ERROR 404   *\n");
	printf("\t\t\t\t*               *");
	printf("\n\t\t\t\t*****************\n");
	system("Color 74");
	system("pause");
	main();
	}
	break;
	
	case 5: printf("\n\t\t      Trivia de animales\n");
	printf("\n\t\tEscoge el nivel de dificultad\n");
	printf("\n\t\t1) Facil\n");							//Niveles de dificultad
	printf("\t\t2) Intermedio\n");
	printf("\t\t3) Dificil\n");
	scanf("%d",&lvl);
	system("cls");
	switch(lvl)
	{
		
	case 1: printf("\n\t\t¿Cuál es el animal terrestre que pone el huevo mas grande?\n");
	printf("\n\t\t1) Gallina\n");
	printf("\t\t2) Camello\n");
	printf("\t\t3) Avestruz\n");									//Pregunta Facil
	printf("\t\t4) Cisne\n");
	printf("\n\t\t------------------------------------------------------------\n");
	printf("\t\tTienes 10 segundos para contesar, piensa bien tu respuesta!!\n");
	printf("\t\t------------------------------------------------------------\n");
	while(seg>=0){
		seg--;
		if(seg==-1){
			seg=seg+12;
			break;
			
			
			
		}
		printf("[%ds]\t",seg);
		Sleep(0500);
	}
	printf("\n\t\t------------------------------------------------------------\n");
	printf("\n\t\t\t\tTu respuesta es: ");
	scanf("%d",&animal);
	switch(animal) 
	{
	case 1: printf("\n\t\t\t\t********************\n");
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t********************\n");		
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	case 2: printf("\n\t\t\t\t********************\n");
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t********************\n");		// ANIMAL (case NIVEL FACIL)
	pts=pts-2;
	system("Color 4");
	system("pause");
	main();
	break;
	
	case 3: printf("\n\t\t\t**********************************\n");
	printf("\t\t\t*                                *");
	printf("\n\t\t\t* CORRECTO, FELICIDADES !! +3pts *\n");                 
	printf("\t\t\t*                                *");
	printf("\n\t\t\t**********************************\n");	
	pts=pts+3;
	system("Color 2");
	system("pause");
	main(); 
	break;
	
	case 4: printf("\n\t\t\t\t********************\n");
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t********************\n");		// ANIMAL (case NIVEL FACIL)
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	default: printf("\n\t\t\t\t*****************\n");
	printf("\t\t\t\t*               *");
	printf("\n\t\t\t\t*   ERROR 404   *\n");
	printf("\t\t\t\t*               *");
	printf("\n\t\t\t\t*****************\n");
	system("pause");
	main();
	}
	break;
	
	case 2: printf("\n\t\t\t¿Qué raza de perro es la más grande en tamaño?\n");
	printf("\n\t\t\t1) Mastín inglés\n");
	printf("\t\t\t2) Taza de té chihuahua\n");
	printf("\t\t\t3) Pastor alemán\n");
	printf("\t\t\t4) Golden retriever\n");
	printf("\n\t\t------------------------------------------------------------\n");
	printf("\t\tTienes 10 segundos para contesar, piensa bien tu respuesta!!\n");
	printf("\t\t------------------------------------------------------------\n");
	while(seg>=0){
		seg--;
		if(seg==-1){
			seg=seg+12;
			break;
			
			
			
		}
		printf("[%ds]\t",seg);
		Sleep(0500);
	}
	printf("\n\t\t------------------------------------------------------------\n");
	printf("\n\t\t\t\tTu respuesta es: ");
	scanf("%d",&animal);
	switch(animal) 
	{
	case 1: printf("\n\t\t\t\t**********************************\n");
	printf("\t\t\t\t*                                *");
	printf("\n\t\t\t\t* CORRECTO, FELICIDADES !! +3pts *\n");                 
	printf("\t\t\t\t*                                *");
	printf("\n\t\t\t\t**********************************\n");	
	pts=pts+3;
	system("Color 2");
	system("pause");
	main(); 
	break;
	
	case 2: printf("\n\t\t\t\t********************\n");
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t********************\n");	
	pts=pts-2;
	system("Color 4");
	system("pause");
	main();
	break;
	
	case 3: printf("\n\t\t\t\t********************\n");
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t********************\n");	
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	case 4: printf("\n\t\t\t\t********************\n");
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t********************\n");	
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	default: printf("\n\t\t\t\t\t*****************\n");
	printf("\t\t\t\t\t*               *");
	printf("\n\t\t\t\t\t*   ERROR 404   *\n");
	printf("\t\t\t\t\t*               *");
	printf("\n\t\t\t\t\t*****************\n");
	system("pause");
	main();
	}
	break;
	
	case 3: printf("\n\t\t\t¿Qué porcentaje de los animales terrestres ha sido descubierto?\n");
	printf("\n\t\t\t1) 25\n");
	printf("\t\t\t2) 14\n");
	printf("\t\t\t3) 55\n");									//Pregunta Dificil
	printf("\t\t\t4) 87\n");
	printf("\n\t\t\t------------------------------------------------------------\n");
	printf("\t\t\tTienes 10 segundos para contesar, piensa bien tu respuesta!!\n");
	printf("\t\t\t------------------------------------------------------------\n");
	while(seg>=0){
		seg--;
		if(seg==-1){
			seg=seg+12;
			break;
			
			
			
		}
		printf("[%ds]\t",seg);
		Sleep(0500);
	}
	printf("\n\t\t\t------------------------------------------------------------\n");
	printf("\n\t\t\t\tTu respuesta es: ");
	scanf("%d",&animal);
	switch(animal) 
	{
	case 1: printf("\n\t\t\t\t\t********************\n");
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t********************\n");	
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	case 2: printf("\n\t\t\t\t**********************************\n");
	printf("\t\t\t\t*                                *");
	printf("\n\t\t\t\t* CORRECTO, FELICIDADES !! +3pts *\n");                 
	printf("\t\t\t\t*                                *");
	printf("\n\t\t\t\t**********************************\n");
	pts=pts+3;
	system("Color 2");
	system("pause");
	main();
	break;
	
	case 3: printf("\n\t\t\t\t\t********************\n");
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t********************\n");	
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	case 4: printf("\n\t\t\t\t\t********************\n");
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t********************\n");	
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	default: printf("\n\t\t\t\t\t*****************\n");
	printf("\t\t\t\t\t*               *");
	printf("\n\t\t\t\t\t*   ERROR 404   *\n");
	printf("\t\t\t\t\t*               *");
	printf("\n\t\t\t\t\t*****************\n");
	system("pause");
	main();
	}
	break;
	default: printf("\n\t\t\t\t*****************\n");
	printf("\t\t\t\t*               *");
	printf("\n\t\t\t\t*   ERROR 404   *\n");
	printf("\t\t\t\t*               *");
	printf("\n\t\t\t\t*****************\n");
	system("Color 74");
	system("pause");
	main();
	}
	break;
	
	case 6: printf("\n\t\t\tTrivia de Series\n");
	printf("\n\t\tEscoge el nivel de dificultad\n");
	printf("\n\t\t1) Facil\n");							//Niveles de dificultad
	printf("\t\t2) Intermedio\n");
	printf("\t\t3) Dificil\n");
	scanf("%d",&lvl);
	system("cls");
	switch(lvl)
	{
		
	case 1: printf("\n\t\tCual es la serie más vista en la actualidad?\n");
	printf("\n\t\t1) Bridgerton\n");
	printf("\t\t2) El Juego Del Calamar\n");
	printf("\t\t3) Dahmer\n");									//Pregunta Facil
	printf("\t\t4) Lucifer\n");
	printf("\n\t\t------------------------------------------------------------\n");
	printf("\t\tTienes 10 segundos para contesar, piensa bien tu respuesta!!\n");
	printf("\t\t------------------------------------------------------------\n");
	while(seg>=0){
		seg--;
		if(seg==-1){
			seg=seg+12;
			break;
			
			
			
		}
		printf("[%ds]\t",seg);
		Sleep(0500);
	}
	printf("\n\t\t------------------------------------------------------------\n");
	printf("\n\t\t\t\tTu respuesta es: ");
	scanf("%d",&peli);
	switch(peli) 
	{
	case 1: printf("\n\t\t\t\t********************\n");
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t********************\n");
	
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	case 2: printf("\n\t\t\t**********************************\n");
	printf("\t\t\t*                                *");
	printf("\n\t\t\t* CORRECTO, FELICIDADES !! +3pts *\n");                 
	printf("\t\t\t*                                *");
	printf("\n\t\t\t**********************************\n");		// SERIES (case NIVEL FACIL)
	pts=pts+3;
	system("Color 2");
	system("pause");
	main();
	break;
	
	case 3: printf("\n\t\t\t\t********************\n");
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t********************\n");	
	
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	case 4: printf("\n\t\t\t\t********************\n");
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t*                  *");
	printf("\n\t\t\t\t********************\n");	
	
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	default: printf("\n\t\t\t\t*****************\n");
	printf("\t\t\t\t*               *");
	printf("\n\t\t\t\t*   ERROR 404   *\n");
	printf("\t\t\t\t*               *");
	printf("\n\t\t\t\t*****************\n");
	system("pause");
	main();
	}
	break;
	case 2: printf("\n\t\t\tEn la serie Breakind Bad,¿Cómo se llamaba el hijo de Walter White?\n");
	printf("\n\t\t\t1) Luis\n");
	printf("\t\t\t2) Saul Jr.\n");
	printf("\t\t\t3) Kevin Jr.\n");                                                            //Pregunta Intermedio
	printf("\t\t\t4) Walter Jr.\n");
	printf("\n\t\t\t------------------------------------------------------------\n");
	printf("\t\t\tTienes 10 segundos para contesar, piensa bien tu respuesta!!\n");
	printf("\t\t\t------------------------------------------------------------\n");
	while(seg>=0){
		seg--;
		if(seg==-1){
			seg=seg+12;
			break;
			
			
			
		}
		printf("[%ds]\t",seg);
		Sleep(0500);
	}
	printf("\n\t\t\t------------------------------------------------------------\n");
	printf("\n\t\t\t\t\tTu respuesta es: ");
	scanf("%d",&peli);
	switch(peli) 
	{
	case 1: printf("\n\t\t\t\t\t********************\n");
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t********************\n");	
	
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	case 2: printf("\n\t\t\t\t\t********************\n");
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t********************\n");			// SERIES (case NIVEL INTERMEDIO)
	pts=pts-2;
	system("Color 4");
	system("pause");
	main();
	break;
	
	case 3: printf("\n\t\t\t\t\t********************\n");
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t********************\n");	
	
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	case 4: printf("\n\t\t\t\t\t**********************************\n");
	printf("\t\t\t\t\t*                                *");
	printf("\n\t\t\t\t\t* CORRECTO, FELICIDADES !! +3pts *\n");                 
	printf("\t\t\t\t\t*                                *");
	printf("\n\t\t\t\t\t**********************************\n");	
	
	pts=pts+3;
	system("Color 2");
	system("pause");
	main(); 
	break;
	
	default: printf("\n\t\t\t\t\t\t*****************\n");
	printf("\t\t\t\t\t\t*               *");
	printf("\n\t\t\t\t\t\t*   ERROR 404   *\n");
	printf("\t\t\t\t\t\t*               *");
	printf("\n\t\t\t\t\t\t*****************\n");
	system("pause");
	main();
	}
	break;
	case 3: printf("\n\t\t\tEn la serie Game Of Thrones ¿Quién es el papá biologico de Jon Snow?\n");
	printf("\n\t\t\t1) Tyrion Lannister\n");
	printf("\t\t\t2) Ned Stark\n");
	printf("\t\t\t3) Rhaegar Targaryen\n");									         //Pregunta Dificil
	printf("\t\t\t4) Ramsay Snow\n");
	printf("\n\t\t\t------------------------------------------------------------\n");
	printf("\t\t\tTienes 10 segundos para contesar, piensa bien tu respuesta!!\n");
	printf("\t\t\t------------------------------------------------------------\n");
	while(seg>=0){
		seg--;
		if(seg==-1){
			seg=seg+12;
			break;
			
			
			
		}
		printf("[%ds]\t",seg);
		Sleep(0500);
	}
	printf("\n\t\t\t------------------------------------------------------------\n");
	printf("\n\t\t\t\t\tTu respuesta es: ");
	scanf("%d",&peli);
	switch(peli) 
	{
	case 1:printf("\n\t\t\t\t\t\t********************\n");
	printf("\t\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t\t********************\n");	
	
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	case 2: printf("\n\t\t\t\t\t\t********************\n");
	printf("\t\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t\t********************\n");		              // SERIES (case NIVEL DIFICIL)
	pts=pts-2;
	system("Color 4");
	system("pause");
	main();
	break;
	
	case 3: printf("\n\t\t\t\t\t**********************************\n");
	printf("\t\t\t\t\t*                                *");
	printf("\n\t\t\t\t\t* CORRECTO, FELICIDADES !! +3pts *\n");                 
	printf("\t\t\t\t\t*                                *");
	printf("\n\t\t\t\t\t**********************************\n");		
	
	pts=pts+3;
	system("Color 2");
	system("pause");
	main(); 
	break;
	
	case 4: printf("\n\t\t\t\t\t\t********************\n");
	printf("\t\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t\t* INCORRECTO -2pts *\n");                             	
	printf("\t\t\t\t\t\t*                  *");
	printf("\n\t\t\t\t\t\t********************\n");	
	
	pts=pts-2;
	system("Color 4");
	system("pause");
	main(); 
	break;
	
	default: printf("\n\t\t\t\t\t\t*****************\n");
	printf("\t\t\t\t\t\t*               *");
	printf("\n\t\t\t\t\t\t*   ERROR 404   *\n");
	printf("\t\t\t\t\t\t*               *");
	printf("\n\t\t\t\t\t\t*****************\n");
	system("pause");
	main();
	}
	break;
	
	default: printf("\n\t\t\t\t\t\t*****************\n");
	printf("\t\t\t\t\t\t*               *");
	printf("\n\t\t\t\t\t\t*   ERROR 404   *\n");
	printf("\t\t\t\t\t\t*               *");
	printf("\n\t\t\t\t\t\t*****************\n");
	system("pause");
	main();
	}
	break;
	case 7:  printf("\n\t\t*********************************************************************\n");
	printf("\t\t*                                                                   *");
	printf("\n\t\t*      Acumulastes una cantidad de %d pts. Gracias por jugar . . .   *\n",pts);
	printf("\t\t*                                                                   *");	
	printf("\n\t\t*                       Hasta la proxima!!!                         *\n");
	printf("\t\t*                                                                   *");
	printf("\n\t\t*********************************************************************\n");
	break;
	
	default: printf("\n\t\t\t\t\t\t*****************\n");
	printf("\t\t\t\t\t\t*               *");
	printf("\n\t\t\t\t\t\t*   ERROR 404   *\n");
	printf("\t\t\t\t\t\t*               *");
	printf("\n\t\t\t\t\t\t*****************\n");
	system("pause");
	main();
	
	break;
	return 0;

	}
}
