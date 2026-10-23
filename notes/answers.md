apt update only downloads the latest list of available packages. It does not install anything.
apt upgrade installs the newer versions of the packages that are already on my server.
We should always run apt update first, so the server knows the newest versions.
After that, we run apt upgrade to actually install the updates.
For example, update is like checking the Play Store for updates, and upgrade is like pressing "Update all".
