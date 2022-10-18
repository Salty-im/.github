# salty.im - secure, easy, self-hosted messaging

<img align="left" width="100" height="100" src="https://salty.im/logo.png" style="padding-right: 5pt" />

[salty.im](https://salty.im) is an open specification for a new
[Saltpack](https://saltpack.org) based e2e encrypted messaging protocol
and platform for secure communications with a focus on privacy, security
and being self-hosted. <br /><br /><br />

## 🎬 Demo

[![asciicast](https://asciinema.org/a/ZfcBdiIEO1XOlPWSCR7WWn2Hc.svg)](https://asciinema.org/a/ZfcBdiIEO1XOlPWSCR7WWn2Hc)

## 🏃‍ Quick Start

1. Install `salty-chat`
1. Create and register an account
1. Start chatting!

```console
$ go install go.mills.io/saltyim/cmd/salty-chat@latest
$ salty-chat register <nick>@mills.io
$ salty-chat chat prologic@mills.io
```

Replace `<nick>` with a nickname / alias you'd like.

To test that everything is working you can talk to our echo bot, for example by
starting a chat with `echo@mills.io` it will echo anything you message it:

```console
$ salty-chat chat echo@mills.io
```

**Note:** This quick start installs our reference command-line client
`salty-chat` and registers an account on the broker running at
[salty.mills.io](https://salty.mills.io).

**Security Warning:** Please note that your IP address is logged and that
[salty.mills.io](https://salty.mills.io) is the personal infrastructure of
[James Mills](https://prologic.shortcircuit.net.au).

For full documentation onw how to setup your own broker, with own domain on
your own infrastructure (**preferred**), please read on...

## 👉 Documentation

The following is more details documentation on setting up your Domain Name (DNS)
records (_optional_) and running our reference broker `saltyd` on your own server
and configuring our reference client `salty-chat`:

1. Make sure you have a Domain Name [Choosing a Registrar](#choosing-a-registrar)
1. Read the [full instructions](instructions.html) and start chatting! 

### 🌏 Choosing a Registrar

There are numerous [Domain Name Registrars](https://en.wikipedia.org/wiki/Domain_name_registrar)
you can choose from to register a domain name. It really doesn't matter which
one you use, but you do need a domain name to use Salty IM. Salty IM will also
work with a sub-domain (a name under someone else's domain).

Some reputable registrars include:

- [Namecheap](https://www.namecheap.com/)
- [GoDaddy](https://www.godaddy.com/en-au)
- [OnlyDomains](https://www.onlydomains.com/)

Once you have a domain name you will also need to run a small Web Server on it
so that Salty Addresses can be looked up automatically by the Discovery process.

As Salty IM is decentralised this is an important step. If you cannot for some
reason obtain a domain name and run a small web server, there are other options
(see below).

### ⁉ Help! What?!

Okay if you don't understand anything about Domains and Web Servers don't worry!

We've got you covered! Currently you can skip these steps and just install
Salty straight away and just following the setup process. Although we _highly_
encourage you to setup your own domain and server as Salty IM is designed to
be decentralised, we realize this is not for everyone. By default Salty IM
will use publicly available free servers so you don't need to worry about this.

## 📕 Specification

- [Read the full specification](/spec.html)

## 💾 Sources

The project is managed by a self-hosted [Gitea](https://gitea.io) instance
at https://git.mills.io/saltyim/

- [saltyim](https://git.mills.io/saltyim/saltyim)
  saltyim is the Go library and reference client and broker implementation for
  Salty IM it contains a command-line client (cli),
  a terminal user interface(tui), builtin server/broker
  and a Mobile / Desktop App PWA (progressive web app)
- [salty.im](https://git.mills.io/saltyim/salty.im)
  This website's source files and the Salty specification.
- [salty](https://git.mills.io/prologic/salty)
  The cryptography library tools used by Salty IM utilising
  [Saltpack](https://saltpack.org) and [keys.pub](https://keys.pub).

## 💬 Collaboration

We have an IRC channel `#salty.im` on the [Libera.Chat](https://libera.chat/)
IRC network. You are welcome to come chat to us, hang out and get involved!

## 🕵️‍♂️ PrivacyPolicy

Salty.IM is a decentralised instant messaging protocol inspired by
[IndieWeb](https://indieweb.org/) and [Twtxt](https://twtxt.readthedocs.io/en/latest/)
and accompanying project of [Yarn.social](https://yarn.social).

Like Yarn.social there is a reference broker (server) and client(s) such as the
command-line client `salty-chat` and a mobile app.

The privacy policy therefore only strictly applies to the reference broker and
clients (including the mobile app) built and provided by the Salty.Im developers.

- [Privacy Policy](/privacy.html)

## 👨‍⚖️ License

Salty IM and Salty Chat are licensed under the terms of the MIT License.
