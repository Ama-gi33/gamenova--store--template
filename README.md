# GameNova — Plantilla de Tienda de Recargas Gaming

Plantilla web completa (HTML/CSS/JS, un solo archivo, sin dependencias) para montar una tienda de recargas de gemas/UC/Robux y gift cards. Diseño gaming original: fondo oscuro, azul neón + morado eléctrico, detalles dorados en ofertas.

![Preview](preview.png)

## ¿Qué incluye?

- **Inicio**: banner principal, juegos populares, ofertas destacadas, ventajas, métodos de pago.
- **Catálogo**: filtros por juego, buscador, tarjetas de producto con precio y descuento.
- **Checkout**: selección de paquete, ID de jugador, métodos de pago en criptomonedas (USDT TRC20/BEP20, BTC, ETH, USDC), muestra la wallet de cobro configurada.
- **Cuenta de usuario**: historial de pedidos, saldo, cupones.
- **Panel de administrador**: alta/edición de paquetes y precios, gestión de estado de pedidos (pendiente/completado), configuración de wallets de cobro y comisión de servicio (visible, nunca oculta).
- 100% responsive (móvil, tablet, escritorio).
- Persistencia de pedidos y ajustes vía `localStorage` del navegador — funciona en cualquier hosting (no depende de ninguna plataforma), sin necesitar backend ni base de datos para empezar.

## Qué NO incluye (léelo antes de comprar)

- **No entrega gemas/UC/Robux reales de forma automática.** El flujo de pago es de confirmación manual: el cliente paga a tu wallet, tú verificas la transacción y marcas el pedido como completado, y entregas el saldo por tu cuenta (a mano, o conectando tu propio proveedor mayorista).
- **No incluye logos oficiales de los juegos** (Free Fire, PUBG, Mobile Legends, Roblox, PSN, Xbox, Nintendo, etc.). Son marcas de sus respectivos dueños — tú decides si usas íconos genéricos (como trae la plantilla) o consigues arte con licencia.
- No incluye pasarela de pago con tarjeta/banco ni integración con ningún proveedor de recargas — el código está preparado para que conectes la API del proveedor que elijas.
- Los pedidos y ajustes se guardan con `localStorage`, es decir, **por navegador/dispositivo**, no en un servidor central. Si el comprador quiere que el admin vea los pedidos desde cualquier dispositivo, necesita conectar una base de datos real (Firebase, Supabase, MySQL, etc.) — el código está estructurado para que eso sea un cambio simple en las funciones `storeGet`/`storeSet`.

## Escalar a base de datos real (opcional)

El archivo incluye, comentada justo arriba de las funciones de almacenamiento, una guía paso a paso para migrar de `localStorage` a **Supabase** (gratis, sin backend que programar) en menos de 10 minutos, además de la equivalencia para Firebase. Ideal para cuando el negocio crece y se necesita ver los pedidos desde cualquier dispositivo.

## Cómo usarla

1. Descarga el archivo `gamenova.html`.
2. Ábrelo en cualquier navegador — funciona directo, sin instalación.
3. Personaliza colores, nombre, juegos y precios editando el archivo (todo está comentado).
4. Configura tus wallets de cobro desde el panel Admin → Ajustes de cobro.

## Precio y licencia

Uso comercial permitido para un (1) proyecto/dominio. Incluye el archivo fuente completo, sin marca de agua.

**Para comprar acceso al código completo:**
Envía el pago a mi wallet USDT (BEP20): `TU_DIRECCION_AQUI` *(0x66d3804eD0c58FCa6Fd5f73a51B82Fa915ce1645)*
Luego escríbeme con el hash de la transacción:
- Telegram: [@amagi33](https://t.me/amagi33)
- Correo: elluismma@gmail.com

## Aviso

Esta es una plantilla de software. No es un negocio operativo, no garantiza ingresos, y quien la use es responsable de cumplir los términos de servicio de los juegos/plataformas con los que decida integrarla.
