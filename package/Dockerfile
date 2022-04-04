FROM registry.suse.com/suse/sle15:15.3
RUN zypper -n update && \
    zypper -n clean -a && \
    rm -rf /tmp/* /var/tmp/* /usr/share/doc/packages/* /usr/share/doc/manual/* /var/log/*
COPY bin/webhook /usr/bin/
USER 1000
CMD ["webhook"]
