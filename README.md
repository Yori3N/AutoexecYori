
//
//       .---.                                                  
//  ___ /_____\                                                 
// /\.-`( '.' )        Counter-Strike: Global Offensive
/// /    \_-_/_                                                 
//\ `-.-"`'V'//-.      ARQUIVO DE CONFIGURACAO PROFISSIONAL
// `.__,   |// , \                                              
//     |Ll //Ll|\ \    AUTOEXEC.CFG                          
//     |__//   | \_\                                            
//    /---|[]==| / /   - FPS BOOST
//    \__/ |   \/\/    - BINDS DE COMPRA NO TECLADO NUMERICO
//    /_   | Ll_\|     - ALIASES PERSONALIZADOS
//     |`^"""^`|       - TROCA DE MIRA NO BOTAO DO SCROLL DO MOUSE
//     |   |   |       - TROCA DE SENSIBILIDADE DO MOUSE PELO MOUSE
//     |   |   |       - BIND PARA MOSTRAR DANO NO CANTO SUPERIOR ESQUERDO DURANTE UM COMPETITIVO
//     |   |   |       - ALERTAS PARA EQUIPE. EX: GO A! / GO B!
//     |   |   |                                                
//     L___l___J                                                
//      |_ | _|        ESSAS CONFIGURACOES SAO GRATUITAS E PODEM E DEVEM    
//     (___|___)       SER COMPARTILHADAS COM OS OUTROS JOGADORES DE CS:GO
//      ^^^ ^^^                                                 
//
//
//                          .-----------------TTTT_-----_______
//                        /''''''''''(______O] ----------____  \______/]_
//     __...---'"""\_ --''   Q                               ___________@
// |'''                   ._   _______________=---------"""""""
// |                ..--''|   l L |_l   |
// |          ..--''      .  /-___j '   '
// |    ..--''           /  ,       '   '
// |--''                /           `    \
//                      L__'         \    -
//                                    -    '-.
//                                     '.    /
//                                       '-./
// 
// TAGS: csgo, competitivo, competitive, cfg, autoexec, conf, free, best, fps boost, melhor cfg para csgo, best cfg, best autoexec.cfg, pro, profissional
//
// ZeroNinja's CS:GO config para modo competitivo -> geralmente este arquivo deve estar em C:\Program Files (x86)\Steam\SteamApps\common\Counter-Strike Global Offensive\csgo\cfg
// 
// Link para baixar a minha cfg mais atualizada -> https://github.com/pedrohiraoka/csgo/blob/master/autoexec.cfg
//
// ¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
// INSTALL/INSTALACAO:
// ¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
// PASSO 1
// Put the File "autoexec.cfg" into the following folder:
// Copie o arquivo "autoexec.cfg" para esta pasta:
// ...\Steam\steamapps\common\Counter-Strike Global Offensive\csgo\cfg
//
// PASSO 2
// Va no menu do jogo > Steam > Biblioteca > Clique direito no jogo Counter-Strike: Global Offensive > Propriedades > Definir Opcoes de Inicializacao > Cole as Opcoes a seguir
// Copie as Opcoes de Inicializacao - Launch Options Steam e troque o 144 pela frequencia do seu monitor: 
// -novid -high -threads 4 -freq 144 -refresh 144 -tickrate 128 -maxplayers_override 50 -nojoy -nod3d9ex1 +exec autoexec.cfg
//
// PASSO 3
// Troque as informacoes nas CONFIGURACOES INICIAIS (linha 69), nas primeiras linhas da CFG. Voce pode descomentar uma opcao que seja de acordo com seu hardware.
// 
// FIM DA INSTALACAO.
// ¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
//
// Last Edit 18.12.2016
//
// ####################################################################
// ## COPIE DA LINHA 70 ATE A ULTIMA E SALVE NO ARQUIVO autoexec.cfg ##
// ####################################################################
// \/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/
// CONFIGURACOES INICIAIS
alias "cfg_nickname" "name CHANGEYOURNICK" // Setar Nickname //
alias "cfg_servidordedicado" "connect CHANGEIP:PORT" // Setar Servidor Dedicado // Atalho no console: meuserver
alias "rconpassword" "rcon_password CHANGERCONPASSWORD" // Setar senha rcon do servidor dedicado
//mat_setvideomode "1360 768 2" // SE ESTA FOR SUA CONF APAGUE OS PRIMEIROS "//"
//mat_setvideomode "1920 1080 1" // SE ESTA FOR SUA CONF APAGUE OS PRIMEIROS "//"
mat_setvideomode "1024 768 1" // SE ESTA FOR SUA CONF APAGUE OS PRIMEIROS "//"
password ""
//cl_clanid "6378373" // ID DO SEU CLAN
//cfg_nickname // Setando o Nickname
//__________         __                 
//\______   \_____ _/  |_  ____   ______
// |       _/\__  \\   __\/ __ \ /  ___/
// |    |   \ / __ \|  | \  ___/ \___ \ 
// |____|_  /(____  /__|  \___  >____  >
//        \/      \/          \/     \/ 
// Rates
rate "307200"
cl_cmdrate "128"
cl_updaterate "128"
cl_interp "0.0"
cl_interp_ratio "1"
cl_interpolate "1"
cl_lagcompensation "1"
net_client_steamdatagram_enable_override "1" // SDR beta
 
