graph TD
    A[Email Sender] -->|MX Email Messages| B["MX Records | Cloudflare<br>route1.mx.cloudflare.net |  Priority: 2<br>route2.mx.cloudflare.net |  Priority: 81<br>route3.mx.cloudflare.net |  Priority: 91"]
    B -->|Terraform : cloudflare_record| C[Cloudflare Worker : workers-n8n-3]
    B -->|Terraform : google_workflows_workflow| D[Custom mx record: a970359.mx.mailhop.org]
   
   

  
