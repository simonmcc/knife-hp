# TODO #
This is a list of features currently lacking and (eventually) under development:
* filter out extraneous images from knife hp image list (requires HP metadata not yet available)
* should the node.name and node.id be the same (might have to fix this in the ohai plugin)
* Add support for associating floating IPs on server create and verify they are automatically disassociated on server delete
* Add /etc/chef/ohai/hints/hp.json, the `openstack` Ohai plugin keys off of it and pulls from the meta-data service.
* Add support for `--no-host-key-verify`
* Add support for `--private-network` for bootstrapping private networks
* take either the flavor ID or the flavor name
* take either the image ID or the image name
* show the flavor and image names in server lists
* switched from hp_account_id to hp_access_key (Hugues Malphettes reported)
  patch didn't make it into Fog 1.4, so reverted for now

* Server list supports many more states
* Support for tenant?
* Added virtual cpus to 'knife openstack flavor list'

## v0.2.0
* support for unenven_columns for prettier output
* added bootstrap-proxy support. (Matt Butcher)
* updated to point to Fog 1.4.0 for `HP` provider
* chef-full is now default bootstrap template
* Add support for floating IPs and address associating
* push the AZ stuff into the hints file

## v0.1.0
* initial developer release