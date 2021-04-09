# Introduction #

On the 29th June 2020 PRIMAR launched the first available S100 service from a RENC. The service contains S-102 (Bathymetric Surface Products) and S-111 (Surface current information). In addition, PRIMAR is also providing full support of the IHO S-100 security scheme (S-100 Part 15).
PRIMAR has implemented support for S-100 services by revising its remote update service to enable delivery of S-100 data, in addition to ENCs. The PRIMAR Remote Update Protocol now supports delivery of S-102 and S-111 datasets, encrypted in accordance with the IHO S-100 Part 15 Data Protection Scheme. PRIMAR has produced a development kit containing a java project and test code for the implementation. PRIMAR has also prepared a test dataset, which has been encrypted in accordance with S-100 Part 15, this can be used to verify that contact can be established with the PRIMAR service, and that this delivers the test datasets.

The request only contains an S-100 Part 15 user permit, however, the test user is set up with ENC coverage in addition to S-102 and S-111 coverage. The service will therefore deliver both ENC, S-102 and S-111 data, encrypted with S-63 and S-100 Part 15, respectively.

# Documentation (PRIMAR Remote Update Protocol) #
The latest Remote Update documentation can be found at:
https://docs.google.com/document/d/e/2PACX-1vTVPVpGRzAnQvGqbutZzS0pFPI2TWnONsT6_FKS6pW-li0u4zCLKVs5Ykm4rHqxeUdk1TZLZg3Zj65k/pub

# Example Code #
An example java project, showing how to use some of PRIMAR APIs, can be found [here](https://github.com/ElectronicChartCentre/gdsclient)

A test-code showing S-100 remote update inclusive parsing of permit files can be found [here](https://github.com/ElectronicChartCentre/gdsclient/blob/master/src/test/java/no/ecc/gdsclient/remote/RemoteUpdateClientTest.java)

This example uses some S-100 part 15 code from: https://github.com/ElectronicChartCentre/s100.

# User Permit and Testdata #
Userpermit: B2BEC75A6831832259DB00A2B0A9FA7D541B9954859868

The S-100 Part15 User Permit (above) will return ENCs, encrypted using S63 v 1.2, and S102 and S111 data, encrypted with S100 Part15.
Testing must be carried out using the following URL: https://primar.ecc.no/primar/

# Contact #
Please contact PRIMAR Support at support@ecc.no for further information or assistance.
