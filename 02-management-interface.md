## Management Interface Configuration 

### 1. Diagram
<img width="1040" height="814" alt="Image" src="https://github.com/user-attachments/assets/0c73bfe0-0a7e-4215-a094-129c79b5a871" />

### 2. Initial Configuration
Login to the device using the default credentials (admin / admin).

```
admin@fw> configure
admin@fw# set deviceconfig system type static
admin@fw# set deviceconfig system ip-address 192.168.100.100 netmask 255.255.255.0
default-gateway 192.168.100.1
admin@fw#commit
```
### 3. Create ZONE
<img width="1040" height="814" alt="Image" src="https://github.com/user-attachments/assets/5d4a451d-bd79-492c-aece-c5cd1cbbd72e" />

### 4. Virtual Router
A virtual router in Palo Alto Networks firewalls is a software-based routing framework 
that enables the firewall to perform Layer 3 routing functions, such as forwarding traffic 
between different networks based on destination IP addresses. Each Layer 3 interface, 
loopback interface, and VLAN interface on the firewall must be associated with a virtual router. 

Each Layer 3 interface (Ethernet, VLAN, loopback, etc.) on the firewall is assigned to 
a specific virtual router. This ensures that traffic traversing those interfaces is 
handled according to the routing rules defined for that virtual router. 
- Default Virtual Router
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/aee9d201-64ab-4e34-876d-74c877b667de" />

- Create a new Virutal Router
<img width="1888" height="972" alt="Image" src="https://github.com/user-attachments/assets/18aa517e-bc29-487a-8551-7bb393a9831a" />

- Create static route
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/2a8777b2-31a8-40a8-b369-3579e3fb81ab" />


### 4. Assign IP on Interface

- Add Interface to Virtual Router
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/af916959-363d-4e1e-b837-aeda6f978709" />

- Assign IP Address
<img width="1920" height="986" alt="image" src="https://github.com/user-attachments/assets/2eabd6a6-6492-4c57-8c65-413cc5d546c2" />

