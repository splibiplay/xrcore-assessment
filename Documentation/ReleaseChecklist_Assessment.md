# XRCore Assessment Release Checklist

Checklist operativo para validar el modulo `xrcore-assessment` antes de publicarlo en Unity Asset Store.

## 1) Scope y versionado

- [ ] Version del paquete actualizada y consistente con release notes.
- [ ] Cambios de API publica revisados (sin roturas no documentadas).
- [ ] Dependencias declaradas correctamente (SDK y Toolkit).

## 2) Validacion funcional

- [ ] Flujo de evaluacion completo ejecutado (`Look -> Grab -> Place` o equivalente).
- [ ] Reglas de score ponderado verificadas en casos nominales y borde.
- [ ] Reglas de fallo critico validadas.
- [ ] Resultado final `pass/fail` consistente con criterios definidos.

## 3) Reportes y trazabilidad

- [ ] Export de reportes JSON validado.
- [ ] Export de reportes CSV validado.
- [ ] Estructura de campos estable para consumo externo.
- [ ] Metadatos de sesion (fecha, escenario, alumno) presentes.

## 4) Integracion y aislamiento

- [ ] Ensamblados (`asmdef`) sin referencias circulares.
- [ ] Integracion opcional no rompe cuando falta un modulo no requerido.
- [ ] Escena demo reproducible en entorno limpio.
- [ ] No hay dependencias editor-only en runtime.

## 5) Calidad de release

- [ ] README y documentacion sincronizados con el comportamiento real.
- [ ] Changelog actualizado.
- [ ] Licencias y terceros revisados.
- [ ] Prueba final en proyecto Unity limpio antes de empaquetar.

## 6) Publicacion

- [ ] Package exportado para Asset Store.
- [ ] Materiales de listing revisados (descripcion, capturas, keywords).
- [ ] Version taggeada internamente para trazabilidad.

