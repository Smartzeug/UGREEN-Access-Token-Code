Codeschnipsel aus diesem Video https://youtu.be/5OmSyJgb-y4

<img width="2902" height="1388" alt="Screenshot 22 07 2025 um 18 39 02 PM" src="https://github.com/user-attachments/assets/8aa3230d-b3f8-4915-90f4-8e707cbf7b14" />


```
services:
  token-api:
    image: ghcr.io/tom-bom-badil/ugreen-api-token:latest
    container_name: ugreen-api-token
    ports:
      - "4115:4115"
    environment:
      UGREEN_NAS_API_SCHEME: "https"
      UGREEN_NAS_API_PORT: "9443"
      UGREEN_NAS_API_VERIFY_SSL: "false"
      USERNAME: "Masteradmin   "
      PASSWORD: "cynkoc-8kadfu-Mifkis"
    extra_hosts:
      - "host.docker.internal:host-gateway"
    restart: unless-stopped
```
