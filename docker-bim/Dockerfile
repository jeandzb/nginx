FROM registry.cn-beijing.aliyuncs.com/alphesh-soft/nginx:1.29.3
ENV TZ=Asia/Shanghai
COPY conf /etc/nginx/
RUN mkdir -p /var/cache/nginx /var/log/nginx \
    && touch /tmp/nginx.pid \
    && chown -R nginx:nginx /var/cache/nginx /var/log/nginx /etc/nginx /tmp/nginx.pid
USER nginx