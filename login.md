Author: Sarthak Goyal
Challenge Page: -[Login](https://login.mars.picoctf.net/) - HTML

Walkthrough

 First check the source code using ctrl+U. Here we will see a condition as
 if("YWRtaW4"!==t.u)?alert("incorrect username"))
 which means that "YWRtaW4" is related to the username. If we check the source code further we can see that our input is coded using btoa function and then decoded as atob function so if we use atob function to decode "YWRtaW4" we will get out username. for that open console and type the following code,

 var u= "YWRtaW4";
 u= atob(u); 
 alert(u);

 this will give "admin" as the output which is our username.

 do the same thing to get the password:-

 var p= "cGljb0NURns1M3J2M3JfNTNydjNyXzUzcnYzcl81M3J2M3JfNTNydjNyfQ"
 p= atob(p);
 alert(p);

 this will give "picoCTF{53rv3r_53rv3r_53rv3r_53rv3r_53rv3r}" as the password.

 Flag
 picoCTF{53rv3r_53rv3r_53rv3r_53rv3r_53rv3r}

