# Download and Install ESXCLI

***Support for linux-x86_64***
```
export VERSION_ESX=v1.0.0 && \
export V_ESX_CLI=6.7_U2_2 && \
mkdir -p /opt/vmware && \
wget -c https://github.com/tarcisiomiranda/esxcli_linux/archive/refs/tags/${V_ESX_CLI}.tar.gz -O - | tar -xz -C /tmp/ && \
cp -a /tmp/esxcli_linux-${V_ESX_CLI}/esxcli /opt/vmware/ && \
ln -s /opt/vmware/esxcli/esxcli /usr/bin/esxcli && \
esxcli --version
```


## Reference
- https://kb.vmware.com/s/article/66988
