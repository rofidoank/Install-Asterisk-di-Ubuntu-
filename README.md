# Install Asterisk di Ubuntu
### Langkah-langkahnya sebagai berikut.

<p>$ sudo su</p>
<p>$ apt-get update</p>
<p>$ apt-get upgrade</p>
<p>$ apt-get install asterisk</p>
<p>$ nano /etc/asterisk/sip.conf</p><hr>
<p>[nomor telepon]</p>
<p>type=friend</p>
<p>context=telepon</p>
<p>username=nama kalian</p>
<p>secret=sesuai kalian</p>
<p>host=dynamic</p><hr>
<p>$ nano /etc/asterisk/extensions.conf</p><hr>
<p>exten => nomor telepon,1,Dial(SIP/nomor telepon)</p><hr>
<p>$ service asterisk restart</p>



