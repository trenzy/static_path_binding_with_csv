# <h1>Ansible Playbook for deploying Static Path Binding from a CSV file</h1>

This playbook provides an example of configuring static path bindings on multiple
interfaces using the read_csv module. It uses the following modules: 

cisco.aci.aci_static_binding_to_epg
community.general.read_csv

Which requires that you have the following collections installed:
- cisco.aci
- community.general

In addition to the playbook, I've included an example csv file.

It makes a few assumptions:

- That you have created the associated Tenants, Application Profiles, EPGs, and Fabric access policies.
- The associated domain has already been configured under the EPG

This was tested with Ansible 2.12 base with ACI version 4.2(6h).