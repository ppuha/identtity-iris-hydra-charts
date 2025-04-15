# Sirius-Broker Charts changelog

## Versions

####    1.3.3 - Improve security context handling for broker and token hook
        
####    1.2.8 - [Broker] Add attributes to ldap request to handle zam roles
        * Image Hydra 1.2.0 Image broker 1.5.0
####    1.2.7 - [Charts] Change ingress config to use className instead of annotation
        * for SIRIUS and SIRIUS-X components
        * Image Hydra 1.2.0 Image broker 1.5.0

####    1.2.6 - [Broker] Add attributes to ldap request to handle zam roles
        * Image Hydra 1.2.0 Image broker 1.5.0

####    1.2.5 Kostya
        
####    1.2.4 - [Hydra] Add roles claims to the /userinfo endpoint response
        * Image Hydra 1.2.0 Image broker 1.4.3

####    1.2.3 Masha

####    1.2.2 Christo

####    1.2.1 - [Hydra] Disable CORS protection for well-known endpoints 
       * Image Hydra 1.1.1 Image broker 1.4.3

####    1.2.0* Kostya

-    *1.1.9* - Update hydra image to 1-2-0 (add roles claims to the /userinfo endpoint response)
-    *1.1.8* - Update hydra image to 1-1-2 (Fix token-exchange flow)
-    *1.1.7* - Update hydra image to 1-1-1 (disable CORS protection for well-known endpoints)
-    *1.1.6* - Update hydra image to 1-0-2
-    *1.1.6* - Update broker image to 1-4-3 (cookie mismatch error fix)
-    *1.1.5* - Use token hook with new claims: azp, originStargate, originZone
-    *1.1.4* - Refactor: Move typ claim from Fosite to Hydra

-    *1.1.3* - Configure Token Hook deployment (disabled)
             - Configure Sirius-x deployment on integration

-    *1.1.2* - Sirius failed 2nd login fix 

-    *1.1.1* - Enable user login metrics

-    *1.1.0* - Change secrets refs to the conjur plugin instead of vault
- 
-    *1.0.2* - Setup startup, liveness, readiness probes, increase auth-sidecar tag version 

-    *1.0.1* - Add configuration for hydra container to enable tracing
     
-    *1.0.0* - initial version of united chart of sirius hydra and sirius broker.
     - below full list of previous charts versions 
         
    -*BROKER*
    -    *1.4.0* merge chart's templates for broker-x and broker. add values for x-preprod
    
    -    *1.3.0* update Error Handling strategy.
    
    -    *1.2.0* change Sirius Broker image to 1.2.2 for live and prod envs
    
    -    *1.1.3* add basicAuth credentials for Preprod env
    
    -    *1.1.1* add basicAuth credentials for Playground env

    -    *1.1.0* use sidecar (Caddy) instead direct hydra admin endpoint
        - For dev and test (team namespace) envs direct access to admin endpoint is used

    *HYDRA*
    -    *1.2.0* - Merge chart's templates for hydra-x and hydra. add values for x-preprod
    
    -    *1.1.4* - Configure token lifetimes
    
    -    *1.1.3* - Update Caddy configuration for customer and prod envs
    
    -    *1.1.1* - Update Caddy configuration for Playground env
    
    -    *1.1.0* - Add sidecar container with Caddy server to use Stargate auth on /admin/clients endpoint \
        - see the [Auth sidecar](https://gitlab.devops.telekom.de/dhei/teams/galatea/products/sirius/auth-sidecar)\
          project for more details
        - For dev and test (team namespace) envs direct access to admin endpoint is used
