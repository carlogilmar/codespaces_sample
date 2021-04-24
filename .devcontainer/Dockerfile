FROM centos
# Install basic utilities
RUN yum -y install gcc openssl-devel bzip2-devel libffi-devel zlib-devel tree wget curl make git ncurses-devel
# Download erlang
RUN wget http://erlang.org/download/otp_src_23.2.tar.gz
RUN tar -zxf otp_src_23.2.tar.gz && rm -rf otp_src_23.2.tar.gz
RUN cd otp_src_23.2 && ./configure && make && make install
