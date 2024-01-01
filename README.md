## GNU/Linux Notlarım 

* Bu repository **GNU/Linux Sistem Mühendisliği** eğitimi alırken tutmuş olduğum notlardan oluşmaktadır. Çalışmalarım sırasında; Linux çekirdeğini kullanan ve özgürce kullanılabilen bir işletim sistemi olan **Debian tabanlı Ubuntu** dağıtımı kullanılmıştır.   

# İçerik Tablosu

* [BÖLÜM 1: GİRİŞ](#BÖLÜM-1-GİRİŞ)

* [BÖLÜM 2: İSTEMCİ (CLIENT) KURULUMLARI](#BÖLÜM-2-İSTEMCİ-CLIENT-KURULUMLARI)

* [BÖLÜM 3: TEMEL KOMUTLAR (SHELL KULLANIMI)](#BÖLÜM-3-TEMEL-KOMUTLAR-SHELL-KULLANIMI)

* [BÖLÜM 4: YETKİLER VE KURULUM YÖNETİMİ](#BÖLÜM-4-YETKİLER-VE-KURULUM-YÖNETİMİ)

* [BÖLÜM 5: SİSTEMSEL VE NETWORKSEL YÖNTEMLER, KOMUTLAR, KURULUMLAR](#BÖLÜM-5-SİSTEMSEL-VE-NETWORKSEL-YÖNTEMLER-KOMUTLAR-KURULUMLAR)

* [BÖLÜM 6: SUNUCU YÖNETİMİ](#BÖLÜM-6-SUNUCU-YÖNETİMİ)

* [BÖLÜM 7: İLERİ SEVİYE SİSTEM YÖNETİMİ](#BÖLÜM-7-İLERİ-SEVİYE-SİSTEM-YÖNETİMİ)

## BÖLÜM 1: GİRİŞ

### İşletim Sistemi 

* Donanımlarının denetimi ve yönetiminden sorumlu yazılımdır. 

* Temel sistem işlemlerinden ve programlarının çalıştırılmasından sorumludur. 

* Yazılımların, donanım katmanlarına ve sistem katmanlarına erişebilmesi için arayüz sunar. 

* İşlem (Process) yönetiminden ve işlenme sıralarından sorumludur. 

* Giriş-Çıkış (Input-Output I/O), Ağ (Network) ve Bellek (RAM) yönetimlerinden sorumludur. 

* İşletim sistemleri, ‘Operating System’in kısaltması olan ‘OS’ ile gösterilir.

* Linux, bir işletim sistemi değil; bir işletim sistemi çekirdeğidir.

### Tarihçesi ve Özellikleri

* **Donanım, Çekirdek ve Kabuk’un İşbirliği:**

* Linux’tan önce, AT&T Bell Laboratuvarları’nda geliştirilen, UNIX adında bir işletim sistemi vardı. 

* Lisansının ücretli olması nedeniyle kısıtlı kullanıcıya hitap ediyordu. 

* Ücret ödemek istemeyenler, kendi işletim sistemlerini yazmaya başladılar... 

* Fakat üretilen işletim sistemlerinde, hatalar nedeniyle stabillik uzun süre sağlanamadı. 

* Sahaya Linus Torvalds çıktı ve 1991’de Linux’u yazdı.

* Linux’un, henüz kararlı bir işletim sistemi yoktu. Linus Torvalds bu konuda endişeliydi... 

* İyi bir ‘çekirdek’ bulamama konusunda da benzer endişeyi o dönem, GNU işletim sisteminin kurucusu Richard Stallman yaşıyordu. Çünkü GNU’nun Hurd        isimli, işlevsiz bir çekirdeği vardı. 

* Linux’un iyi bir işletim sistemine; GNU’nun ise iyi bir çekirdeğe ihtiyacı vardı.

* Richard Stallman’ın işletim sistemi olan GNU ve Linus Torvalds’ın çekirdeği Linux birleşti ve GNU/Linux ortaya çıktı. 

* İsmi için yaygın kullanım ‘Linux’ olsa da, doğrusu GNU/Linux’tur.

### GNU NEDİR?

* **(G)NU's (N)ot (U)nix**

* Kurucusu Richard Stallman’dır. 

* ‘’Bilim ancak kollektif olarak gelişir ve bilgi paylaşılmalıdır.’’ denilerek 1983’te ortaya atılmıştır. 

* Sloganı ve açılımı ‘’Gnu is not Unix’’tir. Bu vurgu, Unix’e benzemesi fakat hiçbir Unix kodu içermemesinden dolayıdır. (GNU’nun çekirdeği Hurd’dur.) 

* Hurd çekirdeği yerini Linux çekirdeğine bırakmıştır. Böylelikle GNU bir shell (kabuk); Linux ise bir kernel (çekirdek)’dır. 

* - Linux, Genel Kamu Lisansı (General Public Lisans / GPL) ile sunulan, Linux Vakfı tarafından sahiplenilen ve geliştirilen bir özgür yazılım projesidir. Özgür yazılımların bir çatı altında toplanmasını ve kullanımını amaçlamış bir projedir.

### GPL NEDİR?

* **(G)ENERAL (P)UBLIC (L)ICENSE**

* Topluma mal edilmiş, yazılımın herkese ait olduğunu belirten bir lisanslama türüdür. 

* Hukuki olarak kullanıcının özgürlüğünü savunur. Gelişimleri önlemek yerine desteklemek ve kullanımı yaygınlaştırma amaçlı bir lisanslama modelidir.

* Yazılımın tüm sürümlerini inceleyebilme, değiştirebilme ve paylaşabilme hakkı sunar. 

* Ücretsiz olduğu anlamına gelmez. GPL lisanslı bir yazılımı, geliştiricisi, ücretli dağıtabilir. Sadece yazılımın kaynak kodlarına erişim, diğer yazılımlarla entegrasyonu ve değiştirilebilme gibi özgürlüklerini sağlamalıdır. 

* Özgür haklarla (GPL lisansıyla) edindiğiniz bir yazılımı, değiştirdikten sonra ücretli veya ücretsiz de dağıtsanız, bir sonraki kullanıcının da özgürlüklerini  gözetmelisiniz. GPL’de, özgürlüklere saygı, ilk kuraldır.  Yazılımı yazan kişi, yazılımı kullanan kişi ve yazılımı değiştirip dağıtan kişi aynı haklara sahiptir. Yazılımı yazan kişinin, kullanan ve değiştiren kişiden daha fazla hakkı yoktur, haklar eşittir. 

* Benzer ve detaylı bilgileri aşağıdaki linklerden edinebilirsiniz. 

    - https://linux.org.tr/ 
    
    - https://www.lkd.org.tr/

### GNU/LINUX ÖZELLİKLERİ

* GNU/Linux’un en belirgin özellikleri şunlardır; 

    1) Güvenlik 

    2) Stabillik 

    3) Esneklik 

    4) Desteklilik 

* Açık kaynak kodlu olduğu için bu özelliklerini, dünya çapındaki binlerce geliştiricinin katkı sunumuyla sağlar.

* Wisconsin Üniversitesi’nde 7 ticari işletim sistemi üzerindeki testlerde Hatalı çalışma ortalaması %23 olarak hesaplanmıştır. Bu testte Linux’un hatalı çalışma ve hizmet dışı kalma skoru %9 olmuştur.

### LINUX DAĞITIMLARI
* **Linux Distributions**

* Bir dağıtım, Linux çekirdeği ve üzerindeki tüm yardımcı programlardan oluşur.

* Dağıtımların çoğunluğu, GNU’dan yazılım kaynağı sağlarlar. Bu yüzden dağıtımlar GNU/Linux olarak adlandırılırlar. 

* Dağıtımlar, hedeflenen kullanım amacına göre ufak farklılıklar gösterirler. Dosya-dizin yapıları, yükleme paketleri, uygulamalar, belgeler vs gibi. Ücretli ve ücretsiz de olabilirler.

    - **DEBIAN** --> Kararlılık ve geliştiricilik

    - **SUSE** --> Çok yönlülük

    - **UBUNTU** --> Bireysel, gündelik kullanım

    - **REDHAT** --> Kurumsal, endüstriyel kullanım

    - **FEDORA** --> RedHat tabanlı ve ücretsiz hali

    - **CentOS** --> RedHat tabanlı, Fedora’dan stabil.

    - **PARDUS** --> Bireysel, gündelik kullanım. Milli.

    - **ARCHLINUX** --> Uzmanlık gerektiren, kararlı, stabil.

    - **KALI** --> Debian tabanlı, güvenlik testleri odaklı.

### PAKET YÖNETİM SİSTEMLERİ

| Paket Uzantısı        | Paket Kullanıcısı            | Paket Yükleyicisi  |
| -------------         |:-------------:                | :-----             |
| .deb                  | Debian, Ubuntu               | dpkg, aptitude, apt, dselect             |
| .rpm              | CentOS, Fedora, RedHat, OpenSUSE | yum, dnf, zypper   |
| .*         | Arch Linux                     |   pacman              |
| .pisi         | Pardus, SolusOS                     |   pisi              |

### LINUX DİZİN YAPISI (Linux Directory Structure)

* **/bin** --> Kullanıcı komutları (Terminalde/Shell’de kullanılabilecek komutlar burada yer alır.)

* **/sbin**	--> Sistem komutları (Root kullanıcısı tarafından çalıştırılabilir sistem komutları buradadır.)

* **/etc** --> Konfigürasyon dosyaları (Tüm kullanıcı ve sistemin ayarları dosyalar halinde buradadır. Örn; resolv.conf)	

* **/dev** --> Donanım dosyaları (Donanımları temsil eden dosyalar buradadır. Diskler gibi. Örn; dev/sda5)

* **/proc**	--> Süreç bilgileri (İşletim sistemi işlem süreçlerinin anlık tutulduğu sanal dosyalar buradadır. Örn; proc/meminfo)

* **/var** --> Değişken dosyalar (Event Log (Olay Kayıtları) gibi değişen dosyalar burada tutulur. Örn; /var/log/auth.log)

* **/tmp** --> Geçici dosyalar (Geçici olarak oluşturulması gereken, silinecek olan dosyalar buradadır.)

* **/home**	--> Kullanıcılar için home (ev) dizinleri (Kullanıcıların uygulamarı ve yazma hakkına sahip dosyaları buradadır. ~ işareti ile gösterilir.)

* **/mnt** --> Geçici kullanımdaki dosya sistemleri (Geçici mount edilmiş dosya sistemlerinin mount edildiği dizindir.)

* **/opt** --> Uygulamaların kütüphane dosyaları (Kendi kütüphanesiyle gelen uygulamaların kütüphane dosyaları buradadır. Örn; /opt/winrar)

* **/srv** --> Servis dosyaları (İşletim sisteminde çalışan tüm servis dosyaları buradadır.)

* **/usr** --> Uygulama dosyaları (Çalıştırılabilir dosyalar ve kullanıcı uygulamalarının depolandığı dizindir)

* **/lost + found** --> Silinen dosyalar (Silinen veya kesinti nedeniyle çalışması yarıda kalmış dosyaların tutulduğu dizindir.)

* **/boot** --> Açılış dosyaları (Açılış için gerekli bilgiler ve Kernel (Çekirdek) imajı burada bulunur. Örn; initrd.img)

* **/lib** --> Sistem kütüphaneleri (Kütüphane ve kernel (çekirdek) modülleri dosyaları buradadır.)

* **/media** --> Kaldırılabilir donanımlar (Flash bellek, USB aygıtları, CD-ROM gibi kaldırılabilir donanımların bilgi dosyaları buradadır.)

### Dosya Sistemi ve Dizin Yapısı Hakkında Unutulmaması Gerekenler

* Program dosyaları Windows’taki gibi tek bir klasör (Program Files) altında toplanmaz. Örn; dil dosyaları /usr/share/locale altında; doküman dosyaları /usr/share/doc altında toplanır. 

* Home dizini, Windows’taki Documents and Sharing veya Application klasörleri görevini görür.

* Home dizini için ~ işareti kullanılır. Bu dizindeki dosyalara ~/oku.txt şeklindeki gibi erişilebilir. 

* .so dosyaları Windows’taki .dll’ler gibi kütüphane dosyalarıdır. /lib ve /usr/lib dizininde toplanırlar. 

* /tmp ve /var/tmp dizinleri Windows’taki Temporary işlevindedir. 

* /usr ve /opt dizinleri arasındaki temel fark; /usr’nin sistem; /opt’nin 3.parti uygulamaları tarafından kullanılmasıdır. 

* Windows’takinin aksine dosya isimlerinde küçük-büyük harf duyarlılığı (case sensitive) vardır. Örn; Kayhan, KAYHAN ve KaYhAn ismindeki dosya veya klasörler aynı yerde bulunabilir, oluşturulabilir. 

* Linux’ta donanımlar dahil her şeyin dosyalardan oluştuğunu unutmayın.

### LINUX AÇILIŞ SÜRECİ

* **Donanım, Çekirdek ve Kabuk’un İşbirliği…**

* RunLevels (6) --> Çalışmak istenen seviyenin devreye girmesini, yüklenmesini sağlar.

* init (5) --> Çekirdek, sağlıklı yüklendikten sonra, kendisinin başlangıç işlemi olan ‘init’ işlemini başlatır. Sistemin açıldığı çalışma seviyesinde (runlevels’da) tanımlı olan işlemleri başlatır.

* Kernel (initrd) (4) --> Initial RAM Disk adında bir imajdır. Çekirdek ve gerçek dosya sistemi yüklenmesi sırasında yardımcı olan, geçici bir dosyadır. Tüm dizinler, işletim sistemine burada bağlanır. İşletim sistemi başarılı şekilde yüklendiğinde işi biter.

* G.R.U.B. (3) --> Açılışta, işletim sistemi için seçim listesi (menüsü) sağlar. Seçilen işletim sistemine göre parametereler yüklenerek işletim sistemi açılışı başlar. Bulunabilmek için MBR bilgisine kendisini de eklemiştir.

* M.B.R. (2) --> BIOS’ta tanımlı ilk disk üzerinde işletim sistemi izi arar ve açar. Disklerin ilk sektöründeki 512 B’lık alandır. Diskin dosya sistemi ve  işletim sistemi hakkında bilgi verir. GRUB bilgisi de buradadır.

* P.O.S.T.	 (1) --> BIOS’tan okuduğu (öğrendiği) donanımlar üzerinde çalışırlık testi yapar. Başarılıysa üst etaba geçer.

    - Run Level 0 --> HALT (Sistem çalışmaz durumdadır. ‘Kapalı’ demek değildir. Kesintiyi bekliyor.) 

    - Run Level 1 --> Tek kullanıcılı konsol modu. Ağ erişimi yoktur. 

    - Run Level 2 --> Çok kullanıcılı konsol (terminal) modu. Ağ erişimi yoktur. 

    - Run Level 3 --> Çok kullanıcılı konsol (terminal) modu. Ağ erişimi vardır. 

    - Run Level 4 --> Boştur. Kişisel olarak kurgulanabilir. 

    - Run Level 5 --> Çok kullanıcılı grafik arayüz (GUI) modu. Sıklıkla buradayızdır. 

    - Run Level 6 --> Yeniden başlatma seviyesi.

* /etc/rc{levelno}.d dizini altında yer alırlar.  		

* Hangi run level’da olduğumuzu öğrenmek için: `runlevel` komutu çalıştırılır.

## BÖLÜM 2: İSTEMCİ (CLIENT) KURULUMLARI

## TERMİNAL

#### KONSOL (CONSOLE)

* Terminal, komut ekranına sahip bir Shell (Kabuk) programıdır, emülatörüdür. 

* Kullanıcı ile Kernel (Çekirdek) arasındaki yorumlayıcı olan Shell’i kullanmamızı sağlar. 

* Grafik arayüzden verilen komutların ve alınan çıktıların metinsel ortamıdır. Grafik arayüzden daha fazla komuta sahiptir. 

* Linux’un birden çok (örn; Bash, C, Korn, Zsh, Dash, Fish vb.) Shell çeşidi bulunmaktadır. En yaygını Bash’tir. (echo $SHELL komutu ile öğrenilebilir.)

#### **Terminal Kısayolları**

| Tuş Kombinasyonu  | İşlev  |
| :-------------    | :------             |
| Ctrl + A          | İmleci satır başına götürür.|
| Ctrl + E          | İmleci satır sonuna götürür.   |
| Ctrl + B          | İmleç, birer karakter geri gider. |
| Ctrl + F          | İmleç, birer karakter ileri gider. |
| Alt + B           | İmleç, bir kelime geri gider.   |
| Alt + F           | İmleç, bir kelime ileri gider.   |
| Ctrl + XX         | İmleç, satır başı ile bulunduğu yer arasında gidip gelir.   |
| Ctrl + L          | Ekranı temizler.  |
| Ctrl + U          | İmlecin solundaki her şey silinir.   |
| Ctrl + K          | İmlecin sağındaki her şey silinir.   |
| ESC + T           | İmleçten önceki iki kelimeyi yer değiştirir.   |
| Ctrl + C          | Komutu veya görevi durdurur.|
| Ctrl + Z          | Çalışan komutu veya görevi arka plana atar. `bg` komutu ile öne çağırılır, `fg` komutu ile arkaya gönderilir.|
| Tab               | Komutları otomatik tamamlar. İki kez basıldığında olası komutları listeler.|
| Ctrl + R          | Komut geçmişinde arama ve kullanım sağlar.|
| Ctrl + D          | Terminali kapatır.|


## BÖLÜM 3: TEMEL KOMUTLAR (SHELL KULLANIMI)

### YARDIM ALMA KOMUTLARI

* `<komut> --help` , `help <komut>` --> Komutun parametre ve argümanı hakkında kullanım bilgisi verir. Bazen tanıtım bilgisi (açıklama) de içerebilir.

* `man <komut>` --> Kılavuz sayfalarıdır. Manuel Pages anlamındadır. Yardım alma dosyalarıdır.

    * Man dosyaları yapısal olarak aşağıdaki gibidir: 
        - **NAME:** Komutun ismi ve açıklaması. 
        - **SYNOPSIS:** Komutun nasıl kullanılacağı. 
        - **DESCRIPTION:** Komutun işlevi hakkında detaylı bilgi. 
        - **EXAMPLES:** Kullanımıyla ilgili örnekler. 
        - **SEE ALSO:** İlgili başlıklar. 

    * **/usr/share/man** path’i (yolu) altında bulunurlar.

        - **man1:** Genel kullanıcı programları hakkındadır.
        - **man2:** Sistem programları hk. 
        - **man3:** Kütüphane fonksiyonları hk. 
        - **man4:** Özel dosyalar hk. 
        - **man5:** Dosya biçimleri hk. 
        - **man6:** Oyunlar ve ekran koruyucuları hk. 
        - **man7:** Diğer kategorideki çeşitli komutlar hk.
        - **man8:** Sistem yönetimi ve bakım hk.

* `apropos <KomutunBirKısmı>` --> Verilen ifadenin geçtiği man dosyalarını listeler.

* `whatis <komut>` --> Komut hakkında kısa hatırlatıcı bilgi ve hangi man dosyasında bulunduğunu gösterir. Joker (wildcard) karekter ile kullanılmak istendiğinde `-w` parametresi eklenmelidir. 

    - Örn; ``whatis –w *`` gibi.

### BİLGİ ALMA KOMUTLARI

| KOMUT  | İŞLEV  |
| :-------------    | :------             |
| lsb_release -a , cat /etc/*release  | Kullanılan Linux dağıtımı (distro’su) hakkında ayrıntılı bilgi verir.|
| cat /etc/issue                      | Kullanılan Linux dağıtımnın adını gösterir   |
| uname –a                            | Kullanılan Linux dağıtımının çekirdek (kernel) adını ve versiyonu hakkında bilgi verir. -n, -m, -r parametreleriyle daha ayrıntısız bilgi alınabilir. |
| hostname                            | Bilgisayar adını (hostname’i) verir.  |
| w , who , whoami                    | w komutu, aktif kullanıcı, oturum açma (login) saati ve son açtığı uygulama bilgisi verir. who komutu, aktif kullanıcı ve login saatini verir. whoami komutu, aktif kullanıcı bilgisi verir. -b ve –r parametleriyle de kullanılır. |
| uptime                              | Sistemin yüklendiğinden itibaren ne kadar saat açık kaldığını gösterir. |
| whereis <argüman>                   | İlgili komut, dosya veya klasörün path’ini (yolunu) ve man dosyasının yerini gösterir. -b, -m ve –s paremetreleriyle de kullanılır.   |
| which <argüman>                     | Komutların yerini gösterir.   |
| cat /proc/cpuinfo                   | CPU hakkında detaylı bilgi verir.    |
| cat /proc/meminfo                   | RAM hakkında detaylı bilgi verir.   |
| df –h –T ve lsblk                   | Fiziksel ve mantıksal disk kullanımı ve dosya sistemi hakkında bilgi verir.   |
| du –h                               | Mevcut klasör ve altındaki klasör, dosya boyutları hakkında bilgi verir.   |
| vmstat                              | Sistemin anlık performansı hakkında genel bilgi verir.    |
| cal                                 | Calendar (takvim) anlamındadır. Bulunduğumuz ayın takvimini görüntüler.    |
| date                                | Günün tarih, saat ve dilimini verir.   |

### İÇERİK KOMUTLARI

| KOMUT  | İŞLEV  |
| :-------------    | :------             |
| pwd  | Hangi dizinde olduğunuzu gösterir.|
| cd <path(yol)>                      | ‘Change Directory’ anlamındadır. Dizinlere girmenizi sağlar.  |
| cd  | Tek başına kullanıldığında, kullanıcı (home/user) dizinine gönderir.|
| cd ..                      | İki nokta ile kullanıldığında, bir üst dizine gönderir.   |
| cd ../../  | İki nokta slaş ile kullanıldığında, iki nokta slaş sayısı kadar üst dizine gönderir.|
| cd ../<path>                      | Önce üst dizene, ardından üst dizinde bulunan ilgili path’e gider.   |
| cd -  | Çalıştığımız son iki dizin arasında geçiş yapar.|
| ls                     | ‘List’ anlamındadır. Bulunulan dizinin altındaki dosyaları ve alt dizinleri listeler.    |

*  
    - `ls -l` parametresiyle daha ayrıntılı listeleme yapar.
    - `ls -la` parametresiyle gizli dosyalar da listelenir. Gizli dosya isimleri .(nokta) ile başlar.
    - `ls -S` parametresiyle dosya büyüklüğüne göre listeleme yapar.
    - `ls -lh` parametresiyle dosya büyüklüklerini daha anlaşılır listeler.
    - `ls -lt` parametresiyle dosya ve dizinleri değişiklik tarihine göre listeler.
 
### DOSYA, DİZİN KOMUTLARI (FILE, DIRECTORY COMMANDS)

| KOMUT  | İŞLEV  |
| :-------------    | :------             |
| touch <dosyaadı>  | Dosya oluşturmak için kullanılır.|
| cat <dosyaadı>    | Dosya okumak için kullanılır. -n parametresiyle satırlar numaralı gösterilir. `nl <dosyaadı>` komutuyla aynı işlevdedir. |
| echo ‘’ifade’’  |Terminale yazı yazdırmak için kullanılır. Dosyaya yazmak için ‘>’ operatörü kullanılmalıdır.|
| more ve less <dosta> | Uzun olan çıktıların daha rahat (bölümlü) okunmalarını sağlarlar. |
| head ve tail <dosya> | Çıktıların ilk 10 veya son 10 satırını görüntüler. –n parametresiyle 10 değeri değiştirilebilir.|
| sort <dosya>  | Dosyaları alfabetik sıralamayla listeler.|
| grep <ifade> <dosya/dizin>  | Bir ifadeyi herhangi bir dosya veya dizinde aramak için kullanılır. -v parametresi, verilen ifadeyi içermeyen aramalar yapar. Tersine davranır. -i parametresi, arama sırasında küçük/büyük harf duyarlılığı gözetmez. -r parametresi, alt dizinlerde de arama yapar. |
| find <dosya> <ifade>  | Belirli bir dosya veya dizin içinde geçen ifadeleri aramak için kullanılır.|

| KOMUT  | İŞLEV  |
| :-------------    | :------             |
| cp <kaynak> <hedef> | Dosya kopyalama komutudur. -i parametresi ile, üzerine yazma işlemlerinde onay istenir. -r parametresi ile dizinler de kopyalanabilir. |
| mv <kaynak> <hedef>  |Dosya taşıma komutudur. cp komutundaki kullanımlar burada da geçerlidir. Dosya uzantılarını değiştirmek için de kullanılır. `mv <dosyaadı> <dosyaadı.uzantısı>` |
| rm <dosya/dizin>  | Dosya silme komutudur. * kullanımı ile ilgili dizin altındaki tüm dosyalar silinebilir. -r parametresiyle alt dosya ve dizinler silinebilir. -ri parametresiyle silme onayı istenir. -rf parametresiyle sorgusuz silme işlemi yapılır.|
| mkdir <dizinadı>  | Dizin oluşturma komutudur. mkdir dizin1 dizin2 dizin3 ... -p parametresi, alt dizinlerle birlikte oluşturur. `mkdir –p dizin/altdizin/enaltdizin` |

### ARŞİV KOMUTLARI (ARCHIVE COMMANDS)

* **Arşivleme komutları:** 

    - `tar cf <dosya.tar> <dosyalar>` --> Dosyaları arşivleme komutudur. Sıkıştırma uygulamaz. c=create, f=file’ı temsil eder. 
    - `tar xvf <dosya.tar>` --> Arşivten çıkarma komutudur. x= extract, v=verbose, f=file’ı temsil eder.

* **Sıkıştırma komutları:**

    - `gzip <dosya>` --> Dosyaları sıkıştırma komutudur. Oluşan dosya, .gz uzantısı alır.
    - `gunzip <dosya.gz>` --> Gz dosyalarını çıkarma komutudur.

    - `bzip2 <dosya>` --> Dosya sıkıştırma komutudur. Oluşan dosya, .bz2 uzantısı olur.
    - `bunzip2 <dosya.bz2>` --> Bz2 dosyalarını çıkarma komutudur.

* **Sıkıştırarak Arşivleme Komutları:**

    - `tar czvf <dosya.tgz/tar.gz> <dosyalar>` --> Dosyaları Gzip kullanarak sıkıştırma ve arşivleme komutudur.
    - `tar xzvf <dosya.tgz/tar.gz>` --> Tgz dosyalarını çıkarma komutudur.

    - `tar cjvf <dosya.tar.bz2> <dosyalar>` --> Dosyaları Bzip2 kullanarak sıkıştırma ve arşivleme komutudur. 
    - `tar xjvf <dosya.tar.bz2>` --> bz2 dosyalarını çıkarma komutudur.

* **İçerik Okuma Komutları:** 

    - `zcat <dosya.tgz>` --> Gzip dosyalarının içeriği okuma/listemele komutudur.
    - `bzcat <dosya.bz2>` --> Bzip2 dosyalarının içeriği okuma/listemele komutudur.

* **Zip ve Rar Sıkıştırma/Açma:**

    - `zip <dosya.zip> <dosyalar>` --> Dosyaları zip kullanarak sıkıştırma komutudur. 
    - `unzip <dosya.zip>` --> Zip dosylarını çıkarma komutudur.

    - `unrar <dosya.rar>` --> Rar dosyalarını çıkarma komutudur.

### KOMUT OPERATÖRLERİ (COMMAND OPERATORS)

| KOMUT  | İŞLEV  |
| :-------------    | :------             |
| `<komut> > <dosyaadı>` | Komutun çıktısını bir dosyaya yazdırır.|
| `<komut> ; <komut>`  | Birinci komut tamamlandığında, ikinci komutu çalıştırır.|
| `<komut> && <komut>` | Birinci komut başarılı olduğunda, ikinci komutu çalıştırır.|

* 
    - `<komut> | <komut>` --> Birinci komutun çıktısını, ikinci komuta girdi olarak gönderir.
    - `<komut> || <komut>` --> Birinci komut başarısız olduğunda, ikinci komutu çalıştırır.

### BASH SHELL İPUÇLARI (BASH SHELL TIPS)

#### Bash Shell Dosyaları

* Bash shell’inin kendisi, /bin/bash dosyasıdır. Buradan çalışır. 

* Bash shell’inin genel ayar dosyası /etc/profile dosyası içindedir. Genel ayarlar buradan okunur. 

* Bash shell’inin kullanıcıya özgü ayarları ~/.bashrc dosyası içindedir. 

* Bash shell’inde kullanılan komutların geçmişi ~/.bash_history içindedir.

| PATH   | AÇIKLAMA  |
| :-------------    | :------             |
| /bin/bash | Bash Shell’i.|
| /etc/profile  | Bash’in genel ayar dosyası.|
| ~/.bashrc | Bash’in kullanıcı ayar dosyası. Kullanıcı için başlatma ayarlarını içerir. Önce /etc/bash.bashrc çalışır, ardından ~/.bashrc dosyasını çağırır.|
| ~/.bash_history | Kullanıcının bash’te kullandığı komutların geçmişini tutar. Default’ta (varsayılanda) son 1000 adet komutu hatırlar.|

### HISTORY KOMUTU

| KOMUT  | İŞLEV  |
| :-------------    | :------             |
| ~/.bash_history | Geçmişte kullanılan komutların saklandığı dosyadır.|
| history  | Geçmişte kullanılan belirli sayıdaki komutu listeler.|
| history <sayı> | Geçmişte en son kullanılan komutları verilen sayı kadar listeler.|
| `! <numara>` | İlgili numaradaki komutun tekrar çalıştırılmasını sağlar.|
| !! | Son çalıştırılan komutun tekrar çalıştırılmasını sağlar.|
| `! <komut> :p` | İlgili komutun, daha önce kullanıldığı son haliyle tekrar çalıştırılmasını sağlar.|
| $HISTSIZE | En son girilen kaç komutun hatırlanacağını görüntüler. ~/.bashrc dosyası içinde $HISTSIZE değeri değiştirilebilir.|
| history -d <satırnumarası> | İlgili satırda hatırlanan komutun unutulmasını (geçmişten silinmesini) sağlar.|
| history -c | Geçmişin silinmesini sağlar.|

### ALIAS TANIMLARI

* Alias’lar, komutlara verilen takma adlardır. 

* Uzun, zorlu veya sık kullanılan komutların, kolay çağırılması için kullanılırlar. 

* Kullanıcının alias tanımları için ~/.bashrc dosyası kullanılır. 

* alias =‘’ formatında oluşturulmalıdır. Örn; alias cl=‘clear’

## BÖLÜM 4: YETKİLER VE KURULUM YÖNETİMİ

### DOSYA VE DİZİN ERİŞİM YETKİLERİ (FILE AND DIRECTORY ACCESS PRIVILEGES)

* Dosya ve dizinlerin (nesnelerin) erişim hakları ls –l komutuyla görüntülenebilir.

* Yetkilerdeki ifadeler, dosya veya dizinler (nesneler) için şöyle anlamlandırılır:

| Karakter   | Anlamı  |
| :-------------    | :------             |
| d | Directory anlamındadır. Nesnenin dizin olduğunu belirtir.|
| -  | Nesnenin bir dosya (file) olduğunu (dizin/directory) olmadığını) belirtir.|
| r  | Read anlamındadır. Nesnede okuma yetkisi bulunduğunu belirtir.|
| w | Write anlamındadır. Nesnede yazma yetkisi bulunduğunu belirtir.|
| x  | Execute anlamındadır. Nesnede çalıştırma yetkisi bulunduğunu belirtir.|

* Yetki ifadeleri 10 adettir. 

* 4 bölümden oluşurlar.

| 1. Bölüm | 2. Bölüm | 3. Bölüm  | 4. Bölüm |
| -------------  |:------------- | :-----| :--------------- |
| Nesne Türü    | Kullanıcının (User’s) Yetkileri | Grubun (Group’s) Yetkileri | Diğerlerinin (Others) Yetkileri |
| - veya d | rwx | rwx | rwx |
| Dosya veya Dizin | Read, Write, Execute (Okuma, Yazma, Çalıştırma) | Read, Write, Execute (Okuma, Yazma, Çalıştırma) | Read, Write, Execute (Okuma, Yazma, Çalıştırma)|

### DOSYA VE DİZİN ERİŞİM YETKİLERİ

* Dosya ve dizinlerin (nesnelerin) erişim hakları chmod komutuyla değiştirilir. 

* Kullanım kalıbı şu şekildedir: 

    - `chmod u/g/o/a +/-/= r/w/x/s/t <nesne>`

* Komuttaki ifadeler şöyle anlamlandırılır:

| 1. Bölüm | 2. Bölüm | 3. Bölüm  | 4. Bölüm | 5. Bölüm |
| -------------  |:------------- | :-----| :--------------- | :-------- |
| Komut | Parametre | Parametre | Parametre | Nesne |
| Chmod | u, g, o, a | +, -, = | r, w, x | nesne |
| | user, group, others, all | ekleme, çıkarma, eşitleme | read, write, execute | |

* Örneğin test isimli bir txt dosyasına, herkes için okuma izni vermek istersek;
    - `chmod a+r test.txt `

### SAYISAL İFADELERLE 

* Yetkiler, rakamlarla da sayısal olarak ifade edilebilirler.

| YETKİ | SAYISAL İFADE |
| ----- |:-----|
| r | 4 |
| w | 2 |
| x | 1 |

| 1. Bölüm | 2. Bölüm | 3. Bölüm  | 4. Bölüm | 
| -------------  |:------------- | :-----| :--------------- |
| Nesne Türü | Kullanıcının (User’s) Yetkileri | Grubun (Group’s) Yetkileri | Diğerlerinin (Others) Yetkileri |
| - veya d| r w x | r w x | r w x |
| Dosya veya Dizin | 4 2 1  | 4 2 1  | 4 2 1 |

* İlgili bölümün yetki rakamları toplanır. Toplam sayı, ilgili bölümün yetkilerini sayısal olarak ifade eder.

| 1. Bölüm | 2. Bölüm | 3. Bölüm  | 4. Bölüm | 
| -------------  |:------------- | :-----| :--------------- |
| Nesne Türü | Kullanıcının (User’s) Yetkileri  | Grubun (Group’s) Yetkileri | Diğerlerinin (Others) Yetkileri |
| - veya d | r w x | r w x | r w x |
| Dosya veya Dizin | 4+2+1 = 7 | 4+2+1 = 7 | 4+2+1 = 7 |

* Yetkinin bulunmadığı durum, 0 (sıfır) değerindedir. - Örnek;

| 1. Bölüm | 2. Bölüm | 3. Bölüm  | 4. Bölüm | 
| -------------  |:------------- | :-----| :--------------- |
| Nesne Türü | Kullanıcının (User’s) Yetkileri | Grubun (Group’s) Yetkileri | Diğerlerinin (Others) Yetkileri |
| - veya d | r - x | - w x | r w - |
| Dosya veya Dizin | 4+0+1 = 5 | 0+2+1 = 3 | 4+2+0 = 6 |

* Chmod komutuna sadece sayısal değer verilmesi yeterlidir. 

* Her bir rakam, bir bölümü temsil edecektir. 

* Örn;	 
    - chmod 777 test.txt 	(Test.txt dosyasına kullanıcı, grup ve diğerleri için rwx yetkisi verilmiş olur.) 

    - chmod 755 test.txt 	(Test.txt dosyasına kullanıcı için rwx, grup için r-x ve diğerleri için r-x yetkisi verilmiş olur.) 

    - chmod 536 test.txt	(Test.txt dosyasına kullanıcı için r-x, grup için -wx ve diğerleri için rw- yetkisi verilmiş olur.)

### LOKAL KULLANICI KOMUTLARI (LOCAL USER MANAGEMENT)

* Sistemdeki en yetkili kullanıcı root’tur. 

* Kullanıcı bilgileri /etc/passwd 

* Kullanıcı şifreleri /etc/shadow dosyasında yer alır. Okumak, root yetkileri gerektirir. 

* Şifresinin bilinmesi halinde, shell’de root yetkileri geçici olarak devralınabilir. 

* root yetkilerine sahip sudo grubunun üyesi olunabilir. Yetki yükseltme gerektiğinde sudo komutu kullanılabilir. 

* Linux: ‘’Sudo is enough.’’

#### Lokal Kullanıcı Yönetimi Komutları

| KOMUT | İŞLEV |
| -------------  |:------------- |
| chage –l <kullanıcıadı> | Kullanıcının bilgilerini görüntüler. |
| chfn <kullanıcıadı> | Kullanıcı bilgilerinin değiştirilmesini sağlar. |
| passwd <kullanıcıadı> | Kullanıcının şifresini değiştirir. |
| adduser <kullanıcıadı> , useradd –m <kullanıcıadı> | Kullanıcı oluşturma komutlarıdır. –m parametresi, home dizini de yaratılmasını sağlar. |
| deluser --remove-all-files <kullanıcıadı> , userdel –remove-all-files <kullanıcıadı> | Kullanıcı silme komutlarıdır. –remove-all-files parametresi kullanılmazsa, home dizini silinmez.|
| su - <kullanıcıadı> | Diğer kullanıcının yetkilerini ve shell’ini devralır. |
| usermod –a –G sudo <kullanıcıadı> | Kullanıcıyı, root yetkilerine sahip sudo grubunun üyesi eder. |
| `sudo <komut>` | Komutu, sudo grubu aracılığıyla, root kullanıcısının yetkileri ile çalıştırır. |

### PAKET KURULUMLARI (PACKET INSTALLATIONS)

#### Paket ve Paket Yöneticileri

* Paketler manuel ya da repository (repo) adındaki depolardan yüklenirler. 

* Debian’da manul paketler dpkg aracı ile; repo paketleri apt aracı ile yüklenirler. 

* CentOS’ta manuel paketler rpm aracı ile; repo paketleri yum aracı ile yüklenirler. 

    - Debian’da repolar /etc/apt/sources.list dosyasında; 
    - CentOS’ta repolar /etc/yum.repos.d dosyasındadır.

* **/etc/apt/sources.list**

#### Paket Komutları

| Araç / Yönetici | Parametre | Argüman | İşlev | 
| -------------  |:------------- | :-----| :--------------- |
| dpkg | -l | | Sistemdeki paketleri listeler. |
| dpkg | --get-selections| | Kurulu ve kaldırılmış programları listeler. |
| dpkg | -s | <programadı> | Kurulan program hakkında bilgi verir.|
| dpkg | -L | <programadı> | Kurulu programın paket içeriğini gösterir. |
| dpkg | --info| <paketadı.deb> | Kurulacak program hakkında bilgi verir. |
| dpkg | -c | <paketadı.deb> | Programın nereye kurulacağını gösterir. |
| dpkg | -i | <paketadı.deb> veya *.deb | Pakedi yükler. * ile çoklu yükleme yapar. |
| dpkg | -reconfigure | <programadı> | Kurulu programı onarır. |
| dpkg | -P | <programadı> | Kurulu programı kaldırır. |
| apt-get | install| <programadı> | Programın depodan (repodan) yükler. |
| apt-cache | Show | <programadı> | Yüklenecek program hakkında bilgi verir. |
| apt-get | remove | <programadı> | Kurulu programı kaldırır. |
| apt-get | purge | <programadı> | Programı tüm dosyalarıyla kaldırır. |

### KAYNAK KOD KURULUMU (SOURCE CODE INSTALLATION)

#### Kaynak Kod Kurulum Komutları

* Programlar, paketlerle kurulabildiği gibi kaynak kodlarıyla da kurulabilirler. 

* Bunun yapılabilmesi için DKMS (Dynamic Kernel Module Support) framework’ü kurulu olmalıdır. 

* Programın kaynak kodlarını indirip dizinine girilir ve aşağıdaki komutlar kullanılır.

| KOMUT | İŞLEV |
| -------------  |:------------- |
| ./configure | Kaynak kodu hakkında ayarlamalar içerir. Her zaman bulunmaz. |
| make | Kaynak kodun makefile dosyasını arar ve yükleme işlemi için hazırlar. | 
| make install | Kaynak kodu yükler. |
| ./<dosyadı>.sh | Kaynak kodu yüklenmesini otomatikleştirir veya kurulumda opsiyonlar sunar. |

### SİSTEM GÜNCELLEME (SYSTEM UPDATE)

#### Sistem Güncelleme Komutları

* Güncelleme işlemi gerekliliği, sistemdeki program versiyonlarının, depolardaki versiyonlar ile karşılaştırılmasıyla belirlenir. (apt-get update) 

* İndirilen update dosyaları için archive (arşiv); indirilen yere de cache (önbellek) adı verilir.

| ARAÇ / YÖNETİCİ | PARAMETRE | İŞLEV |
| -------------  |:------------- | :------- |
| apt-get | update | Mevcut programlar ile depodakiler arasında versiyonları kıyaslar ve güncelleme için indeks yaratır.|
| apt-get | upgrade | Mevcut programların güncellenmesini sağlar. |
| apt-get | dist-upgrade | Bağımlılık problemlerini çözer ve kernel’ı günceller. |
| apt-get | autoclean | Cache’te olup, depoda artık bulunmayan paketleri kaldırır. |
| apt-get | autoremove | Kaldırılmış bir paketin bağımlılığı olarak yüklenen paketleri arar ve kaldırır. |
| apt-get | clean | Cache’teki tüm arşivleri kaldırır. |

### BÖLÜM 5: SİSTEMSEL VE NETWORKSEL YÖNTEMLER, KOMUTLAR, KURULUMLAR

#### SEMBOLİK VE KATI LİNK KAVRAMLARI (SYMBOLIC & HARD LINK SUBJECTS)

* Sembolik link’ler bir dosya için sadece kısayoldurumu oluşturur ve içeriğine erişim için sadece yönlendirme yaparlar. (Bağ adı da verilir.)

* Katı Link’ler ise bir dosyanın, birden fazla yere kopyalanmasını ve erişimini sağlarlar. Orijinal dosyanın silinmesiyle veri kaybolmaz. 

* Dosya ve dizinler, benzersiz olan numaralara (ID’lere) sahiptirler. Her dosya ve dizin benzersiz ID’lere sahiptir. Bu yapının adı inode (düğüm)’dur. Dosya ve dizinlerin ID’lerine de inode ID’si denir.

* Inode ID’ler, ls –li komutuyla görülebilirler. (Dosya sistemi inode’ları içinse df –i komutu kullanılır.)

* Sembolik linkler için inode ID’ler benzersizdir; fakat katı linkler için benzeşiktir.

| KOMUT | İŞLEV |
| -------------  |:------------- |
| `ls –li <dosyaadi>` | Inode ID’leri gösterir. |
| ln <path/dosyaadı> | Hard Link oluşturur. |
| ln -s <path/dosyaadı> | Symbolic Link oluşturur. |
| find -type f -links +1 -ls | Sistemdeki hard link’leri gösterir. |

### SÜREÇ YÖNETİMİ (PROCESS MANAGEMENT)

#### Süreç Yönetim Komutları

| KOMUT | iŞLEV |
| -------------  |:------------- |
| ps aux  | Sistemdeki tüm süreçleri gösterir. |
| ps -e  | Sadece sistem süreçlerini gösterir. |
| `ps –u <user>` | Kullanıcıya ait süreçleri gösterir. |
| top | Süreçleri 3 saniyede bir listeler. |
| `top -d <numara>` | Süreçleri belirtilen numara kadar saniyede bir listeler. |
| pstree –p | Süreçleri, bağımlılıkları ve PID (Process ID)’leri ile gösterir. |
| `pstree <user>`| Kullanıcıya ait süreçleri bağımlılıklarıyla listeler. |
| pgrep <süreçadı> | Belirtilen sürece ait PID’leri görüntüler. |
| `pgrep –lu <user>` | Belirtilen kullanıcıya ait süreçleri en özet şekilde listeler. |
| `kill <PID>`| Belirtilen PID’ye ait sürecin sonlandırılmasını sağlar. |
| `kill -9 <PID>`| Belirtilen PID’ye ait sürecin sonlandırılmasını zorlar.  |
| killall <süreçadı> | Belirtilen sürece bağlı tüm süreçlerin sonlandırılmasını sağlar.  |
| killall -9 <süreçadı> | Belirtilen sürece bağlı tüm süreçlerin sonlandırılmasını zorlar. |
| xkill | GUI’si yanıt vermeyen uygulamayı sonlandırmaya zorlar. |

*   - ps aux | grep <süreçadı> --> İsmi belirtilen işleme ait süreçleri gösterir.

### SERVİS YÖNETİMİ (SERVICE MANAGEMENT)

* Servisleri, çalışma seviyeleri (run levels) başlatır veya sonlandırır. Her çalışma seviyesi, hangi servislerin başlatılması ya da sonlandırılması gerektiğini /etc dizini altındaki kendi dosyalarından okur. (etc/rc0.d, rc1.d, rc5.d gibi 

* Burada okuduğu her servis, aslında bir sembolik linktir. Servisler, etc/init.d altında bulunurlar. 

* Her servis /etc/init.d dizininde bir script’e bağlıdır. Servisler, başlama veya kapanma davranışlarını, /etc/init.d altındaki script’lere göre belirlerler.

#### Servis Yönetim Komutları

| KOMUT | iŞLEV |
| -------------  |:------------- |
|service --status-all|Tüm serivlerin çalışırlık durumunu görüntüler.|
|service <servisadı> status|İlgili servisin durumunu görüntüler.|
|service <servisadı> start|İlgili servisi başlatır.|
|service <servisadı> stop|İlgili servisi durdurur.|
|service <servisadı> restart|İlgili servisi yeniden başlatır. (Kapatıp açar.)|
|systemctl --type=service|Tüm servislerin durumu ve açıklamasını görüntüler.|
|systemctl enable <servisadı>|İlgili servisin sistem açılışında çalışmasını sağlar.|
|systemctl disable <servisadı>|İlgili servisin sistem açılışında çalışmamasını sağlar|

### DİSK YÖNETİMİ (DISK MANAGEMENT)

* Linux’ta Journalling dosya sistemi kullanılır. Journalling, diske yazılan ve diskten okunan işlemleri dosyalara yazar; böylelikle beklenmedik güç kesintilerinde bozulan yapı onarılabilir. 

* Linux’ta diskler de, diğer donanımlar gibi dosya halinde görünürler ve /dev dizini altındadırlar. 

* Linux’ta diskler mount edilerek (bağlanarak) aktifleştirilir. Mount bilgileri /etc/fstab dosyasından okunur. 

* Diskler yaygın olarak EXT3 ve EXT4 dosya sistemini kullanırlar. EXT dosya sistemi, NTFS’e göre daha hızlı, stabil ve güvenlidir. Ayrıca daha da yenidir. 

* Linux’ta RAM ve disk kullanımını organize eden tempfs ve ramfs dosya sistemi özelliği de bulunur. Önce RAM’i disk gibi kullanırlar, RAM’dedirler; RAM’de yer kalmadığında ise diski RAM gibi kullanırlar. Diskin RAM olarak kullanıldığı alana Swap adı verilir. (Ramfs, Swap kullanmaz, sürekli RAM’dedir.)

#### Disk Yönetim Komutları

| KOMUT | iŞLEV |
| -------------  |:------------- |
|df -h|Dosya sistemi ve mount hakkında bilgiler verir|
|sblk –p|Fiziksel diskler hakkında bilgi verir.|
|parted -l|Partition’lar hakkında bilgi verir|
|`fdisk <disk>`|Disk bölümleme aracıdır. -l parametresiyle bilgi verir.|
|`mkfs.<dosyasistemi> <disk>`|Belirtilen diski, belirtilen dosya sistemiyle formatlar|
|`mount <disk> <dizin>`|Belirtilen diskin, belirtilen dizine mount edilmesini sağlar. |
|`umount <disk>`|Belirtilen diskin unmount edilmesini sağlar.|
|blkid|Mount edilen disklerin ID’lerini (UUID’lerini) gösterir.|
|`fsck <disk>`|Diskte bulunan hataları denetler.|
|du –h <dosya/dizin>|İlgili dosya veya dizinin diskte kapladığı alan görüntülenir. |
|du –sh <dosya/dizin>|İlgili dosya veya dizinin alt dizinleriyle birlikte, diskte kapladığı toplam alan görüntülenir.|

### NETWORK YÖNETİMİ (NETWORK MANAGEMENT)

#### Network Komutları

| KOMUT | iŞLEV |
| -------------  |:------------- |
|ip a|Network kartları hakkında bilgi verir.|
|`ip addr del <IP> dev <interface>`|Belirtilen IP’yi, belirtilen interface’ten siler.|
|`ip addr add <IP> dev <interface>`|Belirtilen IP’yi, belirtilen interface’e tanımlar.|
|`ip route add default via <defaultgw>`|Default gateway ekler.|
|vi /etc/resolve.conf|DNS sunucu bilgilerini görüntüler.|
|ip link set <interfaceadı> down / up|Belirtilen interface’in kapatılmasını/açılmasını sağlar.|
|nmcli device status|Interface’lerin bağlantı, aygıt ve tip bilgilerini verir.|
|ip r|Route tablosunu görüntüler.|
|`ip route add <network> via <defaultgw> `|Statik route ekler.*|
|`dev <interface>`|Statik route’ u siler.|
|`ip route del <network>`|*Kalıcı olması için /etc/network/interfaces dosyasına “`up /sbin/ip route add <network> via <defaultgw> `dev <interface>` ‘’ değeri eklenmelidir.|
|ip -s link show|Interface istatistiklerini görüntüler.|
|/etc/init.d/networking stop / start / restart|Interface’leri kapatır/açar/yeniden başlatır.|
|`host <adres>`|Belirtilen adres için IP çözümlemesi yapar.|
|`telnet <IP> <port>`|Belirtilen IP’de, belirtilen portun açık/kapalı durumunu kontrol eder.|
|apt-get install net-tools|ifconfig, netstat, arp, iptables gibi komutları kazandırır.|
|netstat -tunae|Sistemin bağlantı kurduğu IP ve portları görüntüler.|
|lsof –i|Bağlantı kurmuş olan programları listeler.|
|lsof –i :port|Belirtilen porta ait açık bağlantıları listeler.|

### KAYIT YÖNETİMİ (LOG MANAGEMENT)

* Log’lar, sistemde gerçekleşen tüm değişikliklerin kaydını tutan, metin tabanlı dosyalardır.

* Log’lar /var/log dizini altında bulunurlar.

| DOSYA / DİZİN | AÇIKLAMA |
| -------------  |:------------- |
|/var/log/auth.log|Kullanıcı login kayıtlarıdır.|
|/var/log/lastlog|En son oturum açan kullanıcı kayıtlarıdır.|
|/var/log/user.log|Kullanıcı aktivite kayıtlarıdır.|
|/var/log/boot.log|Sistem açılışı (boot) kayıtlarıdır.|
|/var/log/kern.log|Çekirdek (kernel) kayıtlarıdır.|
|/var/log/cron.log|Zamanlanmış görevlerin kayıtlarıdır.|
|/var/log/messages|Sistem aktivite kayıtlarıdır. Sistem mesajlarıdır.|
|/var/log/syslog|Sistem mesaj servisinin kayıtlarıdır.|
|/var/log/debug|Hata ayıklama (debug) için oluştulan kayıtlardır.|
|/var/log/deamon.log|Çalışan servislerin kayıtlarıdır.|
|/var/log/proftpd|FTP servisinin kayıtlarıdır.|
|/var/log/maillog|Mail servisinin kayıtlarıdır.|
|/var/log/dpkg.log|DPKG paket yöneticisinin kayıtlarıdır.|

#### Kayıt Yönetim Komutları

| KOMUT | iŞLEV |
| -------------  |:------------- |
|last -10 –i|Sistemde oturum açmış en son 10 kullanıcıyı, IP bilgisiyle verir.|
|lastlog |Uzaktan sisteme oturum açmış kullanıcı bilgilerini verir. |
|`lastlog –u <user>`|İlgili kullanıcının uzaktan en son ne zaman oturum açtığını verir.|
|dmesg|Sistem açılışı sırasındaki mesajları görüntüler.|
|cat /var/log/auth.log |Kullanıcı login kayıtlarını verir. |
|tail -f /var/log/auth.log|Kayıtları gerçek zamanlı olarak listeler.|

### GÖREV YÖNETİMİ (TASK MANAGEMENT)

* Linux’ta, zamanlanmış görevleri cron adındaki servis yönetir. Durumunu öğrenmek için service cron status komutuyla kontrol edilmelidir. 

* Görev /etc/crontab dosyasına eklenir. Cron servisi, her dakika burayı kontrol eder. 

* "*" ifadesi ‘her’ anlamına gelmektedir.

* Zamanlanmış görevler için tanımlar 6 bölümden oluşur:

|Değer Cinsi:|Dakika|Saat|Gün|Ay|Hafta Günü|Görev|
| --- |:-- |:---|:---|:---|:---|:---|
|**Değer Aralığı:**|0-59|0-23|1-31|1-12|1-7|Komut|

* Örn: 
    - `0 5 * * 1 tar -zcf /var/backups/home.tgz /home/` --> ‘’Sıfırıncı dk’da, saat 5’te, ayın her günü, her ay, Pazartesi günü /home dizinini, /var/backups dizini altına home.tgz adıyla arşivle.

| KOMUT | iŞLEV |
| -------------  |:------------- |
|crontab -l|Kullanıcının zamanlanmış görevlerini listeler.|
|`crontab -u <user> -l`|İlgili kullanıcının zamanlanmış görevlerini listeler.|
|crontab -e|Görev zamanlamak için editör seçimi yaptırır.|
|crontab -r|Zamanlanmış görevleri siler.|

### ORTAM DEĞİŞKENLERİ (ENVIRONMENT VARIABLES)

* Ortam değişkenleri, istenilen bilgiye kısa yoldan erişebilmek için oluşturulan tanımlardır. 

* $ işaretiyle başlar ve büyük harflerden oluşurlar. Örn; $LOGNAME 

* Ortam değişkenleri printenv veya env komutuyla görülebilir. 

* printenv <DEĞİŞKENADI> veya echo $<DEĞİŞKENADI> şeklinde kullanılabilirler. Örn; printenv SHELL veya echo $SHELL 

* Yeni değişken tanımı oluşturmak için DEGİŞKENADI=değer komutu kullanılır. Silmek için de unset DEĞİŞKENADI komutu kullanılır. 

* Değişken isimleri sayısal bir değer ile başlayamaz.

| DEĞİŞKEN | iŞLEV |
| -------------  |:------------- |
|$USER|Oturumunda olunan kullanıcıyı ifade eder.|
|$HOME|Oturumdaki kullanıcının ev dizinini ifade eder.|
|$SHELL|Oturumdaki kullanıcının shell’ini ifade eder.|
|$DESKTOP_SESSION , $GDMSESSION|Oturumdaki kullanıcının masaüstü ortamını ifade eder.|
|$PWD|Bulunulan path’i ifade eder.|
|$PATH|Yazılacak komutların aranacağı path’leri ifade eder.|
|$LANG|Sistemde kullanılan dili ifade eder.|

### BASH BETİKLERİ (BASH SCRIPTS)

* Bash betikleri (scriptleri), çalıştırıldığında bash’e iş yükler. Bash’in, dosyadan okuyarak otomatik işler yürütmesi içindir.

* Bash script’lerinin ilk satırı #!/bin/bash olarak başlamak zorundadır. Böylelikle, alt satırdaki kodların, bash shell’i tarafından yorumlanacağı belirtilir. 

* Bash script’lerinin dosya uzantısı .sh’tır fakat her zaman bulunmak zorunda değildir. Terminalde ./<dosyaadı> şeklinde de çalıştırılabilir. Çalıştırma (execute) yetkisine sahip olmalıdır. 

* Bash script’leri varsayılanda /bin dizini içindedir. Buradaki scriptler, path belirtmeden çalışıtırlabilirdir. Terminalde sadece script ismini belirtmek yeterlidir.

## BÖLÜM 6: SUNUCU YÖNETİMİ

### SUNUCU YÖNETİMİ (SERVER MANAGEMENT)

#### Sunucu Yönetimi Hakkında

* Sunucu işletim sistemi kurulumundaki hazır içeriklerin (rol, tool vs.) seçilmemesi, minimal tercihlerle ilerlenmesi önerilir. 

* Linux’ta sunucu rolü kurulumları repo’lardan veya uygulamanın firmasına ait kaynaklardan yapılır. 

* Roller, distro’lardan bağımsız olarak aynı tür editleme ve kullanıma sahiptir. Sadece kurulum sırasında minör farklılıklar vardır. Örn; path gibi. Mantığının kavranması, tüm distroların uzmanca kullanımını sağlar. 

* Sunucu rolü yapılandırmaları genellikle <isim>.conf dosylarının yoğun şekilde editlenmesiyle veya doldurulmasıyla yapılır. (Conf dosyaları çoğunlukla /etc dizini altında bulunurlar.) 

* Linux C programlama diliyle yazılmıştır. Bu sebeple konfigürasyon dosyalarındaki syntax’lar genellikle C diline aittir. 

* Sunucu işletim sistemi, grafik arayüzsüz (GUI’siz) geldiyse, terminal kullanımından farksız olarak yönetilmeye devam edilebilir. İşletim sistemine GUI de kazandırılabilir. 

* Rollerin hazır olarak kurulu geldiği sunucu işletim sistemleri de vardır. Fakat bu, gelişim sürecindeki bir sistem mühendisi için önerilmez. Yetenekleri körletici ve gelişimi önleyicidir.

### DNS SUNUCUSU (DNS SERVER)
* DNS Server’ın olmadığı LAN’lerde, DNS sorguları cihazları ve hattı -dış DNS sorguları- yorar.

* DNS Server, DNS sorgularına daha kısa sürede cevap vererek iletişim performansını artırır. 

* DNS Server, cache’leme (önbellekleme) yaparak sorguların daha seyrek aralıklarla yapılmasını sağlar. 

* DNS Server, yapılan DNS sorgularının kaydedilmesini sağlayarak takibi kolaylaştırır. 

* DNS Server, erişim yapılması istenmeyen hedeflere erişimi engelleyebilir.

* Çözümleme işlemleri için IP ve isim (hostname) bilgileri içeren kayıtlara Resource Records (RR) adı verilir. 

* RR’lar zone dosyaları içinde bulunurlar. 

* İsimden IP çözümlemesi (Hostname >>> IP) yapılmasını sağlayan zone, Forward Lookup Zone (FLP)’dur. 

* IP’den isim çözümlemesi (IP >>> Hostname) yapılmasını sağlayan zone ise, Reverse Lookup Zone (RLP)’dur. 

* Linux’ta Primary olan öncü sunucu için ’Master’; Secondary olan ikincil sunucu için ’Slave’ ifadeleri yaygındır.

### DOMAİN CONTROLLER (DC) SUNUCUSU (DC SERVER)

* Linux’ta DC (Domain Controller) rolünü en iyi üstlenen uygulamalardan biri Samba’dır. 

* Samba, Windows’lar için PDC (Primary Domain Controller) olabilir ve GC (Global Catalog) tutabilir. 

* Samba, Kerberos ticket’larına cevap verebilir, domain’e join (katılım) işlemlerini yürütebilir. 

* Samba, domain’e katılan (join olan) istemciler için DNS kaydı tutar ve sorgulara cevap verebilir. 

* Samba, bilmediği DNS sorgularını diğer DNS sunuculara da yönlendirebilir. 

* Samba, Unix ve Windows istemciler için File Server (Dosya Sunucu) rolü de üstlenebilir.

#### Samba Kullanıcı ve Grup Komutları

| KOMUT | iŞLEV |
| -------------  |:------------- |
|samba-tool user list |Kullanıcıları listeler. |
|samba-tool group list |Grupları listeler. |
|samba-tool group listmembers ’’<grup_adı>’’|Grup üyelerini listeler.|
|samba-tool user create <kullanıcı adı>|Kullanıcı oluşturur. |
|samba-tool user delete <kullanıcı adı>|Kullanıcı siler.|
|samba-tool user setpassword <kullanıcı adı>|Kullanıcının şifresini belirler.|
|samba-tool user setexpiry <kullanıcı adı> --days=<sayı>|Kullanıcının şifre sona erme süresini belirler.|
|samba-tool user disable <kullanıcı adı>|Kullanıcıyı devre dışı bırakır. |
|samba-tool user enable <kullanıcı adı>|Kulllanıcıyı etkinleştirir.|
|samba-tool group add ’’ <grup_adı>’’ |Grup oluşturur. |
|samba-tool group delete ’’ <grup_adı>’’|Grup siler.|
|samba-tool group addmembers <grup> <kullanıcı>|Gruba kullanıcı ekler. |
|samba-tool group removemembers <grup> <kullanıcı>|Gruptan kullanıcı çıkarır.|

* Not: Bunları, RSAT ile grafik arayüzden de yapabileceğinizi unutmayın.

### DOSYA SUNUCUSU (FILE SERVER (FS))

#### Samba Dosya Sunucusu

* Samba, Unix ve Windows istemciler için File Server (Dosya Sunucu) rolü de üstlenebilir. 

* Yetkili ve yetkisiz erişimler için dosya paylaşımı sağlayabilir. 

* Dosya paylaşımları için temel ayar dosyası /etc/samba/smb.conf’tur.

#### Samba Dosya Sunucusu Komutları

| KOMUT | iŞLEV |
| -------------  |:------------- |
|smbpasswd -a <kullanıcı_adı>|Samba için kullanıcı oluşturur.|
|smbpasswd -e <kullanıcı_adı>|Kullanıcıyı etkinleştirir.|
|smbpasswd -x <kullanıcı_adı>|Kullanıcıyı siler.|
|smbclient //<IP>/<path> -U |Linux ortamlarından paylaşıma erişim sağlar. |
|`\\<IP>\<path>`|Windows ortamlarından paylaşıma erişim sağlar.|
|systemctl restart samba|Değişikliklerin geçerli olabilmesi için Samba servisini yeniden başlatır.|
|watch smbstatus|Açılan bağlantıların anlık olarak gözlenmesini sağlar.|

### WEB SUNUCUSU (WEB SERVER)

* Linux’ta ve dünyada en yaygın kullanılan web sunucusu, Apache’dir. 

* Temel konfigurasyon dosyası Debian-Based işletim sistemlerinde /etc/apache2/apache2.conf ’tur. (RedHat-Based’ta /etc/httpd/httpd.conf’ tur.) 

* Apache’de, birden fazla site yayınlama özelliği, Virtual Host olarak geçer. (IIS’teki Binding) 

* Apache’de varsayılan olarak dinlenen port, 80’dir. /etc/apache2/ports.conf dosyasından bu değiştirilebilir veya çoklanabilir. 

* Apache’de, erişilebilecek dizinlerin denetimini ve yayınlanan sayfaların davranışını .htaccess dosyası belirler. 

* Yüklenen modüller ile, uyumluluk veya yetenekleri genişletilebilir. (Apache modüllerinin listesine şuradan ulaşabilirsiniz. https://en.wikipedia.org/wiki/List_of_Apache_modules ) 

* Apache servisinin adı Debian-Based işletim sistemlerinde apache2’dir. (RedHat-Based’ta httpd’dir.) 

* Giriş kayıtları (Access Log) /var/log/apache2/access.log dosyasında tutulur.

## BÖLÜM 7: İLERİ SEVİYE SİSTEM YÖNETİMİ

### REPO YÖNETİMİ (REPOSITORY MANAGEMENT)

* Repolar, distroların paket dağıtım sunucularıdır. 

* Her distronun kendine özgü resmi repoları vardır ve her distro için birden fazladırlar. 

* Distrolara manuel olarak repo sunucuları eklenebilir veya mavcut olanlar çıkarılabilir. 

* Adı hatırlanmayan ya da türevleri aranan paketler repolarda komutlar yardımıyla aranabilir. 

* Repolar aracılığıyla distroya yüklenmiş olan paketler de listelenebilir. 

* Bir paketin hangi repoda bulunabileceği de aratılabilir. Bunun için web siteleri mevcuttur. 

* Resmi repolarda bulunmayan paketler için PPA (Personal Package Archive) repoları eklenip kullanılabilir. - PPA repoları eklenirken anahtar sunucularının (Key Server) eklenmesi de istenebliir.
    - !! Repolarda bulunmayan paket ihtiyaçlarınız için Software Center, Snap veya source code da kullanabileceğinizi unutmayın.

#### Repo Yönetim Komutları

| KOMUT | iŞLEV |
| -------------  |:------------- |
|cat /etc/apt/sources.list |Debian-Based’ta repo tanımlarının bulunduğu dosyayı gösterir. |
|ls -l /etc/yum.repos.d/* |RedHat-Based’ta repo tanımlarının bulunduğu dizini gösterir. |
|yum -v repolist all |RedHat-Based’ta etkin ve devre dışı tüm repoların listesini verir. |
|yum -v repolist enabled / disabled|Etkin veya devre dışı repoları listeler.|
|apt list --installed |Debian-Based’ta, yüklenmiş olan paketleri listeler. |
|yum list installed|RedHat-Based’ta, yüklenmiş olan paketleri lsteler. (Grep kullanılabilir.)|
|apt list -a <paketadı>|Debian-Based’ta paket arar. (Joker kullanılabilir.) |
|yum search all <paketadı>|RedHat-Based’ta paket arar. |
|https://packages.ubuntu.com/ |Debian-Based’ta paketleri aramak için web sitesi. |
|https://pkgs.org/|Tüm distrolar ve tüm repolarda paket arama yapılabilen web sitesi.|
|add-apt-repository <repo_adı>|Yeni repo ekler. |
|add-apt-repository ‘’<deb URL’i>’’ |Yeni repo ekler. (Sources.list dosyasına manuel de eklenebilir.) |
|add-apt-repository ppa:<ppa_adı> |PPA (Personal Package Archive) repoları ekler. |
|https://www.ubuntuupdates.org/ppas |PPA repolarının listeni veren web sitesi. |
|yum-config-manager --add-repo= `<URL>`|Yeni repo ekler.|
|rm -rf /etc/apt/sources.list.d/<repo_adı>|Repoyu kaldırır. |
|add-apt-repository --remove ppa:<ppa_adı>|PPA reposunu kaldırır. |
|rm -rf /etc/yum.repos.d/<repo_adı>|Repoyu kaldırır.|

### SSH (SECURE SHELL)

* SSH, Telnet’in güvenli bir alternatifi olarak oluşturulmuştur. 

* SSH, uzaktan shell (console) kullanımı ve yönetimi için oluşturulmuş bir uzak yönetim protokolüdür. 

* SSH ile yapılan bağlantılar şifreli (encrypted) olarak sağlanır. İletişim okunamazdır. 

* SSH, TCP 22. porttan çalışır. 

* SSH ile dosya transferleri de yapılabilir. 

* Unix/Linux harici işletim sistemlerinden bağlantı ve kullanımı için Putty, Kitty, WinSCP, OpenSSH gibi 3. parti istemciler (uygulamalar) kullanılabilir. 

* Servisinin adı Debian-Based’ta ssh; Redhat-Based’ta sshd’dir. 

* Konfigürasyon dosyası /etc/ssh/ssh_config’tir. 

* Tanınan uzak sunucu ve onun key’ini barındıran dosya ~/.ssh/authorized_keys’tir.

| KOMUT | iŞLEV |
| -------------  |:------------- |
|apt install openssh-server openssh-client |Debian-Based’ta kurulum komutudur. |
|yum install openssh-server openssh-clients|Redhat-Based’ta kurulum komutudur.|
|systemctl start / stop ssh |SSH servisinin durdurma veya başlatma komutudur. |
|systemctl enable ssh|SSH servisini başlangıçta çalıştırma komutudur.|
|ssh-keygen -t rsa|Güvenli SSH bağlantısı için key üretir.|
|ssh-keygen -p|Oluşturulan key’i tekrar üreterek değiştirir.|
|ssh-keygen -p|Oluşturulan key’i tekrar üreterek değiştirir.|
|ssh-copy-id <kullanıcıadı>@`<IP>`|Oluşturulan key’i uzak makineye tanıtır.|
|ssh <kullanıcıadı>@`<IP>`|SSH’ı aktif olan bir makineye/cihaza bağlanma komutudur.|
|scp <path/dosya> <kullanıcı_adı>@`<IP>:<path>`|SSH ile uzak makineye dosya gönderme (upload) komutudur. |
|scp <kullanıcı_adı>@`<IP>`:<path/dosya> <path/dosya>|SSH ile uzak makineden dosya alma (download) komutudur.|
|pscp.exe <path/dosya> <kullanıcı_adı>@`<IP>:<path>`|Putty ile uzak makineye dosya gönderme (upload) komutudur.|
|pscp.exe <kullanıcı_adı>@`<IP>`:<path/dosya> <path/dosya>|Putty ile uzak makineden dosya alma (download) komutudur.|

### GÜVENLİK DUVARI (FIREWALL)

| KOMUT | iŞLEV |
| -------------  |:------------- |
|service ufw stop / start |UFW (Uncomplicated Firewall) güvenlik duvarı servisini kapatır / açar.|
|systemctl enable / disable ufw|Servisin başlangıçta çalışmasını sağlar.|
|ufw enable / disable|UFW’yi açar / kapatır.|
|ufw status verbose|UFW servisi ve kuralları hakkında detaylı bilgi verir.|
|ufw status numbered|UFW kurallarını numaralı olarak listeler.|
|ufw app list|Sunucuda kurulu ve kurallar uygulayabileceği servisleri listeler.|
|ufw allow / deny from `<IP>` |Belirli bir IP’den gelen paketlere izin verir / engeller.|
|ufw allow / deny to `<IP>`|Belirli bir IP’ye giden paketlere izin verir / engeller.|
|ufw delete <rule_no>|Belirtilen numaralı kuralı siler.|
|ufw allow / deny `<servis>` |Belirtilen servis için gelen paketlere izin verir/engeller. |
|ufw allow / deny `<port>`|Belirtilen port numarası için gelen paketlere izin verir/engeller. |
|ufw allow / deny `<uygulama>`|Belirtilen uygulama için gelen paketlere izin verir/engeller.|
|ufw allow / deny out <port_no>|Belirtilen port numarası için giden paketlere izin verir/engeller.|
|ufw allow / deny in on `<ethernet>` from `<IP>`|Belirtilen ethernet adı üzerinden, belirli bir IP’ye izin verir/engeller.|
|ufw reset|UFW’nin varsayılan ayarlara dönmesini sağlar.|