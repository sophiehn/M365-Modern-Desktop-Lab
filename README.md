# M365-Modern-Desktop-Lab


 1. Open a browser window (not InPrivate) in Microsoft Edge to
    [https://portal.azure.com](https://portal.azure.com)
  
 2. Log in with your global admin credentials: **admin@M365x723661.onmicrosoft.com**, password: sochania@1122
 3. Browse to [https://www.whatismyip.com/](https://www.whatismyip.com/). Make a note of the IP address displayed

**Note:** Azure Multi-Factor Authentication only supports IPv4 addresses. If your ISP is only allocating IPv6 addresses, you will not be able to add the address to the trusted IPs

 4. Close the [https://www.whatismyip.com/](https://www.whatismyip.com/) browser tab

**Configuring location-based conditional access**

1.  In the left-hand navigation, click **Azure Active Directory**.
2. Under **Security**, click **Conditional access**.
3. In the **Manage** section, click **Named locations**.
4. Click **Configure MFA trusted IPs**.
5. In the **trusted ips** text box enter the following IP addresses:  
    192.168.1.0/24  
    192.168.2.0/24  
    192.168.3.0/24
6. Click **Save**.
7. Click **Close**.
8. Close the Multi-factor authentication browser tab.
9. Click **X** to close the **Conditional access – Named locations**
    blade.
10.  Click **Enterprise applications**, and then click **All
    applications**.
11.  In the Enterprise application list, click **Expensify**.
12. Under **Security**, click **Conditional access**.
13. Click **+ New policy**.
14. In the Name field type **Expensify location policy**.
15. In the **Assignments** section, click **Users and groups**.
16. Click **Select users and groups**, and then click **Users and
    groups**.
17. Click **Select**.
18. In the search box, type **sg** and press **Enter**.
19. Click on **sg-Sales and Marketing**.
20. Click **Select**.
21. Click **Done**.
22. In the **Assignments** section, click **Conditions**.
23. On the **Conditions** blade, Click **Locations**.
24. Set Configure to **Yes**.
25. Under **Include**, ensure that **Any location** is selected.
26. Click **Exclude**.
27. Check **All trusted locations**.
28. At the bottom of the **Locations** blade, click **Done**.
29. At the bottom of the **Conditions** blade, click **Done**.
30. In the **Access controls** section, click **Grant**.
31. Select **Block access**.
32. Click **Select**.
33. Set Enable policy to **On**.
34. Click **Create**.
35. In the top right corner of the portal, click **admin@M365x723661.onmicrosoft.com**.
36. Click Sign out.


**Access resources from untrusted location**

 41. Browse to [https://myapps.microsoft.com](https://myapps.microsoft.com).

 42. Click **Use another account**.

 43. Sign in as **meganb@M365x723661.onmicrosoft.com** with the tenant password.

 44. Click on the **Expensify** tile.

 45. On the **You cannot access this right now** message, click **More details**.

Note the message notifying you are unable to access the content right now and it was triggered by conditional access.

 1. Close the Sign in to your account tab.
 2. In the top right corner of the portal, click [meganb@M365x723661.onmicrosoft.com](mailto:isaiahl@%3ctenant%3e.onmicrosoft.com).
 3. Click **Sign out**.
