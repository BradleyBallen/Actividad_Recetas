Documentación del Proyecto - Gestor de Recetas Digitales

Integrantes
- Francisco Torres  
- Julián Santiago Nieto  
- Bradley Jeffrey Ballen  

Ramas creadas y responsables
- **feature/recetas-colombianas** → Francisco  
- **feature/recetas-mexicanas** → Julián  
- **feature/recetas-italianas** → Bradley  

Flujo de trabajo seguido
1. Partimos de la rama **main** que contenía la estructura base del repositorio.
2. Cada integrante creó su rama de características usando:
   ```bash
   git checkout -b feature/recetas-colombianas
   git checkout -b feature/recetas-mexicanas
   git checkout -b feature/recetas-italianas

Luego de esto realizamos por cada rama 3 commits como minimo de las recetas representativas de cada pais y tambien un conflicto.

comandos utilizados en el proyecto 
-configuración inicial 
git clone https://github.com/BradleyBallen/Actividad_Recetas.git
cd Actividad_Recetas
git branch

-Trabajo con ramas
git checkout -b feature/recetas-colombianas
git checkout main
git branch

-El ciclo de cambios (commits)
git status
git add recetas/colombianas.md
git add .
git commit -m "Agregar receta de bandeja paisa"

-Esto es donde hacemos los cambios en el repositorio remoto 
git push origin feature/recetas-colombianas
git push origin main

-Aca sincronizamos y actualizamos 
git pull origin main
git pull origin feature/recetas-colombianas

-Resolución de conflictos 
git status
git add recetas/colombianas.md
git commit -m "Resolver conflicto en colombianas.md"

-Uso de gitinore
# Ejemplo de exclusión
echo "server.log" >> .gitignore
git add .gitignore
git commit -m "Agregar archivo .gitignore"

-Etiquetado de la version final
git tag v1.0.0
git push origin v1.0.0

-Por ultimo inspeccionamos el historial 
# Ver historial de commits
git log --oneline --graph --decorate --all
 
