# More

Each of the following solutions has been proven to be effective and We hope to be helpful to you.

## Domain binding

The precondition for binding a domain is that Scratch can accessed by domain name.

Nonetheless, from the perspective of server security and subsequent maintenance considerations, the **Domain Binding** step cannot be omitted.

Scratch domain name binding steps:

1. Connect your Cloud Server
2. Modify [Nginx vhost configuration file](/stack-components.md#nginx), change the **server_name**'s value *__* to your Domain name
  ```text
    server {
    listen 80;
    server_name _;   # _ to your Domain name
    root /data/wwwroot/scratch-gui/build;
    }
   ```
3. Save it and restart [Nginx Service](/admin-services.md#nginx)


## Other

Coming soon
