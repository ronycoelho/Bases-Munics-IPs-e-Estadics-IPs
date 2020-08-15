
Como sugestão para download da base no R, utilizar: 

```
link <- "https://github.com/ronycoelho/Bases-Munics-IPs-e-Estadics-IPs/raw/master/estadics_ips/Estadic_IPs.xlsx"

tempdir <- tempdir()
setwd(tempdir)
temp = tempfile(fileext = ".xlsx")

download.file(link, destfile=temp, mode= "wb")

base <- readxl::read_excel(temp, sheet = 2)
```

O dicionário pode ser consultado no link acima ou [clicando aqui!](https://github.com/ronycoelho/Bases-Munics-IPs-e-Estadics-IPs/blob/master/estadics_ips/Dicion%C3%A1rio_Simpl_Estadic_IPs.pdf), e pode ser baixado configurando o argumento ```sheet = 1``` do código acima.
