##Calculadora de peso corporal IMC

personas = int(input("Personas: "))

while personas > 0:
     
     n = input("Ingrese su nombre : ")
     ap= input("Ingrese su apellido paterno : ")
     am= input("Ingrese su apellido materno : ")
     e = int(input("Digite su edad : "))
     a = float(input("Ingrese altura en metro :"))
     est = a
     m = float(input("Masa en kilogramo :"))

     IMC = m / est**2

##VALIDACION SI LA PERSONA ES MENOR O MAYOR DE EDAD 

     if(e < 18):
       print("Usted es menor de edad")
     else:
        print("Usted es mayor de edad")
        
     print("IMC: " + str(IMC) )

 ##RANGO DE EDADES Y VALIDACION 

     if IMC >= 0 and IMC <= 15.99 :
       print ("Delgadez severa")
     elif IMC >= 16.00 and IMC <=16.99 :
       print ("Delgadez moderada")
     elif IMC >= 17.00 and IMC <=18.49 :
       print ("Delgadez leve")
     elif IMC >= 18.50 and IMC <=24.99 :
       print ("Normal")
     elif IMC >= 25.00 and IMC <= 29.99:
       print ("Sobrepeso")
     elif IMC >= 30.00 and IMC <= 34.99:
       print ("obesidad leve")
     elif IMC >= 35.00 and IMC <= 39.00:
       print ("obesidad media")
     elif IMC >= 40.00:
       print ("obesidad morbida")

personas = personas -1
