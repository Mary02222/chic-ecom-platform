# Glam Beauty Platform

Quiero crear una tienda online profesional de maquillaje llamada GLAM BEAUTY. No quiero una simple landing page ni una maqueta: quiero una plataforma ecommerce funcional, moderna, elegante, responsive y preparada para continuar desarrollándose en Visual Studio Code.



💗 TECNOLOGÍAS OBLIGATORIAS



La aplicación debe estar construida principalmente con:



- Python + Flask para backend y rutas.

- HTML5 + Jinja2 para las páginas.

- CSS3 para todo el diseño.

- JavaScript Vanilla solo para interacciones necesarias.

- SQLAlchemy para la base de datos.

- SQLite inicialmente, con estructura preparada para PostgreSQL.



NO utilizar React, Next.js, TypeScript ni otros frameworks como base principal. Quiero poder pasar posteriormente el proyecto a VS Code y ejecutarlo con:



"pip install -r requirements.txt"



y Flask.



Mantener una estructura organizada como:



glam_beauty/

├── app.py

├── config.py

├── requirements.txt

├── .env

├── models/

├── routes/

├── templates/

│   ├── base.html

│   ├── index.html

│   ├── productos.html

│   ├── producto.html

│   ├── carrito.html

│   ├── checkout.html

│   ├── login.html

│   ├── registro.html

│   ├── perfil.html

│   └── admin/

└── static/

    ├── css/style.css

    ├── js/main.js

    └── images/



🎀 DISEÑO



Glam Beauty debe sentirse como una marca de maquillaje real, premium y moderna, no como una página escolar.



Paleta:



- Blanco

- Rosa pastel

- Rosa empolvado

- Crema

- Beige claro

- Detalles sutiles champagne/dorado



Usar mucho espacio en blanco, tarjetas elegantes, bordes suaves, sombras delicadas, microanimaciones y tipografías modernas/elegantes.



Debe funcionar perfectamente en PC, tablet y celular.



🛍️ PÁGINA PRINCIPAL



Crear una homepage espectacular con:



- Header con logo, Inicio, Tienda, Categorías, Ofertas, Nosotros, Contacto, buscador, usuario y carrito.

- Hero/banner con imagen o video, frase de marca y botones "Comprar ahora" y "Explorar productos".

- Categorías: Rostro, Ojos, Labios, Cejas, Brochas, Skincare, Accesorios y Sets.

- Productos destacados.

- Novedades.

- Ofertas.

- Productos más vendidos.

- Beneficios de compra.

- Banner visual de Glam Beauty.

- Footer con redes sociales, WhatsApp, correo, políticas y métodos de pago.



Agregar badges como Nuevo, Oferta y Best Seller.



💄 PRODUCTOS



Crear catálogo "/productos" con:



- Búsqueda.

- Filtros por categoría, precio, disponibilidad y ofertas.

- Ordenar por precio, popularidad y novedades.



Cada producto debe tener página individual con:



- Imágenes y galería.

- Video opcional.

- Nombre.

- Categoría.

- Descripción.

- Precio y descuento.

- Stock.

- Tonos/variantes.

- Ingredientes.

- Modo de uso.

- Reseñas.

- Favoritos.

- Productos relacionados.

- Agregar al carrito.

- Comprar ahora.



🛒 CARRITO Y CHECKOUT



Carrito funcional con:



- Agregar/eliminar productos.

- Modificar cantidades.

- Subtotal, descuentos y total.

- Cupones.

- Productos e imágenes.

- Checkout.



Checkout con:



1. Datos del cliente.

2. Dirección.

3. Método de envío.

4. Método de pago.

5. Resumen.

6. Confirmación.



Dejar preparada la estructura para integrar posteriormente Wompi, Mercado Pago, PayPal o Stripe, sin almacenar datos bancarios sensibles.



👤 USUARIOS



Crear registro e inicio de sesión real mediante Flask.



Registro:



- Nombre.

- Apellido.

- Correo.

- Contraseña.

- Teléfono opcional.



Agregar:



- Inicio/cierre de sesión.

- Recuperación de contraseña.

- Contraseñas hasheadas.

- Flask-Login.

- Preparación para Google OAuth.



Crear "/perfil" con:



- Datos personales.

- Direcciones.

- Pedidos.

- Historial.

- Favoritos.

- Cambio de contraseña.



Crear "/favoritos".



📱 WHATSAPP



Agregar botón flotante de WhatsApp que abra una conversación con Glam Beauty y permita utilizar un mensaje automático.



El número debe poder modificarse desde el panel administrativo.



