# REWEMA
(Retrieval Windows Executables Malware Analysis)

## Commercial Antivirus Limitation
Technically, the modus operandi for the identification of malicious files and servers refers to consult in named blacklist databases. The VirusTotal platform issues the diagnoses regarding malignant characteristics related to files and web servers.

When it comes to suspicious files, VirusTotal issues the diagnostics provided by the world's leading commercial antivirus products. Regarding suspicious web servers, VirusTotal uses the database responsible for sensing virtual addresses with malicious practices.

VirusTotal has Application Programming Interface (APIs) that allow programmers to query the platform in an automated way and without the use of the graphical web interface. The proposed paper employs two of the APIs made available by VirusTotal. The first one is responsible for sending the investigated files to the platform server. The second API, in turn, makes commercial antivirus diagnostics available for files submitted to the platform by the first API.

Figure 1 shows the diagram of the methodology proposed in block diagram. Initially, the executable malwares are sent to the server belonging to the VirusTotal platform. After that, the executables are analyzed by the 86 commercial antiviruses linked to VirusTotal. Therefore, the antivirus provides its diagnostics for the executables submitted to the platform. VirusTotal allows the possibility of issuing three different types of diagnostics: malware, benign and omission.

Then, through the VirusTotal platform, the proposed paper investigates 86 commercial antiviruses with their respective results presented in Table 2. We used 3136 malicious executables for 32-bit architecture obtained from the REWEMA database [10]. The goal of the work is to check the number of virtual pests cataloged by antivirus. The motivation is that the acquisition of new virtual plagues plays an important role in combating malicious applications. Therefore, the larger the database of malwares blacklisted, the better it tends to be the defense provided by the antivirus.

As for the first possibility of VirusTotal, the antivirus detects the malignity of the suspicious file. In the proposed experimental environment, all submitted executables are public domain malwares. Therefore, in the proposed study, the antivirus hits when it detects the malignity of the investigated executable. Malware detection indicates that the antivirus provides a robust service against cyber-intrusions. As larger the blacklist database, better tends to be the defense provided by the antivirus.

In the second possibility, the antivirus attests to the benignity of the investigated file. Therefore, in the proposed study, when the antivirus attests the benignity of the file, it is a case of a false negative – since all the samples are malicious. That is, the investigated executable is a malware; however, the antivirus attests to benignity in the wrong way.

In the third possibility, the antivirus does not emit opinion about the suspect executable. The omission indicates that the file investigated has never been evaluated by the antivirus neither it has the robustness to evaluate it in real time. The omission of the diagnosis by the antivirus points to its limitation on large-scale services.

In the third possibility, the antivirus does not emit opinion about the suspect executable. The omission indicates that the file investigated has never been evaluated by the antivirus neither it has the robustness to evaluate it in real time. The omission of the diagnosis by the antivirus points to its limitation on large-scale services.

Table 2 shows the results of the evaluated 86 antivirus products. Five of these antiviruses scored above 98%. These antiviruses were: McAfee-GW-Edition, McAfee, Kaspersky, NANO-Antivirus and Panda. Malware detection indicates that these antivirus programs provide a robust service against cyber-intrusions.

A major adversity in combating malicious applications is the fact that antivirus makers do not share their malware blacklists due to commercial disputes. Through Table 2 analyse, the proposed paper points to an aggravating factor of this adversity: the same antivirus vendor does not even share its databases between its different antivirus programs. Note, for example, that McAfee-GW-Edition and McAfee antiviruses belong to the same company. Their blacklists, though robust, are not shared with each other. Therefore, the commercial strategies of the same company hinder the confrontation with malware. It complements that antivirus vendors are not necessarily concerned with avoiding cyber-invasions, but with optimizing their business income.

Malware detection ranged from 0% to 99.11%, depending on the antivirus being investigated. On average, the 86 antiviruses were able to detect 54.84% of the evaluated virtual pests, with a standard deviation of 39,67. The high standard deviation indicates that the detection of malicious executables may suffer abrupt variations depending on the antivirus chosen. It is determined that the protection, against cybernetic invasions, is due to the choice of a robust antivirus with a large and updated blacklist.

