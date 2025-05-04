FROM ubuntu:20.04

# 환경 설정 및 필수 패키지 설치
RUN apt-get update && \
    apt-get install -y gnupg curl apt-transport-https lsb-release

# 패키지 목록 갱신 및  vsftpd 설치
RUN apt-get update && \
    apt-get install -y vsftpd curl && \
    apt-get clean

# Elastic GPG 키 등록
#RUN curl -fsSL https://artifacts.elastic.co/GPG-KEY-elasticsearch | apt-key add -

# Elastic 8.x 저장소 등록
#RUN echo "deb https://artifacts.elastic.co/packages/8.x/apt stable main" \
#    | tee /etc/apt/sources.list.d/elastic-8.x.list

# filebeat 설정 파일은 나중에 복사하거나 bind mount로 연결

