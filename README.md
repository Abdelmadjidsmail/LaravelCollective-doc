# LaravelCollective-docs

laravelcollective documentation

Please feel free to contribute to the docs. If you wish to issue a Pull-Request please make sure you compare the PR to the version of the docs you wish to update.





### create virtual hosts for LARAVELCOLLECTIVE

1. download the folder  in your  **xampp\htdocs**  name it   laravelcollective 
     
 
2. Open `httpd-vhosts.conf` file under `xampp\apache\conf\extra` 

3.  below code.

   ```
   ​``` 
   <VirtualHost laravelcollective.local>
   DocumentRoot "E:/xampp/htdocs/laravelcollective"
   ServerName laravelcollective.local
   <Directory "E:/xampp/htdocs/laravelcollective">
   AllowOverride All
   Require local</Directory></VirtualHost>
   ​```
   ```

   **VirtualHost**    is used as a group of directives what will apply on a particular virtual host. In my case, I have 2 virtual host test1.local and test2.local.

   **DocumentRoot** directive is used to declare directory route what will bind to server name.

**ServerName** directive set request url. ServerName is used to uniquely identify a virtual host.

 **AllowOverride All** is used to set allow the use to .htaccess with in the current virtual host

**Require** is used for access control and current projects it is local.

4.Open hosts and add hosts

Go to `C:\Windows\System32\drivers\etc` and open hosts file ,paste below code

```
127.0.0.1 	laravelcollective.local
```



5.Restart Apache

[download](LaravelCollective.rar){: .btn}