As for the false negatives, the Zoner, Malwarebytes and SUPERAntiSpyware antiviruses, wrongly stated that malware was benign in more than 90% of cases. On average, antiviruses attested false negatives in 14.34% of the cases, with a standard deviation of 21.67. Tackling the benignity of malware can lead to irrecoverable damage. A person or institution, for example, would rely on a particular malicious application when, in fact, it is malware.

VirusBuster, NOD32, eSafe, eTrust-Vet, Authentium, Prevx, Sunbelt, PCTools, a-squared, WhiteArmor, Command, SAVMail, FileAdvisor,Ewido and Webwasher-Gateway antivirus companies have not omitted opinion on any of the 3136 samples malicious. Therefore, about 17% of antivirus softwares were not able to diagnose any of the malicious samples. On average, the antiviruses were missing in 30.82% of the cases, with a standard deviation of 40.97. The omission of the diagnosis points to the limitation of these antiviruses that have limited blacklists for detection of malware in real time.

It is included as adversity, in the combat to malicious applications, the fact of the commercial antiviruses do not possess a pattern in the classification of the malwares as seen in Table 3. We choose 3 of 3136 REWEMA malwares samples in order to exemplify the miscellaneous classifications of commercial antiviruses. The chosen malware are Backdoor.IRC.Darkirc.exe, Backdoor.Win32.Zomby.exe e Constructor.VBS.Alamar.20.exe. In this way, the time when manufacturers react to a new virtual plague is affected dramatically. As there is no a pattern, antiviruses give the names that they want, for example, a company can identify a malware as "Malware.1" and a second company identify it as "Malware12310". Therefore, the lack of a pattern, besides the no-sharing of information among the antivirus manufacturers, hinders the fast and effective detection of a malicious application.

###### Table 2 Results of 86 commercial antiviruses:

