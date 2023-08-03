<p align="center">
  <a href="#build-framework">
   <img src="https://raw.githubusercontent.com/armbian/build/master/.github/armbian-logo.png" alt="Armbian logo" width="144">
  </a><br>
  <strong>Armbian OS</strong><br>
<br>
<a href=https://github.com/armbian/os/actions/workflows/complete-artifact-matrix-all.yml><img alt="GitHub Workflow Status" src="https://img.shields.io/github/actions/workflow/status/armbian/os/complete-artifact-matrix-all.yml?logo=githubactions&label=Artifacts%20make&style=for-the-badge&branch=main"></a>
<a href=https://github.com/armbian/os/actions/workflows/repository-update.yml><img alt="GitHub Workflow Status" src="https://img.shields.io/github/actions/workflow/status/armbian/os/repository-update.yml?logo=githubactions&label=Repository%20update&style=for-the-badge&branch=main"></a>
<a href=https://github.com/armbian/os#latest-smoke-tests-results><img alt="GitHub Workflow Status" src="https://img.shields.io/github/actions/workflow/status/armbian/os/smoke-tests.yml?logo=githubactions&label=Smoke%20tests&style=for-the-badge&branch=main"></a>
</p>


# What does this project do?

- Keeps build framework [packages artifacts](https://github.com/orgs/armbian/packages) cache up to date
- Keeps stable [apt.armbian.com](https://apt.armbian.com) and nightly [beta.armbian.com](https://beta.armbian.com) packages repository up to date
- Builds [nightly](https://github.com/armbian/os/releases) and [stable images](https://www.armbian.com/download/) and uploads them to Armbian CDN
- Keep synchronizing the selection of [3rd party](external) applications with Armbian repositories
- Tests install of all packages added onto stable and testing Debian and Ubuntu releases

# When is this happening?

- Artifacts cache is updated every eight hours, starting at 0:00 AM UTC
- Repository update is updated once per day, at 3:00 AM UTC
- Smoke tests is executed after **repository update** is finished.
- Nightly images are build once per day, at 5:00 AM UTC
- Manually, when Armbian [release manager](https://github.com/orgs/armbian/teams/release-manager) executes a build action

# Latest smoke tests results:

- installs kernels,dtb and headers that are defined / supported by the board
- runs network and computing performance tests (7z benchmark)
- store armbianmonitor logs

<!--START_SECTION:data-section-->
<table width="100%"><tr><td align="left"><a href="https://paste.armbian.com/ejomemujig">Tinker Board</a></td><td align="left">1691083958</td><td align=left>current</td><td align=right>2022.04</td><td align=right>6.1.42-rockchip</td><td align=right>98</td><td align=right>4871</td></tr><tr><td align="left"><a href="https://paste.armbian.com/ewopihewaw">Tinker Board</a></td><td align="left">1691084349</td><td align=left>edge</td><td align=right>2022.04</td><td align=right>6.4.7-rockchip</td><td align=right>98</td><td align=right>4947</td></tr><tr><td align="left"><a href="https://paste.armbian.com/xinuribaba">Espressobin</a></td><td align="left">1691083819</td><td align=left>current</td><td align=right></td><td align=right>5.15.123-mvebu64</td><td align=right>856</td><td align=right>1118</td></tr><tr><td align="left"><a href="https://paste.armbian.com/jexetigori">Espressobin</a></td><td align="left">1691084551</td><td align=left>edge</td><td align=right></td><td align=right>6.1.42-mvebu64</td><td align=right>885</td><td align=right>1125</td></tr><tr><td align="left"><a href="https://paste.armbian.com/izazonipol">Pine H64</a></td><td align="left">1691083393</td><td align=left>legacy</td><td align=right>2023.07</td><td align=right>5.15.123-sunxi64</td><td align=right>946</td><td align=right>3747</td></tr><tr><td align="left"><a href="https://paste.armbian.com/arugiwafuq">Pine H64</a></td><td align="left">1691083889</td><td align=left>current</td><td align=right>2023.07</td><td align=right>6.1.42-sunxi64</td><td align=right>880</td><td align=right>3679</td></tr><tr><td align="left"><a href="https://paste.armbian.com/idadudejud">Pine H64</a></td><td align="left">1691084275</td><td align=left>edge</td><td align=right>2023.07</td><td align=right>6.4.7-sunxi64</td><td align=right>957</td><td align=right>3642</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">UEFI x86</a></td><td align="left">1691084024</td><td align=left>legacy</td><td align=right></td><td align=right>5.15.123-x86</td><td align=right>850</td><td align=right>4788</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">UEFI x86</a></td><td align="left">1691084397</td><td align=left>current</td><td align=right></td><td align=right>6.1.42-x86</td><td align=right>849</td><td align=right>4741</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">UEFI x86</a></td><td align="left">1691084791</td><td align=left>edge</td><td align=right></td><td align=right>6.4.7-x86</td><td align=right>730</td><td align=right>4748</td></tr><tr><td align="left"><a href="https://paste.armbian.com/joxikojame">Banana Pi M5</a></td><td align="left">1691083368</td><td align=left>current</td><td align=right></td><td align=right>6.1.42-meson64</td><td align=right>880</td><td align=right>5514</td></tr><tr><td align="left"><a href="https://paste.armbian.com/ebakonofes">Banana Pi M5</a></td><td align="left">1691083755</td><td align=left>edge</td><td align=right></td><td align=right>6.4.7-meson64</td><td align=right>842</td><td align=right>5514</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">Rockpi E</a></td><td align="left">1691083738</td><td align=left>legacy</td><td align=right></td><td align=right>6.1.37-rockchip64</td><td align=right>93</td><td align=right>3369</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">Rockpi E</a></td><td align="left">1691083994</td><td align=left>current</td><td align=right></td><td align=right>6.1.37-rockchip64</td><td align=right>93</td><td align=right>3310</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">Rockpi E</a></td><td align="left">1691084250</td><td align=left>edge</td><td align=right></td><td align=right>6.1.37-rockchip64</td><td align=right>93</td><td align=right>3281</td></tr><tr><td align="left"><a href="https://paste.armbian.com/ibikizofaz">Odroid C2</a></td><td align="left">1691083445</td><td align=left>current</td><td align=right>2022.01</td><td align=right>6.1.42-meson64</td><td align=right>880</td><td align=right>3897</td></tr><tr><td align="left"><a href="https://paste.armbian.com/wuhahofeco">Odroid C2</a></td><td align="left">1691083842</td><td align=left>edge</td><td align=right>2022.01</td><td align=right>6.4.7-meson64</td><td align=right>700</td><td align=right>3869</td></tr><tr><td align="left"><a href="https://paste.armbian.com/luqapulene">Orange Pi 4 LTS</a></td><td align="left">1691083373</td><td align=left>current</td><td align=right></td><td align=right>6.1.42-rockchip64</td><td align=right>890</td><td align=right>4454</td></tr><tr><td align="left"><a href="https://paste.armbian.com/lodijikigi">Orange Pi 4 LTS</a></td><td align="left">1691083761</td><td align=left>edge</td><td align=right></td><td align=right>6.3.13-rockchip64</td><td align=right>960</td><td align=right>3720</td></tr><tr><td align="left"><a href="https://paste.armbian.com/mokobizibe">NanoPi R6S</a></td><td align="left">1691083056</td><td align=left>legacy</td><td align=right>2017.09</td><td align=right>5.10.160-rk35xx</td><td align=right>890</td><td align=right>15884</td></tr><tr><td align="left"><a href="https://paste.armbian.com/oqonunisoy">Cubieboard 1</a></td><td align="left">1691083659</td><td align=left>legacy</td><td align=right>2022.07</td><td align=right>5.15.123-sunxi</td><td align=right>77</td><td align=right>579</td></tr><tr><td align="left"><a href="https://paste.armbian.com/ogusicesah">Cubieboard 1</a></td><td align="left">1691084536</td><td align=left>current</td><td align=right>2022.07</td><td align=right>6.1.42-sunxi</td><td align=right>76</td><td align=right>559</td></tr><tr><td align="left"><a href="https://paste.armbian.com/juzuvecure">Cubieboard 1</a></td><td align="left">1691085476</td><td align=left>edge</td><td align=right>2022.07</td><td align=right>6.4.7-sunxi</td><td align=right>76</td><td align=right>558</td></tr><tr><td align="left"><a href="https://paste.armbian.com/asocasavah">Orange Pi 3 LTS</a></td><td align="left">1691083253</td><td align=left>current</td><td align=right>2022.07</td><td align=right>6.1.42-sunxi64</td><td align=right>861</td><td align=right>3911</td></tr><tr><td align="left"><a href="https://paste.armbian.com/umemohipej">Orange Pi 3 LTS</a></td><td align="left">1691083577</td><td align=left>edge</td><td align=right>2022.07</td><td align=right>6.4.7-sunxi64</td><td align=right>929</td><td align=right>3866</td></tr><tr><td align="left"><a href="https://paste.armbian.com/umofamakom">Odroid C4</a></td><td align="left">1691083533</td><td align=left>current</td><td align=right></td><td align=right>6.1.42-meson64</td><td align=right>858</td><td align=right>5647</td></tr><tr><td align="left"><a href="https://paste.armbian.com/ucehovegok">Odroid C4</a></td><td align="left">1691083939</td><td align=left>edge</td><td align=right></td><td align=right>6.4.7-meson64</td><td align=right>880</td><td align=right>5610</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">Rockpi 4B</a></td><td align="left">1691083473</td><td align=left>legacy</td><td align=right>2022.07</td><td align=right>4.4.213-rockchip64</td><td align=right>890</td><td align=right>6079</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">Rockpi 4B</a></td><td align="left">1691083802</td><td align=left>current</td><td align=right>2022.07</td><td align=right>6.1.42-rockchip64</td><td align=right>890</td><td align=right>6239</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">Rockpi 4B</a></td><td align="left">1691084164</td><td align=left>edge</td><td align=right>2022.07</td><td align=right>6.3.13-rockchip64</td><td align=right>960</td><td align=right>6170</td></tr><tr><td align="left"><a href="https://paste.armbian.com/kawelapewu">NanoPi M4</a></td><td align="left">1691083267</td><td align=left>current</td><td align=right></td><td align=right>6.1.42-rockchip64</td><td align=right>870</td><td align=right>6676</td></tr><tr><td align="left"><a href="https://paste.armbian.com/faqoxudihi">NanoPi M4</a></td><td align="left">1691083612</td><td align=left>edge</td><td align=right></td><td align=right>6.3.13-rockchip64</td><td align=right>840</td><td align=right>6749</td></tr><tr><td align="left"><a href="https://paste.armbian.com/tomafazodu">Le potato</a></td><td align="left">1691083427</td><td align=left>current</td><td align=right></td><td align=right>6.1.42-meson64</td><td align=right>93</td><td align=right>3804</td></tr><tr><td align="left"><a href="https://paste.armbian.com/oyafiyatik">Le potato</a></td><td align="left">1691083899</td><td align=left>edge</td><td align=right></td><td align=right>6.4.7-meson64</td><td align=right>89</td><td align=right>3803</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">Raspberry Pi 4</a></td><td align="left">1691083831</td><td align=left>legacy</td><td align=right></td><td align=right>6.3.13-bcm2711</td><td align=right>90</td><td align=right>1927</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">Raspberry Pi 4</a></td><td align="left">1691084233</td><td align=left>current</td><td align=right></td><td align=right>6.3.13-bcm2711</td><td align=right>89</td><td align=right>1982</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">Raspberry Pi 4</a></td><td align="left">1691084640</td><td align=left>edge</td><td align=right></td><td align=right>6.3.13-bcm2711</td><td align=right>90</td><td align=right>1839</td></tr><tr><td align="left"><a href="https://paste.armbian.com/yusorikiru">Orange Pi R1</a></td><td align="left">1691083477</td><td align=left>current</td><td align=right>2023.07</td><td align=right>6.1.42-sunxi</td><td align=right>89</td><td align=right>2816</td></tr><tr><td align="left"><a href="https://paste.armbian.com/tugequwisi">Orange Pi R1</a></td><td align="left">1691083875</td><td align=left>edge</td><td align=right>2023.07</td><td align=right>6.4.7-sunxi</td><td align=right>90</td><td align=right>2368</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">Banana Pi Pro</a></td><td align="left">1691083360</td><td align=left>legacy</td><td align=right>2023.07</td><td align=right>6.4.7-sunxi</td><td align=right>380</td><td align=right>1018</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">Banana Pi Pro</a></td><td align="left">1691083988</td><td align=left>current</td><td align=right>2023.07</td><td align=right>6.4.7-sunxi</td><td align=right>605</td><td align=right>1012</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">Banana Pi Pro</a></td><td align="left">1691084620</td><td align=left>edge</td><td align=right>2023.07</td><td align=right>6.4.7-sunxi</td><td align=right>467</td><td align=right>1019</td></tr><tr><td align="left"><a href="https://paste.armbian.com/cicuwuzoci">ZeroPi</a></td><td align="left">1691084327</td><td align=left>current</td><td align=right>2023.07</td><td align=right>6.1.42-sunxi</td><td align=right>646</td><td align=right>2553</td></tr><tr><td align="left"><a href="https://paste.armbian.com/nodahorofo">ZeroPi</a></td><td align="left">1691084809</td><td align=left>edge</td><td align=right>2023.07</td><td align=right>6.4.7-sunxi</td><td align=right>562</td><td align=right>2546</td></tr><tr><td align="left"><a href="https://paste.armbian.com/hutosoyiki">Cubietruck</a></td><td align="left">1691083539</td><td align=left>legacy</td><td align=right>2023.07</td><td align=right>5.15.123-sunxi</td><td align=right>580</td><td align=right>1029</td></tr><tr><td align="left"><a href="https://paste.armbian.com/emoxeruluk">Cubietruck</a></td><td align="left">1691084402</td><td align=left>current</td><td align=right>2023.07</td><td align=right>6.1.42-sunxi</td><td align=right>645</td><td align=right>1016</td></tr><tr><td align="left"><a href="https://paste.armbian.com/nojerovupi">Cubietruck</a></td><td align="left">1691085197</td><td align=left>edge</td><td align=right>2023.07</td><td align=right>6.4.7-sunxi</td><td align=right>439</td><td align=right>1013</td></tr><tr><td align="left"><a href="https://paste.armbian.com/izukewepuq">NanoPi R4S</a></td><td align="left">1691083393</td><td align=left>current</td><td align=right></td><td align=right>6.1.42-rockchip64</td><td align=right>890</td><td align=right>6451</td></tr><tr><td align="left"><a href="https://paste.armbian.com/ojewozezoj">NanoPi R4S</a></td><td align="left">1691083751</td><td align=left>edge</td><td align=right></td><td align=right>6.3.13-rockchip64</td><td align=right>890</td><td align=right>6464</td></tr><tr><td align="left"><a href="https://paste.armbian.com/magaceyeji">Clearfog Pro</a></td><td align="left">1691083254</td><td align=left>current</td><td align=right>2018.01</td><td align=right>6.1.42-mvebu</td><td align=right>870</td><td align=right>2228</td></tr><tr><td align="left"><a href="https://paste.armbian.com/uguvohesey">Clearfog Pro</a></td><td align="left">1691083567</td><td align=left>edge</td><td align=right>2018.01</td><td align=right>6.2.16-mvebu</td><td align=right>751</td><td align=right>2229</td></tr><tr><td align="left"><a href="https://paste.armbian.com/mugiditigi">NanoPi Neo 3</a></td><td align="left">1691083523</td><td align=left>current</td><td align=right></td><td align=right>6.1.42-rockchip64</td><td align=right>890</td><td align=right>2163</td></tr><tr><td align="left"><a href="https://paste.armbian.com/unuzivobej">NanoPi Neo 3</a></td><td align="left">1691084137</td><td align=left>edge</td><td align=right></td><td align=right>6.3.13-rockchip64</td><td align=right>851</td><td align=right>1831</td></tr><tr><td align="left"><a href="https://paste.armbian.com/ocomihitax">ODROID M1</a></td><td align="left">1691083432</td><td align=left>edge</td><td align=right></td><td align=right>6.3.13-rk3568-odroid</td><td align=right>970</td><td align=right>5288</td></tr><tr><td align="left"><a href="https://paste.armbian.com/uzizigakub">Orange Pi Zero</a></td><td align="left">1691083290</td><td align=left>legacy</td><td align=right>2023.07</td><td align=right>5.15.123-sunxi</td><td align=right>90</td><td align=right>2488</td></tr><tr><td align="left"><a href="https://paste.armbian.com/eluhunasoz">Orange Pi Zero</a></td><td align="left">1691083862</td><td align=left>current</td><td align=right>2023.07</td><td align=right>6.1.42-sunxi</td><td align=right>90</td><td align=right>2595</td></tr><tr><td align="left"><a href="https://paste.armbian.com/xodawisoru">Orange Pi Zero</a></td><td align="left">1691084314</td><td align=left>edge</td><td align=right>2023.07</td><td align=right>6.4.7-sunxi</td><td align=right>90</td><td align=right>2279</td></tr><tr><td align="left"><a href="https://paste.armbian.com/oduzowomib">Orange Pi Zero Plus</a></td><td align="left">1691083261</td><td align=left>legacy</td><td align=right>2023.07</td><td align=right>5.15.123-sunxi64</td><td align=right>654</td><td align=right>2572</td></tr><tr><td align="left"><a href="https://paste.armbian.com/ugilicecip">Orange Pi Zero Plus</a></td><td align="left">1691083829</td><td align=left>current</td><td align=right>2023.07</td><td align=right>6.1.42-sunxi64</td><td align=right>815</td><td align=right>2500</td></tr><tr><td align="left"><a href="https://paste.armbian.com/ipevitupin">Orange Pi Zero Plus</a></td><td align="left">1691084287</td><td align=left>edge</td><td align=right>2023.07</td><td align=right>6.4.7-sunxi64</td><td align=right>834</td><td align=right>2468</td></tr><tr><td align="left"><a href="https://paste.armbian.com/juzimaciwo">Tinker Board 2</a></td><td align="left">1691084025</td><td align=left>current</td><td align=right>2021.07</td><td align=right>6.1.42-rockchip64</td><td align=right>970</td><td align=right>6725</td></tr><tr><td align="left"><a href="https://paste.armbian.com/uququvofar">Tinker Board 2</a></td><td align="left">1691084374</td><td align=left>edge</td><td align=right>2021.07</td><td align=right>6.3.13-rockchip64</td><td align=right>853</td><td align=right>6628</td></tr><tr><td align="left"><a href="https://paste.armbian.com/nofiyakuse">A64 OLinuXino</a></td><td align="left">1691083542</td><td align=left>legacy</td><td align=right>2023.07</td><td align=right>5.15.123-sunxi64</td><td align=right>343</td><td align=right>2469</td></tr><tr><td align="left"><a href="https://paste.armbian.com/sesobihitu">A64 OLinuXino</a></td><td align="left">1691084458</td><td align=left>current</td><td align=right>2023.07</td><td align=right>6.1.42-sunxi64</td><td align=right>719</td><td align=right>2791</td></tr><tr><td align="left"><a href="https://paste.armbian.com/eriraxiyoq">A64 OLinuXino</a></td><td align="left">1691085162</td><td align=left>edge</td><td align=right>2023.07</td><td align=right>6.4.7-sunxi64</td><td align=right>694</td><td align=right>2772</td></tr><tr><td align="left"><a href="https://paste.armbian.com/isebujogem">Khadas VIM2</a></td><td align="left">1691083382</td><td align=left>current</td><td align=right></td><td align=right>6.1.42-meson64</td><td align=right>961</td><td align=right>6197</td></tr><tr><td align="left"><a href="https://paste.armbian.com/gipucujoka">Khadas VIM2</a></td><td align="left">1691083805</td><td align=left>edge</td><td align=right></td><td align=right>6.4.7-meson64</td><td align=right>890</td><td align=right>6223</td></tr><tr><td align="left"><a href="https://paste.armbian.com/pucudikaxe">Khadas VIM1</a></td><td align="left">1691083341</td><td align=left>current</td><td align=right></td><td align=right>6.1.42-meson64</td><td align=right>93</td><td align=right>3720</td></tr><tr><td align="left"><a href="https://paste.armbian.com/babapociko">Khadas VIM1</a></td><td align="left">1691083737</td><td align=left>edge</td><td align=right></td><td align=right>6.4.7-meson64</td><td align=right>90</td><td align=right>3709</td></tr><tr><td align="left"><a href="https://paste.armbian.com/oxoyiwuxox">Orange Pi R1 Plus LTS</a></td><td align="left">1691083655</td><td align=left>current</td><td align=right></td><td align=right>6.1.42-rockchip64</td><td align=right>535</td><td align=right>1928</td></tr><tr><td align="left"><a href="https://paste.armbian.com/ugiyoqeceq">Orange Pi R1 Plus LTS</a></td><td align="left">1691084275</td><td align=left>edge</td><td align=right></td><td align=right>6.3.13-rockchip64</td><td align=right>538</td><td align=right>1863</td></tr><tr><td align="left"><a href="https://paste.armbian.com/ujifomeraf">Orange Pi Zero Plus 2</a></td><td align="left">1691083347</td><td align=left>legacy</td><td align=right>2023.07</td><td align=right>5.15.123-sunxi</td><td align=right>39</td><td align=right>2505</td></tr><tr><td align="left"><a href="https://paste.armbian.com/itecarenuz">Orange Pi Zero Plus 2</a></td><td align="left">1691084021</td><td align=left>current</td><td align=right>2023.07</td><td align=right>6.1.42-sunxi</td><td align=right>40</td><td align=right>2692</td></tr><tr><td align="left"><a href="https://paste.armbian.com/egequgogux">Orange Pi Zero Plus 2</a></td><td align="left">1691084590</td><td align=left>edge</td><td align=right>2023.07</td><td align=right>6.4.7-sunxi</td><td align=right>38</td><td align=right>2394</td></tr></table>
<!--END_SECTION:data-section-->

## Development

- [Pull request](https://github.com/armbian/build/pulls)
- [Weekly developers meetings](https://forum.armbian.com/events/)
- [Forums for developers](https://forum.armbian.com/forum/4-advanced-users-development/)

## OS download

- [Download](https://www.armbian.com/download/)

## Support

- [Using Armbian](https://forum.armbian.com/forum/23-using-armbian/)

## Contact

- [Forums](https://forum.armbian.com) for Participate in Armbian
- IRC: `#armbian` on Libera.chat
- Discord: [https://discord.gg/armbian](https://discord.gg/armbian)
- Follow [@armbian](https://twitter.com/armbian) on Twitter, [Fosstodon](https://fosstodon.org/@armbian) or [LinkedIn](https://www.linkedin.com/company/armbian).
- Bugs: [issues](https://github.com/armbian/build/issues) / [JIRA](https://armbian.atlassian.net/jira/dashboards/10000)
- Office hours: [Wednesday, 12 midday, 18 afternoon, CET](https://calendly.com/armbian/office-hours)

## License

This software is published under the GPL-2.0 License license.
