Hotel Room Booking


Aggregator

Provider - Hotel Vendors
Consumer - Customers

Country - India



1. High level Business Usecases (Security, Onboarding-Business)
2. Deployment Strategy



Three User - CompanyUser(SuperAdmin/OperationalAdmin)/Provider/Consumer

AccomadationMeatadata Service (Metadata/) - 5/7/Home - Max Inventory 


User Service  - Register User , Valid-Token (JWT - header/body/previlege)
Autherization Service  -  (User/Groups) - Previleges/Roles

Onboarding - Registration(Provider) 
             Register Accomodation  -> Workflow (Approval process) -> Approved - Visible 
             
             
             

Front End (Mobile App/Web App)
Backend  - User, Accomadation,OnboardingAndRegistration, 

Database - User/Autherization-RDBMS, 
           AccomadationMeta - RDBMS
           ProviderService - MongoDB (Draft/Approved) 
           
           



Provider -> Login Mobile/Web->APIGateway/Loadbalancer->UserService->Tocken->ProviderOnboardingPortal->ProviderService(Draft/Approved)->







             

            
        
             
             
             

             
 
             
              


               











