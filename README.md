# Public-CDN

## Hoja de estilos: `PIS`

Esta hoja de estilos contiene variables CSS y clases utilitarias para botones, tablas, modales y otros componentes de interfaz, especialmente pensados para integrarse con Ant Design y estilos personalizados.

### Variables CSS

- **Colores:** Definidos bajo `:root` como `--color-gob-*`, `--color-action-*`, y `--color-brand-*` para temas de color institucional y de acciones (éxito, error, advertencia, etc).
- **Bordes y radios:** Variables como `--radius-*` y `--stroke-*` para controlar esquinas redondeadas y grosores de borde.

### Clases principales

#### Botones

- `.ant-btn`, `.ant-btn-default`, `.ant-btn-warning`, `.ant-btn-info`, `.ant-btn-danger`, `.ant-btn-success`, `.ant-btn-reload`, `.ant-btn-enviar`, `.ant-btn-new`, `.ant-btn-view`, `.ant-btn-download`, `.ant-btn-edit`, `.ant-btn-delete`, `.ant-btn-add`
  - **Uso:** Añade la clase al botón para aplicar el estilo correspondiente.
  - **Ejemplo:**
    ```html
    <button class="ant-btn ant-btn-warning">Advertencia</button>
    <button class="ant-btn ant-btn-success">Éxito</button>
    ```

#### Tablas

- `.ant-table-striped`
  - Aplica un fondo alternado a las filas de la tabla.
- `.has-container-data`
  - Resalta las celdas de la tabla con un fondo verde claro.
- `.ant-table-thead > tr:first-child > th`, `.ant-table-thead > tr:nth-child(2) > th`, `.ant-table-thead > tr:nth-child(3) > th`
  - Estilos para los encabezados de la tabla, diferenciando colores por fila.

#### Modales

- `.custom-modal`
  - Mejora la apariencia de los modales de Ant Design.
- `.modal`, `.modal-dialog`, `.modal-content`, `.modal.show`
  - Estilos para modales personalizados.

#### Inputs y Selects

- `.ant-input-affix-wrapper`, `.ant-select:not(.ant-select-customize-input) .ant-select-selector`
  - Bordes redondeados y altura estándar para inputs y selects.

#### Otros

- `.dropzone`
  - Zona de arrastre para subir archivos.
- `.radio`
  - Estilo horizontal para grupos de radio buttons.
- `.error`
  - Texto de error en color rojo.
- `.reserved-day`
  - Fondo rojo claro y forma circular para días reservados en calendarios.
- `.ant-tag`
  - Estilo para etiquetas.

### Ejemplo de uso

```html
<button class="ant-btn ant-btn-success">Guardar</button>
<table class="ant-table-striped has-container-data">
  <thead>
    <tr><th>Columna 1</th><th>Columna 2</th></tr>
  </thead>
  <tbody>
    <tr><td>Dato 1</td><td>Dato 2</td></tr>
  </tbody>
</table>
<div class="custom-modal">
  <!-- contenido del modal -->
</div>