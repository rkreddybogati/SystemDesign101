# Hotel Room Booking - Aggregator

## Actors:
  Provider - Hotel Vendors
  Consumer - Customers
  System Users - Admin/EMployees/CustomerCare etc... 

## Region:
  Support only one country. Eg: Country - India

## Requirement:
  1. High level Business Usecases (Security, Onboarding-Business)
  2. Deployment Strategy to scale well with in India



# Solution

## Actors
Three User - CompanyUser(SuperAdmin/OperationalAdmin)/Provider/Consumer

## Services
AccomadationMeatadata Service (Metadata/) - 5/7/Home - Max Inventory 
User Service  - Register User , Valid-Token (JWT - header/body/previlege)
Autherization Service  -  (User/Groups) - Previleges/Roles

## Databases/DataStore:
Database - User/Autherization-RDBMS, 
           AccomadationMeta - RDBMS
           ProviderService - MongoDB (Draft/Approved) 

## Use Cases:
  Onboarding - Registration(Provider) 
               Register Accomodation  -> Workflow (Approval process) -> Approved - Visible 
             
  Security -         

## Deployment Strategry
  Front End (Mobile App/Web App)
  Backend  - User, Accomadation,OnboardingAndRegistration, 
  Provider -> Login Mobile/Web->APIGateway/Loadbalancer->UserService->Tocken->ProviderOnboardingPortal->ProviderService(Draft/Approved)->
           

