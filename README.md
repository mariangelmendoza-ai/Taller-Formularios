<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Registro de Nuevo Producto</title>
</head>
<body>

    <h1>Registro de Nuevo Producto</h1>
    <p>Rellene el siguiente formulario para registrar un nuevo producto.</p>

    <form action="/submit-product-data" method="POST">

        <div>
            <label for="nombre_producto">Nombre del producto</label>
            <input type="text" id="nombre_producto" name="nombre_producto" placeholder="Introduzca el nombre del producto" required>
        </div>
        <div>
            <label for="sku_producto">SKU del producto</label>
            <input type="text" id="sku_producto" name="sku_producto" placeholder="Introduzca el SKU del producto">
        </div>

        <div>
            <label for="descripcion_producto">Descripción del producto</label>
            <textarea id="descripcion_producto" name="descripcion_producto" rows="4" placeholder="Introduzca la descripción del producto"></textarea>
        </div>

        <div>
            <h3>Categoría del Producto</h3>
            <div>
                <input type="radio" id="cat_electronica" name="categoria" value="electronica" checked>
                <label for="cat_electronica">Electrónica</label>
            </div>
            <div>
                <input type="radio" id="cat_ropa" name="categoria" value="ropa">
                <label for="cat_ropa">Ropa</label>
            </div>
            <div>
                <input type="radio" id="cat_hogar" name="categoria" value="hogar">
                <label for="cat_hogar">Hogar y Jardín</label>
            </div>
        </div>

        <div>
            <label for="fabricante">Fabricante / Proveedor</label>
            <select id="fabricante" name="fabricante">
                <option value="fabricante_a">Fabricante A</option>
                <option value="fabricante_b">Fabricante B</option>
                <option value="fabricante_c">Fabricante C</option>
            </select>
        </div>

        <div>
            <h3>Opciones</h3>
            <div>
                <input type="checkbox" id="destacado" name="opcion_destacado" value="si">
                <label for="destacado">Producto destacado</label>
            </div>
            <div>
                <input type="checkbox" id="envio" name="opcion_envio" value="si">
                <label for="envio">Disponible para envío</label>
            </div>
        </div>
        
        <div>
            <label for="fecha_lanzamiento">Fecha de lanzamiento</label>
            <input type="date" id="fecha_lanzamiento" name="fecha_lanzamiento">
            </div>
        <div>
            <label for="hora_oferta">Hora de oferta especial</label>
            <input type="time" id="hora_oferta" name="hora_oferta">
        </div>
        <div>
            <label for="color_principal">Color principal</label>
            <input type="color" id="color_principal" name="color_principal" value="#000000">
        </div>

        <div>
            <label for="cantidad_stock">Cantidad en stock</label>
            <input type="number" id="cantidad_stock" name="cantidad_stock" value="0" min="0">
        </div>
        <div>
            <label for="calidad_producto">Calidad del producto</label>
            <input type="range" id="calidad_producto" name="calidad_producto" min="0" max="100" value="50">
        </div>

        <div>
            <label for="url_producto">URL del producto</label>
            <input type="url" id="url_producto" name="url_producto" placeholder="https://ejemplo.com">
        </div>
        <div>
            <label for="email_soporte">Email de soporte</label>
            <input type="email" id="email_soporte" name="email_soporte" placeholder="soporte@ejemplo.com">
        </div>
        <div>
            <label for="telefono_contacto">Teléfono de contacto</label>
            <input type="tel" id="telefono_contacto" name="telefono_contacto" placeholder="123-456-7890">
        </div>
        
        <div>
            <label for="buscar_etiquetas">Buscar etiquetas</label>
            <input type="text" id="buscar_etiquetas" name="buscar_etiquetas" placeholder="Buscar...">
            <button type="button">Elegir archivos</button>
        </div>
        <div>
            <label for="imagenes_producto">Imágenes del producto</label>
            <input type="file" id="imagenes_producto" name="imagenes_producto" multiple>
            <span>Ningún archivo seleccionado</span>
        </div>
        
        <div>
            <button type="reset">Limpiar Formulario</button>
            <button type="submit">Registrar Producto</button>
        </div>

    </form>
</body>
</html>
