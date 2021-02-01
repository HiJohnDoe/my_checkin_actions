# my_checkin_actions
### This Repo usage:   scripts for Auto check in .
  

#### Repo url:
> Github: https://github.com/HiJohnDoe/my_checkin_actions.git

Detail:
|    Project            | Dir               |     usage                                                                                       |
| ------------          | ------------------| ---------------                                                                                 |
|  my_checkin_actions   | cloud_189         |  https://cloud.189.cn/ , China Telecom NetDisk auto check in,  get free NetDisk space           |
|                       | mistep            |  APP: XiaoMi health , set any steps u want to archive and upload                                |
|                       | music_163         |  https://music.163.com/ , NetEase CloudMusic auto check in, level up by listening 300+ songs every day |
|                       | note_163          |  http://note.youdao.com/ , NetEase youdao notebook auto check in,  get free space               |
|                       | tieba             |  https://tieba.baidu.com/index.html , Baidu Tieba auto check in,  level up by check in bars     |
|                       | wps               |  https://www.wps.cn/ , Kingsoft Office, auto check in,  get free VIP by invite other users      |

Time schedule:
|    Type           |         Crontab        |       UTC+0         |  Beijing time : UTC+8    |
|--------------     | -----------------------|-------------------  |-------------------       |
|     cloud_189     |       '0 2,14 * * *'   |  every 2:00 14:00   |    every 10:00 22:00     |
|     mistep        |       '0 10 * * *'     |  every 10:00        |    every 18:00           |
|     music_163     |       '0 22,14 * * *'  |  every 22:00 14:00  |    every 6:00 22:00      |
|     note_163      |       '0 1 * * *'      |  every 1:00         |    every 9:00            |
|     tieba         |       '5 16,22 * * *'  |  every 16:05 22:05  |    every 0:05 6:05       |
|     wps           |       '45 0,2 * * *'   |  every 0:45 2:45    |    every 8:45 10:45      |

