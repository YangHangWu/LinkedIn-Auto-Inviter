# LinkedIn-Auto-Inviter
## Main Function
It a convenient tool that helps every job seeker asks for a referral on LinkedIn with a simple python file and Chrome webdriver.
After the one time setup, the only thing you need to modify is change the url of the people you want to ask for referral and the company name. 
The Auto-Inviter will send the connection request (according to the number you set) and send the message notes to the connectors.

## Motivation 
To every job seeker, I know it's challenge to get the first job or internship. 
The whole job seeking process is frustrated because you have to apply hundreds or even thousands of applications to get a few interview opportunities. 
One of the approaches to enhance your chance to stand out from the other applicants is to ask for a referral or connection from the current employees.   
However, not everyone on LinkedIn is willing to build up a connection with a stranger on LinkedIn. 
You have to request connections with more than 10 persons and maybe one of them will respond you.
As a software engineer, I am enthusiastic about applying programming skills to real world, which improves our lives. 
Therefore, I came out with this idea to build up a LinkedIn-Auto-Inviter which can automatically ask for a referral on LinkedIn (save lots of time)!!!  
I do get several offers with this tool so I decided to publish it to public. I hope it can somehow help people who are still struggling.

## Prerequisite
### Python Version and Package
  This project supports python 3.x (I use python 3.7.4)
  <pre><code>pip3 install selenium==4.1.0</code></pre>
### Webdriver
#### Step 1: Check Chrome Version
##### Step 1.1 Go to the 'Settings' of your chrome browser.
<img width="1913" alt="截圖 2022-03-04 上午2 07 09" src="https://user-images.githubusercontent.com/39996866/156744617-278974cd-1b4d-4e1a-914b-d9d1fdc2f633.png">. 

##### Step 1.2 Go to 'Advanced' -> 'About Chrome' to check the version
<img width="1334" alt="截圖 2022-03-04 上午2 07 46" src="https://user-images.githubusercontent.com/39996866/156744931-71cbf22a-2fa2-4fde-aaa4-ff9425876f0c.png">
(Here shows my version of Chrome is 98.xxxx). 

#### Step 2: Download Chrome Webdriver
##### Step 2.1 Go to Selenium website and find out the corresonding version of Chrome webdriver [link](https://chromedriver.storage.googleapis.com/index.html)
##### Step 2.2 Download folder according to your operation system (my laptop is 2020 M1 mac please choose the .zip file according to your os)
<img width="756" alt="截圖 2022-03-04 上午2 28 48" src="https://user-images.githubusercontent.com/39996866/156747036-c3f44bbc-e118-49ec-a268-5b02d8aeff9f.png">

##### Step 2.3 Install to your operation system and move chromedriver to the same floder as the .ipynb
<img width="227" alt="截圖 2022-03-04 上午2 34 51" src="https://user-images.githubusercontent.com/39996866/156747685-50a7182d-207a-4c7b-8de3-05dd62536ea2.png">

### Google Chrome Profile
To avoid the login process on LinkedIn, this program will load google chrome profile so that there is no need to deal with the login process.
(make sure you have already use the auto login on your current google account). 
#### Step 1: Find Out Chrome Profile 
##### Step 1.1 Go to your chrome browser and run the command
  <pre><code>chrome://version/</code></pre>
##### Step 1.2 Find out your profile path
<img width="582" alt="截圖 2022-03-04 下午1 07 41" src="https://user-images.githubusercontent.com/39996866/156841738-a91f164c-9fe6-4d8d-a9d9-603b9025086e.png">.   

(Here shows my file path is '/Users/yanghangwu/Library/Application Support/Google/Chrome/Profile 2')

## How to use?
### Step 1: Find the people you would like to connect with by using the build in filter on LinkedIn and copy the url
<img width="1433" alt="截圖 2022-03-04 下午1 38 24" src="https://user-images.githubusercontent.com/39996866/156845347-8ea98073-3d33-4900-bfc0-1a2ddd5d7189.png">

### Step 2: Parameters Settings
Open Auto_Inviter.ipynb and find the cooreponding code
  <pre><code>
  company_url = 'url of people on LinkedIn you would like to build up connection with'
  company_name = 'company name' 
  num = the number of invitations
  # Note: please don't sent too many invitations at the same time otherwise you will be blocked by the system, my personal experience LOL
  msg = 'the note which will add on invitations'
  </code></pre>
  
  <pre><code>
  # One time setting
  user_profile_path = 'your chrome profile path'
  chromedriver_path = 'your chromedriver path'
  </code></pre>
  
### Step 3: Run Auto_Inviter.ipynb, it should work like the video below.


https://user-images.githubusercontent.com/39996866/156856877-4773ef2b-2a18-4548-b89d-1ae33a1c207e.mp4




  
