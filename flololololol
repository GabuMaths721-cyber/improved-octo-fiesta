import random
import string


def generar_contrasenia(longitud=12):
    # Definimos los caracteres que queremos usar
    caracteres = string.ascii_letters + string.digits + string.punctuation

    # Mezclamos los caracteres de forma aleatoria según la longitud deseada
    contrasenia = "".join(random.choice(caracteres) for _ in range(longitud))

    return contrasenia


# --- Bloque principal de ejecución ---
if __name__ == "__main__":
    print("--- GENERADOR DE CONTRASENIAS SEGURAS ---")

    try:
        largo = int(
            input("Introduce la longitud de la contraseña (mínimo 8): ")
        )
        if largo < 8:
            print("Por seguridad, se recomienda un mínimo de 8 caracteres.")
            largo = 8
    except ValueError:
        print("Entrada no válida. Usando longitud por defecto (12).")
        largo = 12

    password_lista = generar_contrasenia(largo)
    print(f"\nTu nueva contraseña es: {password_lista}")
