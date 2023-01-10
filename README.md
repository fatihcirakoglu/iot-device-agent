# snapd-iot-device-agent

This is a sample REST API that works as a proxy by communicating with snapd's rest api
provided via a unix socket.

## Build and Install

    ```
    $ snapcraft --use-lxd
    $ sudo snap install snapd-iot-device-agent_0.1_amd64.snap --dangerous --devmode
    ```

## Connect Interface

It is not mandatory since you install the snap with `--devmode` but you could connect the interfaces the following command;

    ```
    $ sudo snap connect snapd-iot-device-agent:snapd-control :snapd-control
    ```

## Run
The application starts by using the port 5000.
Open a web browser and go to <your-ip-address>:5000/docs and you could start using it.

## Snap API Documentation
https://snapcraft.io/docs/snapd-api#heading--snaps
