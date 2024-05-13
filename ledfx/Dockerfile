ARG BUILD_FROM
FROM $BUILD_FROM

# Install dependencies
RUN apt-get update && apt-get install -y \
    python3-pip \
    libportaudio2 \
    && rm -rf /var/lib/apt/lists/*

# Install LEDFx
RUN pip3 install ledfx

# Copy data
COPY rootfs/ /

# Set the entry point
CMD [ "/run.sh" ]
