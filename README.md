# Cronometro-en-Python
Cronometro Orientado a Objetos en Python

import time

class cronometro:

    marca = "" 
    
    velocidad = 0
    
    def mostrarDatos(self):
    
        print("Marca :",self.marca)
        print("velocidad :",self.velocidad)
        
    def encender(self):
    
        print("El cronometro se encendio")
        
    def apagar(self):
    
        print("El cronometro se a apagado")

    def acelerar(self,velocidad):
    
        for i in range(0,velocidad,1):
            print("El cronometro esta acelerado a una velocidad de ",i, " seg ")
            time.sleep(0.01)
            
        print("El cronometro llego a la velocidad de ",velocidad," seg ")

    def frenar(self,velocidad,frenado):
    
        for i in range(velocidad,frenado,-2):
            print("El cronometro esta frenando,esta marcamdo " ,i,"km/h")
            time.sleep(0.01)
            
        print("El cronometro a bajado la velocidad hasta ",frenado,"km/h")

cron = cronometro

cron.marca = "Sony"

cron.mostrarDatos()

cron.encender()

cron.acelerar(120)

cron.frenar(120,60) 

cron.apagar()