Antivirus | Detection (%) | False negative (%) | Omission (%)
--------- | ------------- | ------------------ | -------------
McAfee-GW-Edition | 99.11% | 0.89% | 0.00%
McAfee | 98.98% | 1.02% | 0.00%
Panda  | 98.76% | 1.15% | 0.10%
Comodo  | 98.37% | 1.59% | 0.03%
Kaspersky | 98.34% | 1.56% | 0.10%
NANO-Antivirus | 98.25% | 1.69% | 0.06%
Symantec  | 97.64% | 2.26% | 0.10%
GData | 97.23% | 2.77% | 0.51%
BitDefender | 97.23% | 2.77% | 0.00%
MicroWorld-eScan | 96.94% | 2.74% | 0.32%
F-Secure | 98.76% | 3.00% | 1.12%
Qihoo-360  | 95.66% | 1.69% | 2.65%
VIPRE | 95.54% | 4.46% | 0.00%
Sophos | 95.38% | 4.53% | 0.10%
Emsisoft | 95.22% | 4.21% | 0.57%
Avira | 95.18% | 2.39% | 2.42%
CMC  | 95.15% | 4.37% | 0.48%
Arcabit | 94.58% | 4.21% | 1.21%
DrWeb | 94.36% | 5.61% | 0.03%
Ad-Aware | 93.88% | 3.32% | 2.81%
Fortinet | 93.85% | 6.15% | 0.00%
Rising | 93.72% | 5.01% | 1.28%
Antiy-AVL  | 92.38% | 7.21% | 0.41%
Jiangmin | 91.87% | 8.04% | 0.10%
Ikarus | 90.50% | 8.20% | 1.31%
Cyren | 90.34% | 8.67% | 0.99%
Zillya | 89.89% | 8.32% | 1.79%
F-Prot | 89.51% | 10.49% | 0.00%
TheHacker | 87.69% | 12.28% | 0.03%
Avast  | 86.19% | 13.71% | 0.10%
ESET-NOD32  | 86.13% | 13.87% | 0.00%
AVG  | 85.55% | 14.45% | 0.00%
Microsoft  | 85.20% | 14.80% | 0.00%
AegisLab | 82.40% | 17.12% | 0.48%
Tencent | 82.21% | 6.44% | 11.35%
VBA32  | 81.12% | 18.88% | 0.00%
TrendMicro-HouseCal | 79.02% | 17.83% | 3.16%
K7AntiVirus  | 78.95% | 21.05% | 0.00%
K7GW  | 78.83% | 21.17% | 0.00%
AVware | 78.64% | 4.02% | 17.25%
TrendMicro | 78.54% | 18.53% | 2.93%
ALYac | 77.20% | 16.55% | 6.25%
Yandex | 70.22% | 3.19% | 26.59%
AhnLab-V3  | 69.29% | 30.52% | 0.19%
nProtect | 67.22% | 32.49% | 0.29%
ViRobot | 64.06% | 35.94% | 0.00%
ClamAV | 59.41% | 40.31% | 0.29%
ZoneAlarm | 54.37% | 1.02% | 44.61%
Webroot | 52.04% | 2.20% | 45.76%
MAX  | 50.77% | 1.66% | 47.58%
Cylance | 48.60% | 2.87% | 48.53%
TotalDefense | 41.04% | 53.13% | 5.84%
CrowdStrike | 40.88% | 21.78% | 37.34%
Invincea | 40.27% | 27.04% | 32.68%
Endgame | 40.18% | 14.99% | 44.83%
Baidu | 39.48% | 34.98% | 25.54%
CAT-QuickHeal | 39.19% | 60.81% | 0.00%
Agnitum | 25.22% | 0.80% | 73.98%
Bkav | 22.39% | 73.02% | 4.59%
SentinelOne | 20.92% | 32.49% | 46.59%
Kingsoft | 19.87% | 57.59% | 22.54%
Paloalto | 17.60% | 37.12% | 45.28%
SUPERAntiSpyware | 7.33% | 92.67% | 0.00%
Malwarebytes | 7.21% | 92.19% | 0.61%
ByteHero | 2.36% | 23.50% | 74.14%
Zoner | 2.17% | 96.65% | 1.18%
Norman  | 1.18% | 0.03% | 98.79%
AntiVir | 0.99% | 0.00% | 99.01%
Commtouch | 0.89% | 0.10% | 99.01%
Ahnlab | 0.03% | 0.00% | 99.97%
Alibaba | 0.00% | 35.49% | 64.51%
VirusBuster | 0.00% | 0.00% | 100.0%
NOD32  | 0.00% | 0.00% | 100.0%
eSafe | 0.00% | 0.00% | 100.0%
eTrust-Vet | 0.00% | 0,00% | 100.0%
Authentium | 0.00% | 0.00% | 100.0%
Prevx | 0.00% | 0.00% | 100.0%
Sunbelt | 0.00% | 0.00% | 100.0%
PCTools | 0.00% | 0.00% | 100.0%
Squared | 0.00% | 0.00% | 100.0%
WhiteArmor | 0.00% | 0.00% | 100.0%
Command | 0.00% | 0.00% | 100.0%
SAVMail | 0.00% | 0.00% | 100.0%
FileAdvisor | 0.00% | 0.00% | 100.0%
Ewido | 0.00% | 0.00% | 100.0%
Webwasher-Gateway | 0.00% | 0.00% | 100.0%


###### Table 3 Miscellaneous classifications of commercial antiviruses:

