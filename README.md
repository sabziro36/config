conn mytunnel

         auto=start
         authby=secret
         type=tunnel
         ike=3des-sha1;modp2048
         keyexchange=ike
         phase2=esp
         phase2alg=aes-sha2
         pfs=no
         compress=no
         leftsubnets={10.5.5.0/30.192.168.100.0/24,224.0.0.0/24}
         rightsubnets={10.5.5.0/30,172.16.100.0/24,224.0.0.0/24}
         left=10.5.5.1
         right=10.5.5.2
