# Strapi Admin blog

Panel de administrador básico para un blog empleando sqlite y con los siguientes elementos:

- Artículo
- Autor
- Categoría

## Docker

Consta de dos entornos diferentes:

- Desarrollo:

```
# Construir imagen
docker build -t strapi:dev -f Dockerfile.dev
```

```
# Iniciar contenedor
docker run -p1337:1337 --env-file .env strapi:dev
```

- Producción:

```
# Construir imagen
docker build -t strapi:prod -f Dockerfile.prod
```

```
# Iniciar contenedor
docker run -p1337:1337 --env-file .env strapi:prod
```
