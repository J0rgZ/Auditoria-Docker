# Auditoría de Seguridad en Docker
### Alumno: Jorge Briceño Diaz
### Codigo: 2017059611

Este laboratorio permite realizar una auditoría de seguridad en entornos **Docker**, recopilando información de contenedores, imágenes, redes, volúmenes y plugins, generando un informe detallado.

---

## 🚀 Requisitos
- Windows con **Docker Desktop** instalado.
- **Git Bash** o WSL para ejecutar el script en Bash.
- Python 3 con `venv` y `pip`.

---

## 📌 Pasos de Ejecución

1. **Clonar el repositorio**
   ```bash
   git clone https://github.com/OscarJimenezFlores/CursoAuditoria.git
   cd CursoAuditoria/AuditoriaDocker
   ```

2. **(Opcional) Crear un entorno virtual**
   ```bash
   python -m venv venv
   source venv/Scripts/activate   # En Git Bash o PowerShell
   ```

3. **Instalar dependencias**
   ```bash
   pip install -r requirements.txt
   ```

4. **Dar permisos de ejecución (solo si es necesario)**
   ```bash
   chmod +x DockerAuditor.sh
   ```

5. **Ejecutar el script**
   ```bash
   ./DockerAuditor.sh
   ```

6. **Ingresar la ruta donde guardar el informe**  
   Ejemplo en Windows (Git Bash):
   ```bash
   /c/Users/HP/Documents/GitHub/Auditoria-Docker/AuditoriaDocker/
   ```

El informe se generará automáticamente en la ruta indicada.

---

## 📊 Resultado
El script recopila:
- **Información general**: versión de Docker, daemon y sistema.
- **Contenedores**: inspección, comandos de inicio, logs (200 últimas líneas).
- **Imágenes**: inspección e historial de construcción (`docker history`).
- **Redes, volúmenes y plugins**: listado e inspección.
- **Resumen final**: tabla con versión y totales de recursos.

---

## ✅ Conclusión
Este laboratorio permite identificar configuraciones y posibles riesgos en entornos Docker, facilitando la extracción de evidencias y hallazgos para auditorías de seguridad.