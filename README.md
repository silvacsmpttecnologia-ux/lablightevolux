# LabLight Evolux - Release 1.0

Laboratorio virtual de óptica orientado principalmente a estudiantes de enseñanza media.

## Demo pública
https://lablightevolux.netlify.app/

## Pregunta de investigación
¿Cómo cambia la iluminancia al modificar la distancia a la fuente de luz?

## Flujo
Predicción -> Preparación -> Medición -> Análisis -> Conclusión.

## Stack
- HTML5
- CSS3
- JavaScript
- SVG generado en la interfaz
- localStorage
- Netlify para despliegue

## Motor de datos
La Release 1.0 genera datos simulados. El modelo base es `E = I/d^2`, convirtiendo la distancia de cm a m. Se incorpora una variación sinusoidal determinista cercana a ±4,5 %.

Parámetros simulados:
- Vela: 1 cd
- Ampolleta LED: 60 cd
- Linterna con lente: 1500 cd

Estos valores son aproximaciones de simulación y no especificaciones universales de fuentes reales.

## Protocolo
- Una medición por distancia.
- Distancia: 20 a 120 cm, paso 10 cm.
- Mínimo: 5 distancias diferentes antes del análisis.
- El usuario puede repetir la experiencia con otra fuente.

## Validación
Una corrida con seis distancias se contrastó con la referencia inversa al cuadrado:
- Error relativo medio: 2.65 %
- Error máximo observado: 5.35 %

Repetibilidad computacional:
- Condición: Linterna con lente, 50 cm, ejecución nueva
- 5 repeticiones: 6056 lx en las cinco
- Desviación estándar: 0 lx

La validación corresponde al motor de simulación, no a un sensor físico.

## Prueba de usuarios
Se trabajó con cinco participantes externos. La primera versión mostró exceso de texto y un orden poco simple. La interfaz fue rediseñada y se preparó una explicación visual breve. Tras la mejora, 5/5 participantes comprendieron y completaron la experiencia.

No se registraron formalmente tiempos, número de errores o solicitudes de ayuda; por ello no se reportan valores inventados.

## Equipo
- Martín Silva - Product Owner / Líder
- Jaira Oyarzun - Software y Datos
- Luciana Muñoz - Pedagogía y Documentación
- Dominic Zúñiga - UX/UI
- Haiskel Flores - Hardware / Instrumentación
- Ámbar Reyes - Área Científica

## Ejecución local
1. Descargar el repositorio.
2. Abrir `index.html` en un navegador moderno.
3. No requiere servidor ni instalación de dependencias para el funcionamiento básico.

## Estructura
- `index.html`: Release 1.0.
- `docs/`: documentación técnica y pedagógica.
- `evidencias/`: capturas seleccionadas.

## Limitaciones
- No utiliza sensor físico en Release 1.0.
- No existe calibración contra luxómetro.
- La variación simulada no es incertidumbre instrumental.
- El historial Git previo fue incompleto; este repositorio consolida la Release 1.0 y no pretende recrear commits históricos.

## Licencia académica
Proyecto académico desarrollado para la asignatura Proyecto de Innovación Tecnológica, sección 002, Universidad Mayor, 2026.
