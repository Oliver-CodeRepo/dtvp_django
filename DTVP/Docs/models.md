MODEL ARCHITECTURE

Company_reg:
    comp_name
    comp_reg_no
    comp_email
    comp_pass
    confirm_pass

Vehicle_Reg:
    slug
    veh_reg_no
    veh_type           (OneToOneField)
    permit_type        (ManyToManyField) 
    county
    companyName        (foreign Key to company_reg)
    dateOfReg
    status

