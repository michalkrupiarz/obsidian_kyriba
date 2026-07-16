[[Caas-5067]], [[tlsssl]]

Scenario  
Login to kip1

Go to TSL/SSL Certificate Generations (Core Data → Set-up bank communication → TSL/SSL Certificate Generation)  
Click Add

Fill Code, description common name.  
Mark certificate as self signed.  
Click Save and Download  
  
You will see that there is show Error dialog with unexpected error occured  
Expected result is that certificate should be downloaded and view should be closed.  
  
However: certificate is created, and when you close dialog, click cancel to go back to list of certificates, you can search for certificate and download it without a problem.