# Zombie-Reloaded
I use this version from SRCDSLab on my server. Visit their community - https://github.com/srcdslab

// ---------------------------------------------------------------- ----------------------------
// Журнал (ядро)
// ---------------------------------------------------------------- ----------------------------

// Включаем логирование событий в плагине. Фатальные ошибки всегда регистрируются.
// По умолчанию: "1"
zr_log "1"

// Битовое поле, определяющее, какие типы событий регистрировать. Подробную информацию см. в разделе регистрации (3.3) руководства.
// По умолчанию: "2"
zr_log_flags "2"

// Включаем фильтрацию модулей. Будут регистрироваться только события из перечисленных модулей.
// По умолчанию: "0"
zr_log_module_filter "0"

// Не регистрируйте события, вызванные консольными командами, которые выполняются самой консолью, например команды в конфигурациях. Включите эту команду, чтобы избежать спама в журналах с такими событиями, как ограничения на оружие.
// По умолчанию: "1"
zr_log_ignore_console "1"

// Всегда регистрируйте сообщения об ошибках независимо от того, какие флаги журналирования или фильтры модулей включены.
// По умолчанию: "1"
zr_log_error_override "1"

// Распечатываем события журнала в чате администратора в дополнение к файлу журнала.
// По умолчанию: "0"
zr_log_print_admins "0"

// Распечатываем события журнала в публичный чат в дополнение к файлу журнала.
// По умолчанию: "0"
zr_log_print_chat "0"


// ---------------------------------------------------------------- ----------------------------
// Конфигурация (ядро)
// ---------------------------------------------------------------- ----------------------------

// Путь относительно корневого каталога sourcemod к файлу конфигурации модели.
// По умолчанию: "configs/zr/models.txt"
zr_config_path_models "configs/zr/models.txt"

// Путь относительно корневого каталога исходного мода к файлу загрузки.
// По умолчанию: "configs/zr/downloads.txt"
zr_config_path_downloads "configs/zr/downloads.txt"

// Путь относительно корневого каталога sourcemod к файлу конфигурации классов игроков.
// По умолчанию: "configs/zr/playerclasses.txt"
zr_config_path_playerclasses "configs/zr/playerclasses.txt"

// Путь относительно корневого каталога исходного мода к файлу конфигурации оружия.
// По умолчанию: "configs/zr/weapons.txt"
zr_config_path_weapons "configs/zr/weapons.txt"

// Путь относительно корневого каталога sourcemod к файлу конфигурации хит-групп.
// По умолчанию: "configs/zr/hitgroups.txt"
zr_config_path_hitgroups "configs/zr/hitgroups.txt"


// ---------------------------------------------------------------- ----------------------------
// Настройки разрешений
// ---------------------------------------------------------------- ----------------------------

// Используйте групповую аутентификацию вместо флагов для доступа к функциям администратора. Для некоторых функций по-прежнему требуется общий флаг администратора.
// -
// По умолчанию: "0"
zr_permissions_use_groups "0"

// ---------------------------------------------------------------- ----------------------------
// Классы (ядро)
// ---------------------------------------------------------------- ----------------------------

// Общий

// Повторно отображать меню выбора класса при каждом появлении.
// По умолчанию: "0"
zr_classes_menu_spawn "0"

// Отображение меню выбора класса при первом появлении игрока.
// По умолчанию: "0"
zr_classes_menu_join "0"

// Автоматически закрывать меню выбора класса после выбора класса.
// По умолчанию: "1"
zr_classes_menu_autoclose "1"

// Игроку присваивается случайный класс при каждом появлении. [Переопределить: zr_classes_default_*]
// По умолчанию: "0"
zr_classes_random "0"

// Ограничение времени на смену класса человека с мгновенным изменением после появления. Время указано в секундах. Используйте 0 или отрицательное значение для отключения.
// По умолчанию: "20"
zr_classes_change_timelimit "20"

// Сохраняем выбор классов игроков в файлах cookie сервера и восстанавливаем при подключении. [Переопределить: zr_classes_default_*]
// По умолчанию: "1"
zr_classes_save "1"

// (Не реализовано!) Класс только для администраторов, назначаемый администраторам при подключении, если таковой имеется. ["default" = Класс человека по умолчанию | "random" = Случайный класс только для администратора]
// По умолчанию: "случайный"
zr_classes_default_admin «по умолчанию»

// (Неполный) Класс режима администратора, назначаемый администраторам при подключении. Не путайте это с классами только для администратора. ["random" = Случайный класс администратора | "" = Конфигурация класса по умолчанию]
// По умолчанию: "случайный"
zr_classes_default_admin_mode «случайный»

