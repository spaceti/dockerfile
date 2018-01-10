FROM python:3.6.4-alpine3.7
LABEL maintainer: "Sergey Shkarupa <s.shkarupa@gmail.com>"

RUN apk --no-cache add libffi-dev openssl-dev build-base && \
    pip install -U --no-cache-dir --disable-pip-version-check ansible && \
    apk --no-cache del --purge build-base libffi-dev openssl-dev

CMD ["ansible-playbook", "--version"]
