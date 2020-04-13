## SSH Port Forwarding
tunnel From private network via public network with 8080 port
Go to private machine: 

```
ssh -R 8080:0.0.0.0:8080 -i "aws_creditial.pem" ec2-user@aws_hostname_or_ip
```
For client machine: 
Comment out the line in /etc/ssh/sshd_config file:
```
  GatewayPorts yes
```
