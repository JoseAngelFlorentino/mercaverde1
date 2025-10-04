# Merca Verde

Merca Verde es una aplicación móvil multiplataforma desarrollada en Flutter cuyo objetivo es contribuir a la reducción del desperdicio alimentario en la República Dominicana. La aplicación pone en contacto a productores, comercios y consumidores mediante un marketplace digital sostenible, permitiendo que excedentes de alimentos sean comercializados a precios asequibles.

## Características principales
- Registro e inicio de sesión mediante Supabase Auth.  
- Publicación y administración de productos por comercios/productores.  
- Visualización de catálogo con filtros (por categoría, ubicación).  
- Reserva o compra de productos.  
- Pagos digitales seguros (Stripe).  
- Mapas y rutas de entrega con Mapbox.  
- Notificaciones push mediante Firebase Cloud Messaging (FCM).  
- Modelo de negocio híbrido: B2C con suscripción para consumidores y B2B para comercios/productores.

## Arquitectura resumida
- **Frontend:** Flutter + Riverpod (gestión de estado) + GoRouter (navegación).  
- **Backend:** Supabase (PostgreSQL, Auth, Realtime, Storage, Edge Functions).  
- **Servicios externos:** Stripe API (pagos), Mapbox (mapas), Firebase Cloud Messaging (notificaciones).  
- **Infraestructura / CI-CD:** integración continua mediante GitHub Actions (o similar), despliegue en servicios escalables (AWS u otro).  

## Estructura del repositorio (resumen)
- `lib/` — código fuente Flutter  
- `android/` — plataforma Android  
- `ios/` — plataforma iOS  
- `test/` — pruebas unitarias o de integración (cuando se agreguen)  
- `pubspec.yaml` — dependencias del proyecto  
- `README.md` — este archivo  
- `.gitignore` — archivos ignorados  
- `analysis_options.yaml` — reglas de lint / estilo  

## Requisitos previos
- Tener instalado Flutter SDK compatible.  
- Tener una cuenta de Supabase con un proyecto configurado.  
- Claves de API para Stripe, Mapbox, FCM.

## Configuración e instalación
1. Clona el repositorio:
   ```
   git clone https://github.com/JoseAngelFlorentino/mercaverde1.git
   cd mercaverde1
2. Instala dependencias:
   ```
   flutter pub get
   ```
3. Configurar variables de entorno en .env
   ```
   SUPABASE_URL=your-supabase-url
   SUPABASE_ANON_KEY=your-supabase-key
   STRIPE_KEY=your-stripe-key
   MAPBOX_KEY=your-mapbox-key
4. Ejecutar la app en emulador
  ```
    flutter run
```
## Equipo

- Gabriel Alba – Líder de Proyecto
- Rafael Roa – Frontend Developer
- Agner Díaz – Backend Developer
- José Florentino – QA / Testing

## Documentacion Relacionada
- Documento de Arquitectura v2.1
