# Quadra 🧾⚡️

> **Pasa tus facturas y tickets a Excel en segundos con Gemini y auditoría contable en un solo archivo.**

Quadra es una herramienta autónoma diseñada para autónomos, gestores y empresas que necesitan digitalizar y contabilizar rápidamente sus gastos sin instalar nada, sin terminal y con total privacidad.

---

## ✨ Características Principales

- **📦 Un solo archivo (`index.html`)**: Ábrelo directamente con doble clic en cualquier navegador moderno (Chrome, Safari, Edge, Arc...).
- **🤖 Extracción inteligente con Gemini API**: Arrastra PDFs o fotos de tickets; Gemini detecta emisor, NIF/CIF, fecha, número y desgloses.
- **🔒 Privacidad total**: Tu API Key se guarda exclusivamente en tu navegador (`localStorage`) y viaja encriptada y directa a los servidores de Google. Ningún dato ni documento pasa por servidores de terceros.
- **⚖️ Auditoría Contable en Código (sin depender de la IA)**:
  - **Ecuación Contable**: Valida estrictamente que $\text{Base} + \text{IVA} - \text{IRPF} = \text{Total}$ al céntimo.
  - **Algoritmo Oficial NIF/CIF/NIE (España)**: Verificación de dígitos de control para DNI (módulo 23), NIE y sociedades (CIF).
  - **Control de Fechas**: Control de rangos reales y coherencia de calendario.
  - **Detección de Duplicadas**: Alerta inmediata de facturas repetidas del mismo emisor.
  - **Control de Tipos de IVA**: Detección de tipos oficiales españoles (21%, 10%, 4%, 0%).
- **🟢 Estados de Auditoría en Tiempo Real**:
  - 🟢 **Cuadra**: Cuentas exactas y datos contrastados.
  - 🟡 **Revisar**: Cuentas correctas pero requiere comprobación humana (NIF/fecha).
  - 🔴 **No cuadra**: Descuadre en la suma matemática.
  - 🟣 **Duplicada**: Factura idéntica ya existente en el lote.
- **✏️ Edición en Vivo**: Corrige cualquier celda haciendo clic y observa cómo cambian los estados e importes al vuelo.
- **🔍 Visor de Documentos Originales**: Abre el PDF o la foto del ticket al instante en un modal para contrastar las cifras.
- **📊 Exportación a Excel (.xlsx) con 3 Hojas**:
  1. **`Facturas`**: Listado detallado con valores numéricos y formato moneda contable.
  2. **`Desglose IVA`**: Agrupación por tipos impositivos (21%, 10%, 4%, exento/0%) e IRPF.
  3. **`Resumen`**: Cuadro de mando ejecutivo con totales y recuento por estado de auditoría.

---

## 🚀 Inicio Rápido

1. Descarga o clona este repositorio:
   ```bash
   git clone https://github.com/manueladolfo/Quadra.git
   ```
2. Haz doble clic sobre `index.html`.
3. Haz clic en **«Configurar Gemini API»** e introduce tu clave gratuita de [Google AI Studio](https://aistudio.google.com/app/apikey).
4. ¡Arrastra tus facturas y genera tu Excel!

---

## 📄 Licencia

Distribuido bajo la Licencia MIT. Consulta `LICENSE` para más detalles.
