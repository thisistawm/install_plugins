Automate installing plugins on your remote instance.

1. Open the Connection & Credential Alisases
   * Open the CICD Alias [sn_cicd_spoke.CICD]
   * Open & Change the *Credential* [CICD Remote instance] to valid Basic Auth Credentials for your remote instance
1. Open the new table *Install plugin lookup* [x_snc_lh_plugins_lookup]
   * Validate the Plugin you want to install is in the list, else add it
   * Installation subflow installs all plugins per package on the chosen remote instance
   * Add plugin/package entries as you need them
1. Open Flow Designer
   * Open the Flow *Call install plugins*
   * In the Subflow executions, change the Instance URL to your instance URL and make sure the right package and Credential alias is picked
   * Add additional subflow executions as you need them
1. Test the Flow to start installing.
