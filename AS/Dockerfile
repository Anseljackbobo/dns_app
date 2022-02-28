FROM python:3-onbuild


ENV TINI_VERSION v0.9.0
RUN chmod +x /tini
ENTRYPOINT ["/tini", "--"]

# Exposes port 10053 by default
EXPOSE 53533 53533/udp

# Run python
CMD ["python", "auth_server.py"]