// Класс человека, присваиваемый игрокам при подключении. ["random" = Случайный класс людей | "" = Конфигурация класса по умолчанию]
// По умолчанию: "случайный"
zr_classes_default_human "случайный"

// Класс зомби, присваиваемый игрокам при подключении. ["random" = Случайный класс зомби | "" = Конфигурация класса по умолчанию]
// По умолчанию: "случайный"
zr_classes_default_zombie "случайный"

// Класс зомби, присвоенный матерям-зомби. ["motherzombies" = Случайный класс матери-зомби | "random" = Случайный обычный класс зомби | «отключено» = Не менять класс матери-зомби]
// По умолчанию: "матери-зомби"
zr_classes_default_mother_zombie "мать-зомби"

// Разрешить игрокам выбирать классы зомби.
// По умолчанию: "1"
zr_classes_zombie_select "1"

// Разрешить игрокам выбирать человеческие классы.
// По умолчанию: "1"
zr_classes_human_select "1"

// Разрешить администраторам выбирать классы режима администратора. (Не путать с классами только для администраторов!)
// По умолчанию: "1"
zr_classes_admin_select "1"

// Метод скорости, используемый при применении скорости игрока. Не трогайте это, если не знаете, что делаете! ["lmv" = Значение запаздывающего движения | "prop" = свойство скорости игрока]
// По умолчанию: "lmv"
zr_classes_speed_method "lmv"

// КС:ГО
// ---------------------------------------------------------------- ----------------------------
// Zhurnal (yadro)
// ---------------------------------------------------------------- ----------------------------

// Vklyuchayem logirovaniye sobytiy v plagine. Fatal'nyye oshibki vsegda registriruyutsya.
// Po umolchaniyu: "1"
zr_log "1"

// Bitovoye pole, opredelyayushcheye, kakiye tipy sobytiy registrirovat'. Podrobnuyu informatsiyu sm. v razdele registratsii (3.3) rukovodstva.
// Po umolchaniyu: "2"
zr_log_flags "2"

// Vklyuchayem fil'tratsiyu moduley. Budut registrirovat'sya tol'ko sobytiya iz perechislennykh moduley.
// Po umolchaniyu: "0"
zr_log_module_filter "0"

// Ne registriruyte sobytiya, vyzvannyye konsol'nymi komandami, kotoryye vypolnyayutsya samoy konsol'yu, naprimer komandy v konfiguratsiyakh. Vklyuchite etu komandu, chtoby izbezhat' spama v zhurnalakh s takimi sobytiyami, kak ogranicheniya na oruzhiye.
// Po umolchaniyu: "1"
zr_log_ignore_console "1"

// Vsegda registriruyte soobshcheniya ob oshibkakh nezavisimo ot togo, kakiye flagi zhurnalirovaniya ili fil'try moduley vklyucheny.
// Po umolchaniyu: "1"
zr_log_error_override "1"

// Raspechatyvayem sobytiya zhurnala v chate administratora v dopolneniye k faylu zhurnala.
// Po umolchaniyu: "0"
zr_log_print_admins "0"

// Raspechatyvayem sobytiya zhurnala v publichnyy chat v dopolneniye k faylu zhurnala.
// Po umolchaniyu: "0"
zr_log_print_chat "0"


// ---------------------------------------------------------------- ----------------------------
// Konfiguratsiya (yadro)
// ---------------------------------------------------------------- ----------------------------

// Put' otnositel'no kornevogo kataloga sourcemod k faylu konfiguratsii modeli.
// Po umolchaniyu: "configs/zr/models.txt"
zr_config_path_models "configs/zr/models.txt"

// Put' otnositel'no kornevogo kataloga iskhodnogo moda k faylu zagruzki.
// Po umolchaniyu: "configs/zr/downloads.txt"
zr_config_path_downloads "configs/zr/downloads.txt"

// Put' otnositel'no kornevogo kataloga sourcemod k faylu konfiguratsii klassov igrokov.
// Po umolchaniyu: "configs/zr/playerclasses.txt"
zr_config_path_playerclasses "configs/zr/playerclasses.txt"

// Put' otnositel'no kornevogo kataloga iskhodnogo moda k faylu konfiguratsii oruzhiya.
// Po umolchaniyu: "configs/zr/weapons.txt"
zr_config_path_weapons "configs/zr/weapons.txt"

// Put' otnositel'no kornevogo kataloga sourcemod k faylu konfiguratsii khit-grupp.
// Po umolchaniyu: "configs/zr/hitgroups.txt"
zr_config_path_hitgroups "configs/zr/hitgroups.txt"


