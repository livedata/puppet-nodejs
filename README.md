# Puppet Node.js Module

Uses nave to install node 

## Installation

Copy the module to your puppet modules directory of if you're using git
to manage your manifests/modules you can just `git sudmodule add
https://github.com/danheberden/puppet-nodejs modules/nodejs`

Add a nodejs declaration to whatever node in your manifest:

```
node default {
  class { 'nodejs':
    version => '0.6.13',
  }
}
```

Since this uses nave, you can also specify 'latest' or 'stable' as
versions.
