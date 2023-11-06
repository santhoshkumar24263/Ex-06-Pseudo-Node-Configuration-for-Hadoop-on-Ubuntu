# Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu

## AIM

To implement Pseudo Node configuration for Hadoop on ubuntu

## Pre-requisites

a) jdk

Single-Node Configuration

1.	Create a dedicated user account for hadoop

![image](https://github.com/santhoshkumar24263/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/127171952/042ef74a-72f0-4042-a700-682124a636c0)

2.	Install java1.8 in folder /usr/local

![image](https://github.com/santhoshkumar24263/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/127171952/f0e6e94f-079e-4da9-ad0a-dc8c514ac424)


3.	Install Hadoop


![image](https://github.com/santhoshkumar24263/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/127171952/793dccf8-8fce-41dc-9d68-ac8d32bdafb9)



4.	Set the hadoop environment variables: Include the following lines in the
$HOME/.bashrc file


![image](https://github.com/santhoshkumar24263/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/127171952/e0cba209-8c43-41d6-9b0b-0cdf7004a904)


 
5.	Set hadoop environment variables: Include the following lines /etc/profile file


![image](https://github.com/santhoshkumar24263/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/127171952/c7bd3bf4-253d-4804-8f04-9b5a136cd758)



6.	Run the.bashrc & profile files from the $ prompt for updating the changes


![image](https://github.com/santhoshkumar24263/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/127171952/e6222f53-a6e4-4b9b-b8bc-86bca058a882)

![image](https://github.com/santhoshkumar24263/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/127171952/459924c0-56fc-4845-aa7d-9b90e9c5f9de)

![image](https://github.com/santhoshkumar24263/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/127171952/cca0142a-5e37-4df4-a232-560676a4663b)



7.	Configuration of the hadoop files: hadoop-env.sh, core-site.xml, mapred-site.xml, hdfs- site.xml and yarn-site.xml

path ::	/usr/local/hadoop-2.5.1/etc/hadoop

a)	hadoop-env.sh
Include the following lines in hadoop-env.sh file

![image](https://github.com/santhoshkumar24263/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/127171952/7fbd66ad-2051-47a1-ba89-a43d96d4e258)


b)	core-site.xml
Configure the directory for Hadoop to store its data files, the network ports it listens to, etc. Setup will use Hadoop’s Distributed File System (HDFS-single local machine)

![image](https://github.com/santhoshkumar24263/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/127171952/e3640959-6384-4965-b884-5d768ac60bb1)


 
Include the following lines in core-site.xml file between <configuration> and
</configuration> tags

![image](https://github.com/santhoshkumar24263/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/127171952/6e2f19da-646e-4c37-b8ad-2d2b94f3fc72)


c)	mapred-site.xml

 ![image](https://github.com/santhoshkumar24263/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/127171952/5ba2292f-1aef-491d-be84-6080de0259f9)


Include the following lines in mapred-site.xml file

 ![image](https://github.com/santhoshkumar24263/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/127171952/293ee142-9d7c-4e4b-970e-72a0470c9240)


d)	hdfs-site.xml
Include the following lines in hdfs-site.xml file


![image](https://github.com/santhoshkumar24263/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/127171952/d17e18ca-16fd-4514-b0df-fe9cb1821c85)



e)	yarn-site.xml
Include the following lines in yarn-site.xml file

![image](https://github.com/santhoshkumar24263/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/127171952/f4a463ac-a45d-4cd3-9bf4-77aa1facc477)


8.	Format the Hadoop File system implemented on top of the local file system using

![image](https://github.com/santhoshkumar24263/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/127171952/aeb767bb-9a8f-45c4-96e0-46cd99e419e2)


9.	Start Hadoop using

![image](https://github.com/santhoshkumar24263/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/127171952/ab37538d-77cf-431d-9b1c-d1a484aaffc4)


Explore Hadoop using http://localhost:50070/ from the browser	
 
10.	The commonly used HDFS Commands are as follows:


![image](https://github.com/santhoshkumar24263/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/127171952/6ec6863c-5951-4825-a7b8-d0c2ff38c44a)



11.	Create a directory ‘/input’ in HDFS

![image](https://github.com/santhoshkumar24263/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/127171952/bebbd11e-836d-4866-99c6-208abab85069)


12.	Copy the input files into the distributed file system

![image](https://github.com/santhoshkumar24263/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/127171952/e0327f0d-7027-4874-be5e-15f5b656e2bd)


13.	Run some of the examples provided

![image](https://github.com/santhoshkumar24263/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/127171952/67028405-3300-409a-b3b0-b78ec3129906)


14.	Examine the output files

![image](https://github.com/santhoshkumar24263/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/127171952/eaca9b09-f6f3-4a68-a467-010eec09838a)


Copy the output files from the distributed file system to the local file system and examine them:

![image](https://github.com/santhoshkumar24263/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/127171952/3e7793a5-516f-42a9-8a6e-14a125a41883)

 
or
View the output files on the distributed file system

![image](https://github.com/santhoshkumar24263/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/127171952/de6ae420-d1e6-4a14-806a-0047307ff6c1)


## Result:
Thus, the implementation of Pseudo Node configuration for Hadoop on ubuntu is successfully executed.
