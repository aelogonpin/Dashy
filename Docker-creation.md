El -v para la redirección del fichero

metele un port-forward para que funcione con el ngrok


docker run -d \
  -p 8080:80 \
  -v ~/my-conf.yml:/app/public/conf.yml \
  --name my-dashboard \
  --restart=always \
  lissy93/dashy:latest
