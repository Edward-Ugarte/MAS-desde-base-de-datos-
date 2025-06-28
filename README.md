# MAS-desde-base-de-datos-
# 📊 Estimación de Tamaño Muestral e Intervalo de Confianza en Gretl

Este script calcula el tamaño muestral necesario para estimaciones de media con corrección para población finita y genera el intervalo de confianza correspondiente. Utiliza datos reales desde una base cargada en Gretl (`BdD.gdt`), tomando como variable de referencia `ingresos`.

---

## 🎯 Objetivo

Comparar tres métodos de estimación de tamaño muestral (A, B, y C) y aplicar el resultado más operativo (redondeado) para construir un intervalo de confianza del 95 % para la media poblacional esperada.

---

## 📥 Requisitos

- Gretl 2025b o posterior
- Archivo `BdD.gdt` en el mismo directorio o ruta conocida
- Variable `ingresos` incluida en la base

---

## 📐 Fórmulas implementadas

- **Método A (clásico):**  
  

- **Método B (expansión directa):**  
 

- **Método C (forma alternativa):**  
  

- **Intervalo de confianza:**  


## 🛠️ Variables clave

| Nombre     | Descripción                          |
|------------|--------------------------------------|
| `media`    | Media de la variable `ingresos`      |
| `sigma`    | Desvío estándar muestral             |
| `sigma2`   | Varianza muestral (`sigma^2`)        |
| `E`        | Margen de error máximo deseado       |
| `Z`        | Valor z para nivel de confianza      |
| `N`        | Número de observaciones válidas      |

---

## 🔄 Personalización

Para cambiar la variable de interés (por ejemplo, de `ingresos` a `consumo`), reemplaza todas las ocurrencias de `ingresos` en el script. También puedes ajustar:
las formulas se pueden cambiar
- El margen de error `E`
- El nivel de confianza (modificando `Z`)

## 👨‍💻 Autoría

Script desarrollado y optimizado por ** Edward Ugarte**
