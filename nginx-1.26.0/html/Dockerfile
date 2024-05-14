# Используем официальный образ Nginx в качестве базового
FROM nginx:latest

# Копируем HTML-файлы и другие файлы сайта в контейнер
COPY html/ /usr/share/nginx/html/

# Удаляем стандартную конфигурацию Nginx
RUN rm /etc/nginx/conf.d/default.conf

# Копируем свою конфигурацию Nginx (если необходимо)
COPY nginx.conf /etc/nginx/nginx.conf
