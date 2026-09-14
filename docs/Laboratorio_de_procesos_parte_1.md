# 🧪 Laboratorio 1 — Procesos en Sistemas Operativos

<div class="info-box-blue" markdown>
<div class="info-title">ℹ️ Objetivo</div>

Comprender el funcionamiento básico de los procesos en un sistema operativo mediante programas desarrollados en Python.

Durante el laboratorio se trabajará con:

- Procesos padre e hijo.
- PID y PPID.
- Creación y ejecución de procesos.
</div>

---

## 📖 Parte 1 — Introducción a los Procesos

### 1. Preparación

Trabajar utilizando:

<div class="tech-row">
  <span>🖥️ Visual Studio Code</span>
  <span>🐍 Python</span>
  <span>💻 PowerShell</span>
  <span>🐙 Git</span>
</div>

Verifique que Python y Git estén disponibles antes de comenzar.

### 2. Proceso padre e hijo

Analice el ejemplo desarrollado por el auxiliar de docencia. Identifique:

- ¿Cuál es el proceso padre?
- ¿Cuál es el proceso hijo?
- ¿Cómo se crea un proceso?
- ¿Cómo se inicia?
- ¿Cómo se espera su finalización?

### 3. PID y PPID

Observe los valores mostrados durante la ejecución del programa. Identifique:

- PID del proceso padre.
- PID del proceso hijo.
- PPID del proceso hijo.

Determine la relación existente entre el proceso padre y el proceso hijo.

### 4. Ejecución del proceso

Observe el comportamiento del programa durante su ejecución. Identifique:

1. Inicio del proceso padre.
2. Creación del proceso hijo.
3. Ejecución del proceso hijo.
4. Finalización del proceso hijo.
5. Continuación del proceso padre.

<div class="info-box-green" markdown>
<div class="info-title">💡 Preste Atención al Uso de</div>

`Process` · `start()` · `join()`
</div>

### 5. Primer commit

Una vez que el ejemplo funcione correctamente, registre la versión inicial utilizando Git. Compruebe posteriormente el historial mediante:

<div class="terminal-box">
  <code><span class="prompt">Visual Code:</span> git log</code>
</div>

---

## 🚀 Parte 1 — Desafíos

Los siguientes desafíos deberán realizarse individualmente.

### Desafío 1 — Modificación del proceso

Modifique el programa trabajado durante la clase para que el proceso hijo realice una tarea diferente. Debe mostrar información que permita identificar el proceso.

### Desafío 2 — Múltiples procesos

Modifique el programa para trabajar con más de un proceso hijo. Cada proceso deberá poder ser identificado mediante su PID.

### Desafío 3 — Git

Guarde una nueva versión del programa mediante un commit. El historial debe permitir identificar claramente las diferentes versiones. Utilice:

<div class="terminal-box">
  <code><span class="prompt">Visual Code:</span> git log</code>
</div>

### Desafío 4 — Recuperación de una versión

Realice una modificación adicional en el programa. Posteriormente, utilice Git para regresar a una versión anterior. Debe demostrar qué versión recuperó y qué commit utilizó.

### Desafío 5 — Explicación

Explique al auxiliar de docencia el funcionamiento de su programa y las modificaciones realizadas.