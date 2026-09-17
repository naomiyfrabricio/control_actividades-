# Descripción

Control de Actividades es una propuesta de aplicación para organizar actividades personales.

En esta etapa solamente se prepara la estructura inicial del proyecto.
EOF
8. Contenido de docs/funcionalidades.md
bash
cat > docs/funcionalidades.md << 'EOF'
# Funcionalidades previstas

- Registrar actividades.
- Consultar actividades.
- Modificar actividades.
EOF
9. Contenido de README.md
bash
cat > README.md << 'EOF'
# Control de Actividades

Proyecto desarrollado como parte del primer examen parcial.

## Objetivo 

Preparar la estructura inicial de un proyecto utilizando Python, Git y GitHub.

## Herramientas

- Visual Studio Code
- Python
- Git
- GitHub

## Autor

Tu Nombre Completo
EOF

(En Windows, si cat > archivo << 'EOF' ... EOF no funciona en PowerShell, más fácil: abre cada archivo en VS Code y pega el contenido a mano.)

10. Poner los PDFs de las partes 2, 3 y 4

Copia dentro de parte_2/, parte_3/ y parte_4/ los PDFs que ya te generé (los que venían en el .zip), o arrástralos ahí desde el explorador de archivos / VS Code. Deben quedar como parte_2/parte_2.pdf, parte_3/parte_3.pdf, parte_4/parte_4.pdf.

11. Inicializar Git y revisar estado
bash
git init
git status

Confirma que .venv/ no aparezca en la lista.

12. Primer commit
bash
git add .
git commit -m "Crea estructura inicial del proyecto"
13. Segundo commit — actualizar README

Agrega al final de README.md:

markdown
## Estado del proyecto

Proyecto en etapa inicial.
bash
git add README.md
git commit -m "Agrega estado del proyecto en README"
14. Tercer commit — actualizar funcionalidades

Agrega al final de docs/funcionalidades.md:

markdown
- Marcar actividades como terminadas.
- Asignar una fecha a las actividades.
bash
git add docs/funcionalidades.md
git commit -m "Agrega nuevas funcionalidades previstas"
15. Verificar historial
bash
git log --oneline

Debes ver 3 commits.

16. Crear el repo en GitHub

En github.com → New repository → nombre: control-actividades → NO marcar README/.gitignore/licencia → Create repository.

17. Enlazar y publicar
bash
git remote add origin https://github.com/TU-USUARIO/control-actividades.git
git branch -M main
git push -u origin main
18. Cambio adicional final

Agrega al final de README.md:

markdown
## Control de versiones

El proyecto utiliza Git para control de versiones y GitHub como repositorio remoto.
bash
git status
git add README.md
git commit -m "Agrega sección de control de versiones en README"
git push

Verifica en GitHub que estén los 4 commits, los PDFs, y que .venv/ no aparezca. Esa URL es lo que entregas.

Claude es una IA y puede cometer errores.