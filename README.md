locale
=========

[![Build Status](https://travis-ci.org/lborguetti/ansible-role-system-locale.svg?branch=master)](https://travis-ci.org/lborguetti/ansible-role-system-locale)

Ansible role for setting locale.

Requirements
------------

Nothing.

Role Variables
--------------

        locale_lang: en_US.UTF-8

This variable define your locale.

        locale_language_pack: language-pack-en

This variable define your [language-pack][1] (required for Ubuntu cloud image)

Default values see defaults/main.yml

Dependencies
------------

Nothing.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: lborguetti.locale, locale_lang: en_US.UTF-8 , locale_language_pack: language-pack-en }

License
-------

BSD

Author Information
------------------

[Luciano Antonio Borguetti Faustino](https://github.com/lborguetti)

[1][http://packages.ubuntu.com/search?suite=default&section=all&arch=any&keywords=language-pack&searchon=names]
