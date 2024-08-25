# Description
Simple bash script for changing ***Buffer Size*** and ***Sample Rate*** for your **PipeWire** instance.

# Pre-Requisites
Add your user to ***audio*** and ***pipewire*** groups:

>sudo usermod -a -G audio your_username
>sudo usermod -a -G pipewire your_username

**IMPORTANT:** Restart your machine afterwards

# Usage
**By default**, running this script will set ***1024 bit Buffer Size*** and ***48000 Hz Sample Rate*** (that are **optimal values** for daily usage on **Non-Professional Audio Interfaces, like your Built-In Audio or Bluetooth Audio**). 
In order to set your **custom values** just **parse** ***"buffer_size/sample_rate"*** **values to script**.

# Example

> **$# ./audio-configurator 1024/96000**
>*Found "settings" metadata 30*
>*set property: id:0 key:clock.force-quantum value:1024 type:(null)*
>*Found "settings" metadata 30*
>*set property: id:0 key:clock.force-rate value:96000 type:(null)*
>*INFO: Setting custom PipeWire Quantum values ...*
>*INFO: BUFFER SIZE - 1024*
>*INFO: SAMPLE RATE - 96000*
