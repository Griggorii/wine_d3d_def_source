# wine_d3d_def_source
linux wine d3d def source my reversing code 

Возможно этот wine собранный мною в моей 16.04 сборке работает только от root

wine 5.0 wine_4.0.3-1_amd64  https://drive.google.com/open?id=1k_SzvG09sURl4EwmEGQd37GtZ2aNd2UM

wine 5.0 replace wine , fonts-wine , wine1.6-amd64

$ sudo rm -rf ~/.wine

$ winecfg

$ regedit

И вроде есть возможность теперь менять что либо 

$ sudo regedit

$ su

$ regedit

HKEY_LOCAL_MACHINE\Hardware\Description\System\CentralProcessor

HKEY_LOCAL_MACHINE\Software\Wow6432Node\Classes\Protocols\Filter

HKEY_LOCAL_MACHINE\System\CurrentControlSet\Enum\DISPLAY\DEFAULT_MONITOR\0000&0000\Properties\{233A9EF3-AFC4-4ABD-B564-C32F21F1535B}

HKEY_LOCAL_MACHINE\System\CurrentControlSet\Enum\ROOT\WINE\WINEBUS\Device Parameters

HKEY_LOCAL_MACHINE\System\CurrentControlSet\Control\DeviceClasses\{378DE44C-56EF-11D1-BC8C-00A0C91405DD}\##?#HID#VID_0000&PID_0000#0&WINEMOUSE&0&0#{378DE44C-56EF-11D1-BC8C-00A0C91405DD}

HKEY_LOCAL_MACHINE\System\CurrentControlSet\Control\SecurityProviders\Schannel\Protocols\SSL 2.0\Client



Good idea ? Теперь можно внутри и кое где сам linux отредактировать таким способом выдал пока интересные параметры , но возможно кто то найдёт что то более лучшее

Где я нашел кое какую информацию про то что wine может работать от рут https://unixforum.org/viewtopic.php?t=89089

Какие есть ошибки 
000f:err:service:process_send_command receiving command result timed out 
000f:fixme:service:scmdatabase_autostart_services Auto-start service L"winebus"

От рут
wine: configuration in L"/root/.wine" has been updated
Wine cannot find the ncurses library (libncurses.so.5).

Ошибки при запуске программ
wine: Unimplemented function shell32.dll.SHGetFolderPathW called at address



Скоро мы избавимся от прокладок в виде протон и так далее я ранее как предупреждал работал над операционной системой и я начал сравнивать свою старую операционную систему в которо был очень быстрый directx даже через playonlinux и обнаружил что именно этих фаилов нету в более новых версиях всяких различных дистрибутивов как будто они их скрыли и решили сделать что то новое из них хотя я может и ошибаюсь , но как я иногда делаю так это если не понимаю проект то замораживаю его до того как не поиму и не перекомпилирую допустим с подменой инклюдов с более новых на более старые или наоборот и вразброс.

Так же вы заметите после инсталяции возможно меню вашего linux дистрибутива видо изменится и станет более широким так как я использовал свои максимально собранный дистрибутив версии 16.04 , причина торможении в wine может оказаться более высокой версии чем 8.0 pulseaudio версия от xenial 16.04 pulseaudio 8.0 последняя работала с wine и игры не тормозили на некоторых моментах , но не суть не суть , а то в сторону игромании скатимся так что бы проще понять двигатель системы если где то тормозит это не хорошо и это подобно тому как хочешь ли ты что бы в твоей Ладе Спорт стоял двигатель от Мотоцикла или фары светили одна хуже другой тут как бы все параметрики связаны и по этому есть еще одна причина люди не правильно допустим организовали блютус аудио драивера и тому подобное т.е ранее звук был не 3Д и по этому часть каких либо звуков отсутствовала так как канал был моно , ну это мои мысли не более , но то что обдумываю то и пишу , но ведь можно было сделать как то по другому , но уже пока поздно делать в более новых дистрибутивах чем 16.04 хотя минт навярняка уже все заслуги себе приписал и тот же миникс тоже так как ранее видели мой еще три года назад собранный дистрибутив из разных ppa , а глупая убунта почему то не стала продолжать именно мой дистрибутив который можно было просто обтянуть новыми декорациями гтк3 чем терять ускорение в directx , но подозреваю что у них какие то проблемы либо они продали некие эти части фаилов от ксениал в коммерчискую сторону реализации тем самым дав понять что в принципе вероятно что с деньгами лучше чем без.
