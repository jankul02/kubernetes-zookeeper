FROM confluentinc/cp-zookeeper:6.2.0  
USER root
RUN dnf install https://dl.fedoraproject.org/pub/epel/epel-release-latest-8.noarch.rpm -y && dnf install dnf-plugins-core -y && \
  dnf install epel-release -y && yum -y install yum-utils && yum repolist && dnf -y install vim-enhanced  && \
    dnf install http://rpms.remirepo.net/enterprise/remi-release-8.rpm -y && \
    dnf update -y && \
    dnf install -y wget && \
    dnf update
    
    #  && \
    # dnf install snapd -y && \
    # systemctl enable --now snapd.socket && \
    # ln -s /var/lib/snapd/snap /snap && \
    # snap install tcpdump   
 
USER root
COPY --chown=appuser:appuser scripts /etc/confluent/docker/

