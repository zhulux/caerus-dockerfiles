FROM elasticsearch:2.4
MAINTAINER Daniel Wei <danielwii0326@gmail.com>

ADD https://raw.githubusercontent.com/danielwii/docker_base_scripts/master/entrypoint.sh /entrypoint.sh
RUN chmod +x /entrypoint.sh

RUN usermod -u 1000 elasticsearch

ENTRYPOINT ["/entrypoint.sh"]
CMD ["gosu", "elasticsearch", "elasticsearch"]