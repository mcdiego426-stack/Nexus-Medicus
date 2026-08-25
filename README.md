# Nexus Medicus - Plataforma Inmobiliaria de Salud

Plataforma completa para la comercialización y administración de consultorios médicos premium en Valle Real, Zapopan, Jalisco.

## 🏢 Descripción

Nexus Medicus es una plataforma dirigida a inversores y médicos especialistas (45-60 años) que buscan oportunidades de inversión en consultorios médicos premium con retornos garantizados de 11% a 16% ROI anual.

## 📱 Fases del Proyecto

### Fase 1: Landing Page (`index.html`)
- Hero section con propuesta de valor
- Catálogo de 8 modelos de consultorios (Ten a Two Hundred)
- Información financiera: Precio, Renta Est., ROI, Cap Rate
- 3 modales de captura de leads:
  - Agendar Cita Presencial
  - Descargar Brochure & Corrida Financiera
  - Solicitar Cotización
- Información de ubicación (Valle Real, Zapopan)
- Footer con contacto e información legal

### Fase 2: Calculadora ROI (`fase2_calculadora_roi.html`)
- Selector dinámico de perfil (Inversionista vs. Médico)
- Calculadora interactiva con sliders:
  - Seleccionar modelo de consultorio
  - Down payment (20%-100%)
  - Ocupancy rate (70%-100%)
- Cálculos en tiempo real:
  - Inversión total requerida
  - Down payment exacto
  - NOI mensual y anual
  - Cap Rate
  - Proyección de ROI
- Botón WhatsApp dinámico con detalles del modelo

### Fase 3: PDF Generator & WhatsApp (`fase3_generador_pdf_whatsapp.html`)
- Generador de PDF client-side con html2pdf.js
- Lead Magnet Grid con 3 recursos:
  - Brochure Oficial (12 páginas)
  - Technical Sheet (Specs + COFEPRIS)
  - Financial Report (ROI analysis 5-10 años)
- Modal de captura con generación automática de PDF
- Botón WhatsApp flotante animado
- Confirmación de descarga exitosa

### Fase 4: CRM Dashboard (`admin_dashboard.html`)
- Dashboard administrativo privado
- 4 KPI cards (Leads, Valor Potencial, Inventario, Conversión)
- Pipeline de Ventas con tabla interactiva:
  - Búsqueda por nombre/email
  - Filtro por estado (6 opciones)
  - Filtro por perfil
  - Edición de estado inline
  - Links WhatsApp directos
  - Exportación a CSV
- Control de Inventario en Tiempo Real:
  - 8 modelos con toggles trilaterales
  - Estados: Disponible, Reservado, Vendido
  - Persistencia en localStorage
- Datos almacenados en localStorage

## 🎨 Diseño & UX

- **Paleta de colores:** Azul marino (#0f172a), Teal (#14b8a6), Blanco
- **Tipografía:** Plus Jakarta Sans, Outfit
- **Accesibilidad:** 
  - Textos mínimo 16px
  - Botones 48px+
  - Alto contraste
  - Navegación intuitiva
- **Responsive:** Mobile-first, adaptable a todos los dispositivos

## 🛠 Stack Técnico

- **Frontend:** HTML5, CSS3 (Tailwind), JavaScript Vanilla
- **PDF:** html2pdf.js
- **Storage:** localStorage
- **Integración:** WhatsApp API (wa.me)
- **Despliegue:** Vercel

## 📦 Archivos

- `index.html` - Fase 1: Landing Page
- `fase2_calculadora_roi.html` - Fase 2: ROI Calculator
- `fase3_generador_pdf_whatsapp.html` - Fase 3: PDF Generator
- `admin_dashboard.html` - Fase 4: CRM Dashboard
- `README.md` - Este archivo

## 🚀 Cómo usar

1. Abre cualquier archivo HTML en tu navegador
2. Navega entre las diferentes fases
3. Prueba los formularios, calculadora, y descarga de documentos

## 📊 Información Financiera (8 Modelos)

| Modelo | Superficie | Precio | Renta/mes | ROI | Cap Rate |
|--------|-----------|--------|-----------|-----|----------|
| Ten | 18 m² | $2.2M | $18,900 | 11.39% | 8.78% |
| Twenty | 22 m² | $3.3M | $23,100 | 13.86% | 7.21% |
| Thirty | 33 m² | $4.4M | $32,340 | 13.26% | 7.54% |
| Forty | 44 m² | $5.5M | $41,400 | 13.82% | 7.24% |
| Fifty | 53 m² | $6.4M | $47,100 | 14.54% | 6.96% |
| Sixty | 65 m² | $7.9M | $57,850 | 16.39% | 6.10% |
| Ninety | 95 m² | $11.5M | $80,750 | 14.21% | 7.04% |
| Two Hundred | 223 m² | $25.7M | $156,100 | 16.76% | 5.97% |

## 📍 Ubicación

**Avenida Central Guillermo Gonzalez Camarena #500**
Valle Real, 45136 Zapopan, Jalisco, México

## 👨‍💼 Target Audience

- Médicos especialistas (45-60 años)
- Inversionistas en bienes raíces de salud
- Profesionales que buscan diversificación de portafolio

## 📞 Contacto

Para más información, agendar cita o solicitar cotización, usa los formularios en la plataforma.

---

**© 2026 Nexus Medicus. Todos los derechos reservados.**
