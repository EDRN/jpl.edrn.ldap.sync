# 👯‍♀️ EDRN LDAP Sync

This package updates the `All EDRN` group in the [EDRN](https://edrn.nci.nih.gov/) directory service. It scans for all users and keeps the group `All EDRN` updated so that every user is a member of the group.


## 🚗 Getting Started

Do something like the following:

```console
$ python3 -m venv venv
$ venv/bin/pip install --quiet --upgrade setuptools pip wheel
$ venv/bin/pip install --editable .
```

and you should be good to go to run `venv/bin/edrn-ldap-sync`.


## 🎥 Production Use

Just add a crontab entry like the following:

```crontab
@hourly /usr/local/edrn/edrn/all-edrn-sync/bin --password PASSWORD
```

replacing PASSWORD with the password of the manager account of the EDRN Directory Service.


## 📀 Software Environment

This is written in Python 3 and requires Python 3.7 or later (but probably not Python 4 or later).


### 👥 Contributing

You can start by looking at the [open issues](https://github.com/EDRN/jpl.edrn.ldap.sync/issues), forking the project, and submitting a pull request. You can also [contact us by email](mailto:ic-portal@jpl.nasa.gov) with suggestions.


### 🔢 Versioning

We use the [SemVer](https://semver.org/) philosophy for versioning this software. For versions available, see the [releases made](https://github.com/EDRN/jpl.edrn.ldap.sync/releases) on this project.


## 👩‍🎨 Creators

The principal developer is:

- [Sean Kelly](https://github.com/nutjob4life)


## 📃 License

The project is licensed under the [Apache version 2](LICENSE.md) license.
