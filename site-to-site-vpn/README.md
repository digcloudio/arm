# Site to Site VPN Connection

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fdigcloudio%2Farm%2Fmaster%2Fsite-to-site-vpn%2Fazuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>

This template will create a Virtual Network, a subnet for the network, a Virtual Netowork Gateway and Connection to your network outside of Azure (defined as your `local` network). This could be anything such as your on-premises network and can even be used with other cloud networks such as [AWS Virtual Private Cloud](https://github.com/sedouard/aws-vpc-to-azure-vnet). It also provisions an Ubuntu instance attached to the Azure Virtual Network so that you can test connectivity.

Please note that you must have a Public IP for your other network's VPN gateway and cannot be behind an NAT.

Although only the parameters in [azuredeploy-parameters.json](./azure-deploy-parameters.json) are necessary, you can override the defaults of any of the template parameters below:
https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/201-site-to-site-vpn/azuredeploy.json
https://raw.githubusercontent.com/digcloudio/arm/master/site-to-site-vpn/azuredeploy.json