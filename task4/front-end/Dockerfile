# Nginx-in ən son versiyasından istifadə edirik
FROM nginx:latest

# Front-end fayllarını konteynerin daxilinə köçürürük
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Öz konfiqurasiya faylımızı Nginx-in standart konfiqurasiyası ilə əvəz edirik
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf
