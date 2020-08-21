# Componentes
## docker-compose.yaml
Contiene la configuración que levanta los contenedores de nginx-duckdns-ssl
-Uso nginx y nginx-proxy para el funcionamiento web. En nginx hace falta modificar estas lineas con tu información para que funcione
  
  
  `  volumes:
    
      - directorio donde esta el index.html:/usr/share/nginx/html:ro
     
    environment:
    
      - VIRTUAL_HOST=tuhost.duckdns.org
      - LETSENCRYPT_HOST=tuhost.duckdns.org
      - LETSENCRYPT_EMAIL=tumail@prueba.com
  `
      


-Uso duckdns ya que tengo configurado un dominio ahí y el servicio mantiene actualizada la ip pública para que siempre pueda estar activa la página
  En este módulo hay que configurar estas lineas:


`    environment:
    
      - TZ=America/Argentina/Buenos aires
      - SUBDOMAINS=tusubdominio
      - TOKEN=11111111111111111
`
       


-Uso letsencrypt para aplicar el certificado ssl en la web que voy a levantar


## index.html
Contiene una página sensilla para utilizar como prueba de funcionamiento del sistema. 