// Mouse
sensitivity "2.2" // MUDE PARA SUA SENSIBILIDADE E CONFIGURE O MOUSE PARA 400 DPI
zoom_sensitivity_ratio_mouse "1.0"
m_rawinput "1"
//m_rawinput "0" // Raw esta desativado por que utilizamos o MouseFix igual aos profissionais
m_pitch "0.022"
m_customaccel "0"
m_mouseaccel1 "0"
m_mouseaccel2 "0"
m_mousespeed "0"
/////////////////////////////////////////////////////////////////////////////////////////////////////
// Mouse - Alternando Sensibilidade via Bind
alias Toggler "HighSpeed"
alias HighSpeed "Sensitivity 2.5; alias Toggler LowSpeed"
alias LowSpeed "Sensitivity 2.2; alias Toggler HighSpeed"
bind "mouse4" "Toggler"
HighSpeed
//Change the 'sensitivity 3' to the faster of the two sensitivities you want,
//and then sensitivity 1 to about a third of that value. 
//"mouse4" can be replaced by any key or mouse button you want.
/////////////////////////////////////////////////////////////////////////////////////////////////////
//Mouse - Press/Release quick Sensitivity Bind
//Sensitivity 1
alias +SensChange "Sensitivity 2.6"
alias -SensChange "Sensitivity 2.2"
bind "mouse5" "+SensChange"
//To use this you keep your finger on mouse4 constantly, and release it when
//you need to make a more precise shot. (do not set "Sensitivity 3" higher
//than you can handle comfortably)
//Alternatively don't press mouse4 until someone sneaks up behind you and
//then press it to whip around quickly and return fire. (do not set "sensitivity 1" 
//lower than you can handle comfortably)
//"mouse4" can be replaced with any key or mouse button you wish.
/////////////////////////////////////////////////////////////////////////////////////////////////////
//Mouse - Bind Triplo Para Alternar Sensibilidade
alias faster "HighSens"
alias slower "LowSens"
alias HighSens "High; alias faster; alias slower MedSens"
alias MedSens "Med; alias faster HighSens; alias slower LowSens"
alias LowSens "Low; alias faster MedSens; alias slower"
//alias High "sensitivity 1.5"
//alias Med "sensitivity .75"
//alias Low "sensitivity .375"
//bind mouse4 slower
//bind mouse5 faster
alias High "sensitivity 3.0"
alias Med "sensitivity 2.5"
alias Low "sensitivity 2.0"
bind F9 slower
bind F10 faster
MedSens
//Altere os valores de sensibilidade para o seu Maximo e Minimo de sensibilidades.
//Pressing one button increases speed, pressing the other button decreases speed.
//Bind them to any key or mouse buttons you want.
//This can make an MX510 emulate the DPI changing buttons on a Logitech G5 or MX518
//since with the driver the top two buttons could be set to keystrokes bound to slower and faster.
//http://www.overclock.net/t/173255/cs-s-mouse-optimization-guide
/////////////////////////////////////////////////////////////////////////////////////////////////////
// Video
//mat_setvideomode "1360 768 2" // ESCOLHA SUA CONFIGURACAO DE VIDEO
//mat_setvideomode "1920 1080 1" // ESCOLHA SUA CONFIGURACAO DE VIDEO
//mat_setvideomode "1024 768 1" // ESCOLHA SUA CONFIGURACAO DE VIDEO
mat_monitorgamma "1.6" // 1.6=Brightest  2.6=Darkest
mat_queue_mode "-1" // auto detect multi-core rendering
//mat_vsync "0"
fps_max "999"
fps_max_menu "145"
r_dynamic "0"
r_drawtracers_firstperson "0"
mat_savechanges // Escreve as configuracoes de video no registro / Write video settings to registry
// Audio
volume "0.55"
voice_enable "1"
voice_scale "1" // receive volume
windows_speaker_config "1" // headphone audio output
snd_musicvolume "0"
snd_mixahead "0.05" // sound delay
snd_headphone_pan_exponent "2"
snd_headphone_pan_radial_weight "2"
snd_legacy_surround "0" // emulated surround sound
snd_mute_losefocus  "1" // mute game when alt-tabbed
snd_front_headphone_position "45"
snd_rear_headphone_position "135"
lobby_voice_chat_enabled "0" // voice chat in lobby
snd_pitchquality "1"
dsp_enhance_stereo "0"
cl_mute_all_but_friends_and_party "0"
snd_async_flush
// HUD
safezonex 1.0;
safezoney 1.0;
hud_scaling "0.8" // CS:S sized HUD
hud_showtargetid "1"
cl_hud_background_alpha "0.7"
cl_hud_bomb_under_radar "1"
cl_hud_color "5" // Aqua 1 Green 2 Yellow 3 Orange 4 Red 5 Pink 6 Purple 7 Blue 8 Light blue 9 White 10
cl_hud_healthammo_style "1"
cl_hud_playercount_pos "1"
cl_hud_playercount_showcount "1"
cl_hud_radar_scale "1.2" // default 2
cl_draw_only_deathnotices "0"
cl_righthand "0" // Para Olho Dominante direito http://steamcommunity.com/sharedfiles/filedetails/?id=326618495
cl_showloadout "1"
cl_showpos "1" // mostra dados no canto superior esquerdo da tela / fps, velocidade do boneco etc
cl_showfps "0"
net_graph "1"
net_graphheight "0"
net_graphproportionalfont "0" // small netgraph font
net_graphpos "1"
// Radar
cl_radar_always_centered "0"
cl_radar_rotate "1"
cl_radar_scale "0.35"
cl_radar_icon_scale_min "0.7"
cl_radar_square_with_scoreboard "0"
// Reposition gun model to mimic CS:S
viewmodel_presetpos "3" // classic
viewmodel_fov "68"
viewmodel_offset_x "2"
viewmodel_offset_y "2"
viewmodel_offset_z "-2"
// Reduce gun shifting when crouching
cl_viewmodel_shift_left_amt "0.5"
cl_viewmodel_shift_right_amt "0.5"
// Reduce gun and scope shifting/bobbing when moving
cl_bobcycle "2" // 0.98 is enforced by ESEA/ESL
cl_bob_lower_amt "0"
cl_bobamt_lat "0"
cl_bobamt_vert "0"
//   _____  .__               
//  /     \ |__|___________   
// /  \ /  \|  \_  __ \__  \  
///    Y    \  ||  | \// __ \_
//\____|__  /__||__|  (____  /
//        \/               \/ 
// Crosshair/Mira
// # INICIO DA ATUAL MIRA DO ZERONINJA
cl_crosshairalpha "255"
cl_crosshaircolor "5"
cl_crosshaircolor_b "0"
cl_crosshaircolor_r "255"
cl_crosshaircolor_g "0"
cl_crosshairdot "1"
cl_crosshairgap "-2"
cl_crosshairsize "1"
cl_crosshairstyle "4"
cl_crosshairusealpha "1"
cl_crosshairthickness "1"
cl_fixedcrosshairgap "-2"
cl_crosshair_outlinethickness "0"
cl_crosshair_drawoutline "0"
// # FIM DA ATUAL MIRA DO ZERONINJA
// MIRA-DEFAULT-CFG
//cl_crosshairstyle "4"
//cl_crosshairsize "2"
//cl_crosshairthickness "0.5"
//cl_crosshairgap "-1" // classic
//cl_fixedcrosshairgap "3" // new
//cl_crosshairdot "0"
//cl_crosshairusealpha "1"
//cl_crosshairalpha "999"
//cl_crosshair_drawoutline "1"
//cl_crosshair_outlinethickness "1"
//cl_crosshairgap_useweaponvalue "0"
// White crosshair
//cl_crosshaircolor "5"
//cl_crosshaircolor_r "255"
//cl_crosshaircolor_g "255"
//cl_crosshaircolor_b "255"
// Debug accuracy (sv_cheats)
weapon_debug_spread_show "0" // show possible shot accuracy 
weapon_debug_spread_gap "0.67"
// MUDAR MIRA COM O BOTAO DO SCROLL - MOUSE3
bind "mouse3" "snade"
alias "snade" "nade1"
bind "mouse3" "snade"
alias "snade" "nade1"
alias "nade1" "use cl_crosshairsize 3;cl_crosshairgap 1.5;cl_crosshairsize 3.5; cl_crosshairgap -1;cl_crosshairsize 4;cl_crosshairgap 0; cl_crosshairsize 5;cl_crosshairgap -1; alias snade nade2"
alias "nade2" "cl_crosshairalpha "255";cl_crosshaircolor "5";cl_crosshaircolor_b "255";cl_crosshaircolor_r "255";cl_crosshaircolor_g "0";cl_crosshairdot "1";cl_crosshairgap "0";cl_crosshairsize "5";cl_crosshairstyle "4";cl_crosshairusealpha "1";cl_crosshairthickness "1";cl_fixedcrosshairgap "0";cl_crosshair_outlinethickness "0";cl_crosshair_drawoutline "0";alias snade nade3"
alias "nade3" "cl_crosshairalpha "255";cl_crosshaircolor "4";cl_crosshaircolor_b "250";cl_crosshaircolor_r "50";cl_crosshaircolor_g "250";cl_crosshairdot "0";cl_crosshairgap "0";cl_crosshairsize "2";cl_crosshairstyle "4";cl_crosshairusealpha "1";cl_crosshairthickness "0.5";cl_fixedcrosshairgap "0";cl_crosshair_outlinethickness "0";cl_crosshair_drawoutline "0";alias snade nade4"
alias "nade4" "cl_crosshairalpha "200";cl_crosshaircolor "2";cl_crosshaircolor_b "50";cl_crosshaircolor_r "50";cl_crosshaircolor_g "250";cl_crosshairdot "0";cl_crosshairgap "0";cl_crosshairsize "5";cl_crosshairstyle "4";cl_crosshairusealpha "1";cl_crosshairthickness "1.5";cl_fixedcrosshairgap "0";cl_crosshair_outlinethickness "0";cl_crosshair_drawoutline "0";alias snade nade1"
//http://tools.dathost.net/
// Misc
developer "0"
con_enable "1"
con_filter_enable "2" // print console on screen
con_filter_text "Damage" // highlight damage in console
con_filter_text_out "Player:"
ui_steam_overlay_notification_position "bottomright"
player_nevershow_communityservermessage "1"
mm_dedicated_search_maxping "70" // altere aqui o ping maximo para criacao de partidas
mm_dedicated_force_servers ""
gameinstructor_enable "0"
option_duck_method "0"
option_speed_method "0"
cl_forcepreload "1"
//cl_downloadfilter "mapsonly"
cl_downloadfilter "ALL"
cl_disablehtmlmotd "0"
cl_autohelp "0"
cl_showhelp "0"
cl_disablefreezecam "1"
cl_dm_buyrandomweapons "0"
cl_teammate_colors_show "1"
cl_autowepswitch "0" // auto weapon switch on pickup
cl_use_opens_buy_menu "0" // E openeing buy menu
cl_scoreboard_mouse_enable_binding "showmouse" // enable mouse on the scoreboard
cl_resend "6"
cl_timeout "9999999"
r_dynamic "0"
r_eyegloss "0"
r_eyemove "0"
r_eyeshift_x "0"
r_eyeshift_y "0"
r_eyeshift_z "0"
r_eyesize "0"
muzzleflash_light "0"
sys_antialiasing "0"
sys_aspectratio "-1"
sys_refldetail "0"
closeonbuy "1"
hud_takesshots "0" // scoreboard screenshot at end of match
func_break_max_pieces "0"
cl_detail_avoid_force "0"
cl_detail_avoid_radius "0"
cl_detail_avoid_recover_speed "0"
cl_detail_max_sway "0"
cl_showpluginmessages "1"
mm_server_search_lan_ports "27015,27016,27017,27018,27019,27020"
cl_color "2" // Preferred teammate color // 0 = yellow - 1 = purple - 2 = green - 3 = blue - 4 = orange
//unbindall
unbindalljoystick // Unbind all joystick keys
//Displaydamage - Switch Script - Mostrar DANO/DAMAGE no canto superior esquerdo
bind "ins" "displaydamage" // APERTE A TECLA INSERT / INS PARA ATIVAR E DESATIVAR
alias displaydamage "displaydamage_on"
alias displaydamage_on "con_filter_text Damage; con_filter_text_out Player:; con_filter_enable 2; developer 1; alias displaydamage "displaydamage_off"; echo Displaydamage ligado!"
alias displaydamage_off "con_filter_enable 0; developer 0; alias displaydamage "displaydamage_on"; execme; echo Displaydamage desligado!"
//___.   .__            .___      
//\_ |__ |__| ____    __| _/______
// | __ \|  |/    \  / __ |/  ___/
// | \_\ \  |   |  \/ /_/ |\___ \ 
// |___  /__|___|  /\____ /____  >
//     \/        \/      \/    \/ 
// Binds
unbind y
unbind u
//unbind k
unbind alt
unbind ;
bind enter "messagemode"
bind home "messagemode2"
bind v "+voicerecord"
bind "TAB" "+ng"
bind space "+jump"
bind w "+forward"
bind a "+moveleft"
bind s "+back"
bind d "+moveright"
bind MWHEELDOWN "invnext"
bind MWHEELUP "invprev"
bind end "spectate"
bind mouse1 "+attack"
bind mouse2 "+attack2"
//bind mouse3 "bhopon" // toggle scroll wheel bhop
//bind mouse4 "use weapon_smokegrenade"
//bind mouse5 "use weapon_flashbang"
bind del "exec autoexec"
bind shift "+speed" // default
bind r "+reload"
bind f "+lookatweapon" // default
bind g "drop" // default
bind h "show";alias show show1;alias show1 "+cl_show_team_equipment; alias show show2";alias show2 "-cl_show_team_equipment; alias show show1"
//bind h sm_admin // Admin Menu (SourceMod)
//bind h "bot_place" // places bot for practice
bind n "+jumpthrow" // consistent smoke jump throws
bind - "toggle voice_scale 1 0" // toggle voice volume
bind = "toggle volume 0.55 0.08 0" // toggle game volume
bind , "showmouse"
bind . "say .ready;say !ready" // custom ready for pugs / comando do mix
bind / toggleconsole // Toggle Console on the Key above Tabulator
bind i ignorerad // Toggle ignoring of radio Messages ("Fire In The Hole" and similar)
//bind l "serverconfig" // carregando as confs do servidor dedicado no arquivo autoexec.cfg
//bind "" "ai_clear_bad_links; clear_anim_cache; clear_debug_overlays; cl_soundemitter_reload; cl_soundemitter_flush; cl_soundscape_flush (cheat-protected); cl_clearhinthistory; fs_clear_open_duplicate_times; fs_fios_flush_cache; r_cleardecals; scene_flush; snd_async_flush; snd_sos_flush_operators; r_flushlod; snd_soundmixer_flush; soundscape_flush (cheat-protected); ui_reloadscheme; hud_reloadscheme; record x; stop"
bind l "limpeza"
// Binds Testes
//BIND PARA MOSTRAR DANO NO FINAL DA RODADA
alias displaydamage "displaydamage_on"
alias displaydamage_on "con_filter_text Damage Given To; con_filter_text_out Player:; con_filter_enable 2; developer 1; playvol buttons\blip1 0.5; alias displaydamage "displaydamage_off""
alias displaydamage_off "con_filter_enable 0; developer 0; playvol buttons\blip2 0.5; alias displaydamage "displaydamage_on""
bind "p" "displaydamage"
 
