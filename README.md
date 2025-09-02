Sigrok MFM decoder
==================

Original project: https://www.sardis-technologies.com/ufdr/pulseview.htm

* Fixed for modern PulseView
* Ported to support DSView
* Added support for hard drives

Thanks to [rasz_pl](https://github.com/raszpl) for the bulk of the work, and the rest of the Twitch chat for helping
crack the troublesome CRC32 problems.

Usage
=====

Copy the `mfm` folder into your `libsigrokdecocde/decoders` or `libsigrokdecode4DSL/decoders`
folder. You should then find the decoder in your normal decoders list.

It requires three channels:

* Read data - the actual data being read from the drive
* Extra pulses - a channel of extra pulses to include in the data
* Suppression - a channel that suppresses (gates) processing of the information.


