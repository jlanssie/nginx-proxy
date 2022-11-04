# nginx-proxy

An Nginx proxy for testing locally built web apps.

## Install Nginx 

Install Nginx

## Configure Nginx

Set the user (and user group on Mac brew installation), e.g. 

`user  me staff;`

Comment existing `server block` lines in nginx.conf but make sure configurations are still loaded.

## Open topics 

proxy.conf works for reaching local apps on a developer machine from a testing machine (e.g. a phone). But it only allows forward-proxying http requests. It will fail with `ERR_TUNNEL_CONNECTION_FAILED` on https requests.