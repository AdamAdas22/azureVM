# azureVM
<h1>How to Create a Virtual Machine in Microsoft Azure</h1>
  <h2>Prerequisites</h2>
<ul>
<li>A <strong>Microsoft Azure account</strong> (Sign up at <a href="https://portal.azure.com" target="_blank">Azure Portal</a>).</li>
<li>An active <strong>Azure subscription</strong> with VM creation permissions.</li>
</ul>

<h2>Step 1: Log in to the Azure Portal</h2>
<p>1. Visit <a href="https://portal.azure.com" target="_blank">Azure Portal</a>.</p>
<p>2. Sign in with your Microsoft account.</p>

<h2>Step 2: Create a Virtual Machine</h2>

![image](https://github.com/user-attachments/assets/faace06b-c591-4322-9edc-9c3a579354d0)

<p>1. In the <strong>Azure Portal</strong>, search for <strong>"Virtual Machines"</strong>.</p>
<p>2. Click <strong>"Create" > "Azure virtual machine"</strong>.</p>

<h2>Step 3: Configure Basic Settings</h2>
<ul>
<li><strong>Subscription:</strong> Choose your subscription.</li>
<li><strong>Resource Group:</strong> Create or select an existing group.</li>
  
  ![image](https://github.com/user-attachments/assets/8bd5d6e9-87ed-471b-ae65-ca4bc3e87295)

<li><strong>VM Name:</strong> Example: <code class="code">MyAzureVM</code></li>
<li><strong>Region:</strong> Select the nearest location.</li>
<li><strong>OS Image:</strong> Choose between <strong>Windows</strong> or <strong>Linux</strong>.</li>
<li><strong>VM Size:</strong> Pick based on requirements (e.g., <strong>Standard B2s</strong> for small projects).</li>
<li><strong>Authentication:</strong> Set up username and password (or SSH key for Linux).</li>
</ul>

![image](https://github.com/user-attachments/assets/547c3652-880b-49fc-b39a-3b834332b089)

<h2>Step 4: Configure Disks</h2>
<ul>
<li>Select <strong>Standard SSD</strong> for best balance of cost and performance.</li>
<li>Attach additional storage if needed.</li>
</ul>

![image](https://github.com/user-attachments/assets/82bb5878-e3b6-4c31-b3bf-03bc4d72d088)

<h2>Step 5: Configure Networking</h2>
<ul>
<li>Choose a <strong>Virtual Network</strong>.</li>
<li>Select an available <strong>Subnet</strong>.</li>
<li>Enable <strong>Public IP</strong> if needed.</li>
<li>Allow inbound ports:
<ul>
<li>Windows: <code class="code">RDP (3389)</code></li>
<li>Linux: <code class="code">SSH (22)</code></li>
</ul>
        </li>
</ul>

   <h2>Step 6: Review & Create VM</h2>
  <p>1. Click <strong>"Review + Create"</strong> to validate settings.</p>
  <p>2. Click <strong>"Create"</strong> to start VM deployment.</p>

![image](https://github.com/user-attachments/assets/eb63bcee-a841-4196-8977-c28844ee1e0f)

   <h2>Step 7: Connect to Your VM</h2>
    
  <h3>For Windows VM</h3>
   <ul>
      <li>Go to your VM in <strong>Azure Portal</strong>.</li>
     <li>Click <strong>"Connect"</strong> > <strong>"RDP"</strong>.</li>
      <li>Download and open the <strong>RDP file</strong>.</li>
       <li>Enter your VM credentials to log in.</li>
   </ul>

  <h3>For Linux VM</h3>
   <ul>
        <li>Open a terminal (Mac/Linux) or PowerShell (Windows).</li>
        <li>Run the SSH command:</li>
        <pre class="code">ssh username@your-vm-public-ip</pre>
        <li>Enter your password or use an SSH key.</li>
    </ul>

   <h2>Step 8: Manage and Monitor Your VM</h2>
   <ul>  
    <li>Use <strong>Azure Monitor</strong> for performance tracking.</li>
     <li>Start/Stop your VM from the <strong>Azure Portal</strong>.</li>
      <li>Enable <strong>auto-shutdown</strong> to save costs.</li>
    </ul>

   <h2>Conclusion</h2>
   <p>Congratulations! 🎉 You have successfully set up a Virtual Machine in <strong>Microsoft Azure</strong>.</p>
   <p>For automation, explore using <strong>Azure CLI</strong> or <strong>Terraform</strong> for faster deployment.</p>



