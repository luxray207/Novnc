### CARA RUN
unzip wanz.zip

docker build -t novnc-desktop .

docker run -it --rm \
  -e USERNAME=andi \
  -e VNC_PASSWORD=rahasia \
  -e NOVNC_PORT=9090 \
  -e DISPLAY_RESOLUTION=1600x900 \
  -p 9090:9090 \
  novnc-desktop
