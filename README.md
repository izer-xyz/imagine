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

Hardware

 * RPi 4b - more the RAM the better
 * SD Card (maybe optional with usb boot)
 * External Drive

Steps

  1. Download the latest image (rpi-4-squashfs-factory.img.gz) from [Release](https://github.com/izer-xyz/imagine/releases/latest)
  2. Write image to the SD Card (balenaEtcher)
  3. ...


## Upgrade 

 1. ssh to the box
 2. ```# sysupgrade https://github.com/izer-xyz/imagine/releases/download/[latest]/rpi-4-squashfs-sysupgrade.img.gz ```
