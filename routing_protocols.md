# ...choose your Projects for Routing!
<br/>
Here you find the list of available routing protocols.  

**Choose & Commit ... 2 students per group**


| Routing Protocol			| Description			          	| References	         | Team Members   | Presentation Date 
|:---------------------:|:---------------------------:|:--------------------:|:--------------:|:-----------------:|
| BMX6 & BMX7 | Mesh Routing Protocol | https://github.com/bmx-routing/ | Alexander, Moritz, Jonas | 22.6. 14:15 Uhr
| Babel | Mesh Routing Protocol | https://www.irif.fr/~jch/software/babel/ | Christin Rudolph | 29.6. 14:15 Uhr
| Batman-adv | Mesh Routing Protocol | https://www.open-mesh.org | Florian Wenzel, Andy Hattenhauer | 15.6.
| OLSR v1 | Optimized Link State Routing Protocol | http://www.olsr.org |Dinh Huy Nguyen  Philipp Büchler| 15.6.
| ISIS | Intermediate System to Intermediate System Protocol | https://en.wikipedia.org/wiki/IS-IS| Nico Trapp, Jennifer Haase 
| DSR |Dynamic Source Routing | https://en.wikipedia.org/wiki/Dynamic_Source_Routing| Valerius Begau, Oliver Schröder | 22.6.
| no talk| | | Maurice T. | 

# Important points/questions to consider while presenting a routing protocol
* What is the cool thing about your routing protocol ?
* Classification into links state / distance-path vector / something special
* ground truth / first publication / RFC ?
* What kind of networks are a typical use case for your routing protocol ?
* What is the routing metric about, how is it calculated? (e.g. hop-count, throughput, packet errors...)
* How well does your routing protocol scale ? (can you find a plot of scaling analysis - number of routers vs. memory usage/cpu usage/network load)
* Is there a public, open-source codebase and/or proprietary ? (e.g. Github Link ?)
* Who is the maintainer / Mailing List ? 

# OpenWrt VM playground
* make sure you can connecte to the 3 VMs of your team by ```telnet 170.30.1.1 210XY```
* check internet connectivity & dns (e.g. ping www.google.de)
* install routing protocol OLSR v1: ```opkg update``` und dann ```opkg install olsrd```

| Team Members   | # OpenWrt VM | Telnet Port | IP/netmask of **br-lan** |
|:--------------:|:------------:|:-----------:|:----------------:|
| **Alexander, Moritz, Jonas** | |||
|               | 1 | 21040 |  |
|               | 2 | 21041 |  |
|               | 3 | 21042 |  |
| **Christin** | |||
|               | 1 | 21050 |  |
|               | 2 | 21051 |  |
|               | 3 | 21052 |  |
| **Florian, Andy** | |||
|               | 1 | 21000 |  |
|               | 2 | 21001 |  |
|               | 3 | 21002 |  |
| **Dinh Huy, Philipp** | |||
|               | 1 | 21010 | 172.30.1.6/24 |
|               | 2 | 21011 | 172.30.1.7/24 |
|               | 3 | 21012 | 172.30.1.8/24 |
| Nico Trapp, Jennifer Haase |  |
| **Valerius, Oliver**| |||
|               | 1 | 21030 |  |
|               | 2 | 21031 |  |
|               | 3 | 21032 |  |
| **Maurice**| |||
|               | 1 | 21020 | 172.30.1.9 |
|               | 2 | 21021 | 172.30.1.10 |
|               | 3 | 21022 | 172.30.1.11 |


# list of public ssh keys to grand OpenWrt VM access
* Please generate a ssh public/private keypair und post the public key in the list below
* e.g. in a command line trigger: ```ssh-keygen -t rsa -b 4096```

Team or Student:	```public ssh-key```

* Alexander, Moritz, Jonas:
```ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAACAQCwqQQaLOL9kPS6TRNaNnjEy0OUqgrkFBb7Vx3tdMyZJoYC7F2rJTRCeS6l7xxWswMNaux+I5HZLIvuSXaxwingOtmDjIieW8mDAV8jbjD9peWUS5oA71TFmxeOG9tlLJFpeLy3zY19oteBDSJclhKm+V7a66RYMSeOs+GjnyeplbDJceQJA64tZUxZFa2KjBIcOYC4qlSBK3Cjry3qqyCryTcB1wTQzjHXV/GzS0z7at6sMKNlLrD8Dlr1ET1AdhHCSVbdUUgkSzddnIn6IklzijDXi304NqsHEElTJobReEmsXmTdrUoP2Ab/B1twwPmE2rb2ewQQYUsjOUqmlCPCXqUAv9U20R/eCvf1VyK/aaEOG0hqtz/W7idYhw5BJbF+Dm/rfxKihM0h6xKl9bw4QSpzbIg0nH7tgehvWVW7GLnobGSmrXvyp/dGpWRgcSgT+V/o3UfIVfMwIR7KHJ9/D6oa2DTLGtM3A6eKQa0bi7IhXdZiYRTVewfR3Of2jKpfTAwvINZxT0VvQJhiYdRcBoRjPWd2NkS/Itqy17SSWMdPckdfeamIpNq6z0bwgiaBWqDsX2jUa5Sd3zxjhhl/pCk/TDSeaKiH/bi5cr+XOCYGk0znwLqWUWM5vp82j+GC1fMOuvG3/g/VH/SYEeZG5IBt/54cvQ6vHUV0KlUOsw== jaaalexander@Alexanders-MBP.fritz.box```

