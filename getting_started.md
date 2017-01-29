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
      You are welcome to try using my VMs, but they are probably too "heavy" for your
      machine to handle.  Instead, follow the instructions in the
      <a href="#bit-alternative">32bit Alternative</a> section at the bottom.
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
- [CornellBox](https://cornell.box.com/s/zup914jek0rrfizyshidnix065acv548)
- [Dropbox](https://www.dropbox.com/s/b40c4zsqi2j504r/cs2043_fedora.ova?dl=0)
- [Google Drive](https://drive.google.com/open?id=0B47IM_slYhMnUTViMzVWQkhPRWM)

#### Ubuntu 16.04 Hosts

```console
File: cs2043-ubuntu.ova
Size: 2.4 GB (2,402,733,568 bytes)
md5:  c4b29fa6c10d9316917f53accf8c2023
```

##### Download Mirrors
- [CornellBox](https://cornell.box.com/s/jr5fn7wdbfm5rozpm26cefze69lgam7v)
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

{% include no_64bit_or_vtx.html %}

### 4. Run it!

For both VMs, the username is <kbd>student</kbd> and the password is
<kbd>student</kbd>.  You are encouraged to change your password to something
else.

The <kbd>root</kbd> password is also <kbd>root</kbd>.  Basically, for the sake
of convenience, the VMs are not secure.  So don't store sensitive data on them.

### 5. Customize the Virtual Machine

<div class="panel-group" id="configs_accordian">
  <div class="panel panel-default">
    <!-- Part 1: Both VMs -->
    <div class="panel-heading">
      <h4 class="panel-title"><a data-toggle="collapse" data-parent="#configs_accordian" href="#part_1_both">
        5.1: Give the VM More Resources (Fedora and Ubuntu)
      </a></h4>
    </div>
    <div id="part_1_both" class="panel-collapse collapse">
      <div class="panel-body">
        <div class="embed-responsive embed-responsive-16by9">
          <iframe width="560" height="315" class="embed-responsive-item" src="https://www.youtube.com/embed/Wyt2FBwWFSg"></iframe>
        </div>
      </div>
    </div>
    <!-- Part 2: Fedora -->
    <div class="panel-heading">
      <h4 class="panel-title"><a data-toggle="collapse" data-parent="#configs_accordian" href="#part_2_fedora">
        5.2: Install VirtualBox Guest Additions for Fedora
      </a></h4>
    </div>
    <div id="part_2_fedora" class="panel-collapse collapse">
      <div class="panel-body">
        <!-- Fedora VM -->
        <div class="embed-responsive embed-responsive-16by9">
          <iframe width="560" height="315" class="embed-responsive-item" src="https://www.youtube.com/embed/ADJVRCD5tpY"></iframe>
        </div>
      </div>
    </div>
    <!-- Part 2: Ubuntu -->
    <div class="panel-heading">
      <h4 class="panel-title"><a data-toggle="collapse" data-parent="#configs_accordian" href="#part_2_ubuntu">
        5.2: Install VirtualBox Guest Additions for Ubuntu
      </a></h4>
    </div>
    <div id="part_2_ubuntu" class="panel-collapse collapse">
      <div class="panel-body">
        <div class="embed-responsive embed-responsive-16by9">
          <iframe width="560" height="315" class="embed-responsive-item" src="https://www.youtube.com/embed/qw4r3ZCrAQA"></iframe>
        </div>
      </div>
    </div>
  </div>
</div><!-- end accordian-->

## 32bit Alternative
----------------------------------------------------------------------------------------

If you are running a Tablet, netbook, cannot get your BIOS configured to enable
hardware virtualization, etc, let's use a 32bit VM instead.  For greatest support, I
have chosen [Lubuntu](http://lubuntu.net/) in order to give the widest support for
different hardware / problems you may be having.

### 2-4. Download the VM Archive, Extract, and Install

The folks over at OSBoxes do an excellent job of preparing many different options.  In
the video that follows I show you how to configure their Lubuntu 16.04 32bit VM, but of
course you could go browse around and choose one of the other **many** options they
provide.

Please refer to the comments in the video for the links you will need to follow to
download, extract, and install the VM.

<div class="panel-group" id="alt_accordian">
  <div class="panel panel-default">
    <!-- Part 1: Both VMs -->
    <div class="panel-heading">
      <h4 class="panel-title"><a data-toggle="collapse" data-parent="#alt_accordian" href="#osboxes_howto">
        Click to Expand the video.
      </a></h4>
    </div>
    <div id="osboxes_howto" class="panel-collapse collapse">
      <div class="panel-body">
        <div class="embed-responsive embed-responsive-16by9">
          <iframe width="560" height="315" class="embed-responsive-item" src="https://www.youtube.com/embed/ZV9np2nAP3Q"></iframe>
        </div>
        <hr>
        <blockquote>
          <p>
            Steps 2-4 of <a href="https://cs2043-sp17.github.io/getting_started.html">https://cs2043-sp17.github.io/getting_started.html</a>
          </p>
          <p>
            If you are running a tablet / netbook / not-as-strong computer, or are
            having trouble configuring your BIOS to enable 64bit virtualization, use the
            32bit version instead.
          </p>
          <p>
            The 32bit VM courtesy of OSBoxes: <a href="http://www.osboxes.org/lubuntu/#lubuntu-1604-vbox">http://www.osboxes.org/lubuntu/#lubuntu-1604-vbox</a>
          </p>
          <p>
            This will download a .7z file:
            <ul>
              <li>
                OSX: install Keka: <a href="http://www.kekaosx.com/en/">http://www.kekaosx.com/en/</a>
              </li>
              <li>
                Windows: install 7z: <a href="http://www.7-zip.org/download.html">http://www.7-zip.org/download.html</a>
              </li>
            </ul>
          </p>
        </blockquote>
      </div>
    </div>
  </div>
</div><!-- end alt accordian -->

You can now proceed with step 5.  As the end of the video describes, you are encouraged
to create a "Snapshot" in case things don't work out.  For Lubuntu, the instructions
posted for step 5 of the **Ubuntu** VM should work for you.
