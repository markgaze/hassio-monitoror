![Supports armhf Architecture][armhf-shield]
![Supports armv7 Architecture][armv7-shield]
![Supports aarch64 Architecture][aarch64-shield]
![Supports amd64 Architecture][amd64-shield]
![Supports i386 Architecture][i386-shield]
![Maintained][maintained-shield]

![](logo.png)

## Monitoror for Home Assistant

This add-on allows you to host your own version of [Monitoror](https://github.com/monitoror/monitoror) within Home Assistant.

Monitoror is a wallboard monitoring app to monitor server status; monitor CI builds progress or even display critical values.

#### Installation

1. Follow the instructions to [install the add-on repository](https://github.com/markgaze/hassio/#installation)
3. This add-on should then be shown below. Click on it and click on "Install".

### Usage

Once the add-on is running, you can visit the Monitoror instance at `http://[YOUR_HOME_ASSISTANT_IP]:8080`

You will need a configuration file, which is outlined in the [Monitoror docs](https://monitoror.com/documentation/#configuration). This can be stored in your `config` directory in Home Assistant or at any accessible URL.

If you store your configuration file in the `config` directory (for example, at the following location `config/monitoror/test.json`), you can access it in Monitoror by adding it to the config in Home Assistant with the following information:

```yaml
configs:
  - name: TEST
    path: /config/monitoror/test.json
```

You can then see the dashboard by visiting: `http://[YOUR_HOME_ASSISTANT_IP]:8080?config=test`

#### Live demo

You can see a live demo of Monitoror [here](https://demo.monitoror.com/?configUrl=https://monitoror.com/assets/demo.monitoror.com-config.json).

[aarch64-shield]: https://img.shields.io/badge/aarch64-no-red.svg
[amd64-shield]: https://img.shields.io/badge/amd64-no-red.svg
[armhf-shield]: https://img.shields.io/badge/armhf-no-red.svg
[armv7-shield]: https://img.shields.io/badge/armv7-yes-green.svg
[i386-shield]: https://img.shields.io/badge/i386-no-red.svg
[maintained-shield]: https://img.shields.io/maintenance/yes/2020.svg