* Florian, Andy:
```ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAACAQDJf8c473DNgoCn9OwErqLRs8KYrgxtKw0jLenGzu7C4aHIfyjflqNQAj4u3BLjFwiJHYrNKsfCKuZ9+SXXFyHHk53JeNAkTeXqjheiOglmg3tanSzFAe2GqxgPbfp/oiPyPXjDDUtA8bvK+WuPfkpxyh4HtgVF0vJLjKuhbKCaY5+OPkxZ/qI/vZ3idH6pr7xdWTuJO94mOtiUbjglpeP6wwUbB8lEfhVZMdlTR3RMqubKq9/oCDqmSiTqMXcH6OBUjPLTU/yAaErig0tBm5xK6122k3kJ6pJBuFsM1Cc++/d62N8SKsUUgss+SRzfJjxx4absN8kwVsodTQckJrBr1bNSHYdbWYgwO8BZCoXU5CgG5O6INgC15K6locuBpLyjM+7ZnFHyCBxXKClce1/xWhicvRyrUQLHFIrNO/gydap8ytCmri3dyBIRxOFkrxlSFWKxPKc0wpZ9XX5sgj774yK5d6ltEdEaVj2DKpIP9IgU1kaElCyhKH/6UboorWaq5GZ6J3rf0qgv+KTtaAOXEHpbAG+usn3oyauN2Jn+dOBnYkAK5LbBxTIpQVmpPpYW+y6RsQXVXXV3OMzfAJTj/1EzTyJHDaONQiDLP6nHKLg49wj1MY36XdWwR1v1oVEcv3LO2CUov0ZzjDFtM4jNqNWf6xxFfoOqXY2s3juygQ== mega-@Florian-MSI-PC```

* Dinh Huy, Philip:
```ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAACAQCWu6/8RRhDAsCFqyCmJLyRwoj2f/VbiD61NEiHKRHtyCB6cTuxfQJa4POtdAXgylxltNXLePWmoErwAlQqUBFhYX6lbt7wlOyArZcG5ftHjYAIgBsdAgKBWSOIdaj5pgDCIYY6hFaYxKIGiuSk/OjIKMw9yxtZFNAdsLDGlK2HnF6zdXs0GMJZvWKHpC3IQ7psA7MnvJyVE/9jdLELmEdpkiGVo21GFDFDJ2+WxAJSUuDPtku4osqUCqrAP3gg3gyLjjmuZgXeLSaz76oodzTDPCUU8Yu+3AIxOtFRkPD/k03MoFQxdPTVpoWwTpVxii3xEFla+9WIXfgBJnsJHEX/gtW02t81NStBTXjKt2GXzfm6997rqRClCebFdNFjeZq3DdDSy8LA/i+ao5xyqweP5xTVMuRcuWW+Mm/ZDFeKCqI/ciMzx1LFora8hHjh/kQwon4JWgIz6HBoe+XRk3YD5fpwYOf9cVE9sY8p7qmdvGPMbeOTMZzrmH4DBk9eBd3/0HLSv+OZIKdybe8VVXsVrGY9LNWMvYRCwf4R2OZflcNk1QNRsMqnCYdgceC1O1xXjsfF4x0C842CRrGgMD0VFBAN2+nngNaGnXP0XkQ3TbGwBztAaCPOYJGN5bOGSfRq4bDdLcuSWu717oZwyw73LqzWskg5D3Rcn+BPFidBAw== ginhavana@Gin-Havana```

