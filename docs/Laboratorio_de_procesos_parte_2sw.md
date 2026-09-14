---
search:
  exclude: true
---
# 🧪 Laboratorio 1 — Procesos en Sistemas Operativos Parte 2

<div class="info-box-blue" markdown>
<div class="info-title">ℹ️ Objetivo</div>

Comprender el funcionamiento básico de los procesos en un sistema operativo mediante programas desarrollados en Python.

Durante el laboratorio se trabajará con:

- Múltiples procesos.
- Procesos huérfanos.
- Concepto de procesos zombie.
- Control de versiones mediante Git.
</div>

---

## 📖 Parte 2 — Múltiples Procesos, Huérfanos y Zombies

### 1. Múltiples procesos

Analice el ejemplo desarrollado por el auxiliar de docencia. Identifique:

- Proceso padre.
- Procesos hijos.
- PID de cada proceso.
- PPID de cada proceso.

Represente la relación:

```
             PADRE
           /   |   \
        HIJO  HIJO  HIJO
```

Observe el uso de `start()` y `join()`.

### 2. Proceso huérfano

Analice el ejemplo desarrollado por el auxiliar de docencia. Observe qué ocurre cuando el proceso padre termina mientras el proceso hijo continúa ejecutándose. Identifique:

- Qué proceso termina primero.
- Qué proceso continúa ejecutándose.
- Por qué se denomina proceso huérfano.

```
PADRE
  │
  └── HIJO

PADRE TERMINA

  └── HIJO CONTINÚA
```

<div class="info-box-green" markdown>
<div class="info-title">⚠️ Nota</div>

El comportamiento del PPID puede ser diferente en Windows respecto a Linux/Unix.
</div>

### 3. Proceso zombie

Analice el ejemplo presentado por el auxiliar de docencia. Comprenda la diferencia entre:

**Proceso huérfano**

```
PADRE TERMINA
      ↓
HIJO CONTINÚA
```

**Proceso zombie**

```
HIJO TERMINA
      ↓
PADRE CONTINÚA
      ↓
NO SE HA RECOGIDO SU ESTADO
```

<div class="info-box-green" markdown>
<div class="info-title">💡 Dato Clave</div>

El proceso zombie se estudiará como concepto y simulación, debido a las diferencias entre Windows y Linux/Unix.
</div>

### 4. Commits de los ejemplos

Después de trabajar correctamente cada ejemplo desarrollado durante la clase, registre las versiones correspondientes mediante Git. Compruebe el historial con:

<div class="terminal-box">
  <code><span class="prompt">Visual Code:</span> git log</code>
</div>

---

## 🚀 Parte 2 — Desafíos

### Desafío 1 — Múltiples procesos

Crear un programa que ejecute varios procesos hijos. Cada proceso deberá realizar una tarea identificable y mostrar información que permita determinar:

- Proceso.
- PID.
- PPID.
- Inicio y finalización.

### Desafío 2 — Proceso huérfano

Modificar un programa para demostrar el comportamiento de un proceso huérfano. Deberá explicar qué ocurre con el padre y qué ocurre con el hijo.

### Desafío 3 — Concepto zombie

Realizar una demostración conceptual del proceso zombie. Deberá explicar:

- Cuándo termina el hijo.
- Qué ocurre con el padre.
- Qué significa que el estado del hijo no haya sido recogido.
- Por qué la demostración en Windows es conceptual.

### Desafío 4 — Git y versiones

Realizar diferentes commits durante el desarrollo de los desafíos. El historial deberá mostrar el desarrollo progresivo del trabajo. Compruebe las versiones mediante:

<div class="terminal-box">
  <code><span class="prompt">Visual Code:</span> git log</code>
</div>

### Desafío 5 — Recuperación

Modificar intencionalmente el programa y posteriormente recuperar una versión anterior utilizando Git. Deberá demostrar el procedimiento y explicar qué versión recuperó.