

# Technology Preview: IBM Business Process Manager plug-in for IBM Content Navigator

IBM Business Process Manager plug-in for IBM Content Navigator provides a unified content workflow by bringing your IBM BPM Process Portal Work dashboard into a IBM Content Navigator desktop. You can then view your Work dashboard tasks in the navigator desktop, claim them and work on them just as you do in IBM BPM Process Portal.

## Product installation and SSO setup

The IBM BPM plug-in for IBM Content Navigator requires the following product versions:

IBM Business Process Manager V8.6.0 cumulative fix 2017.12

IBM Content Navigator V3.0.1 on top ofContent Platform Engine V5.2.1.7

(Optional) IBM Case Manager V5.3.1

If you need to install the required products, see the following links for installation information.

For IBM Content Navigator installation instructions, see the product documentation: 

https://www.ibm.com/support/knowledgecenter/en/SSEUEX_3.0.1/com.ibm.installingeuc.doc/eucao000.htm

To download IBM BPM 8.6 cumulative fix 2017.12, go to:

http://www.ibm.com/support/docview.wss?uid=swg24044264

For IBM BPM installation instructions, see the product documentation:  

https://www.ibm.com/support/knowledgecenter/SSFPJS_8.6.0/com.ibm.wbpm.imuc.doc/topics/cins_inst_cnfg_bpm.html

For instructions on configuring  single sign-on (SSO) between the products, see: 

https://www.ibm.com/support/knowledgecenter/SSTLXK_7.5.1/com.ibm.wbpm.bspace.imuc.doc/topics/tcfg_bsp_case_xcell.html

Ensure that your server is using signed certificates. If the server has self signed certificates, follow the appropriate browser documentation to add the certificates in the truststore.

## Install the IBM Business Process Manager plug-in

**Prerequisite:** You must be in the admin desktop and have the appropriate access to add a plug-in to IBM Content Navigator.

1. Download the zip file into a temporary directory that is on the same machine as the IBM Content Navigator administrator desktop.

2. In a browser, enter the IBM Content Navigator administrator desktop URL in the following format:
   http://_host\_name_:_port\_number_/_navigator?_desktop=admin

**Important:**  You must open the IBM Content Navigator admin desktop on the local computer where the .jar file is located.

3. Add and configure the IBM Business Process Manager plug-in:

a. Click **Plug-ins** and then click **New Plug-in**.  
b. Enter the Jar file path and click **Load**.  
c. Enter the plug-in parameters:  

For **IBM BPM Work dashboard origin**, enter the secure protocol, the hostname and port number (if any) of your IBM BPM server.  
For **IBM BPM Work dashboard context root**, enter the context root of the IBM BPM server (the default is teamworks).

## Add the IBM BPM Work Dashboard feature to the IBM Content Navigator desktop

You can add the IBM BPM Work Dashboard feature to an existing IBM Content Navigator desktop or to a new desktop.  To create a new desktop, follow steps 1 and 2.  An IBM Content Navigator repository must be available for use when creating a new desktop.

1. Click **Desktops** in the left pane and then click **New Desktop**.
2. Name your new desktop (for example, BPM).
3. Scroll down the page and expand the Plug-ins section.
4. Select the IBM Business Process Manager plug-in.
5. To add the IBM BPM Work dashboard feature to your desktop, click the **Layout** tab on your desktop and select the IBM BPM Work Dashboard as one of the displayed features.
6. You&#39;re done! You can now load the IBM Content Navigator desktop in a browser, using the following type of URL:

    http://<icn_hostname>:<icn_port>/navigator/?desktop=<your_icn_desktop>
	
7. Click the IBM BPM Work Dashboard icon on the left.  
   You will see the BPM Work dashboard with the current task list for the user that is logged in.
8. Click a task to view the details and to work on it.




