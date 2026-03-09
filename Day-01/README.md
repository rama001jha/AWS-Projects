<h1 align="center">☁️ Day 01 – Introduction to AWS</h1>

<hr>

<h2>☁️ 1. What is Cloud Computing?</h2>

<p>
Cloud computing is the <b>on-demand delivery of computing resources</b> such as servers, storage, networking, and databases over the internet.
</p>

<p>
Instead of purchasing and maintaining physical servers, companies can rent infrastructure from cloud providers and pay only for what they use.
</p>

<h3>Example</h3>

<b>Earlier:</b>

<ul>
<li>Companies purchased physical servers , Managed hardware inside data centers , but many times suppose a server is of 100GB RAM and 10 core CPU but my application needs only 20GB RAM to run
 so most of the resources used to get wasted , so to tackle this problem the concept of virtualization was introduced where a virtual partition on servers was created to utilize the resources that
was being wasted and to create virtual separation on the server to run many applications on one physical server by creating virtual partitions of one server.</li>
</ul>

<b>Now:</b>

<ul>
<li>Infrastructure is rented from cloud providers like AWS , Resources are created and managed via the internet i.e, no need to create physical data centers of your own , you can rent infrastructure on the go and pay for only what you use , with no maintenance overhead of managing the data center.</li>
</ul>

<hr>

<h2>🌍 2. Types of Cloud Deployment Models</h2>

<h3>Public Cloud</h3>

<p>A public cloud is a type of cloud computing where servers, storage, and other resources are owned and managed by a cloud provider and shared with many customers over the internet.
Instead of buying your own computers and servers, you rent computing resources from a cloud company whenever you need them.

Simple Real-Life Example

Think of a public cloud like using electricity from the power grid. You do not build your own power plant You use electricity whenever needed You pay only for what you usePublic cloud works the same way.

Instead of owning servers:
The cloud provider owns the servers You access them through the internet You pay based on usage.</p>

<b>Examples:</b>

<ul>
<li>AWS</li>
<li>Microsoft Azure</li>
<li>Google Cloud Platform</li>
</ul>

<b>Benefits:</b>

<ul>
<li>No hardware management</li>
<li>Pay-as-you-go pricing</li>
<li>Highly scalable</li>
</ul>

<hr>

<h3>Private Cloud</h3>

<p>
Infrastructure dedicated to a single organization.
</p>

<b>Example:</b>

<ul>
<li>A company running its own internal data center</li>
</ul>

<b>Used when:</b>

<ul>
<li>Security requirements are strict</li>
<li>Sensitive data must remain private</li>
</ul>

<hr>

<h3>Hybrid Cloud</h3>

<p>
A combination of <b>public cloud</b> and <b>private cloud , where some resources are running on public cloud and some resources are running on private cloud.</b>.
</p>

<b>Example:</b>

<ul>
<li>Sensitive data stored in private infrastructure</li>
<li>Applications running on AWS</li>
</ul>

<hr>

<h2>🚀 3. Why Companies Move to the Cloud</h2>

<h3>Problems with Traditional Infrastructure</h3>

<ul>
<li>High hardware cost</li>
<li>Long infrastructure setup time</li>
<li>Difficulty scaling resources</li>
<li>Maintenance overhead</li>
</ul>

<h3>Benefits of Cloud Computing</h3>

<b>Scalability</b>
<ul>
<li>Increase or decrease resources based on demand</li>
</ul>

<b>High Availability</b>
<ul>
<li>Applications remain available even if one server fails</li>
</ul>

<b>Elasticity</b>
<ul>
<li>Resources automatically adjust based on workload</li>
</ul>

<b>Cost Efficiency</b>
<ul>
<li>Pay only for the resources you use</li>
</ul>

<hr>

<h2>🛠 4. Introduction to AWS</h2>

<p>
<b>Amazon Web Services (AWS)</b> is the world's most widely used cloud platform.
</p>

<p>
AWS provides <b>200+ cloud services</b> that help organizations build scalable and reliable applications.
</p>

<b>Core Service Categories:</b>

<ul>
<li><b>Compute</b> – EC2, Lambda</li>
<li><b>Storage</b> – S3</li>
<li><b>Networking</b> – VPC</li>
<li><b>Security</b> – IAM</li>
<li><b>Databases</b> – RDS</li>
</ul>

<hr>

<h2>🌐 5. AWS Global Infrastructure</h2>

<p>
AWS infrastructure is distributed globally to provide high availability and reliability.
</p>

<h3>Regions</h3>

<p>
A <b>Region</b> is a geographical area where AWS has multiple data centers.
</p>

<b>Examples:</b>

<ul>
<li>Asia Pacific (Mumbai)</li>
<li>US East (N. Virginia)</li>
</ul>

<h3>Availability Zones (AZ)</h3>

<p>
Each region contains multiple <b>Availability Zones</b>, which are isolated data centers.
</p>

<b>Benefits:</b>

<ul>
<li>High availability</li>
<li>Fault tolerance</li>
</ul>

<p>
If one Availability Zone fails, applications can continue running in another zone.
</p>

<hr>

<h2>☁️ Cloud Repatriation</h2>

<p>
<b>Cloud repatriation</b> is the process of moving applications, data, or workloads 
from a <b>public cloud environment</b> back to <b>on-premises infrastructure</b> or a 
<b>private cloud</b>.
</p>

<p>
In many cases, organizations initially migrate to the cloud to take advantage of 
scalability, flexibility, and faster infrastructure deployment. However, after some time,
they may decide to move certain workloads back to their own data centers.
</p>

<hr>

<h3>🔄 Example</h3>

<b>Cloud Migration</b>
<ul>
<li>Company moves applications from on-premises infrastructure to the cloud.</li>
</ul>

<b>Cloud Repatriation</b>
<ul>
<li>Company moves some workloads from the cloud back to its own data center.</li>
</ul>

<hr>

<h3>📌 Why Companies Choose Cloud Repatriation</h3>

<ul>
<li><b>Cost Optimization</b> – Running large, predictable workloads can sometimes be cheaper on owned infrastructure.</li>
<li><b>Performance Requirements</b> – Certain applications need very low latency and better hardware control.</li>
<li><b>Security & Compliance</b> – Some industries require strict control over sensitive data.</li>
<li><b>Workload Predictability</b> – Stable workloads may not need the elasticity provided by cloud platforms.</li>
</ul>

<hr>

<h3>⚡ Key Point</h3>

<p>
Cloud repatriation does not mean the cloud is bad. Most modern organizations use a 
<b>hybrid approach</b>, where some workloads run in the cloud while others remain 
on-premises to optimize cost, performance, and security.
</p>
