#menu
print("Bienvenido, Aquí puedes calcular tu IMC")
print("1. Sistema Internacional")
print("2. Sistema Inglés")
print("3. Salir")
preferencia = input("")
#if con preferencia en tipos de medidas
if preferencia == "1" or preferencia.lower() == "sistema internacional":
    print("¡Bien! Será en Sistema Internacional. Ahora responde las siguientes preguntas:")
    peso = float(input("¿Cuánto pesas (Kilogramos)? "))
    estatura = float(input("¿Cuánto mides (Metros)? "))
    operacion = estatura * estatura
    imc = peso / operacion
    print("Tu IMC es:", imc)
    
elif preferencia == "2" or preferencia.lower() == "sistema inglés":
    print("¡Bien! Será en Sistema Inglés. Ahora responde las siguientes preguntas:")
    peso = float(input("¿Cuánto pesas? (Libras) "))
    estatura = float(input("¿Cuánto mides? (Pulgadas) "))
    operacion = estatura * estatura
    imc = peso / operacion
    final = imc * 703
    print("Tu IMC es:", final)
    
elif preferencia == "3" or preferencia.lower() == "salir":
    print("¡Hasta luego!")

else:
    print("Ese número no existe.")
