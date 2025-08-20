class Persona:
    def __init__(self, nombre, edad, genero):
        self.nombre = nombre
        self.edad = edad
        self.genero = genero

    def saludar(self):
        print(f"Hola, mi nombre es {self.nombre}")

    def cumplir_años(self):
        self.edad += 1
        print(f"{self.nombre} ha cumplido {self.edad} años.")

    def __str__(self):
        return f"Persona [nombre={self.nombre}, edad={self.edad}, genero={self.genero}]"


persona = Persona("Juan", 22, "Masculino")
persona.saludar()
persona.cumplir_años()
print(persona)