// ---------------------------------------------------------------- ----------------------------
// Nastroyki razresheniy
// ---------------------------------------------------------------- ----------------------------

// Ispol'zuyte gruppovuyu autentifikatsiyu vmesto flagov dlya dostupa k funktsiyam administratora. Dlya nekotorykh funktsiy po-prezhnemu trebuyetsya obshchiy flag administratora.
// -
// Po umolchaniyu: "0"
zr_permissions_use_groups "0"

// ---------------------------------------------------------------- ----------------------------
// Klassy (yadro)
// ---------------------------------------------------------------- ----------------------------

// Obshchiy

// Povtorno otobrazhat' menyu vybora klassa pri kazhdom poyavlenii.
// Po umolchaniyu: "0"
zr_classes_menu_spawn "0"

// Otobrazheniye menyu vybora klassa pri pervom poyavlenii igroka.
// Po umolchaniyu: "0"
zr_classes_menu_join "0"

// Avtomaticheski zakryvat' menyu vybora klassa posle vybora klassa.
// Po umolchaniyu: "1"
zr_classes_menu_autoclose "1"

// Igroku prisvaivayetsya sluchaynyy klass pri kazhdom poyavlenii. [Pereopredelit': zr_classes_default_*]
// Po umolchaniyu: "0"
zr_classes_random "0"

// Ogranicheniye vremeni na smenu klassa cheloveka s mgnovennym izmeneniyem posle poyavleniya. Vremya ukazano v sekundakh. Ispol'zuyte 0 ili otritsatel'noye znacheniye dlya otklyucheniya.
// Po umolchaniyu: "20"
zr_classes_change_timelimit "20"

// Sokhranyayem vybor klassov igrokov v faylakh cookie servera i vosstanavlivayem pri podklyuchenii. [Pereopredelit': zr_classes_default_*]
// Po umolchaniyu: "1"
zr_classes_save "1"

// (Ne realizovano!) Klass tol'ko dlya administratorov, naznachayemyy administratoram pri podklyuchenii, yesli takovoy imeyetsya. ["default" = Klass cheloveka po umolchaniyu | "random" = Sluchaynyy klass tol'ko dlya administratora]
// Po umolchaniyu: "sluchaynyy"
zr_classes_default_admin «po umolchaniyu»

// (Nepolnyy) Klass rezhima administratora, naznachayemyy administratoram pri podklyuchenii. Ne putayte eto s klassami tol'ko dlya administratora. ["random" = Sluchaynyy klass administratora | "" = Konfiguratsiya klassa po umolchaniyu]
// Po umolchaniyu: "sluchaynyy"
zr_classes_default_admin_mode «sluchaynyy»

// Klass cheloveka, prisvaivayemyy igrokam pri podklyuchenii. ["random" = Sluchaynyy klass lyudey | "" = Konfiguratsiya klassa po umolchaniyu]
// Po umolchaniyu: "sluchaynyy"
zr_classes_default_human "sluchaynyy"

// Klass zombi, prisvaivayemyy igrokam pri podklyuchenii. ["random" = Sluchaynyy klass zombi | "" = Konfiguratsiya klassa po umolchaniyu]
// Po umolchaniyu: "sluchaynyy"
zr_classes_default_zombie "sluchaynyy"

// Klass zombi, prisvoyennyy materyam-zombi. ["motherzombies" = Sluchaynyy klass materi-zombi | "random" = Sluchaynyy obychnyy klass zombi | «otklyucheno» = Ne menyat' klass materi-zombi]
// Po umolchaniyu: "materi-zombi"
zr_classes_default_mother_zombie "mat'-zombi"

// Razreshit' igrokam vybirat' klassy zombi.
// Po umolchaniyu: "1"
zr_classes_zombie_select "1"

// Razreshit' igrokam vybirat' chelovecheskiye klassy.
// Po umolchaniyu: "1"
zr_classes_human_select "1"

// Razreshit' administratoram vybirat' klassy rezhima administratora. (Ne putat' s klassami tol'ko dlya administratorov!)
// Po umolchaniyu: "1"
zr_classes_admin_select "1"

// Metod skorosti, ispol'zuyemyy pri primenenii skorosti igroka. Ne trogayte eto, yesli ne znayete, chto delayete! ["lmv" = Znacheniye zapazdyvayushchego dvizheniya | "prop" = svoystvo skorosti igroka]
// Po umolchaniyu: "lmv"
zr_classes_speed_method "lmv"

// KS:GO
Ещё
