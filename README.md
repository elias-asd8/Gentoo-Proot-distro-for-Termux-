# Gentoo-Proot-distro-for-Termux-
Here's a guide to get a Gentoo System on Termux in 3 Steps

# STEP 1
so lets confirm u have the bash script, run this:
```bash
pkg install proot-distro -y
```
this installs the bash script that lets u run linux distributions on ur phone

# STEP 2
install Gentoo itself, this command will install the gentoo system on ur phone:
```bash
curl -L -O https://distfiles.gentoo.org/releases/arm64/autobuilds/20260614T234629Z/stage3-arm64-openrc-20260614T234629Z.tar.xz
```
this uses the curl installer to install the system on ur phone as a .tar.xz

# STEP 3
now u give PRoot-Distro the file and it will do all the work for u:
```bash
proot-distro install -n gentoo stage3-arm64-openrc-20260614T234629Z.tar.xz
```

# QUICK GENTOO INFO
so when u log in itll be BARE BONES, REALLY BARE BONES, And if u wanna install Software u need to use emerge (GUIDE ON EMERGE 👇)

# Emerge
If u want to use the prebuilt package manager emerge u first need to run this command to get synced to the repos, this makes EVERY PACKAGE IN THE UNIVERSE accessible:
```bash
emerge --sync
```
this installs build files for EVERY PACKAGE IN THE UNIVERSE


But EMerge is different from other package managers, u need to specify the category and name of the package like this:
```bash
emerge --ask <CATEGORY>/<PACKAGE-NAME>
```
(I intentionally didnt add a script cuz if u rely on random scripts Gentoo will be HELL for u)

# Have fun and dont throw ur phone out the window! 😄
