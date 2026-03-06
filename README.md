<!DOCTYPE html>
<html lang="es" class="scroll-smooth">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Alto Nivel Reformas - Reformas en Madrid</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            'rojo-principal': '#c8102e',    // rojo vivo como en muchas webs de reformas
            'rojo-oscuro': '#a00d24',
            'gris-claro': '#f8f8f8',
          }
        }
      }
    }
  </script>
</head>
<body class="bg-gray-50 font-sans text-gray-800">

  <!-- Header / Navbar -->
  <header class="bg-white shadow-md sticky top-0 z-50">
    <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-4 flex justify-between items-center">
      <div class="text-2xl font-bold text-rojo-principal">Alto Nivel Reformas</div>
      <ul class="hidden md:flex space-x-8">
        <li><a href="#inicio" class="hover:text-rojo-principal">Inicio</a></li>
        <li><a href="#servicios" class="hover:text-rojo-principal">Servicios</a></li>
        <li><a href="#nosotros" class="hover:text-rojo-principal">Nosotros</a></li>
        <li><a href="#contacto" class="hover:text-rojo-principal">Contacto</a></li>
      </ul>
      <a href="#contacto" class="bg-rojo-principal text-white px-6 py-3 rounded-md hover:bg-rojo-oscuro">Pídenos Presupuesto</a>
    </nav>
  </header>

  <!-- Hero -->
  <section id="inicio" class="bg-rojo-principal text-white py-20 md:py-32 text-center">
    <div class="max-w-5xl mx-auto px-4">
      <h1 class="text-4xl md:text-6xl font-bold mb-6">Reformas en Madrid</h1>
      <p class="text-xl md:text-2xl mb-10">Empresa especializada en reformas integrales, interiorismo y decoración. Más de 15 años transformando espacios.</p>
      <a href="#contacto" class="bg-white text-rojo-principal px-10 py-5 rounded-md text-xl font-semibold hover:bg-gray-100">Empieza tu reforma ahora</a>
    </div>
  </section>

  <!-- Servicios -->
  <section id="servicios" class="py-20 bg-white">
    <div class="max-w-7xl mx-auto px-4">
      <h2 class="text-4xl font-bold text-center mb-12 text-rojo-principal">Nuestros Servicios</h2>
      <div class="grid md:grid-cols-3 gap-8">
        <div class="bg-gris-claro p-8 rounded-lg shadow-lg hover:shadow-xl transition">
          <h3 class="text-2xl font-semibold mb-4">Reformas Integrales</h3>
          <p>Transformación completa de viviendas y locales con diseño personalizado y máxima calidad.</p>
        </div>
        <div class="bg-gris-claro p-8 rounded-lg shadow-lg hover:shadow-xl transition">
          <h3 class="text-2xl font-semibold mb-4">Reformas de Lujo</h3>
          <p>Materiales premium, acabados exclusivos y atención al detalle para proyectos de alto standing.</p>
        </div>
        <div class="bg-gris-claro p-8 rounded-lg shadow-lg hover:shadow-xl transition">
          <h3 class="text-2xl font-semibold mb-4">Reformas de Pisos y Locales</h3>
          <p>Aprovechamiento óptimo del espacio, rapidez y sin molestias innecesarias.</p>
        </div>
        <div class="bg-gris-claro p-8 rounded-lg shadow-lg hover:shadow-xl transition md:col-span-2">
          <h3 class="text-2xl font-semibold mb-4">Interiorismo Gratuito</h3>
          <p>Diseño profesional incluido en todos nuestros proyectos. Hacemos que tu idea cobre vida.</p>
        </div>
        <div class="bg-gris-claro p-8 rounded-lg shadow-lg hover:shadow-xl transition">
          <h3 class="text-2xl font-semibold mb-4">Reformas de Oficinas</h3>
          <p>Espacios productivos, modernos y adaptados a tu equipo.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Nosotros -->
  <section id="nosotros" class="py-20 bg-gris-claro">
    <div class="max-w-5xl mx-auto px-4 text-center">
      <h2 class="text-4xl font-bold mb-8 text-rojo-principal">¿Quiénes Somos?</h2>
      <p class="text-xl mb-10">Líderes en reformas en Madrid con +15 años de experiencia y más de 500 obras realizadas. Equipo propio: arquitectos, interioristas y oficiales cualificados. Sin intermediarios, calidad garantizada.</p>
      <a href="#contacto" class="bg-rojo-principal text-white px-10 py-5 rounded-md text-xl font-semibold hover:bg-rojo-oscuro">Conócenos mejor</a>
    </div>
  </section>

  <!-- Contacto / Formulario (Netlify Forms) -->
  <section id="contacto" class="py-20 bg-white">
    <div class="max-w-4xl mx-auto px-4">
      <h2 class="text-4xl font-bold text-center mb-12 text-rojo-principal">Pídenos Presupuesto GRATIS</h2>
      <form name="presupuesto" method="POST" data-netlify="true" class="space-y-6 max-w-lg mx-auto">
        <input type="hidden" name="form-name" value="presupuesto" />
        <input type="text" name="nombre" placeholder="Nombre completo" required class="w-full p-4 border border-gray-300 rounded-md focus:outline-none focus:border-rojo-principal" />
        <input type="email" name="email" placeholder="Email" required class="w-full p-4 border border-gray-300 rounded-md focus:outline-none focus:border-rojo-principal" />
        <input type="tel" name="telefono" placeholder="Teléfono" required class="w-full p-4 border border-gray-300 rounded-md focus:outline-none focus:border-rojo-principal" />
        <textarea name="mensaje" placeholder="Cuéntanos sobre tu proyecto (pisos, local, integral...)" rows="5" required class="w-full p-4 border border-gray-300 rounded-md focus:outline-none focus:border-rojo-principal"></textarea>
        <button type="submit" class="bg-rojo-principal text-white w-full py-4 rounded-md text-xl font-bold hover:bg-rojo-oscuro">Enviar y que te llamemos</button>
      </form>
      <p class="text-center mt-6 text-gray-600">O llámanos directamente: 91 778 62 53</p>
    </div>
  </section>

  <!-- Footer -->
  <footer class="bg-rojo-principal text-white py-8 text-center">
    <p>&copy; 2026 Alto Nivel Reformas - Reformas en Madrid | info@altonivelreformas.es</p>
  </footer>

</body>
</html>
