# sistemas-de-ec-lineales-
%Funcion sistema de ecuaciones lineales para hallar las intensidades.
%Parte A
r1=input('Ingrese el valor de R1 : ');%Resistencias en KiloOhmios
r2=input('Ingrese el valor de R2: ');
r3=input('Ingrese el valor de R3: ');
r4=input('Ingrese el valor de R4: ');
r5=input('Ingrese el valor de R5: ');
v=input('Ingrese el valor de V: ');%Voltaje en Vatios

%sistema de 6 ecuaciones con 6 incognitas
A=[0 -r2  0 -r4 0 0;r1 -r2 r3 0 0 0;0 0 -r3 -r4 r5 0;1 1 0 -1 0 0;1 0 -1 0 -1 0;-1 -1 0 0 0 1]%Coeficientes de las ecuaciones dadas
B=[-v;0;0;0;0;0]%Resultados de cada ecuacion
Ab=[A B];
R=rref(Ab)
%Se imprimen los valores de cada intensidad obtenida en la matriz R
in1=R(1,7)
in2=R(2,7)
in3=R(3,7)
in4=R(4,7)
in5=R(5,7)
in6=R(6,7)
%Parte B

r1=1000;%Resistencias en KiloOhmios
r2=5000;
r3=2000;
r4=10000;
r5=5000;
v=  100;%Voltaje en Vatios
%sistema de 6 ecuaciones con 6 incognitas
A=[0 -r2  0 -r4 0 0;r1 -r2 r3 0 0 0;0 0 -r3 -r4 r5 0;1 1 0 -1 0 0;1 0 -1 0 -1 0;-1 -1 0 0 0 1]%Coeficientes de las ecuaciones dadas
B=[-v;0;0;0;0;0]%Resultados de cada ecuacion
Ab=[A B];
R=rref(Ab)
%Se imprimen los valores de cada intensidad obtenida en la matriz R
in1=R(1,7)
in2=R(2,7)
in3=R(3,7)
in4=R(4,7)
in5=R(5,7)
in6=R(6,7)
