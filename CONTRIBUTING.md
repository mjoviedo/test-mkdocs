# 🚀 Guía rápida para colaborar

¡Hola! Gracias por querer ayudar en este proyecto. No te preocupes si no eres experto en programación o Git, aquí te explicamos cómo hacerlo paso a paso de la manera más sencilla.

## 1. Haz un "Fork" del proyecto
El primer paso es tener tu propia copia del proyecto para hacer pruebas sin afectar el original.
1. Mira la parte superior derecha de esta página.
2. Haz clic en el botón que dice **Fork**.
3. Esto creará una copia del repositorio en tu cuenta personal.

## 2. Crea una "Rama" (Branch)
Imagina que las ramas son borradores. Es mejor trabajar en un borrador que en el documento principal.
1. En **tu copia** del proyecto, haz clic en el botón que dice `main`.
2. Escribe un nombre para tu mejora (ejemplo: `mi-mejora-texto`).
3. Haz clic en **Create branch**.



## 3. Realiza tus cambios
Puedes editar archivos directamente desde el navegador:
1. Busca el archivo que quieras cambiar y haz clic en él.
2. Haz clic en el icono del **lápiz** (Edit this file).
3. Haz tus cambios.
4. Cuando termines, ve al botón verde **Commit changes...** arriba a la derecha.
5. Escribe un resumen corto de qué cambiaste y dale a "Commit".

## 4. Envía tus cambios (Pull Request)
Ahora que tus cambios están listos en tu copia, avísanos para que los revisemos e incluyamos en el proyecto original.
1. Ve a la pestaña **Pull requests** en el repositorio original.
2. Haz clic en el botón verde **New pull request**.
3. Haz clic en el enlace azul que dice **compare across forks**.
4. Asegúrate de que en la derecha aparezca tu copia y tu rama.
5. Haz clic en **Create pull request**, ponle un título y ¡listo!

---
### 💡 Recomendaciones
- **Haz cambios pequeños:** Es más fácil revisar un cambio pequeño que uno gigante.
- **Sé descriptivo:** Cuéntanos un poquito por qué decidiste hacer ese cambio.
- **No tengas miedo:** Si algo sale mal, ¡siempre se puede corregir!



## Llamados de atención

Si ves códigos extraños en los archivos, como por ejemplo: `!!! abstract "Contenidos"` aquí te explicamos:

La plataforma tiene 12 tipos de llamados de atención. Cada uno tiene su propio color e icono, categorizados según la "intención" del mensaje.

1. Informativas (Azul/Cian)
Se usan para información suplementaria neutral.

'note:' El tipo más común. Información general.

abstract: Para resúmenes o secciones "TL;DR" (demasiado largo; no lo leí). (Alias: summary, tldr).

info: Similar a la nota, a menudo usada para datos útiles. (Alias: todo).

2. Éxito y Listas de Verificación (Verde)
Se usan cuando una tarea se completa o se logra un resultado positivo.

tip: Sugerencias útiles o "pro-tips". (Alias: hint, important).

success: Confirma una acción exitosa. (Alias: check, done).

3. Advertencias y Críticas (Naranja/Rojo)
Se usan para evitar que el usuario cometa errores o para resaltar riesgos.

question: Para preguntas frecuentes (FAQs) o dudas. (Alias: help, faq).

warning: Alerta de nivel medio. Ten cuidado. (Alias: caution, attention).

failure: Algo salió mal. (Alias: fail, missing).

danger: Alerta de nivel alto. Riesgo de perder datos o romper algo. (Alias: error).

4. Técnicas y Estructurales (Púrpura/Gris)
Se usan para tipos específicos de contenido técnico.

bug: Específicamente para reportar o señalar errores de software.

example: Para fragmentos de código o demostraciones de casos de uso.

quote: Para citas o testimonios. (Alias: cite).

Cómo usarlas en Markdown
La sintaxis es un bloque que comienza con !!! seguido del tipo. También puedes añadir un título personalizado entre comillas.

Markdown
!!! note "Nota del curso"
    Este es un bloque de información general usando Reforma 2018.

!!! danger "¡Cuidado!"
    No borres la carpeta `overrides` o perderás tu diseño personalizado.

!!! abstract inline "Resumen rápido"
    Puedes usar `inline` para que el texto fluya alrededor del bloque.
Bloques colapsables
Si quieres que el bloque esté cerrado por defecto (ideal para "SPOILERS" o "SOLUCIONES"), usa ??? en lugar de !!!.

Markdown
??? success "Ver solución del ejercicio"
    Aquí está el código que resuelve el problema anterior.
Personalizar los colores de las Admonitions
Como acabamos de configurar tus colores institucionales (Rojo #B5121B y Oro #FFD200), quizás quieras que las notas combinen con tu marca. Puedes sobrescribir los colores específicos en tu extra.css:

CSS
:root {
  /* Esto cambia el color de 'note' a tu Rojo institucional */
  --md-admonition-icon--note: url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M13 14h-2V9h2m0 9h-2v-2h2m-9 2h14a2 2 0 0 0 2-2V6a2 2 0 0 0-2-2H5a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2Z"/></svg>');
  --md-typeset-admonition-fallback-color--note: var(--brand-red);
}

/* Esto hace que el borde de 'tip' sea de tu color Oro institucional */
.md-typeset .admonition.tip {
  border-left-color: var(--brand-gold);
}
¿Te gustaría que te ayude a crear un tipo de nota completamente personalizado (por ejemplo, una llamada !!! ai) con un icono de robot específico y tus colores institucionales?