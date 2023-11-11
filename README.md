# imagine

Custom openwrt image to run dockerd on RPi 4. 

## Goals

 * Minimal reproductible host OS
 * Easy upgrade

## How

 * OpenWRT base
   * Well maintained and tested
   * Automated build (ImageBuilder + Action)
   * Rich list of packages
   * Secure by default

# Components

## The Image

Look around this repo.

## The File System

 * [SquashFS](https://openwrt.org/docs/techref/filesystems#squashfs) - Compressed read-only file system
 * Default image size ~100Mb
 * [Layout](https://openwrt.org/docs/techref/flash.layout#partitioning_of_nor_flash-based_devices)

## The Supervisor 

 * dockerd
 * Docker Swarm
 * Portainer

## The Services

See [beast](https://github.com/izer-xyz/beast)

# Usage 

## Install / Initial Setup 

...

## Upgrade 

...
