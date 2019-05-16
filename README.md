# ArielRightClick_Context_Menu
Custom Ariel Context Menu for QRadar (Right Click Menu)

This repo contains the custom Ariel context menu I utilize with my QRadar instance running in my homelab. This will add support for Windows Event IDs, destination ports, and URLs. These OSINT sources I utilize daily when performing incident response. If you have any questions you can create an issue for the GitHub project or open a question/reply on the IBM QRadar CE forms located at: https://ibm.biz/qradarceforums

# OSINT Sources:
  - [Bluecoat Site Review](https://sitereview.bluecoat.com)
  - [Cisco Talos](https://talosintelligence.com/)
  - [Speed Guide](https://www.speedguide.net/)
  - [Virus Total](https://www.virustotal.com/)
  - [Ultimate Windows Security](https://www.ultimatewindowssecurity.com)
  - [X-Force Exchange Lookup](https://exchange.xforce.ibmcloud.com/)

# Install Guide
1. Using SSH, log in to the QRadar Console as the root user.
2. cp /opt/qradar/conf/arielRightClick.properties /opt/qradar/conf/arielRightClick.properties.bak
3. wget -nv -O /opt/qradar/conf/ip_context_menu.xml https://raw.githubusercontent.com/Xboarder56/ArielRightClick_Context_Menu/master/arielRightClick.properties
4. systemctl restart tomcat

# Change Log
  - 05-15-2019 - Initial creation of custom Ariel Context Menu

# Sources/References
- https://www.ibm.com/support/knowledgecenter/sl/SS42VS_7.2.7/com.ibm.qradar.doc/t_qradar_ariel_db_integration_right_click.html
