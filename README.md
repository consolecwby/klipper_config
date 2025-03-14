#This is a fork of Floris of Belgium's CR-10 Config Code to make it match mine. Worked with belgium engineers in the past and they are some of the best to work with so more trusting of this code. 

# Klipper configs for CR10 / CR10s

### Hostname

Set the hostname of your printers' pi in `sudo raspi-config`. This hostname will be used to hardlink the correct files. Your current hostname can be seen by `echo ${HOSTNAME}`.

### Installing

Starting from a clean rpi image, issue the following:

```text
git clone git@github.com:fl0r1s/klipper_config.git
cd klipper_config 

# optionally checkout a branch
git checkout complete_revamp

# hardlink the files. 
./install.sh
```

### Uploading calibration settings etc

You'll have to log in to your github.

```text
cd ~/klipper_config
./upload.sh
```

### Klipper + Frontend

The easiest way to update klipper is by using [kiauh](https://github.com/th33xitus/KIAUH). Install klipper, moonraker and a frontend.