* Maurice Töpfer: 
```ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAACAQDiuP9l8hT1dlynH2GFTs2OVZeKh50fkg87VMTYMy1A1H744LHNJVQag/2VjBajF/wHRdUfAYBlhf9DQ5B27DuptnmkYeqpLiGGErFTe0Zr3RTS/i7xPDYzFwEVu45V1O7FgUxzJ3Z+FtPo6mWu7sizeaZPg+Ah2zuTjSHySgxiFPYgAD8mVrhxazrwE66ZXYla+agkR3uSnVT28nlCUQFE+0004g3ePlFBTBzLQ/3jHprbl5hNrzPO5yNJ93wxs/USqpLba2GFtleNTLNhrgu8IR6qYw62MXYqxwu7z0dBsyZ6H70wtlo55gVivmu9xoPMNHz+TLmh8TuBa+lJJdPItqt+SwZzhXIyXhAkZpGkaHj4cpKoFG2s4Bj+HwKJg3iBfxnxF99CvU6LkCeLoV1mK9vK1e+zs5f9t/WcUxKhMt0kYZZ0R3y1hi6jAPjIefIIyrQK0nEHP6Slljapb7aIArp4oTPSXZJ/dVrgjS5fs3nv3cq4s5WHSP9wvVDc2uaVAVY6Y+T3YKOSdBOOuuSBjcHlIegf793rYqK8NWtuNcI2Y8yBB3vd//3rf2CwJoCQaCOFUs44fPHa5jRHjZ7i9iRGd8C98ZSQLFNAZpcVW1/kect38rNBSY9DYHKlMvj9u/X9RKl5f/ki4dKyRTZSVLIBV7o71daqvkeGLvaxmQ== maurice töpfer@DESKTOP-LQ6T8OE```

* Valerius, Olli:
```ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAACAQDQBxX7A69xuA+hcE07ZQOmE9NoVMfsbYhE12kc7iMlsERONnVZ20btVz/49r0FZxTElysktx13NX9FJjsUVUmeXcZU5pGRcSBdZ5rbu7Pdqx4yjiSPzx2n58gW8h9uN6TDl6taUvgf/eXDs33nnXCgfwznw6WFJgn2H/3ablrTKI1PHec2G6HiCmi2PRH565opbOqVM9HpeiCJ+tQOiZ6f7NYXICW9I2XMUf/oU5//PcAm9qfc5iIs8QCUQ9OQuNsmZe7QS3aLfv8kFyFb74Kel2/dUA0WbhUQQZqTPBwTCnwe4+sCl+P2c2Wvyn9EaSdFol6cc1A33hzV47lE2M0M1jBZKKWb4kO8DYBMGrH0Uw8hTtGGkwx/lX0O0vmR3DXwsr65DWndNZcvteRqSaflYhWd1EcpODFRW156sr5PZZPR20zDL7RO8kJRG/s2CMhCCu2iZG7uLxHn3/4YGCwP1vSVe5xBpqtmOdhH2R6C8f0/B46eXeamGILHgB1EO2fO82w2/kS8Pn2oaL5ndcr31Eay29UCp19O3PCw6X2zWwxSIW+N45EVbe92s2faJNEY8UM2fIuyVHvlw2mvHd2N3M+4SwFQcBV6yi9b+rbAdNK2ARPY0bBVK3sJfPwqmDrUtsnUmP47JC/TwhzZPqLyUejpdlkNp3A/EK6VyBA9jQ== valerius@LAPTOP-T5S6NION```

* Christin:
```ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAACAQDmG1H2gvygmBr5XQWzI5dyxyChHJ5Buln0DSGlbtrdcalpgj6K7rq50ym1tezQ8InmG/K+uuVR//TU0B3sj5kciPpFbnNLqQ+BdkknY5ZxpYCDOM18frij2pOoaiC6heSfNEMQxsnhI/u5/kPqqgJEoGugLR1cdWD6H75wOv2TvXixAKeftUHfrPn0rTpgX5U4WzvCLSUh7JFN18g2dAUUcivZYreddPIkbAUpEa52pmD0IoB6VidkiCeujArt78kex4Gib6hpsfFO3FfRRU5zBIm1zd00cM5IFVPK60Zo5rMR57QvoEv7i8J3JZhpw7905EPr34725gAYSaTA/m1CZINCmMSvibbkrT3E7BhRHLCZURTBwR6o3aHfOV/uZFrS9mX/v4qRQNKIgUddc2x1ts3cy4W3xGTEpR4G7SovG1dp1UTMNuaeOF3DExSH6iBfIgYeXSdt1keJNp0Tkd2w61hfybtKSi7qIimynnCRI3i3wR1rncejGPz6Qd2Sx84icGq0VqWWeVAyz8Q8zlBwVzjz9IKGWLEZ3jCVDLSpPU4rDX6M8G4h6cc34r+nDYoEimW/gda6lUwm/53XioymnebNI2cWu9yeXEKzkSllpyEV0ABNNw3uROJtJwupET8GRRZFNbd3Y7cXJsRusR2UWrG43MVVfjLbWqSJ4LesIQ== christin@LAPTOP-7SV26BR8```
