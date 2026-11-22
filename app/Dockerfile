# the official nginx image runs every *.template in /etc/nginx/templates through
# envsubst into /etc/nginx/conf.d when it starts - only variables that are set
# are replaced, so nginx's own ($uri and so on) are left alone. default.conf.template
# therefore becomes conf.d/default.conf, in place of the image's stock site
FROM nginx:stable-alpine

COPY default.conf.template /etc/nginx/templates/
COPY html /var/www/html
