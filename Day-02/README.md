<h2>AWS Identity and Access Management (IAM)</h2>

<p>
<b>IAM (Identity and Access Management)</b> is an AWS service used for 
<b>authentication and authorization</b>.
</p>

<ul>
<li><b>Authentication</b> → Who are you?</li>
<li><b>Authorization</b> → What are you allowed to do?</li>
</ul>

<p>
IAM helps us securely control who can access AWS resources and what actions they can perform.
</p>

<hr>

<h2>1. What is an IAM User?</h2>

<p>
An <b>IAM User</b> is a person or application that is allowed to use AWS services.
</p>

<p>
Instead of using the <b>root account</b> for daily work, we create IAM users for different people.
</p>

<p><b>Example:</b></p>

<ul>
<li>Developer</li>
<li>DevOps Engineer</li>
<li>Data Analyst</li>
</ul>

<p>
Each user gets their own login credentials and only the permissions they need.
</p>

<p><b>Simple Definition:</b></p>

<p>
An IAM user is a <b>person or application that can log in to AWS and use services based on given permissions</b>.
</p>

<p><b>Diagram:</b></p>

<pre>
AWS Account
     |
     |---- IAM User (Developer)
     |---- IAM User (DevOps)
     |---- IAM User (Analyst)
</pre>

<hr>

<h2>2. What is an IAM Group?</h2>

<p>
An <b>IAM Group</b> is a collection of IAM users.
</p>

<p>
Instead of giving permissions to each user individually, we can put users into a group and assign permissions to the group.
</p>

<p><b>Example Groups:</b></p>

<ul>
<li>Developers Group</li>
<li>DevOps Group</li>
<li>Analytics Group</li>
</ul>

<p>
All users inside the group automatically get the permissions assigned to that group.
</p>

<p><b>Simple Definition:</b></p>

<p>
An IAM group is a <b>collection of users that share the same permissions</b>.
</p>

<p><b>Diagram:</b></p>

<pre>
DevOps Group
     |
     |---- User 1
     |---- User 2
     |---- User 3
</pre>

<hr>

<h2>3. What is an IAM Policy?</h2>

<p>
An <b>IAM Policy</b> is a set of rules that defines what actions are allowed or denied in AWS.
</p>

<p>
Policies control what users, groups, or roles can do with AWS resources.
</p>

<p><b>Example Permissions:</b></p>

<ul>
<li>Start EC2 instances</li>
<li>Stop EC2 instances</li>
<li>Read files from S3</li>
<li>Deny deleting resources</li>
</ul>

<p>
Policies are written in <b>JSON format</b> and attached to users, groups, or roles.
</p>

<p><b>Simple Definition:</b></p>

<p>
An IAM policy is a <b>set of permissions that decides what actions are allowed in AWS</b>.
</p>

<p><b>Diagram:</b></p>

<pre>
Policy
   |
   |---- Allow: Start EC2
   |---- Allow: Stop EC2
   |---- Deny: Delete EC2
</pre>

<hr>

<h2>4. What is an IAM Role?</h2>

<p>
An <b>IAM Role</b> gives <b>temporary permissions</b> to users or AWS services.
</p>

<p>
Roles do not have permanent login credentials like IAM users.
They are used when temporary access is required.
</p>

<p><b>Example:</b></p>

<p>
An EC2 instance needs permission to access files stored in S3.
Instead of storing credentials inside the application, we attach an IAM role to the EC2 instance.
</p>

<p><b>Simple Definition:</b></p>

<p>
An IAM role is a <b>temporary set of permissions that can be assumed by users or AWS services</b>.
</p>

<p><b>Diagram:</b></p>

<pre>
EC2 Instance
     |
     |---- IAM Role
            |
            |---- Permission to access S3
</pre>

<hr>

<h2>Quick Summary</h2>

<table border="1" cellpadding="8">
<tr>
<th>Concept</th>
<th>Meaning</th>
</tr>

<tr>
<td>IAM User</td>
<td>A person or application that can log in to AWS</td>
</tr>

<tr>
<td>IAM Group</td>
<td>A collection of users with the same permissions</td>
</tr>

<tr>
<td>IAM Policy</td>
<td>A set of rules that defines permissions</td>
</tr>

<tr>
<td>IAM Role</td>
<td>Temporary permissions used by users or AWS services</td>
</tr>

</table>

<hr>

<h2>Steps to Create IAM Resources</h2>

<h3>1. Steps to Create an IAM User</h3>

<ol>
<li>Login to the AWS Console.</li>
<li>Search for <b>IAM</b>.</li>
<li>Click <b>Users</b>.</li>
<li>Click <b>Create User</b>.</li>
<li>Enter the username.</li>
<li>Choose console access if needed.</li>
<li>Set a password.</li>
<li>Click <b>Next</b>.</li>
<li>Attach permissions or add to a group.</li>
<li>Click <b>Create User</b>.</li>
</ol>

<hr>

<h3>2. Steps to Create an IAM Group</h3>

<ol>
<li>Go to the IAM dashboard.</li>
<li>Click <b>User Groups</b>.</li>
<li>Click <b>Create Group</b>.</li>
<li>Enter the group name.</li>
<li>Attach permission policies.</li>
<li>Add users to the group.</li>
<li>Click <b>Create Group</b>.</li>
</ol>

<hr>

<h3>3. Steps to Attach a Policy</h3>

<ol>
<li>Open IAM dashboard.</li>
<li>Select <b>User</b>, <b>Group</b>, or <b>Role</b>.</li>
<li>Click <b>Add permissions</b>.</li>
<li>Select <b>Attach policy</b>.</li>
<li>Choose the policy.</li>
<li>Click <b>Add permissions</b>.</li>
</ol>

<hr>

<h3>4. Steps to Create an IAM Role</h3>

<ol>
<li>Go to IAM dashboard.</li>
<li>Click <b>Roles</b>.</li>
<li>Click <b>Create Role</b>.</li>
<li>Select the trusted entity (example: EC2).</li>
<li>Attach permission policies.</li>
<li>Enter role name.</li>
<li>Click <b>Create Role</b>.</li>
</ol>

<hr>
