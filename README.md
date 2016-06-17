This is a an example of a Hiera config setup for a customer. It was used with Satellite, to apply specific configuration to hosts post build from Satellite.

The hierarchy being used, is visible from the files directory, and it shows the paths which will be used/searched by Puppet when its attempting to apply content to hosts.

We are filtering from ::location , ::zone , ::env and ::hostgroup. Location refers to the locations defined in Satellite. Zone refers to a parameter set on the host group, as does env. Hostgroup is the name of the hostgroup as defined in Satellite. Ideally you set the zone + env parameter on the hostgroup.

You need to ensure that ALL of the puppet modules to be used, are in the content views to be consumed by the hosts. You need to ensure ONLY the auto module is attached to a hostgroup. The auto module contains an include to use hiera classes.

<<<<<<< HEAD
I am Batman V2
=======
<<<<<<< HEAD
BATMAN

=======
This is a git commit on development branch, with a pull request V10
>>>>>>> parent of 5f6ffec... Merge pull request #7 from viralmakwana/development
>>>>>>> parent of 976a6fd... Update README.md
