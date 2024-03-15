# WiggleGate Service

## Via CLI

Run `wiggle-gate` to gather sensor data from the [WiggleGate](https://github.com/wiggle-bin/wiggle-gate) sensor.

```
wiggle-gate
```

## Install WiggleGate Service

In the terminal run `wiggle-gate-install`. This will install and start a service which runs `wiggle-gate` on boot.

```
wiggle-gate-install
```


You can check the status with:

```
systemctl --user status wiggle-gate.service
```

To stop the service run:

```
systemctl --user stop wiggle-gate.service
```

To start the service run:

```
systemctl --user start wiggle-gate.service
```

## Installation for development

Updating packages on Raspberry Pi
```
pip install --upgrade pip setuptools wheel
python -m pip install --upgrade pip
apt-get install libjpeg-dev zlib1g-dev
```

Installing package
```
pip3 install -e .
```

For installation without dev dependencies
```
pip install --no-dev -r requirements.txt
```