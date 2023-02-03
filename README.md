# Netflix Password Sharing With Vpn Risks / vulnerabilities

| Table of contents  | 
| ------------- |  
| [1.Situation](#situation)      | 
| [2.Risk](#risk)      | 
| [3.Proof of concept](#proof-of-concept) | 


## Situation

As of JAN 31, 2023, Netflix has decided to [crackdown](https://thestreamable.com/news/confirmed-netflix-unveils-first-details-of-new-anti-password-sharing-measures) on [password sharing](https://sea.ign.com/netflix-1/194903/news/netflix-unveils-plans-to-prevent-password-sharing).

Specifically: ```Users must log in to Netflix via their primary location's Wi-Fi network once every 31 days.```

Methods to circumvent this involve the usage of VPNs, namely:

![alt text](https://github.com/zlw9991/netflix-password-sharing-with-vpn-risks/blob/main/1.PNG)

^ Letting your friend's device temporarily connect to your VPN-Capable-and-vpn-enabled home router linked to your netflix account. 

![alt text](https://github.com/zlw9991/netflix-password-sharing-with-vpn-risks/blob/main/2.PNG)

^ Letting your friend's device temporarily connect to the VPN-Server software running on your PC / Device registered with your netflix account.

Such a connection involves the duration of watching one movie / episode? on netflix.

These techniques are documented [here](https://www.top10vpn.com/vpn-setup/home-vpn-server/).

## Risk

Naturally, connecting to a remote VPN server on the basis of 'trust' between 'friends' or 'shared netflix accounts you can trust to use and connect to' can be insecure, specifically (even more so when party which provides the VPN server insists on using old or insecure protocols):
  - IP Address [exposure](https://security.stackexchange.com/questions/29649/does-the-vpn-provider-know-my-dedicated-ip)
  - Scenarios where a user is convinced to:
    - Run an insecure VPN client.
    - Use an insecure VPN configuration.
    - Host an insecure VPN Server.
    - Connect to an insecure VPN server.

Documentation involving such risks are shown in these examples:
  -  https://www.exploit-db.com/exploits/34879
  -  https://arxiv.org/pdf/1912.04669.pdf#:~:text=We%20find%20that%20the%20VPN,VPN%20user's%20username%20and%20password
  -  https://rhinosecuritylabs.com/aws/cve-2022-25165-aws-vpn-client/
  -  https://medium.com/tenable-techblog/reverse-shell-from-an-openvpn-configuration-file-73fd8b1d38da
  -  https://www.bleepingcomputer.com/news/security/downloading-3rd-party-openvpn-configs-may-be-dangerous-heres-why/


## Proof of concept
WIP
