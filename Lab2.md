1. Creating VPC with CIDR 10.0.0.0/16.
![image](https://user-images.githubusercontent.com/126765452/230574104-8894b173-df03-48f7-991e-8f7696569023.png)

 2. Creating subnets & attach to VPC.
 ![image](https://user-images.githubusercontent.com/126765452/230574274-dac29b69-84d1-43c7-bd23-d6aeccd97ce3.png)


3. Creating Gateway & Attach gateway to VPC and attach to public subnet.
![image](https://user-images.githubusercontent.com/126765452/230574394-d4b4613f-a3ed-4410-b405-20c0e4540350.png)
![image](https://user-images.githubusercontent.com/126765452/230574413-f594c5f1-37db-4218-acf5-4e450a0ffd63.png)


4. For public subnet: edit routing table and create pub-instance with Bootstrapping to install and start Apache2 HTTP Server.
![image](https://user-images.githubusercontent.com/126765452/230574513-d519d923-5d2a-4bcb-9d04-e3e00ea74d9f.png)
![image](https://user-images.githubusercontent.com/126765452/230574552-5be14c24-f75b-45ed-a277-673df6be8a60.png)
![image](https://user-images.githubusercontent.com/126765452/230574611-a12c32a8-6988-47d6-968d-938d2f175cd8.png)
![image](https://user-images.githubusercontent.com/126765452/230574643-a98d3105-6159-4b09-a1c3-e9f821697e3b.png)


5. Opening web page for public instance.
![image](https://user-images.githubusercontent.com/126765452/230574732-00ca8892-baef-480e-991f-600b8275faad.png)


6. For private subnet: add NAT gateway in public subnet and attach to route table of private subnet.
![image](https://user-images.githubusercontent.com/126765452/230574863-e8d6fdfd-f605-4ff8-8d08-cbe895e7ed4b.png)
![image](https://user-images.githubusercontent.com/126765452/230574888-e36c1fd1-e35f-4d7b-a273-f5092a54a595.png)


7. Creating new instance in private subnet and install apache2 without ssh(using user data).
![image](https://user-images.githubusercontent.com/126765452/230574972-58b6c2d6-1af5-49e4-ad95-2c028868e1c0.png)
![image](https://user-images.githubusercontent.com/126765452/230574996-146b7264-6e7a-4e3a-96ce-5f16762b8ffa.png)
