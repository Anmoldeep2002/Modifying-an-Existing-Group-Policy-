<h1>Modifying an Existing Group Policy (Account Lockout Policy)</h1>


<h2>Description</h2>
<p>In this section, I want to access the "GROUP POLICY MANAGEMENT" section for this domain. That's because I want to view the current policies and change the "ACCOUNT LOCKOUT" policy that is now in operation. This will make the domain more secure against unauthorised access and lock accounts if the password is incorrectly typed many times.</p>


<br />

<h2>Step-by-Step Walk-Through:</h2>


<p align="center"> 
STEP 1: <br/>
<img src="https://i.imgur.com/81NOMhG.png" height="70%" width="70%"/> </p>


<p align="center">So, the first step would be to access "SERVER MANAGER" and then "Group Policy".</p>


<hr width="100%" size="2">

<br />

<p align="center"> 
STEP 2: <br/>
<img src="https://i.imgur.com/2kvJ0fe.png" height="40%" width="40%"/> </p>


<p align="center">I navigate to the "Tools" area and then select "GROUP POLICY MANAGEMENT". This allows me to view the "Group Policy" section of the domain "office123.com".</p>


<hr width="100%" size="2">

<br />

<p align="center"> 
STEP 3: <br/>
<img src="https://i.imgur.com/jEehClo.png" height="70%" width="70%"/> </p>


<p align="center">As you can see, this is the "GROUP POLICY" section for the domain "office123.com". As you can see, there are plenty of options available, but in this case, I selected the "Default Domain Policy" section, which is located directly beneath the domain name.</p>


<br />
<br />

<p align="center"> 
<img src="https://i.imgur.com/TUIXPiS.png" height="70%" width="70%"/> </p>


<p align="center">As can be seen, this is the domain's group policy section. In this scenario, I am interested in the "Account Policies/Lockout Policy" area. As you can see, the "Account lockout threshold" is now set to zero. This is not secure, and it indicates that there is no account lockout system in place to protect the domain in the event of unauthorised access. A user has an unlimited amount of attempts to log in to the device, which is extremely risky for an organisation.</p>


<hr width="100%" size="2">

<br />

<p align="center"> 
STEP 4: <br/>
<img src="https://i.imgur.com/vWN2G8O.png" height="40%" width="40%"/> </p>


<p align="center">To update the "Account Lockout Policy", I first right-clicked on the domain policy section and then selected "EDIT". This will allow me to modify the policy.</p>


<br />
<br />

<p align="center"> 
<img src="https://i.imgur.com/oHnrVi3.png" height="70%" width="70%"/> </p>

<br />
<br />

<p align="center"> 
<img src="https://i.imgur.com/zGBZiC0.png" height="70%" width="70%"/> </p>



<p align="center">Now I'm in the "EDIT" section of the domain policy. I then open the "Policies" folder to access other policies. Then I click on the "Security Settings" section to view the domain's security policies.</p>

<hr width="100%" size="2">

<br />

<p align="center"> 
STEP 5: <br/>
<img src="https://i.imgur.com/oEmXxoS.png" height="70%" width="70%"/> </p>


<p align="center">From here, I click on "Account Policies," which allows me to access the policies in effect for all the user accounts in the domain. In this example, I'm interested in the "Account Lockout Policy" area, so I click on it to view its options.</p>


<hr width="100%" size="2">

<br />

<p align="center"> 
STEP 6: <br/>
<img src="https://i.imgur.com/NRevcue.png" height="70%" width="70%"/> </p>


<p align="center">As you can see, I am in the "Account Lockout Policy" section, and there are 4 settings that can be adjusted. All of the policies have no value specified, therefore they are extremely unsecure; you can see that the "lockout duration" and "account lockout threshold" are set to "NOT DEFINED". In the second image below, I've modified the policies to reflect a more secure policy for the domain. I increased the lockout time to 30 minutes and the threshold to 5 logon attempts. This implies that after 5 incorrect login attempts, the account will be locked for 30 minutes. After 30 minutes, the account will be unlocked again.</p>


<br />
<br />

<p align="center"> 
<img src="https://i.imgur.com/1XdxCdh.png" height="70%" width="70%"/> </p>


<p align="center">Now I'm back on the main "Default Domain Policy" page, checking to see if the domain's "Account Policies" have been updated globally. As you can see, the changes were applied successfully and will be reflected for all domain users. The domain is now more secure, preventing unauthorised access.</p>


<a href="https://www.example.com">
  <button>NEXT</button>
</a>
