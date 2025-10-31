AIM- To launch a Windows Virtual Machine (VM) in AWS and access it from a local Windows system. 

Procedure: Step 1: Login to AWS Console
 1. Open a web browser and go to amazon free tier account. 
2. Click on sign in to the console using your AWS credentials.
 3. From the AWS Management Console, search for Ec2 and open the EC2 dashboard.
 Step 2: Launch a Windows Instance 
1. Click on launch instance.
 2. Enter the Instance name. 
3. Under Application and OS Images (AMI), select Microsoft Windows Server 2022 Base 4. Choose Instance Type → t2.micro
 5. Under Key Pair (Login) → click Create new key pair → download the .pem file.
 6. In Network Settings, add a rule to Allow RDP from My IP. 
7. Leave other settings default and click Launch Instance.
 Step 3: Retrieve Windows Password 
1. Go to EC2 → Instances → Select your instance.
 2. Wait until the instance state shows Running. 
3. Click Connect → RDP client tab → Get Password. 
4. Upload the downloaded .pem file and click Decrypt Password.
 5. Note down the Username: Administrator and the Decrypted Password. 
Step 4: Connect to the Instance from Local Machine
 1. On your Windows system, press Windows + R, type mstsc, and press Enter. 
2. In the Remote Desktop Connection window, enter the Public IPv4 Address of the instance.
 3. Click Connect.
 4. Enter the credentials: ◦ Username: Administrator ◦ Password: (Decrypted password from AWS) 
5. Click OK and accept the certificate warning. 
Step 5: Access the Windows Server 
1. The Windows VM desktop will appear in a new window.
 2. You can now operate it like a normal Windows system — install software, browse, etc. Result: Successfully launched a Windows Virtual Machine in AWS and accessed it from the local Windows system using Remote Desktop Protocol (RDP).

 YOUTUBE LINK:
 https://youtu.be/xLb5y3eoSco
