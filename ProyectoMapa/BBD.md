Ciudad:
  id_ciudad (clave primaria)
  nombre_ciudad
  pais
  coordenadas_ciudad
  
Categoría de Sitio:
  id_categoria (clave primaria)
  nombre_categoria
  
Sitio de Interés:
  id_sitio (clave primaria)
  nombre_sitio
  descripcion
  coordenadas_sitio
  id_ciudad (clave foránea referenciando a Ciudad)
  id_categoria (clave foránea referenciando a Categoría de Sitio)



  Ejemplo de Datos:

Ciudad:
  
  1, "Ciudad A", "Pais A", [latitud, longitud]
  2, "Ciudad B", "Pais B", [latitud, longitud]
  
Categoría de Sitio:

  1, "Museo"
  2, "Parque"
  3, "Restaurante"

Sitio de Interés:

  1, "Museo de Arte", "Un museo increíble", [latitud, longitud], 1 (Ciudad A), 1 (Museo)
  2, "Parque Central", "Hermoso parque para pasear", [latitud, longitud], 2 (Ciudad B), 2 (Parque)
  3, "La Pizzería", "Deliciosa pizza italiana", [latitud, longitud], 1 (Ciudad A), 3 (Restaurante)



