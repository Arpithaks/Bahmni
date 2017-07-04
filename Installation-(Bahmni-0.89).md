Note: This is based on a blue-green deployment configuration.

## Preparing the pre-production machine
1. Take the backup of the current preprod database and config files
2. To enable offline installation, make sure to enable to yum cache (refer https://bahmni.atlassian.net/wiki/display/BAH/Bahmni+Installation+Without+Internet) so that the downloaded packages can be used when offline
3. "Install the Bahmni on preprod by following the steps mentioned here
https://bahmni.atlassian.net/wiki/pages/viewpage.action?pageId=35291242
4. Make sure to mention the IP address in the inventory file (not the current prod IP), instead of ""localhost"". Also make sure to copy the right config into deployment-artifacts"
5. Check whether all the applications are up and running (MRS, ELIS, ERP, PACS, Reports)
6. "Check if the sync between applications are working fine.
7. Make sure the markers tables has the right IP address mentioned in the entries"
8. Check for the sanity on all applications
9. Make sure the custom erp module for Possible is added in OpenERP. Also make sure the "assets" module is setup properly
10. Conduc UAT on it 