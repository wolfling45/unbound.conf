# unbound.conf

![unbound.conf](https://i.imgur.com/zoFgNsM.png)

[DNSCrypt](https://dnscrypt.org/) is a piece of lightweight software that everyone should use to boost online privacy and security. It works by encrypting all DNS traffic between the user and DNS resolver, preventing any spying, spoofing or man-in-the-middle attacks.

[Unbound](https://www.unbound.net/) is a validating, recursive, and caching DNS resolver. 

[NirCmd](http://www.nirsoft.net/utils/nircmd.html) is a small command-line utility that allows you to do some useful tasks without displaying any user interface.

## ʹ�÷���

* ���� [DNSCrypt 32-bit](https://download.dnscrypt.org/dnscrypt-proxy/dnscrypt-proxy-win32-full-1.7.0.zip)��[DNSCrypt 64-bit](https://download.dnscrypt.org/dnscrypt-proxy/dnscrypt-proxy-win64-full-1.7.0.zip)��[Unbound](http://unbound.net/downloads/unbound-1.5.9.zip)��[NirCmd 32-bit](http://www.nirsoft.net/utils/nircmd.zip)��[NirCmd 64-bit](http://www.nirsoft.net/utils/nircmd-x64.zip)

* ��ѹ`dnscrypt-proxy-win32-full-1.7.0.zip`��`dnscrypt-proxy-win64-full-1.7.0.zip`��`E:\Program Files\DNSCrypt\`����ѹ`unbound-1.5.7.zip`��`E:\Program Files\unbound\`����ѹ`nircmd.zip`��`nircmd-x64.zip`��`C:\Windows\System32\`

* ����[�����ļ�](https://github.com/CNMan/unbound.conf/archive/master.zip)����ѹ��`E:\Program Files\unbound\`

* ����ʵ������޸�[localdns.cmd](https://github.com/CNMan/unbound.conf/blob/master/localdns.cmd)��[�����ļ�](https://github.com/CNMan/unbound.conf/blob/master/unbound.conf)�е����Ŀ¼

* ����localdns.cmd����DNSCrypt��Unbound

* ���������������DNS���������ó�127.0.0.1

* ��localdns.cmd�ŵ�`C:\ProgramData\Microsoft\Windows\Start Menu\Programs\StartUp\`Ŀ¼�������Զ�����

![localdns](https://i.imgur.com/4WN9qit.png)

## ˵��

����hosts����������unbound.local-zone.hosts.conf����������Ͷ����������������unbound.local-zone.block.conf������˵���ɲο�[Unbound+DNSCrypt˫���շ�DNS��Ⱦ���ٳ�](https://goo.gl/IG3K27)

��������Ĭ����114.114.114.114��223.5.5.5������������[unbound.forward-zone.China.conf](https://github.com/CNMan/unbound.conf/blob/master/unbound.forward-zone.China.conf)����������Ĭ���ɼ�����9999�˿ڵ�DNSCrypt����

�޸�unbound�����ļ������ȼ����û�д������ã�������unbound��ˢ��DNS��������

```
cd /d "E:\Program Files\unbound\"
unbound-checkconf unbound.conf
unbound-control -c unbound.conf reload
ipconfig /flushdns
```

![unbound-control](https://i.imgur.com/FWjHwjh.png)

## ��л

* hosts�����б�ȡ��[https://github.com/racaljk/hosts](https://github.com/racaljk/hosts)

* ��������б�ȡ��[http://pgl.yoyo.org/adservers/serverlist.php?showintro=0](http://pgl.yoyo.org/adservers/serverlist.php?showintro=0)

* ������������б�ȡ��[http://www.malware-domains.com/files/immortal_domains.zip](http://www.malware-domains.com/files/immortal_domains.zip)

* ���������б�ȡ��[dnsmasq-china-list](https://github.com/felixonmars/dnsmasq-china-list)�����������������������Ҫ��ӣ���ֱ����`dnsmasq-china-list`��Ŀ����
