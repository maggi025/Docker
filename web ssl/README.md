#Web con ssl en Docker
#Docker compose
contiene la configuración que levanta los contenedores de nginx-duckdns-ssl
-Uso nginx y nginx-proxy para el funcionamiento web donde en la parte de entorno le direcciono la carpeta donde contengo mi archivo 'index.html'
-Uso duckdns ya que tengo configurado un dominio ahí y el servicio mantiene actualizada la ip pública para que siempre pueda estar activa la página
-Uso letsencrypt para aplicar el certificado ssl en la web que voy a levantar
