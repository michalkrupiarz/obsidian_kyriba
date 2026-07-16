[[Deployment]] [[Deployment snappa]]
Na samym dole jest jest jenkins builder 
skopiowac snapa 

pozniej na gitops-bank-api [https://github.com/kyriba-eng/gitops-bank-api](https://github.com/kyriba-eng/gitops-bank-api)
przejsc na brancha dev
znalezc values -> platform isntances i tam wybrac CI dev 01 dla kip1 
otworzyc ten plik i tam jest cahrtsVersion w pliku i parametr bank api i tam wkleic snapa
wejsc na argo cd dla kip1 i nacisnac synca [https://argocd.dev.kod.kyriba.com/applications/app.bank-api-kip1.ci-dev-01?resource=](https://argocd.dev.kod.kyriba.com/applications/app.bank-api-kip1.ci-dev-01?resource=)
i pozniej jak bedzie sync ok to mozna sprawdzic czy jest ok