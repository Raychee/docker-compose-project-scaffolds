FROM raychee/python3

RUN yum install -y gcc

ENTRYPOINT ["/entrypoint.sh"]
COPY entrypoint.sh /entrypoint.sh

COPY environment.yml /environment.yml
RUN conda env update -n root

COPY . /src/
