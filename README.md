# Send A Email Notification Using Ansible Playbook with Gmail Authentication
[![Builds](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

----
# Description
This is an ansible playbook to Send a Email Notification Using Ansible Playbook with the help of a gamil account authentication

----
### Features 

This Ansible playbook will perform following operations;

- Use with any mail host (eg: gmail)
- Send email notfication to recepient address which we set.
- Can setup a notification from playbook side on CI/CD time

----
## How to Use

With Ansible installed, you are ready to Send Email Using Ansible Playbook via Gmail app password by following the below steps.
```sh
yum install git -y
amazon-linux-extras install -y ansible2
git clone https://github.com/yousafkhamza/Notification-Ansible.git
cd ansible-email
```
###  Open the file 'email.yml' and update the Email login credentials and recipiant address which you need.

The Sample format is provided below,
```sh
        host: smtp.gmail.com
        port: 587
        username: "username@gmail.com"
        password: "email password"
        to: Yousaf K Hamza <yousaf.k.hamza@gmail.com>
        subject: Notification-from-Ansible
        body: 'System {{ ansible_hostname }} has been successfully provisioned.'
```

- host :  Hostname of Email Server
- port: SMTP port number
- username: Username of email 
- password: Gmail app password or your email normal password
- to: Recpient Email address

Run the ansible-playbook from your master server by below command,

```sh
$ ansible-playbook email.yml
```

----
# Conclusion

It's just a simple playbook for sending a notification from ansible-playbook the main use case when we use any playbooks with automated tools with CI/CD time which that time we use this playbook. 


### ⚙️ Connect with Me

<p align="center">
<a href="mailto:yousaf.k.hamza@gmail.com"><img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>
<a href="https://www.linkedin.com/in/yousafkhamza"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/></a> 
<a href="https://www.instagram.com/yousafkhamza"><img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"/></a>
<a href="https://wa.me/%2B917736720639?text=This%20message%20from%20GitHub."><img src="https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white"/></a>
