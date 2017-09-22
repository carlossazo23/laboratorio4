# laboratorio4
### ESTos son los metodos con que se sacan las operaiones normales 
int sumar(int a, int b){
    return a+b;
}
int restar(int a, int b){
    return a-b;
}
int mult(int a, int b){
    return a*b;
}
int dividir(int a, int b){
    return a/b;
}
### Estos son los metodos con los que se sacan las operaciones con punteros 
int sumapunteros(int a, int b, int* resultadoPS){
    *resultadoPS = a+b;
}
int restapunteros(int a, int b, int* resultadoPR){
    *resultadoPR = a-b;
}
int multpunteros(int a, int b, int* resultadoPM){
    *resultadoPM = a*b;
}
int divpunteros(int a, int b, int* resultadoPD){
    *resultadoPD = a/b;
} 

### Main
int main()
{    
### Se asignan los valores a las operaciones normales 
    int resultadoS = sumar(5, 7);    
    int resultadoR = restar(5, 7);
    int resultadoM = mult(5, 7);
    int resultadoD = dividir(5, 7);
### Se asignan los valores a las operaciones con punteros     
    int resultadoPS = 29;
    sumapunteros(8, 5, &resultadoPS);
    int resultadoPR = 23;
    restapunteros(8, 5, &resultadoPR);
    int resultadoPM = 4;
    multpunteros(8, 5, &resultadoPM);
    int resultadoPD = 22;
    divpunteros(8, 5, &resultadoPD);
  ###Se muestra en pantalla las operaciones normales 
   std::cout << "Hola master de progra avanzada :)" << std::endl;
  std::cout << "SUMA "<< resultadoS << std::endl;
  std::cout << "RESTA "<< resultadoR << std::endl;
  std::cout << "MULTIPLICACION "<< resultadoM << std::endl;
  std::cout << "DIVISION "<< resultadoD << std::endl; 
    ### se muestra en pantalla las operaciones con punteros 
   std::cout << "ES EL PUNTERO SUMA " << resultadoPS << std::endl;  
   std::cout << "ES EL PUNTERO RESTA " << resultadoPR << std::endl;  
   std::cout << "ES EL PUNTERO MULTI¨PLICACION " << resultadoPM << std::endl;  
   std::cout << "ES EL PUNTERO DIVISION " << resultadoPD << std::endl;  
  return 0;
}


