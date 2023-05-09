### Date proposed

2023/05/09

### Summary

We should stop supporting Xorg/X11. I propose that we drop any xorg support from our main images (except XWayland) and only ship wayland.

### Motivation

With the rapid development of wayland and the stagnating Xorg development, wayland is clearly the future in terms of display managers. Even Red Hat acknowledges this and [officially sees xorg as deprecated in RHEL](https://access.redhat.com/documentation/pt-br/red_hat_enterprise_linux/9/html/9.0_release_notes/deprecated_functionality).
This is a clear sign that wayland is ready for the majority of linux users and we should follow with this decision.

### Changes

We would remove any xorg support from our main images. This should simply involve not installing the `xorg` package group from the arch repositories.

### Drawbacks

Some people are not yet ready to use wayland. This could be due to hardware support (Nvidia) or simply some applications not properly working.

If the demand is high enough, we could also make xorg enabled images that people can use. Otherwise users can simply install required xorg packages without having to use a special image.

### Submitted by
@axtloss
