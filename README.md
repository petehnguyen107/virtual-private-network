# virtual-private-network
<h1>Virtual Machine Network in Microsoft Azure</h1>
This tutorial outlines how to set up an Virtual Private Netowkr (VPN) in a virtual machine.<br />

<h2>Environments and Technologies Used</h2>

<ul>
<li>Microsoft Azure (Virtual Machines)</li>
<li>Microsoft Remote Desktop</li>
<li>ProtonVPN</li>
</ul>

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

<ol>
<li>Microsoft Azure Account and Subscription</li>
<li>Microsoft Remote Desktop Connection</li>
<li>Internet Connection</li>
  
</ol>

<h2>Installation Steps</h2>

<h3>Create Virtual Machine in Azure</h3>
<p>

<ol>
  
<li>Browse to https://whatismyipaddress.com/ on your computer and take note of this in a text file</li>
<img src="https://i.imgur.com/6Xl4FxR.png" height="80%" width="80%" alt="Default IP Address"/>
<li>Create a Resource Group in the Azure portal</li>
<li>Create a Windows 10 Virtual Machine in another geographic location (another country than the one you live in). In this case, we're choosing somewhere in Europe.</li>
<li>Log into the VM with Remote Desktop and browse to https://whatismyipaddress.com/ and record this in a text file</li>
<img src="https://i.imgur.com/odoqgHG.png" height="80%" width="80%" alt="VM IP Address"/>

</ol>

<h3>Sign up for ProtonVPN and test the VPN connection</h3>
<ol>
<li>On your actual computer (not the VM), sign up for the free version of Proton VPN on the web browser (https://account.protonvpn.com/signup?plan=free&language=en) </li>
<li>Back within your VM, download the Proton VPN client and login once it's installed.</li>
<li>Once you're in the VPN, choose a VPN server from a different country than the one you're living in</li>
<li>Browse to https://whatismyipaddress.com/  and record this in a text file</li>
  <img src="https://i.imgur.com/Nw45UoN.png" height="80%" width="80%" alt="VM VPN IP Address"/>
<li>Browse to Google, Disney, and/or Amazon and see if there is anything different about the sites in relation to the location of your VPN server. The language or URL may be different from you're used to seeing.</li>
</ol>
  


<h3>Clean up to save resources</h3>

<ol>

<li>Log off Remote Desktop Connection</li>

<li>Delete your Resource Group and VMs after finishing tinkering with them to prevent future costs, deletion of assets on Azure require verification by entering the name of the asset. Also, the Resource Group NetworkWatcherRG is created when creating NSGs for Virutal Machines; be sure to delete NetworkWatcherRG too.</li>

  
</ol>

</p>
<br />
