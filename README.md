# 4dra 🧾⚡️

> **Pasa tus facturas y tickets a Excel en segundos con Gemini y auditoría fiscal contable en un solo archivo.**

**4dra** (pronunciado *Cuadra*) es una herramienta autónoma y 100% responsiva diseñada para autónomos, gestores y empresas que necesitan digitalizar y contabilizar rápidamente sus gastos sin instalar nada, sin terminal y con total privacidad.

---

## ✨ Características Principales

- **📦 Un solo archivo (`index.html`)**: Ábrelo directamente con doble clic en cualquier navegador (Chrome, Safari, Edge, Arc...) en Mac, Windows, Linux, iPad, iPhone o Android.
- **📱 100% Responsiva (PC, Tablet y Móvil)**:
  - **PC / Escritorio**: Tabla compacta optimizada que aprovecha el 100% del ancho sin necesidad de desplazamientos laterales incómodos.
  - **Tablet y Teléfono**: Vista automática en **Tarjetas Inteligentes** que presentan toda la información fiscal, importes y botones adaptados a la pantalla vertical.
  - **Selector de Vista**: Alterna entre Vista de Tabla y Vista de Tarjetas con un solo clic.
- **🤖 Extracción multimodal con Gemini API**: Arrastra PDFs o fotos de tickets; Gemini detecta proveedor, NIF/CIF, fecha, número y bases de impuestos.
- **🔒 Privacidad total**: Tu API Key se guarda exclusivamente en tu navegador (`localStorage`) y viaja directa a los servidores de Google. Ningún dato ni documento pasa por servidores de terceros.
- **⚖️ Auditoría Contable en Código (sin depender de la IA)**:
  - **Ecuación Contable**: Valida estrictamente que $\text{Base} + \text{IVA} - \text{IRPF} = \text{Total}$ al céntimo.
  - **Algoritmo Oficial NIF/CIF/NIE (España)**: Verificación de dígitos de control para DNI (módulo 23), NIE y sociedades (CIF).
  - **Control de Fechas**: Control de rangos reales y coherencia de calendario.
  - **Detección de Duplicadas**: Alerta inmediata de facturas repetidas del mismo emisor.
  - **Control de Tipos de IVA**: Detección de tipos oficiales españoles (21%, 10%, 4%, 5%, 0%).
- **🟢 Estados de Auditoría en Tiempo Real**:
  - 🟢 **Cuadra**: Cuentas exactas y datos contrastados.
  - 🟡 **Revisar**: Cuentas correctas pero requiere comprobación humana (NIF/fecha).
  - 🔴 **No cuadra**: Descuadre en la suma matemática.
  - 🟣 **Duplicada**: Factura idéntica ya existente en el lote.
- **✏️ Edición en Vivo**: Corrige cualquier celda haciendo clic/doble clic y observa cómo cambian los estados e importes al vuelo.
- **🔍 Visor de Documentos Originales**: Abre el PDF o la foto del ticket al instante en un modal para contrastar las cifras.
- **📊 Exportación a Excel (.xlsx) Profesional con 3 Hojas**:
  1. **`Facturas`**: Listado detallado con badges de color, formato contable (`#,##0.00 "€"`), fórmulas dinámicas `=SUM(...)` y leyenda explicativa.
  2. **`Desglose IVA`**: Agrupación por tipos impositivos (21%, 10%, 4%, 5%, exento/0%) y retenciones IRPF (Modelos 303, 390, 111, 190).
  3. **`Resumen`**: Cuadro de mando ejecutivo con KPIs de calidad y totales económicos consolidados.
- **📲 Soporte PWA y Multiplataforma**: Iconos nativos para Web, iPad/iPhone (Apple Touch Icon), Android (PWA) y archivo `manifest.json` para instalación local como app de escritorio o móvil.

---

## 🚀 Inicio Rápido

1. Descarga o clona este repositorio:
   ```bash
   git clone https://github.com/manueladolfo/4dra.git
   ```
2. Haz doble clic sobre `index.html`.
3. Haz clic en **«Configurar Gemini API»** e introduce tu clave gratuita de [Google AI Studio](https://aistudio.google.com/app/apikey).
4. ¡Arrastra tus facturas o tickets y descarga tu Excel!

---

## 📄 Licencia

Distribuido bajo la Licencia MIT.
