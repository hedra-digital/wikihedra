====
Odoo
====

.. odoo-shortcuts:

Atalhos/Shortcuts
-----------------

https://goo.gl/hMocou


+--------------------------------+---------+----------------+
| Função                         | Linux   | Função         |
+================================+=========+================+
| Gravar/salvar registro         | ALT + s | CTRL + ATL + s |
+--------------------------------+---------+----------------+
| Editar um registro (_A_daptar) | ALT + a | CTRL + ALT + a |
+--------------------------------+---------+----------------+
| Descartar (_J_unk)             | ALT + j | CTRL + ALT + j |
+--------------------------------+---------+----------------+
| Criar um novo registro         | ALT + c | CTRL + ALT + c |
+--------------------------------+---------+----------------+
| Abrir modo lista               | ALT + l | CTRL + ALT + l |
+--------------------------------+---------+----------------+
| Abrir modo kanban              | ALT + k | CTRL + ALT + k |
+--------------------------------+---------+----------------+
| Abrir registro anterior        | ALT + p | CTRL + ALT + p |
+--------------------------------+---------+----------------+
| Abrir registro posterior       | ALT + n | CTRL + ALT + n |
+--------------------------------+---------+----------------+
| Ir para menu principal         | ALT + h | CTRL + ALT + h |
+--------------------------------+---------+----------------+

Importações
-----------

https://goo.gl/MVbvx1

* Produtos

+--------------------------------+---------------+----------------+--------------------+---------------+----------+------------+--------------------+-------------------+
| Name                           | Barcode       | Preço de venda | Referência interna | ID Externo    | NCM      | Empresa    | Categoria Interna  | Tipo de produto   |
+--------------------------------+---------------+----------------+--------------------+---------------+----------+------------+--------------------+-------------------+
| 14                             | 9788573265743 | 42             | 9788573265743      | 9788573265743 | 49019900 | Casa Plana | product_category_5 | Produto Estocável |
+--------------------------------+---------------+----------------+--------------------+---------------+----------+------------+--------------------+-------------------+
| 1930: a crítica e o Modernismo | 9788573261707 | 53             | 9788573261707      | 9788573261707 | 49019900 | Casa Plana | product_category_5 | Produto Estocável |
+--------------------------------+---------------+----------------+--------------------+---------------+----------+------------+--------------------+-------------------+


* Tabela de preços de fornecedor

+------------------+-------+---------+------------------+
| Product template | price | Vendor  | Minimal quantity |
+------------------+-------+---------+------------------+
| 0001             | 20    | ASUSTeK | 1                |
+------------------+-------+---------+------------------+

===============
Odoo (Avançado)
===============

Como importar imagens 

* Criar um arquivo com "External ID", "Name", "image".
* Utilizar o script abaixo para rodar 
* Rodar `sh script.sh arquivo.csv resultado.csv`
* Importar arquivo

```
#!/bin/bash
# Usage : script.sh infile.csv outfile.csv
# infile.csv columns are : externalID, name, filename or identifier
# infile.csv separator MUST BE |

while IFS="|" read f1 f2 f3; do

    # recopy external ID and name
    echo -n $f1,\"$f2\", >> $2

    # If third column represents the picture's filename (not the key), please use this command
    cat $(echo ${f3} | tr -d '\r' | tr -d '"') | base64 --wrap=0 >> $2

    #Carrier return at end of line
    echo  >> $2
done < $1
```
