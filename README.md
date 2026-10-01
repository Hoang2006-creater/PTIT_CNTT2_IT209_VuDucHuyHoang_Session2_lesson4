# Exercise 4 - UFW Firewall

## 1. Mục tiêu

Thiết lập UFW Firewall trên Ubuntu Server để chỉ cho phép các kết nối SSH và HTTP.

## 2. Cấu hình UFW

Đã thiết lập:

- Default incoming: DENY
- Default outgoing: ALLOW
- SSH: TCP port 22
- HTTP: TCP port 80

Các lệnh đã sử dụng:

```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw allow 22/tcp
sudo ufw allow 80/tcp
sudo ufw enable
sudo ufw status verbose