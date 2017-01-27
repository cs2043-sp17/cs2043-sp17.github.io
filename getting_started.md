---
title: Getting Started
layout: main
---

To complete the assignments, you will need access to a Unix development environment.  If
you do not already have a native Unix installation, you will need to configure a
"Virtual Machine (VM)."  The short version is that a VM is just another application that
your native operating system runs, where this application is another operating system.
Think Inception.

## Do I need a Virtual Machine?
----------------------------------------------------------------------------------------

Not everybody needs to setup a Virtual Machine.

- If you are running Windows on your computer / tablet, the answer is **yes**.
  - **No**, "Bash for Windows" is not sufficient (yet).
  - **No**, Cygwin and MinGW are not sufficient (and never will be).
- If you are running Mac OSX, the answer is **not necessarily**.  Mac OSX _is_ a
  Unix-based operating system.  Though I encourage you to configure one so you can
  play with Linux.
- If you are running some form of Linux already, then the answer is **no**.
- If you have a VM from another course and want to use that, go for it.  But my VMs have
  been tailored to try and give you a more full Linux experience ;)

### Already have a Linux VM from another course?

Go ahead and use it!  My VMs are customized to try and give you a few more bells and
whistles, but they are in no way necessary to complete the coursework.  We just need
"pure" Linux.

## Configuring the Virtual Machine (VM)
----------------------------------------------------------------------------------------

<div class="panel panel-default">
  <div class="panel-heading">
    <h3 class="panel-title">Suggestion</h3>
  </div>
  <div class="panel-body">
    <p>
      Campus internet is <em>exceptionally</em> fast, if you live off campus you should
      consider downloading the VM before leaving.
    </p>
  </div>
</div>

### 1. Install the Tools

Install [VirtualBox](https://www.virtualbox.org/wiki/Downloads) (current version is
5.1.14).

1. First, install the "VirtualBox platform" (this is the application).
2. Next, install the "VirtualBox Extension Pack" (make sure you download the same
   version of the extension pack as you did the platform package).
  - This allows you to setup connecting a USB stick as well as various other features,
    but isn't strictly speaking necessary.

### 2. Select a VM

If you don't want to read anymore, just select the Ubuntu VM and enjoy.

{% include vm_choices.html %}

<div class="panel panel-info">
  <div class="panel-heading">
    <h3 class="panel-title">Using a Tablet / Netbook / "Weak" Computer?</h3>
  </div>
  <div class="panel-body">
    <p>
      Later today with the videos I will post instructions for a more
      lightweight 32bit VM that older / not as powerful machines will be able to
      handle.  This panel will link to the section describing it when it is live.
      Some students with tablets last year were able to run my VMs without issue,
      some were not.  If you would rather only do the VM process just once, just
      wait until later tonight.
    </p>
  </div>
</div>

#### Fedora 25 Hosts

```console
File: cs2043-fedora.ova
Size: 3.2 GB (3,182,565,376 bytes)
md5:  b20180b838c76c9d26b48a558387e536
```

##### Download Mirrors:
<!-- - [Cornell Course Website](http://www.cs.cornell.edu/courses/cs2043/2017sp/vms/cs2043_fedora.ova) -->
- [Dropbox](https://www.dropbox.com/s/b40c4zsqi2j504r/cs2043_fedora.ova?dl=0)
- [Google Drive](https://drive.google.com/open?id=0B47IM_slYhMnUTViMzVWQkhPRWM)

#### Ubuntu 16.04 Hosts

```console
File: cs2043-ubuntu.ova
Size: 2.4 GB (2,402,733,568 bytes)
md5:  c4b29fa6c10d9316917f53accf8c2023
```

##### Download Mirrors
<!-- - [Cornell Course Website](http://www.cs.cornell.edu/courses/cs2043/2017sp/vms/cs2043_ubuntu.ova) -->
- [Dropbox](https://www.dropbox.com/s/4le4refjqutc2bk/cs2043_ubuntu.ova?dl=0)
- [Google Drive](https://drive.google.com/open?id=0B47IM_slYhMnMFpNdTUtWTlDUWc)

### 3. Install the Virtual Machine

What you just downloaded is an archive of a Virtual Machine (think of it like a
.zip file).  All you need to do is have VirtualBox extract it.

1. Launch VirtualBox.
2. From the menubar, choose "File->Import Appliance".
3. Navigate to where you downloaded the `.ova` file from step 2 and select it.
4. Click continue.
5. Check the box that says "Reinitialize the MAC address of all network cards."
6. Click import, and let VirtualBox take over.

{% include no_64bit.html %}

### 4. Run it!

For both VMs, the username is <kbd>student</kbd> and the password is
<kbd>student</kbd>.  You are encouraged to change your password to something
else.

The <kbd>root</kbd> password is also <kbd>root</kbd>.  Basically, for the sake
of convenience, the VMs are not secure.  So don't store sensitive data on them.

### 5. Customize the Virtual Machine

> Customizing instructions and accompanying videos will be released later
> tonight, but the above steps can be completed now :)
