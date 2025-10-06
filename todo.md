TODO – Sitio “Sanador Virtual”

1. Páginas del sitio

Inicio (/)

Mensaje principal: telemedicina accesible para comunidades rurales de Oaxaca; enfoque cultural y lenguas indígenas.

Estudio de Mercado_FINAL

Estudio de Mercado_FINAL

Beneficios rápidos: triaje por IA, teleconsulta segura, modo offline, historias clínicas, costo bajo.

Estudio de Mercado_FINAL

CTAs: “Pedir información del piloto” (pacientes) y “Soy clínica” (B2B).

Estudio de Mercado_FINAL

Características (/caracteristicas)

Tarjetas con: Triaje IA, Teleconsulta, Historias clínicas, Soporte en lenguas, Modo offline-first (explicar cada una en 2–3 líneas).

Estudio de Mercado_FINAL

Precios (/precios)

Micropago por consulta (meta: <$50 MXN como referencia), y espacio para planes/alianzas/subsidios.

Estudio de Mercado_FINAL

Estudio de Mercado_FINAL

Clínicas (/clinicas)

Beneficios para clínicas rurales: atención remota, reducción de traslados, requisitos mínimos de conectividad, apertura a pilotos.

Estudio de Mercado_FINAL

Estudio de Mercado_FINAL

Mini FAQ B2B: adopción en 12 meses si demuestra ahorro/impacto.

Estudio de Mercado_FINAL

Promotores (/promotores)

Rol de promotores de salud comunitarios, materiales descargables y registro de interés.

Estudio de Mercado_FINAL

FAQ (/faq)

Temas: conectividad intermitente, privacidad de datos, idiomas, cómo funciona el triaje/teleconsulta.

Estudio de Mercado_FINAL

Contacto (/contacto)

Formulario simple (pacientes, clínicas, prensa/alianzas). Mencionar interés en regiones rurales y posibles socios (IMSS-Bienestar/ONGs).

Estudio de Mercado_FINAL

Privacidad y Términos (/privacidad, /terminos)

Tratamiento de datos sensibles en telemedicina; lenguaje claro y accesible (pendiente revisión legal).

2.Contenido por página (resumen práctico)

Inicio

Hero con promesa de valor + botón “Únete al piloto”.

3–5 beneficios con iconos (IA, offline, lenguas, costo, seguridad).

Bloque “Cómo funciona” en 3 pasos (Triaje → Teleconsulta → Seguimiento).

Testimonio corto (comunidad/promotor).

CTA final doble: Pacientes / Clínicas.

Características

Una sección por feature con ejemplo sencillo (texto + ilustración).

Nota sobre funcionamiento en baja conectividad y lenguas.

Estudio de Mercado_FINAL

Precios

Tarjeta de “pago por consulta” (<$50 MXN como meta/objetivo) + espacio para convenios.

Estudio de Mercado_FINAL

Aclaración: precios sujetos a piloto y subsidios locales.

Estudio de Mercado_FINAL

Clínicas

Beneficios en viñetas (menos traslados, acceso a especialistas, historiales digitales).

“¿Listos para un piloto?” + formulario.

Conectividad: estable/intermitente (indicaciones).

Estudio de Mercado_FINAL

Promotores

Qué harás como promotor, recursos imprimibles, capacitación básica.

Formulario para recibir materiales/seguimiento.

Estudio de Mercado_FINAL

FAQ

8–12 preguntas con respuestas cortas (datos, conectividad, idiomas, seguridad).

Enlace a Contacto.

Blog

Publicaciones cortas, enfoque educativo y progreso del piloto.

Estudio de Mercado_FINAL

Contacto

Campos mínimos + selector de tipo de interés (Paciente/Clínica/Prensa/Alianzas).

3.Detalles técnicos para la Landing (Astro)

Proyecto base

npm create astro@latest sanador-virtual-web

Integraciones recomendadas: @astrojs/tailwind (o CSS propio), @astrojs/sitemap.

Estructura simple:

/src
/components # Header, Footer, Hero, Feature, CTA, Testimonial
/layouts # BaseLayout.astro
/pages # index.astro, otras
/i18n # es.ts, (placeholders para lenguas locales)
/public

Componentes mínimos de la landing

<Header/> con logo + selector de idioma.

<Hero/> (título, subtítulo, CTA principal).

<FeatureList/> (grid 3–5 features).

<HowItWorks/> (3 pasos).

<Testimonial/> (1–2 tarjetas).

<CTASection/> (botones Pacientes/Clínicas).

<Footer/> con links a FAQ, Precios, Contacto.

i18n básico

Diccionario es y placeholders para 1–2 lenguas indígenas priorizadas (definir más adelante).

Estudio de Mercado_FINAL

Selector de idioma sencillo (no bloquear lanzamiento si faltan traducciones).

Formularios (landing)

Form “Únete al piloto” (nombre, comunidad, WhatsApp/SMS, idioma preferente).

Envío a un endpoint simple (Cloudflare Workers/Netlify Functions) o servicio de formularios.

Mensaje de confirmación accesible y claro.

Rendimiento y SEO

Imágenes optimizadas (Astro <img/> con loading="lazy").

Metadatos OG/Twitter y <link rel="alternate" hreflang="..."> cuando i18n esté listo.

Lighthouse objetivo: >90 en Performance/SEO/Accesibilidad.

Accesibilidad rápida

Contraste AA, foco visible, navegación por teclado.

Alternativas de texto en imágenes.

Lenguaje sencillo y botones descriptivos.

Despliegue

Hosting estático (Vercel/Netlify/Cloudflare Pages).

@astrojs/sitemap + robots.txt.

Dominio propio cuando esté listo.
