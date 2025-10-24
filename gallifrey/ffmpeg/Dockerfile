ARG UBUNTU_VERSION="noble"

FROM ubuntu:${UBUNTU_VERSION}
# Arguments
ARG UBUNTU_VERSION
ARG TARGETARCH
ARG FFMPEG_VERSION="7.1.2-2"
ARG FFMPEG_DEB_FILE="jellyfin-ffmpeg7_${FFMPEG_VERSION}-${UBUNTU_VERSION}_${TARGETARCH}.deb"
ARG FFMPEG_DEB_URL="https://github.com/jellyfin/jellyfin-ffmpeg/releases/download/v${FFMPEG_VERSION}/${FFMPEG_DEB_FILE}"

ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update && \
    apt-get install -y --no-install-recommends \
        software-properties-common \
        curl \
        openssh-server \
        ca-certificates && \
    add-apt-repository universe && \
    apt-get update && \
    echo "Downloading ${FFMPEG_DEB_URL}" && \
    curl -fL -o /tmp/${FFMPEG_DEB_FILE} ${FFMPEG_DEB_URL} && \
    apt-get install -y /tmp/${FFMPEG_DEB_FILE} && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/* /tmp/*

RUN ln -s /usr/share/jellyfin-ffmpeg/ffmpeg /usr/bin/ffmpeg && \
    ln -s /usr/share/jellyfin-ffmpeg/ffprobe /usr/bin/ffprobe && \
    ln -s /usr/share/jellyfin-ffmpeg/vainfo /usr/bin/vainfo

RUN sed -i 's/#PermitRootLogin prohibit-password/PermitRootLogin no/' /etc/ssh/sshd_config && \
    sed -i 's/#PasswordAuthentication yes/PasswordAuthentication no/' /etc/ssh/sshd_config && \
    mkdir -p /var/run/sshd && \
    chmod 0755 /var/run/sshd

EXPOSE 22

CMD ["/usr/sbin/sshd", "-D"]