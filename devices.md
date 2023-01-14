---
title: Devices
layout: page
permalink: /devices/
---

# Device Support

<table>
    <thead><tr><td>Device</td><td>Model Numbers</td><td>Supported?</td></tr></thead>
    <tbody>
      {% for device in site.devices %}
        <tr>
            <td><a href="{{ device.url }}">{{ device.title }}</a></td>
            <td>{{ device.models | map: 'id' | join: ', ' }}</td>
            <td>{{ device.supported }}</td>
        </tr>
      {% endfor %}
    </tbody>
</table>

TODO - investigate other devices
- <https://github.com/CrashOverride85/collar/blob/master/extra/Type1.MD>
- <https://ripper121.com/dogs-education-collar-433-mhz-arduino-pilight/>
- <https://github.com/biribiribiri/shockcollar>
- <https://github.com/remoshock/remoshock>
