Créer CDS views simples sur on-prem

Utiliser annotations pédagogiques

Exemple : Business Partner minimal

@AbapCatalog.sqlViewName: 'ZC_BP_SIMPLE'

define view entity zm_i_bp_simple

  as select from but000
  
{

  key partner as BusinessPartner,
  
      name_org1 as Name  
      
}
