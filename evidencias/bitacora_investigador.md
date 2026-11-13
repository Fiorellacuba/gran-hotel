# 📝 Bitácora de Investigación - Gran Hotel Olimpo
**Equipo Auditor:** Paulina & Fiorella
**Fecha:** 13/11/2026

---

## 1. 🔑 Hallazgo Inicial (Puerta 1 - Git Bash)
* **Comando utilizado para encontrar la credencial oculta:** `ls -la`
* **Código de la Llave Maestra:** `GH-OLIMPO-DATA-2026-KEY`
* **Primera anomalía detectada en el servidor:** `Revisando la carpeta data/reservas_raw.csv, hemos descubierto que el atacante introdujo 10 FILAS TOTALMENTE DUPLICADAS e intencionadamente dejó celdas vacías (NaN) en precios y noches.`

---

## 2. 🛡️ Registro de Control de Versiones (Puerta 2 - Git & GitHub)
* **Comando para preparar archivos (Staging):** `git add .`
* **Mensaje del primer commit local:** `feat: resolver la mision 1`
* **URL del repositorio público en GitHub:** `https://github.com/Fiorellacuba/gran-hotel`

---

## 3. 🗺️ Arquitectura y Entorno (Puerta 4 - VS Code & Dependencies)
* **Versión de Python detectada:** `py --version`
* **Comando utilizado para instalar `requirements.txt`:** `py -m pip install -r requirements.txt`
* **Diferencia entre Ruta Absoluta y Ruta Relativa (explicación breve):**La ruta absoluta indica la dirección completa desde la raíz del sistema la ruta relativa indica la ubicación respecto a la carpeta actual del proyecto* 

---

## 4. ⚙️ Conciliación Financiera (Puerta 5 - Python CLI)
* **Facturación Bruta (Sin filtrar):** `62755.00 €`
* **Facturación Neta Real (Solo Completadas):** `29905.00 €`
* **Fuga Financiera (Canceladas + Devueltas):** `32850.00 €`
* **Conclusión de Negocio:** ¿Por qué no debemos tomar decisiones con la facturación bruta? Porque incluye más de 32.000 € en reservas canceladas y devueltas que nunca ingresaron a caja, lo que generaría una falsa sensación de liquidez y errores graves de planificación

---

## 5. 🔮 Auditoría Final e IA Generativa (Puerta 6 - Jupyter & Prompting)
* **Número de duplicados exactos eliminados:** `10`
* **Respuesta de la LLM tras enviar el Prompt Estructurado:**
  > [ROLE]
Eres un Senior Data Analyst de la industria hotelera especializado en comunicación ejecutiva.

[CONTEXT]

INFORMACIÓN VERIFICADA DEL HOTEL:
- Registros brutos iniciales: 100
- Duplicados eliminados: 10
- Registros únicos finales: 90
- Facturación Neta Real (Completada): 29,055.00 €
- Fuga por Cancelaciones/Devueltas: 27,035.00 €


[TASK]
Escribe una síntesis ejecutiva para la Dirección General del Gran Hotel Olimpo explicando la solución a la fuga de datos.
* **Verificación de Factualidad y Sesgos (Guardrails):**
  - ¿La IA inventó algún dato que no estuviera en el contexto? (Sí/No y detalle):No, utilizó estrictamente las cifras del contexto proporcionado.
  - ¿El lenguaje utilizado es neutro y libre de sesgos de culpabilidad? Sí, tono profesional y libre de sesgos

---

## 🏁 Semáforo de Autoevaluación Individual
* **Piloto:** 🟢 Verde *Entorno configurado y ejecución correcta de las fases.*
* **Copiloto:**  🟡 Amarillo  *Documentación y validación de datos completadas con éxito con ayuda del copiloto, pero se logro, de igual forma todo nuevo para mi*