//BIND DE JOGAR SMOKES
alias "+jumpthrow" "+jump;-attack"
alias "-jumpthrow" "-jump"
bind "mouse8" "+jumpthrow"
 
//BIND PARA DESCOBRIR O MAPA
developer 1
con_filter_enable 2
con_filter_text_out "game:mapgroupname"
con_filter_text "game:map"
con_filter_text "game:map"
// Binds Fs
//bind "F1" "say ;noclip;say .noclip;sv_cheats 1;impulse 101;sv_showimpacts 1;sv_showimpacts_penetration 1;sv_infinite_ammo 1;sv_grenade_trajectory 1;sv_grenade_trajectory_thickness 0.5;mp_freezetime 0;mp_roundtime_defuse 60;mp_buytime 60;mp_buy_anywhere 1;bot_stop 1;mp_warmup_end;" // noclip and sv_cheats practice
//bind "F2" "buy flashbang; buy hegrenade; buy smokegrenade;"
//bind "F3" "buy vesthelm; buy vest; buy defuser;"
//bind "F4" "buy defuser; buy vest; buy vesthelm; buy flashbang; buy smokegrenade; buy hegrenade;"
// Avisos Personalizados
bind pgup "say_team > GO A! > A <" // TECLA PAGE UP
bind pgdn "say_team > GO B! > B <" // TECLA PAGE DOWN
//bind "" "say BOM JOGO GALERA! VAMOS TENTAR JOGAR COMO ADULTOS! SEM BRIGAS! SEM OFENSAS! <3 #GOGOGO :)"
alias "bj" "say BOM JOGO GALERA! VAMOS TENTAR JOGAR COMO ADULTOS! SEM BRIGAS! SEM OFENSAS! <3 #GOGOGO :)"
//http://csgobuynds.com/buy-binds-generator.html
// Righthand ON / Ativando Mao Direita / Trocando a Mao
alias togglestuffon "cl_righthand 1;cl_radar_scale 1;bind k togglestuffoff"
alias togglestuffoff "cl_righthand 0;cl_radar_scale 0.4;bind k togglestuffon"
bind k togglestuffon;
// Aliases default cfg
alias "dc" "disconnect"
alias "showmouse" // for mouse on scoreboard
alias "+ng" "+showscores; net_graph 1"
alias "-ng" "-showscores; net_graph 0"
alias "+jumpthrow" "+jump;-attack"
alias "-jumpthrow" "-jump"
alias mmrates "cl_interp 0.031;cl_interp_ratio 2;rate 80000" // testing rates for mm (via tesseract)
// Aliases Personalizados
alias "serverconfig" "rconpassword;rcon exec autoexec.cfg;echo CFG Server carregada.." // execulta as confs contidas no servidor dedicado no arquivo cfg/autoexec.cfg
alias "execme" "limpeza; exec autoexec"
alias "meuserver" "cfg_servidordedicado"
alias "meuserver2" "connect 189.1.171.47:27018"
alias "pauseon" "rconpassword;rcon mp_pause_match"
alias "pauseoff" "rconpassword;rcon mp_unpause_match"
alias "ativarcasual" "rconpassword;rcon exec server;rcon exec gamemode_casual.cfg"
alias "ativarcompetitivo" "rconpassword;rcon exec server;rcon exec gamemode_competitive.cfg"
alias "abrirvotemap" "rconpassword;rcon sm_votemap de_cbble de_inferno de_dust2 de_nuke de_mirage de_cache de_overpass"
alias "serversinfo" "say [TS3] ts3.ZeroNinja.tk:9502 [SERVERMIX] connect mix.ZeroNinja.tk;echo [TS3] ts3.ZeroNinja.tk:9502 [SERVERMIX] connect mix.ZeroNinja.tk"
alias "minhastream" "say [!!!LIVE!!!] twitch.tv/ZeroNinjaTV"
alias "infoz" "status;users"
alias "abrirconsole" "showconsole"
alias "limparmemoria" "clear_anim_cache"
alias "sair" "quit prompt"
alias "limpeza" "ai_clear_bad_links; clear_anim_cache; clear_debug_overlays; cl_soundemitter_reload; cl_soundemitter_flush; cl_soundscape_flush ; cl_clearhinthistory; fs_clear_open_duplicate_times; fs_fios_flush_cache; r_cleardecals; scene_flush; snd_async_flush; snd_sos_flush_operators; r_flushlod; snd_soundmixer_flush; soundscape_flush (cheat-protected); ui_reloadscheme; hud_reloadcheme; record fix; stop"
alias "surf" "bind mouse4 +left;bind mouse5 +right;"
alias "bots" "sv_cheats 1;god;mp_warmup_start;mp_warmup_pausetimer 1;mp_autoteambalance 0;mp_limitteams 0;mp_buy_anywhere 1;mp_randomspawn 1;mp_spawnprotectiontime 0;mp_respawn_immunitytime 0;sv_infinite_ammo 1;bot_difficulty 3;bot_dont_shoot 1;bot_kick;mp_restartgame 
alias "smokesmouse" "bind mouse4 use weapon_smokegrenade;bind mouse5 use weapon_flashbang"
//sound_toggles
alias mute "volume 0; echo ~~~~volume_off~~~~; "
alias unmute "volume 0.2; echo ~~~~volume_on~~~~; "
alias voicemute "voice_enable 0; echo ~~~~voice_off~~~~; say_team voice_enable 0; "
alias voiceunmute "voice_enable 1; echo ~~~~voice_on~~~~; say_team voice_enable 1; "
//bunnyhop
alias bhop "bind mwheeldown +jump; bind mwheelup +jump; bind CAPSLOCK norm;"
alias norm "bind mwheeldown invprev; bind mwheelup invnext; bind CAPSLOCK bhop;"
alias bhopon "bind MWHEELDOWN +jump;bind MWHEELUP +jump;bind CAPSLOCK bhopoff"
alias bhopoff "bind MWHEELDOWN invnext;bind MWHEELUP invprev;bind CAPSLOCK bhopon"
//Configuracao de servidor dedicado
rconpassword
//rcon removeallids // Remove all user IDs from the ban list.
//rcon writeid // Writes a list of permanently-banned user IDs to banned_user.cfg
//rcon writeip // Save the ban list to banned_ip.cfg.
//xsave // Saves current game to a console storage device*
//ping // Display ping to server
//log on // and udp < on | off >
//pingserver 189.1.171.55:27015
//_autosave // Autosave*
// Compra de armas no teclado numerico
bind kp_ins "buy vesthelm" // 0
bind kp_del "buy vest" // .
bind kp_enter "buy defuser" // Enter
bind kp_end "buy hegrenade;give weapon_hegrenade" // 1
bind kp_downarrow "buy flashbang;give weapon_flashbang" // 2
bind kp_pgdn "buy smokegrenade;give weapon_smokegrenade" // 3
bind kp_leftarrow "buy deagle;give weapon_deagle" //4
bind kp_5 "buy incgrenade;buy molotov;give weapon_incgrenade;give weapon_molotov" // 5
bind kp_rightarrow "buy decoy;give weapon_decoy" // 6
bind kp_home "buy awp;give weapon_awp" // 7
bind kp_uparrow "buy m4a1;buy m4a4;buy ak47;give weapon_m4a1_silencer;give weapon_ak47;" // 8
bind kp_pgup "buy famas;buy galilar;give weapon_famas;give weapon_galilar" // 9
bind kp_slash "buy p90;give weapon_p90" // /
bind kp_multiply "buy mp7;" // *
//bind kp_multiply "buy mp7;give weapon_mp7" // *
//bind "kp_multiply" "buy mp9; buy mac10;" // *
//bind kp_multiply "buy ump45;give weapon_ump45" // *
//bind kp_multiply "buy sg556; buy aug;" // *
//bind kp_minus "buy sawedoff;buy mag7;give weapon_sawedoff;give weapon_mag7" // -
bind kp_minus "buy tec9; buy fiveseven;" // - TEC9
bind kp_plus "buy p250;give weapon_p250" // +
//http://csgobindsgenerator.com/
clear	// apaga no console o texto para melhorar a apresentacao do texto abaixo
echo "" // esta linha serve para imprimir uma linha vazia no console, apenas para melhorar a apresentacao do texto abaixo
clear
echo "__________                   _______  .__            __        "
echo "\____    /___________  ____  \      \ |__| ____     |__|____   "
echo "  /     // __ \_  __ \/  _ \ /   |   \|  |/    \    |  \__  \  "
echo " /     /\  ___/|  | \(  <_> )    |    \  |   |  \   |  |/ __ \_"
echo "/_______ \___  >__|   \____/\____|__  /__|___|  /\__|  (____  /"
echo "        \/   \/                     \/        \/\______|    \/ "
echo "Steam ZeroNinja > http://steamcommunity.com/id/ZeroNinjaTV"
echo ""
echo "BINDS DE COMPRA NO TECLADO NUMERICO (COMPRA RAPIDA):"
// INFORMACOES DAS TECLAS PERSONALIZADAS ////////////////////////////////
// . -------------------------------------------------------------------.
// | [Esc] [F1][F2][F3][F4][F5][F6][F7][F8][F9][F0][F10][F11][F12] o o o|
// |                                                                    |
// | [`][1][2][3][4][5][6][7][8][9][0][-][=][_<_] [I][H][U] [N][/][*][-]|
// | [|-][Q][W][E][R][T][Y][U][I][O][P][{][}] | | [D][E][D] [7][8][9]|+||
// | [CAP][A][S][D][F][G][H][J][K][L][;]['][#]|_|           [4][5][6]|_||
// | [^][\][Z][X][C][V][B][N][M][,][.][/] [__^__]    [^]    [1][2][3]| ||
// | [c]   [a][________________________][a]   [c] [<][V][>] [ 0  ][.]|_||
// `--------------------------------------------------------------------'
/////////////////////////////////////////////////////////////////////////
echo "" // alterar estas binds utilizando o F1 ate o F12 se seu teclado nao tem numpad
echo "+=====================================================+"
echo "|     NUM     |      /      |      *      |     -     |"
echo "|     PAD     |     P90     |     MP7     |    TEC9   |"
echo "|-------------|-------------|-------------|-----------|"
echo "|      7      |      8      |      9      |     +     |"
echo "|     AWP     | M4A4 ou AK  | GALIU/FAMAS |           |"
echo "|-------------|-------------|-------------|   P250    |"
echo "|      4      |      5      |      6      |           |"
echo "|  DESERT E.  |   MOLOTOV   |    DECOY    |           |"
echo "|-------------|-------------|-------------|-----------|"
echo "|      1      |      2      |      3      |           |"
echo "| GRANADA EXP |  LIGHT/LUZ  |    SMOKE    |   ENTER   |"
echo "|-------------|-------------|-------------|           |"
echo "|             0             |      .      |   DEFUSE  |"
echo "|   COLETE / KEVLAR-VEST    |   HELMET    |           |"
echo "+=====================================================+"
echo "+======================================================+"
echo "|     INSERT     |       HOME       |     PAGE UP      |"
echo "|  Mostrar Dano  |   Mensagem Time  |  SAY >> GO A <<  |"
echo "|----------------|------------------|------------------|"
echo "|     DELETE     |       END        |    PAGE DOWN     |"
echo "|  Reload .CFG   |   Ir para SPEC   |  SAY >> GO B <<  |"
echo "|----------------|------------------|------------------|"
echo "|    bunnyhop    |    MUTAR SONS    |    MUTAR VOZ     |"
echo "|  bhop / norm   |   mute / unmute  | voicemute/unvoice|"
echo "+======================================================+"
echo "+============================================================+"
echo "|  TECLAS MODIFICADAS/PERSONALIZADAS:                        |"
echo "|  [v] Falar com a equipe  [,] Show Mouse                    |"
echo "|  [.] say !ready  [l] Liberar memoria  [k] Trocar de mao    |"
echo "+============================================================+"
echo "+===================================================================+"
echo "|       F1       |       F2       |       F3       |       F4       |"
echo "|     HOLDPOS    |COVERME/CUBRA-ME|ROGER/AFIRMATIVO|   NEEDBACKUP   |"
echo "|----------------|----------------|----------------|----------------|"
echo "|       F5       |       F6       |       F7       |       F8       |"
echo "|   Helm FULL    |  Granadas FULL |     DEFUSER    |High-ExplosiveHE|"
echo "|----------------|----------------|----------------|----------------|"
echo "|       F9       |      F10       |      F11       |      F12       |"
echo "|  Mouse Slower  |  Mouse Faster  | Workshop ARMAS |ScreenShot/Print|"
echo "+===================================================================+"
echo "*Abra o console antes de apertar o F8 e o F11"
echo "*Troque a sua mira apertando o botao do scroll do mouse"
//bind "F2" " buy vest;"
//bind "F3" " buy vesthelm; buy vest;"
//bind "F4" " buy defuser;"
//bind "F5" " buy hegrenade;"
//bind "F6" " buy flashbang;"
//bind "F7" " buy smokegrenade;"
//bind "F8" " buy molotov; buy incgrenade;"
bind "F1" "holdpos" // Aviso para o bot ficar na base
bind "F2" "coverme" // Aviso para o bot te seguir e te ajudar
bind "F3" "roger" // Aviso de Afirmativo
bind "F4" "needbackup" // Aviso de Precisando de Backup
//bind "F1" "mp_restartgame 1"
//bind "F2" "toggle sv_showimpacts"
//bind "F3" "toggle sv_infinite_ammo"
//bind "F4" "toggle bot_dont_shoot"
alias "botkick" "bot_kick; rcon bot_kick"
alias "botaddtr" "bot_add_t; rcon bot_add_t"
alias "botaddct" "bot_add_ct; rcon bot_add_ct"
//bind "F5" "botkick"
//bind "F6" "botaddtr"
//bind "F7" "botaddct"
//bind "F8" "demoui"
bind "F5" "buy vest; buy vesthelm; buy defuser;"
bind "F6" "buy incgrenade; buy molotov; buy flashbang; buy hegrenade; buy smokegrenade;"
bind "F7" "buy defuser;"
bind "F8" "buy hegrenade;"
//bind "F9" "host_timescale 0.5;demo_timescale 0.4"
//bind "F10" "host_timescale 1;demo_timescale 1"
bind "F11" "workshop_workbench"
//bind "F11" "host_timescale 2;demo_timescale 3" // 150%
unbind "F12" // Print Screen Default CS:GO // Take a jpeg screenshot: jpeg <filename> <quality 1-100> // screenshot
//bind "F5" "buy ak47; buy m4a1;"
//bind "F6" "buy awp;"
//bind "F7" "buy mp7;"
//bind "F8" "buy mac10; buy mp9;"
//bind "F11" "buy p90;"
//bind "F12" "buy tec9; buy fiveseven;"
// Gerador de Binds - http://csgobindsgenerator.com
echo ""
echo "===================================================="
echo "===[    ZeroNinja Autoexec.CFG carregada!     ]====="
echo "===================================================="
soundscape_flush
host_writeconfig // write settings to config.cfg
stop
//#
