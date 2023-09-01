

terraform plan --out=nat-terraform-oci-nat-instance.tfplan --var-file=config/vars_fra.tfvars



oci compute image list -c $C --all --query 'data[*].{Name:"display-name",OCID:id}' --output table

+---------------------------------------------+---------------------------------------------------------------------------------------------+
| Name                                        | OCID                                                                                        |
+---------------------------------------------+---------------------------------------------------------------------------------------------+
| Canonical-Ubuntu-22.04-aarch64-2023.07.20-0 | ocid1.image.oc1.eu-frankfurt-1.aaaaaaaap7velf36uvsguk7e6eyg5tefp74ymj4gnc7rwka3v7flpq74p7gq |
| Canonical-Ubuntu-20.04-aarch64-2023.07.19-0 | ocid1.image.oc1.eu-frankfurt-1.aaaaaaaaz4nlk7etxmvkuvyw2a7nurjqiswcyfeglure56jamnaim6d2hpaq |
| Canonical-Ubuntu-18.04-aarch64-2023.05.10-0 | ocid1.image.oc1.eu-frankfurt-1.aaaaaaaauecgx5izmgfz5a3aj2qdutbtldpzde4etf5qwditir7xzvplcfwq |
+---------------------------------------------+---------------------------------------------------------------------------------------------+
