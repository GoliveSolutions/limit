## Limit

Limit Frappe Erpnext usage 

### v13, module link under 'Administrator' section-->Limit
<ul>
<li>Check Usage Limit</li>
<li>Set Usage Limit</li>
</ul>

### set usage limits : can be done only user 'Administrator'
Set Usage Limit : https://site.com/app/set-limit
<ul>
<li>When not using a particular limit restriction, increase its value to a high no. Ex no. of users = 1000 </li>
<li>Uninstall the limit app if not using restrictions/li>
</ul>

### Usage information
http://site.com/desk#usage-info
Link is made visible under user icon (top right corner) , last option 'Dashboard Usage' (before logout)

### site_config.json, will be updated via set limit doctype
```sh
{
 "db_name": "xxxxxxxxxx",
 "db_password": "xxxxxxxxxxxx",
 "limits": {
  "emails": 1500,
  "space": 0.157,
  "expiry": "2016-07-25",
  "users": 1,
  "support_email": "help@xx.com",
  "support_phone": "0112533399"
    }
}
```
The valid limits you can set are:
* users - Limit on the number of maximum users for a site
* emails - Limit on the number of emails sent per month from the site. 
            When limit is reached, emails will become muted. They will be blocked up in email queue.
* space - Limit on the maximum space the site can use (GB). In above example it is 157 MB
* expiry - Expiry date for the site (YYYY-MM-DD within quotes)
* support_email - Email id to be displayed
* support_phone - Contact no to be displayed

#### License

Contact