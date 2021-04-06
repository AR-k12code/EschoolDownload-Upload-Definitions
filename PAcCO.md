Parent HAC access code download, allows for searching by student ID </br>
Additional SQL:</br>
join reg_stu_contact</br>
on reg_contact.contact_id = reg_stu_contact.contact_id</br>
where reg_contact.ONBOARD_TOKEN NOT LIKE  '%-%'</br>

![image](https://user-images.githubusercontent.com/72268962/113720729-8c79bc00-96b4-11eb-890d-052d7314e2e3.png)
![image](https://user-images.githubusercontent.com/72268962/113720811-9dc2c880-96b4-11eb-8a86-1417342646eb.png)

Please note you can name the file whatever you would like, and set the deliminter whatever you would like.
