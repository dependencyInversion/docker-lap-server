# docker-lap-server
## Install



## Usage

### Building the conainer

1. Navigate into the repos directory using the terminal
2. Replace `<IMAGE_NAME>` with the image name you want e. g. `apache2-php` or `lap-server`
3. Run the command



```bash
docker build -t <IMAGE_NAME> .
```





### Start container

1. Navigate into the repos directory using the terminal
2. Use bash or replace `"$(pwd)"` with absolute path
3. Run the following command after replacing the placeholders



```bash
docker run --name <CONTAINER_NAME> \
  -d -p <PORT>:80 \
  --mount type=bind,source="$(pwd)"/htdocs,target=/var/www/html \
  <IMAGE_NAME>
```



## Resources

- [Running the Apache HTTP Server with PHP inside Docker](https://nelkinda.com/blog/apache-php-in-docker/)