👑 PANEL ADMINISTRATIVO



Crear "/admin", completamente protegido mediante autenticación y rol "admin".



Debe incluir un dashboard con:



- Ventas totales.

- Ventas del día/mes.

- Pedidos.

- Clientes.

- Productos activos.

- Productos agotados.

- Stock bajo.

- Gráficas de ventas y productos más vendidos.



Inventario



Crear "/admin/inventario".



El administrador debe poder:



- Agregar productos.

- Editarlos.

- Eliminarlos.

- Activarlos/desactivarlos.

- Cambiar precios.

- Cambiar descuentos.

- Modificar stock.

- Establecer stock mínimo.

- Subir imágenes/videos.

- Gestionar tonos y variantes.



Cuando se confirme una compra, el stock debe disminuir automáticamente.



Si llega al mínimo, mostrar alerta. Si llega a 0, mostrar Agotado y bloquear la compra.



Registrar movimientos:



- Entrada.

- Salida.

- Ajuste.

- Devolución.



Pedidos



Crear "/admin/pedidos" para visualizar clientes, productos, total, fecha, pago, dirección y estado.



Estados:



Pendiente → Confirmado → Preparando → Enviado → Entregado / Cancelado



Usuarios



Crear "/admin/usuarios" para consultar y gestionar usuarios y roles.



Configuración



Crear "/admin/configuracion" para modificar:



- Logo.

- Nombre.

- Correo.

- WhatsApp.

- Redes sociales.

- Dirección.

- Horarios.

- Costos de envío.

- Métodos de pago.

- Banners.

- Productos destacados.



🗄️ BASE DE DATOS



Crear una base de datos REAL mediante SQLAlchemy.



Modelos principales:



- User

- Product

- Category

- ProductVariant

- Cart

- CartItem

- Order

- OrderItem

- Favorite

- Review

- Address

- Coupon

- InventoryMovement

- Payment

- ContactMessage



Relacionarlos correctamente mediante claves foráneas.



🔐 SEGURIDAD



Implementar:



- Contraseñas hasheadas.

- Flask-Login.

- Roles y permisos.

- Protección de rutas.

- Validación de formularios.

- ORM contra SQL injection.

- Variables ".env".

- Ninguna contraseña, API key o secreto en el frontend.

- Verificación del rol administrador desde backend.



✨ DETALLES "WOW"



Agregar cuando sea apropiado:



- Wishlist.

- Productos relacionados.

- Productos recientemente vistos.

- Recomendaciones.

- Newsletter.

- FAQ.

- Contacto.

- Sobre nosotros.

- Notificaciones.

- Toasts.

- Loading states.

- Skeleton loaders.

- Animaciones suaves.

- Página 404.

- Estados vacíos.

- Buscador dinámico.



No saturar el diseño: todo debe seguir siendo minimalista, elegante y premium.



💋 PRODUCTOS DEMO



Agregar productos de ejemplo como:



- Base.

- Corrector.

- Rubor.

- Iluminador.

- Labial.

- Gloss.

- Máscara de pestañas.

- Paleta de sombras.

- Brochas.

- Sets.



Usar imágenes atractivas y coherentes con la identidad de Glam Beauty.



🎯 OBJETIVO FINAL



Quiero que al abrir Glam Beauty la reacción sea:



"Esto parece una tienda de maquillaje real."



Debe ser funcional, visualmente impresionante, segura, organizada y escalable, pero sobre todo fácil de trasladar y continuar en Visual Studio Code con Python + Flask + HTML + CSS + JavaScript.



Antes de finalizar, comprobar que funcionen correctamente el registro, login, carrito, productos, CRUD, inventario, pedidos, usuarios, panel admin, base de datos y rutas protegidas.



Si alguna función externa como Google OAuth, pagos, almacenamiento de imágenes o variables de entorno requiere configuración adicional, dejarla preparada y explicar exactamente qué debo configurar posteriormente.

This project was built with [Lovable](https://lovable.dev).

## Build with Lovable

Continue developing this project in the [Lovable editor](https://lovable.dev/projects/b34c63c7-223f-4f71-98ed-6030d0b86379).

- **Ship faster**: describe what you want to build and Lovable handles the code.
- **Stay in sync**: every change made in Lovable is committed straight to this repository.
- **Full ownership**: this code is yours. Push to `main` on GitHub and your changes sync back into Lovable, ready for your next prompt.

## Development

Prefer working locally? You need Node.js and npm — [install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating).

```sh
git clone <this-repository-url>
cd <repository-name>
npm i
npm run dev
```
