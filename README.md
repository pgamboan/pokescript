# Pokescript

Este es un script en Bash que consulta la API de PokéAPI para obtener información de un Pokémon específico. 
El script muestra en pantalla los datos del Pokémon y los guarda en un archivo CSV para futuras referencias.

## 📌 Requisitos

Para ejecutar este script, necesitas tener instalado:
- **Ubuntu (o cualquier distribución de Linux con Bash)**
- **curl** (para hacer peticiones HTTP)
- **jq** (para procesar JSON)

Si no tienes `curl` o `jq`, instálalos con:
```bash
sudo apt update
sudo apt install curl jq -y
```

## 🚀 Cómo Ejecutarlo

1. Clona este repositorio en tu máquina local:
   ```bash
   git clone https://github.com/tu-usuario/pokescript.git
   cd pokescript
   ```

2. Dale permisos de ejecución al script:
   ```bash
   chmod +x pokescript.sh
   ```

3. Ejecuta el script con el nombre del Pokémon que deseas consultar:
   ```bash
   ./pokescript.sh pikachu
   ```

   **Ejemplo de salida:**
   ```bash
   Pikachu (No. 25)
   Id = 25
   Weight = 60
   Height = 4
   Order = 35
   ```

4. Los datos también se guardarán en `pokemon_data.csv` en formato CSV:
   ```csv
   id,name,weight,height,order
   25,pikachu,60,4,35
   ```

## 📖 Notas
- Si el Pokémon no existe o el nombre está mal escrito, el script mostrará un error.
- El archivo `pokemon_data.csv` **no se borra**, sino que se va actualizando con cada consulta.

## 🎓 Actividad
Este script fue desarrollado como parte del curso de **DevOps** de la **Universidad Autónoma de Yucatán (UADY)**.

## 📜 Licencia
Este proyecto es de uso libre. ¡Siéntete libre de modificarlo y mejorarlo! 🚀

