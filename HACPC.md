Set HAC guardian Login to Y and allow the HAC Utility (Registration->Utilities->Generate HAC credentials) to set Logins for Guardians and generate the access code.</br>
This is a change from some previous methods, due to the password encryption in eschool and a not great way to automate the process </br>
</br>
Additional SQL needed:</br>
<p>join reg
on
reg.student_id=reg_stu_contact.student_id</br>
where reg.current_status='A'</br>
and reg_stu_contact.contact_type='G'</br>
and reg_stu_contact.web_access<>'Y'
</p>
![image](https://user-images.githubusercontent.com/72268962/113721912-89cb9680-96b5-11eb-91f8-19bde97cce64.png)
![image](https://user-images.githubusercontent.com/72268962/113721964-964fef00-96b5-11eb-925b-6f6a950dd33d.png)

Please note our fields are unique here at RPS, you only need the Contact_ID and Student_ID in the hacparent.txt file
