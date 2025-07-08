FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
ADD https://raw.githubusercontent.com/Tarunuu/terraform-aws-vpc/refs/heads/main/peering.tf /usr/share/nginx/html/index.html
CMD ["nginx", "-g", "daemon off;"]