Antivirus | Backdoor.IRC.Darkirc.exe | Backdoor.Win32.Zomby.exe | Constructor.VBS.Alamar.20.exe
--------- | ------------------------ | ------------------------ | ------------------------------
McAfee-GW-Edition | BehavesLike.Win32.Dropper.hh | BehavesLike.Win32.Ramnit.lh | BehavesLike.Win32.Almanahe.dm
McAfee | BackDoor-QZ | W32/Kernl | W32/Generic.a@MM
Panda | Backdoor Program | Backdoor Program | VBS/VBSWGKit.200.B
Comodo | Backdoor.IRC.Dark.A | Backdoor.Win32.Zomby.B | Constructor.Alamar.20.B
Kaspersky | Backdoor.IRC.Darkirc.a | Backdoor.Win32.Zomby.b | Constructor.VBS.Alamar.20.b
NANO-Antivirus | Trojan.Win32.Darkirc.gymm | Trojan.Win32.Zomby.fyqd | Riskware.Win32.Alamar-20.hpxt
Symantec | Backdoor.Darkirc | W32.Ernl | Suspicious.Cloud.9
GData | Gen:Trojan.Heur.LG0@kBd4oubi | Gen:Trojan.Heur.FU.bu0@amWsPhc | Gen:Trojan.Heur2.VP2.mm0@auxTBiH
BitDefender | Gen:Trojan.Heur.LG0@kBd4oubi | Gen:Trojan.Heur.FU.bu0@amWsPhc | Gen:Trojan.Heur2.VP2.mm0@auxTBiH
MicroWorld-eScan | Gen:Trojan.Heur.LG0@kBd4oubi | Gen:Trojan.Heur.FU.bu0@amWsPhc | Gen:Trojan.Heur2.VP2.mm0@auxTBiH
F-Secure | Gen:Trojan.Heur.LG0@kBd4oubi | Gen:Trojan.Heur.FU.bu0@amWsPhc | Gen:Trojan.Heur2.VP2.mm0@auxTBiH
Qihoo-360 | Omission | Malware.Radar01.Gen | Win32/Trojan.64c
VIPRE | Trojan.Win32.Ircbot!cobra (v) | Trojan.Win32.Generic!BT | Trojan.Win32.Generic!BT
Sophos | Troj/Bdoor-QZ | Troj/Kernl | Troj/VB-EBO
Emsisoft | Gen:Trojan.Heur.LG0@kBd4oubi (B) | Gen:Trojan.Heur.FU.bu0@amWsPhc (B) | Gen:Trojan.Heur2.VP2.mm0@auxTBiH (B)
Avira | BDS/DarkIRC.A.Srv | BDS/Zomby.B.Srv | KIT/VBS.Alamar.20
CMC | Generic.Win32.ae234d7c34!MD | Generic.Win32.03f0793a06!MD | Generic.Win32.56c37100ce!MD
Arcabit | Trojan.Heur.ED7F69 | Trojan.Heur.FU.EC280C | Trojan.Heur2.VP2.E85FD5
DrWeb | BackDoor.Darkirc.40 | BackDoor.Zomby | VBSWG.Generator
Ad-Aware | Gen:Trojan.Heur.LG0@kBd4oubi | Gen:Trojan.Heur.FU.bu0@amWsPhc | Gen:Trojan.Heur2.VP2.mm0@auxTBiH
Fortinet | IRC/Bdoor.QZ!tr.bdr | W32/Zomby.B | W32/VBSWG.A!tr
Rising | PE:Trojan.IRC.Dark.a!17014 [F] | PE:Backdoor.Zomby.b!49750 [F] | PE:Constructor.VBS.ALAMAR.02.b!100036554 [F]
Antiy-AVL | Trojan[Backdoor]/IRC.Darkirc | Trojan[Backdoor]/Win32.Zomby | HackTool[Constructor]/VBS.Alamar
Jiangmin | Backdoor/IRC.Darkirc.a | Backdoor/Zomby.b | Constructor.VBS.Alamar.20.b
Ikarus | Backdoor.Win32.FTP.Ics | Backdoor.Win32.Zomby | Constructor.VBS.Alamar
Cyren | W32/Risk.CGSZ-3998 | W32/Risk.VRJN-5887 | Benign
Zillya | Backdoor.Darkirc.Win32.14 | Backdoor.Zomby.Win32.2 | Tool.Alamar.Win32.11
F-Prot | W32/Malware!59a6 | W32/Malware!969ª | Benign
TheHacker | Trojan/Hami | Backdoor/Zomby.b | Trojan/Alamar.20.b
Avast | Win32:Darkirc [Trj] | Win32:Evo-gen [Susp] | Win32:Alamar [Trj]
ESET-NOD32 | IRC/Dark.A | Win32/Zomby.B | Alamar.20.B Constructor
AVG | IRC/BackDoor.Darkirc.A | BackDoor.Zomby | Constructor.HN
Microsoft | Backdoor:IRC/Dark | Backdoor:Win32/Zomby | Constructor:VBS/Alamar.B
AegisLab | Benign | Backdoor.W32.Zomby.b!c | Benign
Tencent | Omission | Omission | Omission
VBA32 | Backdoor.IRC.Darkirc | Backdoor.Zomby | Constructor.VBS.Alamar.20
TrendMicro-HouseCal | BKDR_DARKIRC.A | TROJ_ZOMBY.B | TROJ_VBSWG.A
K7AntiVirus | Trojan ( 00070c071 ) | Riskware ( 0040eff71 ) | Benign
K7GW | Trojan ( 00070c071 ) | Riskware ( 0040eff71 ) | Benign
AVware | Omission | Trojan.Win32.Generic!BT | Omission
TrendMicro | BKDR_DARKIRC.A | TROJ_ZOMBY.B | TROJ_VBSWG.A
ALYac | Omission | Benign | Benign
Yandex | Omission | Omission | Omission
AhnLab-V3 | Win-Trojan/Darkirc | Win-Trojan/Zomby.16896 | Constructor/VBSWG.208896
nProtect | Backdoor/W32.IRCBot.608256.B | Backdoor/W32.Zomby.16896 | Constructor/W32.VBS-Alamar.208896
ViRobot | Backdoor.Win32.DarkIRC[h] | Backdoor.Win32.Zomby.16896[h] | Benign
ClamAV | Trojan.IRC.Darkirc.A | Benign | Kit.VBS.Alamar.20
ZoneAlarm | Omission | Omission | Omission
Webroot | Omission | Omission | Omission
MAX | Omission | Omission | Omission
Cylance | Omission | Omission | Omission
TotalDefense | Win32/DarkIRC.40 | Benign | Win32/Alamar.Kit.20b
CrowdStrike | Omission | Omission | Omission
Invincea | Omission | Omission | Omission
Endgame | Omission | Omission | Omission
Baidu | Trojan.IRC.Dark.A | Backdoor.Win32.Zomby.b | Trojan.VBS.Alamar.20
CAT-QuickHeal | Backdoor.IRC.Darkirc.a.n8 | Backdoor.Zomby.r5 | Constructor.VBS_2.0
Agnitum | Backdoor.IRC.Darkirc.A | Backdoor.Zomby!n5cvmDuGKio | HackTool.Agent!yQKDt6dVyX8
Bkav | Benign | Omission | Benign
SentinelOne | Omission | Omission | Omission
Kingsoft | Omission | Omission | Omission
Paloalto | Omission | Omission | Omission
SUPERAntiSpyware | Benign | Benign | Benign
Malwarebytes | Benign | Benign | Trojan.ConstructionKit
ByteHero | Benign | Benign | Benign
Zoner | Benign | Benign | Benign
Norman | Omission | Omission | Omission
AntiVir | Omission | Omission | Omission
Commtouch | Omission | Omission | Omission
Ahnlab | Win-Trojan/Darkirc | Omission | Omission
Alibaba | Benign | Benign | Benign
VirusBuster | Omission | Omission | Omission
NOD32 | Omission | Omission | Omission
eSafe | Omission | Omission | Omission
eTrust-Vet | Omission | Omission | Omission
Authentium | Omission | Omission | Omission
Prevx | Omission | Omission | Omission
Sunbelt | Omission | Omission | Omission
PCTools | Omission | Omission | Omission
Squared | Omission | Omission | Omission
WhiteArmor | Omission | Omission | Omission
Command | Omission | Omission | Omission
SAVMail | Omission | Omission | Omission
FileAdvisor | Omission | Omission | Omission
Ewido | Omission | Omission | Omission
Webwasher-Gateway | Omission | Omission | Omission

## Materials and Methods

This paper proposes a database aiming at the classification of 32-bit benign and malware executables. The database is referred to as REWEMA (Retrieval of 32-bit Windows Architecture Executables Applied to Malware Analysis). There are 3136 malicious executables, and 3136 other benign executables. Therefore, the REWEMA base is suitable for learning with artificial intelligence, since both classes of executables have the same amount.

As for malicious executables, REWEMA is the junction of several malware databases. Virtual plagues were extracted from databases provided by enthusiastic study groups such as Vxheaven and TheZoo. As for benign executables, the acquisition came from benign applications repositories such as sourceforge, github and sysinternals. It should be noted that all benign executables were submitted to VirusTotal and all were its benign attested by the main commercial antivirus worldwide. The diagnostics, provided by VirusTotal, corresponding to the benign and malware executables are available in the virtual address of the REWEMA database.

The purpose of the creation of the REWEMA database is to give full possibility of the proposed methodology being replicated by third parties in future works. Therefore, the proposed article, by making its database freely available, enables transparency and impartiality to research, as well as demonstrating the veracity of the results achieved. Therefore, it is hoped that the methodology, to be reported in chapter 6, will serve as a basis for the creation of new scientific works.
