OBS Studio <https://obsproject.com>
===================================

.. image:: https://github.com/obsproject/obs-studio/actions/workflows/main.yml/badge.svg?branch=master&event=push
   :alt: OBS Studio Build Status - GitHub Actions
   :target: https://github.com/obsproject/obs-studio/actions/workflows/main.yml?query=event%3Apush+branch%3Amaster

.. image:: https://badges.crowdin.net/obs-studio/localized.svg
   :alt: OBS Studio Translation Project Progress
   :target: https://crowdin.com/project/obs-studio

.. image:: https://img.shields.io/discord/348973006581923840.svg?label=&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2
   :alt: OBS Studio Discord Server
   :target: https://obsproject.com/discord

What is OBS Studio?
-------------------

OBS Studio is software designed for capturing, compositing, encoding,
recording, and streaming video content, efficiently.

It's distributed under the GNU General Public License v2 (or any later
version) - see the accompanying COPYING file for more details.
---------------------------------------
---------------------BUILD ON MANJARO LINUX (portable)---------------------------

wget https://cdn-fastly.obsproject.com/downloads/cef_binary_5060_linux64.tar.bz2

tar -xjf ./cef_binary_5060_linux64.tar.bz2

git clone --recursive https://github.com/obsproject/obs-studio.git

cd obs-studio

mkdir build && cd build

 cmake -DLINUX_PORTABLE=ON -DCMAKE_INSTALL_PREFIX="${HOME}/obs-studio-portable" -DENABLE_BROWSER=ON -DCEF_ROOT_DIR="../../cef_binary_5060_linux64" -DENABLE_AJA=OFF -DENABLE_WEBSOCKET=OFF ..
 
make -j4 && make install
----------------------------------------------------------------------------------
After that, you should have a portable install in ~/obs-studio-portable. Change to bin/64bit or bin/32bit and then simply run: ./obs
----------------------------------------------------------------------------------
Quick Links
-----------

- Website: https://obsproject.com

- Help/Documentation/Guides: https://github.com/obsproject/obs-studio/wiki

- Forums: https://obsproject.com/forum/

- Build Instructions: https://github.com/obsproject/obs-studio/wiki/Install-Instructions

- Developer/API Documentation: https://obsproject.com/docs

- Donating/backing/sponsoring: https://obsproject.com/contribute

- Bug Tracker: https://github.com/obsproject/obs-studio/issues

Contributing
------------

- If you would like to help fund or sponsor the project, you can do so
  via `Patreon <https://www.patreon.com/obsproject>`_, `OpenCollective
  <https://opencollective.com/obsproject>`_, or `PayPal
  <https://www.paypal.me/obsproject>`_.  See our `contribute page
  <https://obsproject.com/contribute>`_ for more information.

- If you wish to contribute code to the project, please make sure to
  read the coding and commit guidelines:
  https://github.com/obsproject/obs-studio/blob/master/CONTRIBUTING.rst

- Developer/API documentation can be found here:
  https://obsproject.com/docs

- If you wish to contribute translations, do not submit pull requests.
  Instead, please use Crowdin.  For more information read this page:
  https://obsproject.com/wiki/How-To-Contribute-Translations-For-OBS

- Other ways to contribute are by helping people out with support on
  our forums or in our community chat.  Please limit support to topics
  you fully understand -- bad advice is worse than no advice.  When it
  comes to something that you don't fully know or understand, please
  defer to the official help or official channels.
