# Cold Chain Temperature Report — Beta v1.1

Add-in para **MyGeotab** que permite generar informes de temperaturas de la cadena de frio filtrados por activo, rango de fechas y horas, con agrupacion por intervalos de tiempo.

## Caracteristicas

- Filtro por activo (busqueda en tiempo real)
- Rango de fechas **y horas**
- Selector de origen de datos: Termografo, Maquina de frio o Sondas
- Intervalos de agrupacion: 5 min, 15 min, 30 min, 1 hora (promedio)
- Grafica interactiva de temperaturas (Chart.js)
- Exportacion a PDF (grafica + tabla de datos)
- Estilos Geotab Zenith Design System (Nunito Sans, paleta #0064A8)
- Badge "Beta" integrado

## Diagnosticos incluidos

| Origen | Diagnostic ID | Descripcion |
|--------|--------------|-------------|
| Termografo | ThermographTemperature1Id | Temperatura termografo zona 1 |
| Termografo | ThermographTemperature2Id | Temperatura termografo zona 2 |
| Maquina de frio | RefrigerationUnitTemperatureZone1Id | Retorno zona 1 |
| Maquina de frio | RefrigerationUnitSetTemperatureZone1Id | Consigna zona 1 |
| Maquina de frio | RefrigerationUnitTemperatureZone2Id | Retorno zona 2 |
| Maquina de frio | RefrigerationUnitSetTemperatureZone2Id | Consigna zona 2 |
| Sondas | RemoteProbe1TemperatureId | Sonda remota 1 |
| Sondas | RemoteProbe2TemperatureId | Sonda remota 2 |
| Sondas | RemoteProbe3TemperatureId | Sonda remota 3 |

## Instalacion en MyGeotab

1. Sube el repositorio a GitHub Pages bajo el nombre **Cold_Chain_Beta_1.1**
2. Asegurate que la URL en `config.json` apunta a: `https://<usuario>.github.io/Cold_Chain_Beta_1.1/index.html`
3. En MyGeotab > Administracion > Sistema > Add-Ins, sube el archivo `config.json`

## Tecnologias

- Chart.js 4.4.3
- jsPDF 4.2.1 + jspdf-autotable 5.0.8
- Geotab Zenith Design System (CSS vanilla port)
- Nunito Sans (Google Fonts)