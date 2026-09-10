# 2026_TRABAJO_POO                  

## Lista de integrantes: 
 -Ioan Alexander Valenzuela Vasquez

 -Dire Daniel Espinal Pecho
    
## Flujo de trabajo en equipo (Fork + Sincronización)

Antes de empezar, cada colaborador ya debe tener:
- El repositorio clonado (`git clone`)
- Su propio Fork configurado como `origin`
- El repo principal configurado como `upstream`

### Pasos para modificar código

1. **Sincronizar tu rama `main` con el repo principal**
```bash
   git fetch upstream
   git checkout main
   git merge upstream/main
```

2. **Crear una nueva rama para tu tarea**
```bash
   git checkout -b nombre-tarea
```

3. **Realizar tus cambios en el código**
   - Trabaja únicamente en tu rama.
   - Evita modificar archivos que no correspondan a tu tarea.

4. **Guardar tus cambios (commit)**
```bash
   git add .
   git commit -m "Descripción clara del cambio"
```

5. **Subir tu rama a tu Fork**
```bash
   git push origin nombre-tarea
```

6. **Abrir un Pull Request**
   - Ve a tu Fork en GitHub.
   - Crea un Pull Request desde tu rama hacia `main` del repositorio principal.
   - Escribe una descripción clara de lo que hiciste.

7. **Revisión y aprobación**
   - El propietario del repositorio revisa el Pull Request.
   - Si todo está correcto, se aprueba el Merge.

8. **Sincronizar nuevamente antes de la siguiente tarea**
```bash
   git fetch upstream
   git checkout main
   git merge upstream/main
```

### Buenas prácticas
- No trabajar directamente sobre `main`.
- Un archivo o módulo por persona, para evitar conflictos.
- Commits pequeños y descriptivos.
- Sincronizar siempre antes de iniciar una nueva tarea.