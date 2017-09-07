# docker-cyon-apache

build a cyon shared apache like container for local development

usage:

In your php project, create a compose file:

```
version: '2'
services:
  cyon:
    image: jangalinski/cyon-apache
    container_name: <YOUR_CONTAINER_NAME>
    ports:
      - "<YOUR_LOCAL_PORT>:80"
    volumes:
      - ./:/var/www/html
```

then run with `docker-compose up` and enjoy.