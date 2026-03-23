<h2 align="center">AWS 3-Tier Architecture Setup</h2>

<h2 align="center">Steps to be followed</h2>

<p align="center">
  <img src="https://github.com/rama001jha/AWS-Projects/blob/676ff40d1edfff482f9b2350f9d3d7db0435ce45/04-AWS-3-tier-architecture/images/Screenshot%202026-03-23%20185126.png" 
       alt="AWS 3 Tier Architecture Diagram" 
       width="900"/>
</p>

<br>
<br>
<br>

<h2 align="center">Step 1: VPC Creation</h2>

<div dir="rtl">
  <p>Go to the VPC service in AWS Management Console.</p>
  <p>Click on "Create VPC" and select "VPC only".</p>
  <p>Provide the name as "3tierapplication".</p>
  <p>Enter the IPv4 CIDR block as 10.0.0.0/16.</p>
  <p>Select the default tenancy option.</p>
  <p>Click on "Create VPC" to complete the setup.</p>
</div>


<br>
<br>
<br>


<p align="center">
  <img src="https://github.com/rama001jha/AWS-Projects/blob/85a72369fc244669d3fe5afe6944c2234cebe618/04-AWS-3-tier-architecture/images/Screenshot%202026-03-23%20191107.png" 
       alt="AWS 3 Tier Architecture Diagram" 
       width="1000"/>
</p>

<br>
<br>
<br>

<p align="center">
  <img src="https://github.com/rama001jha/AWS-Projects/blob/85a72369fc244669d3fe5afe6944c2234cebe618/04-AWS-3-tier-architecture/images/Screenshot%202026-03-23%20191122.png"
       alt="AWS 3 Tier Architecture Diagram" 
       width="1000"/>
</p>

<br>
<br>
<br>

<p align="center">
  <img src="https://github.com/rama001jha/AWS-Projects/blob/85a72369fc244669d3fe5afe6944c2234cebe618/04-AWS-3-tier-architecture/images/Screenshot%202026-03-23%20191152.png"
       alt="AWS 3 Tier Architecture Diagram" 
       width="1000"/>
</p>

<br>
<br>
<br>

<h2 align="center">Step 2: Create Subnets</h2>

<div dir="rtl">
  <p>Go to the Subnet section in the AWS VPC service and click on "Create subnet".</p>
  <p>Select your VPC named "3tierapplication".</p>
  <p>Create six subnets in total, two for the web tier, two for the application tier, and two for the database tier.</p>
  <p>Provide the IPv4 CIDR blocks for each subnet according to the architecture design.</p>
  <p>Ensure that the database tier subnets are created in different availability zones for high availability.</p>
  <p>Click on "Create subnet" to complete the setup.</p>
</div>

<br>
<br>

<p align="center">
  <img src="https://github.com/rama001jha/AWS-Projects/blob/b9e2dcd372f0538394cb19e49490aa3ae26a8d16/04-AWS-3-tier-architecture/images/screencapture-ap-south-1-console-aws-amazon-vpcconsole-home-2026-03-23-19_57_47.png"
       alt="AWS 3 Tier Architecture Diagram" 
       width="1000"/>
</p>

<br>
<br>
<p> database subnet in different availability zones</p>
  
<p align="center">
  <img src="https://github.com/rama001jha/AWS-Projects/blob/b9e2dcd372f0538394cb19e49490aa3ae26a8d16/04-AWS-3-tier-architecture/images/Screenshot%202026-03-23%20200417.png"
       alt="AWS 3 Tier Architecture Diagram" 
       width="1000"/>
</p>

<br>
<p>After creation of subnet</p>
<br>

<p align="center">
  <img src="https://github.com/rama001jha/AWS-Projects/blob/b9e2dcd372f0538394cb19e49490aa3ae26a8d16/04-AWS-3-tier-architecture/images/Screenshot%202026-03-23%20195919.png"
       alt="AWS 3 Tier Architecture Diagram" 
       width="1000"/>
</p>

<br>
<br>

<h2 align="center">Step 3: Setting up the Internet gateway</h2>


