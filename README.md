# Commit History Evidence — 蜜蜂打卡-考勤工时记 (BeeClock)

Prepared as supporting material for the App Review discussion
(Guideline 4.3(a) response) — October 2026.

This document contains the complete, unabridged commit history of the
"蜜蜂打卡-考勤工时记" (BeeClock) app, exported directly from the developer's
private git repositories. It demonstrates that the app is an original work,
independently developed over multiple years:

- **Phase 1 — Original prototype (October – December 2019), 18 commits.**
  From the first working version (clock-in / clock-out recording) through
  v1.2 (make-up check-in, day-record editing, holiday-date checking,
  welcome / splash screens). Preserved in the developer's private GitHub
  repository "worktime".
- **Phase 1.5 — Continued prototype (December 2019 – July 2020), 35 commits.**
  The same project carried further: server-side holiday-calendar
  synchronization, background refresh, monthly and yearly history views,
  cross-midnight (overnight) check-in support, settings refinements, and
  map/location exploration. Preserved on branch "syncday" of the same
  private repository.
- **Phase 2 — Current app (April 2025 – present), 320 commits.**
  The same personal project, rebuilt and extended into today's BeeClock:
  companion honeybee animation tied to attendance state, geofence
  arrival/departure reminders, Chinese statutory holiday calendar,
  7-day free trial with a one-time purchase.

No purchased template, third-party app source, or repackage was used at
any point. Commit messages are written in the developer's native language
(Chinese). The very first commit (October 2019) carries the developer's
earlier name signature ("WangQi"); all subsequent commits use the current
signature ("jamescss" / "james"). All commits are from the same author's
own repositories.

---

## Phase 1: 2019 prototype — oldest first (source: private repo "worktime")

2019-10-11 14:19:43  ca0866c  WangQi — Initial Commit
2019-10-20 10:19:28  c9bc188  jamescss — v0.1
2019-10-20 15:07:50  33df830  jamescss — v0.2 上班打卡和下班打卡区分
2019-10-24 15:34:48  8fe12d8  jamescss — V0.3 HTTPQUERY
2019-11-03 12:26:49  4558e07  jamescss — v0.3 调整为多VC之前
2019-11-10 04:46:54  7107e74  jamescss — v0.4 beforeDBchange
2019-11-12 14:37:57  63c56f3  jamescss — v0.5 下移打卡视图前
2019-11-14 14:32:56  bf9840a  jamescss — v0.6 调整视图布局
2019-11-17 07:57:48  b9d91c4  jamescss — v0.7 判断检查假期的日期是否改变
2019-12-01 12:06:53  30e18d3  jamescss — 0.9 添加图标和启动画面时后出错
2019-12-05 14:39:18  bec69b9  jamescss — v1.0 修复到没有更好icon之前的版本
2019-12-07 13:10:05  be53ea7  jamescss — v1.1 前台欢迎图
2019-12-07 13:37:32  b9cb4f0  jamescss — v1.2 启动前台不同图
2019-12-09 14:28:42  d170b2b  jamescss — v1.2 点击cell事件触发
2019-12-09 14:33:42  177b6e3  jamescss — v1.2 触发cell点击事件
2019-12-10 14:36:48  b20453b  jamescss — 弹出cell视图
2019-12-15 13:26:30  e773d59  jamescss — 完成了修改某天记录功能
2019-12-22 10:21:42  a1f3169  jamescss — 完成补卡功能

---

---

## Phase 1.5: 2019-12 – 2020 continued prototype — oldest first
(source: private repo "worktime", branch "syncday"; it branches off
the Phase 1 history, so the 16 commits it shares with Phase 1 are not
repeated here)

2019-12-22 18:15  87b980d  jamescss — 支持跨天打卡的之前版本
2019-12-25 22:02  494fddb  jamescss — 更新api之前
2019-12-31 20:29  12a0b96  jamescss — 同步节日数据前
2019-12-31 21:04  6f9a2b5  jamescss — 同步假日信息前
2019-12-31 21:14  a073f8e  jamescss — 同步假日
2020-01-02 23:26  a5acde8  jamescss — 搭建background处理
2020-01-04 23:06  64e13e5  jamescss — 查询服务端信息基本可运行，但synstat为空
2020-01-05 20:30  4c39390  jamescss — 分离calendar和synstat类定义之前
2020-01-05 22:48  6dfa333  jamescss — 初步完成从服务端查询日历的功能，但还没有特殊处理年底的查询提前量；使用已查询保存的日历数据，避免重复查询服务端
2020-01-07 22:12  85ad3cd  jamescss — 前后台切换的timer暂停恢复
2020-01-11 18:36  014bb22  jamescss — 本地查询假日信息
2020-01-16 23:14  f476acd  jamescss — 月历史TVC
2020-01-17 23:30  809e1b0  jamescss — 获取工作月列表
2020-01-21 23:00  c63cbbf  jamescss — 历史打卡数据按年拆分
2020-01-28 19:07  406dfdd  jamescss — 点击history list弹出窗口
2020-01-30 18:28  e2bd7f1  jamescss — 调整onoff布局
2020-01-30 21:50  fef77b0  jamescss — 为iphone8挑战layout之前的版本
2020-02-03 12:46  766ecbf  jamescss — before优化启动app查询api之前显示节日类型有误的版本
2020-02-03 21:46  0aaecfa  jamescss — 补卡前支持跨天打卡之前的版本
2020-02-08 22:34  12629be  jamescss — addsubview实现切前台动画
2020-02-09 14:52  10d1751  jamescss — 尝试在MainVC监听事件之前的版本
2020-02-11 22:32  74efc0f  jamescss — 执行推荐操作之前的版本
2020-02-16 16:23  8cb466b  jamescss — 使用小文件回前台画面可减少显示白屏的时长
2020-02-17 22:17  0519bb6  jamescss — 修正app切后台时跨天时钟处理bug
2020-03-11 09:50  a6d47bb  jamescss — 优化跨天工作的处理
2020-03-11 10:20  317cf3a  jamescss — 修正addcross bug
2020-04-07 00:01  f442b1d  jamescss — 修正判断某天类型值长度0的bug
2020-04-26 22:25  75be650  jamescss — 0426 调整保存按钮位置（优化app之前）
2020-04-26 22:58  33808ca  jamescss — 添加始终显示上班打卡switch
2020-04-28 23:06  6a4a32f  jamescss — 是否强制显示上班打卡按钮
2020-05-12 22:50  84fff0c  jamescss — 首次进入强制设置
2020-05-27 23:10  6f818e6  jamescss — NUT改进
2020-05-28 23:22  394486d  jamescss — 调整NUT显示
2020-05-30 23:43  41ffbaf  jamescss — NUTVC dismiss
2020-07-05 22:36  6a96e62  jamescss — 解析baidu结果成功

---

## Phase 2: current app, April 2025 – present — oldest first (source: private repo "worktime", main branch)

2025-04-16 21:29  7a24cd4  james — first commit
2025-04-16 22:31  a9152e1  james — 打卡按钮添加图标
2025-04-17 14:42  d6e696a  james — 取消切前台的画面显示
2025-04-17 16:24  67040de  james — 打卡按钮的图标化
2025-04-17 23:22  c8de6af  james — 按钮图标透明化
2025-04-18 22:53  bf4330f  james — 打卡图标onoff灰
2025-04-21 18:49  dbd8fc2  james — 打卡按钮双态显示
2025-04-21 21:42  0390487  james — 打卡按钮的inset函数简化
2025-04-22 10:09  2443184  james — 已下班打卡后再上班打卡的提醒
2025-04-22 11:19  0be034c  james — 上班打卡按钮的各场景逻辑补充
2025-04-22 14:38  516bb82  james — 非凌晨下班打卡的各场景处理
2025-04-22 16:16  7c3dad9  james — 给功能按钮添加图标，当月表添加了表头
2025-04-25 14:53  5f8db88  james — 添加flipclock前
2025-04-26 19:38  cf0adb7  james — 显示上班时长和加班时长
2025-04-26 21:26  3b70f10  james — 新增加班计时模式的配置
2025-04-28 11:42  30a573a  james — 修复配置扩展后启动报错的问题
2025-04-28 15:18  b9df8d4  james — 设置的模式选择联动
2025-05-06 16:31  043fef4  james — 支持新增配置的公用调参界面
2025-05-06 22:15  78159ba  james — 新增配置的调参OK
2025-05-07 11:17  b7c3f25  james — 配置的调参优化
2025-05-07 20:05  eaf0f5e  james — 禁止设置#0和#4号tbviewcell的点击
2025-05-08 13:25  db6b9e5  james — 显示弹性下班时间
2025-05-08 18:28  cec7454  james — 将当天工作的3个指标聚合到模型组件实现之前
2025-05-13 16:28  5412196  james — 完善每日工作综合信息功能的部分信息’ q wxit exit
2025-05-13 21:57  d74587e  james — 单日工作综合信息的函数集编写完成
2025-05-14 20:49  d38f50a  james — 使用单日工作综合信息的函数集展示当日工作仪表盘
2025-05-14 20:58  7dd99ea  james — 当日仪表盘的主字体改白，修改设置界面的按钮变灰
2025-05-21 16:24  cf69de3  james — 修正加班时长缺陷之前
2025-05-22 21:05  ec3f5b6  james — 设置界面的字符串合一‘
2025-05-22 22:49  3457aec  james — 加班模式的字符串合一
2025-05-23 22:06  8311aaa  james — 添加地理位置功能前
2025-05-23 22:50  d7e9c1d  james — 设置界面添加了地理位置属性
2025-05-25 20:48  a5e46f8  james — 完成打卡设置界面的布局
2025-05-26 21:35  85ef486  james — 将地址搜索移入地图之前
2025-05-26 22:39  26aaef3  james — 将地址搜索移入地图，调整打卡位置界面的布局优化
2025-05-27 20:54  350cca2  james — 添加图钉之前
2025-05-30 15:35  0446644  james — 简化打卡位置的选项
2025-05-30 23:16  8664396  james — 添加打卡位置相关的配置项
2025-05-31 15:29  ef5c49d  james — 位置保存的部分功能
2025-06-01 23:16  1602f41  james — 打卡位置设置基本完成
2025-06-02 19:26  5c21f3a  james — 增加午休时长的配置，用于计算有效工作时长
2025-06-03 22:33  302a464  james — 增加午休时长的配置
2025-06-06 14:26  e69876e  james — 配置说明优化
2025-10-07 09:10  32969b0  james — 基于地理围栏的自动打卡
2025-10-08 11:34  427b5e5  james — 修复地理围栏功能的编译错误
2025-10-08 20:06  09cc850  james — 优化了打卡类型的显示
2025-10-08 20:28  3e39624  james — 实现手动打卡优先级和可配置围栏半径
2025-10-08 21:39  ddbb101  james — 实现完整的跨天打卡功能优化
2025-10-09 10:32  5da314e  james — 修复应用前后台切换时界面不刷新的问题
2025-10-09 10:34  81644e9  james — 修复前后台切换时上班按钮不显示的问题
2025-10-09 10:48  2b38185  james — 修复AppDelegate.m中的变量重复定义错误
2025-10-09 11:28  9afa932  james — 使用SettingVC替代NutVC实现首次启动初始化
2025-10-09 11:34  2dbf797  james — 修复打卡位置设置界面布局问题
2025-10-09 11:40  7ecd71f  james — 调整打卡位置设置界面布局：将定位控件移入MapView内部
2025-10-09 12:48  843586d  james — 优化打卡位置设置界面的用户体验
2025-10-09 14:31  98c1cd0  james — 优化SettingVC界面的布局、交互和视觉效果
2025-10-09 15:00  2bb4b8c  james — 完成设置下级页面全部三个阶段的优化
2025-10-09 15:03  bac1db4  james — 修复ChgSetVC闪退问题
2025-10-09 15:51  6706067  james — 优化设置界面：实现分组TableView，体现配置项逻辑关系
2025-10-09 20:23  1e47993  james — 优化HistoryTVC历史记录界面的布局和交互
2025-10-09 20:40  220278c  james — 优化DayTVCell每日打卡记录界面
2025-10-09 20:47  a6c4adf  james — 优化editDayTimeVC编辑/补卡界面
2025-10-09 21:52  af1fd87  james — 优化MonthlistTVC界面：实现周分组折叠 + 汇总视图
2025-10-10 11:04  9adf1db  james — 新增地理围栏自动打卡功能 + 围栏半径配置
2025-10-10 12:09  9194b04  james — 修复HistoryTVC闪退问题 + 添加工作总时长显示 + 优化周汇总布局
2025-10-10 13:05  2589309  james — 界面优化：年度汇总简化、背景色修复、间距优化
2025-10-10 21:55  23d9006  james — 增强地理围栏状态跟踪：修复地下环境下班未打卡问题
2025-10-11 10:50  606546d  james — 优化打卡位置设置界面布局
2025-10-11 14:05  1ea2879  james — 新增图标帮助功能 + 优化ChgSetVC界面 + 日志优化
2025-10-13 10:39  bb7da1c  james — 使用通义灵码优化前版本
2025-10-13 19:47  5fae638  james — 修复地理围栏自动打卡闪退问题
2025-10-13 22:09  3ed5c2f  james — 完善主界面蜜蜂动画设计方案
2025-10-13 22:33  0378aa2  james — 实现蜜蜂动画主界面（方案A）
2025-10-14 09:21  3c23fe2  james — 修复ClockTimerEvent中上班按钮显示逻辑
2025-10-14 22:22  753cf4b  james — 修复地理围栏状态持久化问题，支持跨天校验
2025-10-15 16:32  b0b9d19  james — 位置坐标换算以正确计算距离
2025-10-16 08:27  08e4922  james — 修复地理围栏自动下班打卡失败问题
2025-10-16 08:29  0f6ed03  james — 修复自动下班打卡导致的线程安全崩溃
2025-10-16 08:35  845b503  james — 月视图周列表改为递减排序显示
2025-10-16 10:11  5a20f8a  james — 🔥 修复系统围栏状态判断错误导致的打卡失败bug
2025-10-16 10:12  066c49c  james — 修复MonthlistTVC周分组与NSFetchedResultsController不一致导致的崩溃
2025-10-17 12:45  467b340  james — 修复MonthlistTVC中的Auto Layout崩溃问题
2025-10-17 22:23  7418229  james — feat: 优化地理围栏状态判断逻辑，解决系统状态与实际距离不一致问题
2025-10-18 11:20  7464536  james — 修复计时器不工作问题并优化UI布局\n\n1. 修复AppDelegate中ClockTimerFunc方法，解决rootNVC为nil导致计时器无法正常工作的问题\n   - 实现三种获取OnOffRecordVC实例的备选方案\n   - 添加nil检查和错误处理\n   - 添加详细的日志输出便于调试\n\n2. 重新组织UI布局，改善MonthlistTVC显示问题\n   - 修改CurMonthSumVC的位置，将其移动到OnOffRecordVC下方\n   - 实现点击详情按钮时MonthlistTVC的显示/隐藏切换\n   - 调整MonthlistTVC的高度以避免被遮挡\n\n3. 完善SceneDelegate中的生命周期管理\n   - 在scene连接和激活时重新初始化计时器\n\n4. 优化MonthlistTVC界面\n   - 调整帮助按钮位置\n   - 移除可能引起冲突的约束设置\n\n5. 增强撤销打卡功能\n   - 添加撤销打卡记录后重置围栏状态并重新检查位置的逻辑\n   - 完善撤销操作后的UI刷新
2025-10-18 19:33  1474612  james — 调整主界面两个视图上下顺序和增加本月详情按钮
2025-10-19 21:46  6a24c76  james — feat: 完成蜜蜂动画功能开发与测试代码清理
2025-10-22 21:44  cb78aa3  james — 蜜蜂动画的完善
2025-10-22 23:27  8b8c04e  james — feat: 更换应用图标为蜜蜂图标并优化主界面蜜蜂动画联动
2025-10-23 11:41  615a20c  james — fix: 修复取消打卡后蜜蜂动画错误触发自动打卡的问题
2025-10-23 15:37  b969a7d  james — feat: 使用beeclock.png生成新的应用图标，解决黑边问题
2025-11-26 22:07  ab78308  james — revert: 撤销蜜蜂飞行动画的错误修改，恢复到稳定版本
2025-12-06 20:00  0e00e33  james — fix: 修复蜜蜂动画系统的多个关键问题
2025-12-06 20:04  d96d644  james — fix: 补充之前遗漏的文件变更
2025-12-06 20:10  cd00f15  james — chore: 更新 .gitignore 排除 Xcode 生成文件
2025-12-06 20:11  6fb704a  james — chore: 从版本控制中移除 Xcode 生成文件
2025-12-06 22:34  567b5c8  james — feat: OnOffRecordVC UI优化和蜜蜂状态管理改进
2025-12-06 23:11  d4bd9de  james — docs: 添加项目设计文档
2025-12-09 14:43  65a88c6  james — fix: 修复上班打卡按钮不显示和地理围栏自动打卡问题
2025-12-09 21:39  957145b  james — fix: 修复地理围栏自动下班打卡不触发问题
2025-12-09 21:54  af25b85  james — refactor: 优化CurMonthSumVC视图布局，提升可读性
2025-12-09 21:57  c81f219  james — fix: 修复CurMonthSumVC卡片高度约束问题
2025-12-10 10:04  b819bb5  james — refactor: 简化CurMonthSumVC布局为单行紧凑显示
2025-12-10 10:06  af26788  james — refactor: 调整OnOffRecordVC和CurMonthSumVC位置向上移动
2025-12-10 10:10  b222738  james — fix: 将CurMonthSumVC中的月份显示从'12月'改为'本月'
2025-12-10 11:18  341f9d3  james — fix: 修复考勤记录详情页崩溃和优化UI显示
2025-12-11 20:58  bcec795  james — fix: 修复BeeAnimationView中注释掉NSLog导致的语法错误
2025-12-11 21:10  e134ab8  james — feat: 下班打卡支持手动选择时间
2025-12-11 21:13  9a0c47a  james — fix: 修复showManualOffTimePickerForDate方法的编译错误
2025-12-11 21:28  5bf27fb  james — fix: 修复手动选择时间崩溃问题
2025-12-11 21:57  3c184ae  james — fix: 使用模态视图控制器实现时间选择器
2025-12-11 22:03  bcdb82a  james — fix: 改用文本输入方式选择下班时间
2025-12-11 22:07  859500b  james — fix: 修复手动选择时间的线程安全问题
2025-12-11 22:10  0023fe5  james — fix: 延迟显示手动时间选择对话框
2025-12-12 22:31  18de8e0  james — feat: 实现下班打卡多场景处理和手动时间选择功能
2025-12-13 21:00  15a34b4  james — feat: 刷新上班时间时验证是否晚于下班时间并提示用户
2025-12-13 22:41  8763c2f  james — fix: 修复时间显示格式和时间比较逻辑
2025-12-14 15:51  f4f6b30  james — feat: 扩展打卡记录以支持位置和触发机制追踪，优化自动下班打卡逻辑
2025-12-15 08:48  6adac36  james — fix: 修复撤销打卡后蜜蜂姿态不更新的问题
2025-12-15 21:43  c9335e2  james — fix: 修复中午离开围栏返回后，下午下班仍显示中午打卡时间的问题
2025-12-16 21:20  1fc2f4d  james — refactor: 移除蜜蜂姿态检查的调试日志输出
2025-12-16 21:30  b545c18  james — feat: 将打卡成功提示改为自动消失的Toast模式
2025-12-16 21:35  d1945a9  james — fix: 将清除下班打卡的成功提示改为Toast
2025-12-16 21:38  79271d1  james — refactor: 统一所有打卡成功提示为带动画的成功提示
2025-12-17 22:06  bd5c8de  james — fix: 修复中途离开围栏返回后再次离开时不更新下班时间的问题
2026-01-10 20:08  25587cd  james — fix: 修复iOS 13+兼容性问题并改进UI布局
2026-01-11 13:41  9bdada7  james — feat: 跨天打卡功能全面优化
2026-03-17 21:30  2f051ec  james — 通过opencil修改UI前
2026-04-12 16:14  4dfe551  james — fix: 修复 isTransitioning 防护机制导致的蜜蜂状态不同步问题
2026-04-12 16:49  8c3d7c3  james — docs: 在UI设计规范文档中添加应用功能说明
2026-04-12 17:05  b78e4b6  james — docs: 在应用简介中添加iOS平台和硬件信息
2026-04-12 17:59  711344b  james — docs: 添加蜜蜂元素和运动动画的详细说明
2026-04-16 15:13  41dbc06  james — fix: 修复中午外出返回后未清除自动下班打卡的问题
2026-04-20 11:59  3085274  james — 调整主界面的垂直布局
2026-04-20 21:30  ffa6ec0  james — 蜜蜂回到蜂巢中心
2026-04-21 20:41  450eb52  james — 蜜蜂视图加入storyboard
2026-04-22 14:12  364f3b6  james — fix: 修复汇总区详情按钮点击无响应的问题
2026-04-22 14:14  41b79df  james — chore: 移除调试用蓝色背景
2026-04-23 15:26  c00ed4a  james — fix: 详情按钮与设置按钮 centerX 精确对齐
2026-04-24 09:26  e410da9  james — feat: 统一全局蓝色UI主题，调整设置页面及子页面代码结构
2026-04-24 22:09  8aa78d9  james — fix: 修复 UIDatePicker.locale 在 iOS 16+ 上崩溃的问题
2026-04-24 22:33  24c1018  james — UI: LocationSetVC 和 ChgSetVC 应用蓝色主题风格
2026-04-24 22:46  b23d56d  james — UI: ChgSetVC 对照 Pencil 设计稿完善蓝色主题
2026-04-24 22:55  da7cd0a  james — fix: ChgSetVC 修复 DatePicker 尺寸和保存按钮全宽问题
2026-04-24 23:19  97faee6  james — fix: ChgSetVC DatePicker 和保存按钮尺寸修复
2026-04-24 23:23  59f5789  james — fix: ChgSetVC DatePicker 改为 Wheels 样式完整展示时间
2026-04-24 23:35  ebfa8ab  james — fix: ChgSetVC 修复卡片底部约束和 DatePicker 文字颜色
2026-04-24 23:37  79e4367  james — fix: ChgSetVC 卡片包住 DatePicker —— 改用固定高度约束
2026-04-26 21:54  36be646  james — chore: 保存 ChgSetVC 卡片布局探索版本（纯代码重建前的节点）
2026-04-27 09:44  aa2619f  james — fix: ChgSetVC 卡片成功包住 DatePicker 和输入框
2026-04-27 10:06  40a729a  james — fix: ChgSetVC 界面细节优化
2026-04-28 09:47  49de80f  james — feat: 设置界面全面重构为蓝色系卡片风格，修复打卡位置界面崩溃
2026-04-29 10:04  3df88fa  james — fix: 修复回家后打开 app 导致下班时间被错误覆盖的问题
2026-04-29 10:06  42fb6e3  james — feat: 本月汇总区监听 WorkStatusChangedNotification 实现自动刷新
2026-04-29 10:07  d9d3f71  james — fix: editDayTimeVC 保存后改用通知刷新本月汇总区
2026-04-29 10:08  fdf8bc5  james — fix: 设置界面保存参数后改用通知刷新本月汇总区
2026-04-29 10:19  4f739d0  james — feat: 打卡位置界面视觉优化
2026-04-29 11:00  3f87f75  james — fix: 修复打卡位置界面约束冲突和崩溃
2026-04-29 17:31  93aa781  james — feat: 打卡位置界面UI优化——位置卡片加标题、选择区胶囊组件、距离标签下移
2026-04-30 09:20  016d19b  james — feat: 新增每日围栏进入标志，修复手动修正上班时间后无法自动下班打卡的问题
2026-04-30 10:05  953fb10  james — fix: didEnterRegion 和 autoWorkOnCheckin 改用严格日期查询，修复昨天未下班导致今天无法自动上班打卡的问题
2026-05-03 22:26  981b7b6  james — feat: 过往界面Pencil设计稿优化 + LocationSetVC UI改动 + UI设计规范文档
2026-05-11 18:31  4df94c4  james — fix: 修复MonthlistTVC点击卡住 + UI布局优化
2026-05-12 17:16  34c4170  james — fix: 主界面本月周汇总数据未及时更新
2026-08-09 22:26  5de385f  james — fix: 修复补卡按钮在子页面残留 + 编辑页面UI优化
2026-08-13 11:28  5866208  james — fix: 应用返回前台时刷新周月汇总数据，修复运行一段时间后显示为空的问题
2026-08-14 09:42  f99d636  james — fix: 修复打卡栏时间显示闪动和左右移动问题
2026-08-14 10:47  f0633a5  james — feat: 围栏半径调整界面支持实时预览
2026-08-14 11:04  6ecea95  james — fix: 围栏半径页面与打卡地址页面分离
2026-08-14 11:09  a74aa04  james — fix: 围栏半径页面圆心逻辑
2026-08-14 11:19  18d61be  james — fix: 移除无效提示并优化围栏半径页面间距
2026-08-14 15:31  c829321  james — fix: 围栏半径页面地图视图高度调整
2026-08-14 15:37  b8a4769  james — fix: 围栏半径页面按钮底部间距
2026-08-15 11:17  90bc6ec  james — feat: 按钮脉冲引导动画系统
2026-08-15 11:42  b1c732d  james — feat: 上班/下班按钮添加文字标签
2026-08-15 11:47  95fed70  james — fix: 修复按钮标签ID冲突导致的崩溃
2026-08-15 21:28  d90a000  james — fix: 恢复使用新版按钮图片
2026-08-15 21:31  af8e111  james — fix: 修复tag冲突导致中间元素被误删
2026-08-15 21:34  d5de5d6  james — fix: 修复tag 9902冲突导致上班按钮下元素消失
2026-08-15 22:28  ee9d9b3  james — feat: 统一周月汇总卡加班时长颜色与打卡区一致
2026-08-15 22:36  8b53793  james — feat: 时长显示格式改为中文'xx小时yy分钟'
2026-08-16 20:58  5d89a93  james — feat: 将详情按钮移到表头左侧
2026-08-16 21:02  576cec1  james — fix: 修复表头与数据行对齐问题
2026-08-16 21:06  57fb5d0  james — fix: 详情按钮移到最左侧与本周标签对齐
2026-08-16 21:07  d0257fa  james — fix: 增加工作时长与加班时长列间距
2026-08-16 21:09  ff63e04  james — fix: 详情按钮移到最左侧与本周标签对齐
2026-08-16 21:13  0f7a064  james — fix: 详情按钮与本周标签中心对齐
2026-08-16 21:16  cd9c582  james — fix: 限制详情按钮容器高度，防止表头扩展
2026-08-16 21:27  819664a  james — feat: 调整列间距 - 工作时长与出勤天数间隔缩小，工作时长与加班时长间隔增大
2026-08-16 21:31  f2b9be1  james — fix: 添加容器高度约束修复布局问题
2026-08-16 21:35  793ddcb  james — fix: 调整列宽和间距
2026-08-16 21:37  422d3e8  james — fix: 重新添加字体自动缩小，确保工作时长完整显示
2026-08-16 21:53  1b4f170  james — fix: 优化周月汇总卡列间距和列宽
2026-08-16 21:56  efea2d2  james — feat: 详情和过往视图时长显示改为中文格式
2026-08-16 22:24  fbaaa26  james — feat: 每天打卡记录时长显示改为中文格式
2026-08-16 22:28  6e9a323  james — fix: 调整工作时长和加班时长布局，确保加班时长完整显示
2026-08-16 22:30  cec28cb  james — fix: 进一步调整布局确保加班时长完整显示
2026-08-16 22:32  6846e35  james — fix: 给加班时长label添加最小宽度约束
2026-08-16 22:35  8d4e58c  james — fix: 工作时长向左移动并增加宽度
2026-08-17 08:39  1902cde  james — fix: 工作时长向左移动增加宽度，留出足够间隔
2026-08-17 08:43  fc56c6b  james — fix: 继续向左移动工作时长，减小间隔防止超出边缘
2026-08-17 08:50  eb00844  james — fix: 缩小工作时长与加班时长之间的间隔
2026-08-17 08:55  d029d92  james — fix: 缩小下班时间与工作时长之间的间隔
2026-08-17 08:57  cd7071b  james — fix: 间隔缩小为当前的一半
2026-08-17 09:17  bb752dd  james — fix: 大幅缩小跨天标签宽度，增加工作时长显示区域
2026-08-17 09:20  323c1c2  james — fix: 统一详情视图与主视图的图标
2026-08-20 09:47  7a6866a  james — feat: 统一详情视图图标与主视图一致，添加中文日期显示
2026-08-20 11:06  a154c6c  james — fix: 修复蜜蜂动画初始状态不正确的问题
2026-08-20 14:33  25689b1  james — fix: 非工作日记录文字颜色保持正常，仅通过背景色区分
2026-08-20 14:43  068dd35  james — fix: 非工作日背景色改为清爽绿色
2026-08-20 15:11  478e836  james — fix: 加深非工作日背景绿色
2026-08-20 15:15  920a5d8  james — fix: 同时设置cell和contentView背景色
2026-08-20 15:51  131fa7d  james — fix: 周列表非工作日背景色改为清爽绿色
2026-08-20 16:00  e4d1961  james — fix: 周末标签改为绿色主题
2026-08-20 22:37  f152445  james — fix: 统一工作时长字符串颜色与打卡区一致
2026-08-21 09:35  3432764  james — fix: 过往视图年度统计使用颜色区分工作时长和加班时长
2026-08-21 11:40  1c19d53  james — fix: 过往视图月度/年度汇总使用颜色区分工作时长和加班时长
2026-08-21 11:55  6803838  james — fix: 详情视图（月度/周汇总）使用颜色区分工作时长和加班时长
2026-08-21 12:03  c6db2f8  james — fix: 蓝底头部使用高对比度亮色显示工作时长和加班时长
2026-08-22 15:22  6be376f  james — fix: 每日打卡视图的类型标签颜色与打卡视图保持一致
2026-08-22 16:57  f2afd40  james — fix: 所有日期cell背景统一白色，通过类型标签区分
2026-08-22 17:44  544ba8c  james — fix: 修复蜜蜂位置约束错误
2026-08-22 17:47  6556468  james — fix: 增加周月汇总视图工作时长字符串宽度
2026-08-22 20:30  374661d  james — fix: 跨天打卡处理问题全面优化
2026-08-22 21:28  063bf70  james — fix: 优化首次启动配置引导和验证
2026-08-31 09:41  bb44248  james — feat: 悬空打卡记录（缺下班卡）分时段处理与高亮标识
2026-08-31 09:41  d68153f  james — chore: App Store 发布准备——更名蜜蜂打卡、隐私合规、版本号1.0.0
2026-08-31 15:22  70a5a68  james — fix: 定位权限改为按需请求 + 锁定浅色模式
2026-08-31 15:29  4d62516  james — perf: 节假日查询增加两级缓存，消除主线程重复网络阻塞
2026-08-31 15:53  bec13d5  james — chore: App Store 截图自动化与素材（6.9英寸 1320×2868）
2026-09-01 11:47  aed0239  james — feat: 蜜蜂飞行条幅——打卡时随蜜蜂运动显示祝福文本
2026-09-05 21:51  b8c6571  james — feat: 小蜜蜂主题通知体系——自动打卡提醒覆盖Apple Watch
2026-09-05 22:47  27edd67  james — feat: 首启蜜蜂欢迎页 + 完成设置奖励动画（方案A+C）
2026-09-09 22:27  b30eb3c  james — fix: 清除桌面图标常驻红圈角标
2026-09-12 14:24  f1652ec  james — feat: 切前台时段过渡图——按考勤时间显示screenpicture时段图片
2026-09-12 14:58  375c6ce  james — fix: LaunchScreen老照片替换为蜜蜂图标——启动画面与时段过渡图职责分离
2026-09-12 15:22  c686157  james — fix: LaunchScreen启动图采用散文件模式（LaunchBee catalog引用不渲染）
2026-09-12 17:35  3bf4ac3  james — fix: LaunchScreen简化为纯背景色——图像展示职责归Onboarding演示页
2026-09-12 21:04  94b4880  james — fix: 时段过渡图启动显示——scene选择放宽+didFinishLaunching立即触发
2026-09-12 21:15  a654022  james — feat: 启动首帧即显示时段图——彻底消灭启动白屏
2026-09-12 21:30  7bd3c24  james — feat: 深夜时段过渡图替换为夜晚湖面图（FrontNight）
2026-09-12 21:40  ad7cd27  james — revert: 深夜时段图恢复为 moonhill2（撤下夜晚湖面图）
2026-09-12 22:13  32dd1b3  james — fix: 图标说明对齐实际图标 + 每日行移除实物型图标
2026-09-12 22:50  0c3e4ec  james — fix: 修复详情页闪退——DayTVCell残留nil锚点约束
2026-09-13 18:56  2d2c60c  james — feat: 图标说明弹窗改为真实图标可视化展示
2026-09-13 19:23  1548810  james — refactor: 图标说明视图抽取为公共方法——过往视图与月明细共用
2026-09-13 19:43  fd24037  james — fix: 修复月明细帮助按钮闪退——action指向已被改名的旧selector
2026-09-13 21:03  04818e8  james — fix: 编辑页周六加班计算对齐 + 未保存保护 + 类型标签去emoji
2026-09-13 21:30  4ea1cfc  james — fix: 补齐编辑页下滑关闭保护——modalInPresentation禁下滑+尝试关闭转保护弹窗
2026-09-13 21:48  098fbee  james — feat: 编辑页时间控件改紧凑样式 + 连接下滑保护delegate
2026-09-13 22:32  3a36603  james — test: 编辑页UITest全流程验证通过——紧凑样式/月明细去图标/下滑保护
2026-09-14 09:53  552c587  james — fix: 编辑页时间卡片高度250→100——适配紧凑时间控件
2026-09-14 12:44  670ac8e  james — fix: 关闭按钮改用closeSelf统一关闭方式（模态dismiss/pop自动判断）
2026-09-14 14:41  cb7d2be  james — feat: 通知权限测试开关（-skip_notif_perm）——自动化测试不再被权限弹窗阻断
2026-09-14 18:04  b9e4494  james — feat: 周月汇总区支持点击本周/本月行进入详情——详情按钮改为隐藏
2026-09-14 21:18  72822a2  james — feat: 未捕获异常处理器——崩溃时自动记录name/reason/调用栈
2026-09-14 21:45  ed3a11e  james — fix: 底部关闭按钮action改名bottomCloseAction——绕开方法注册异常
2026-09-14 22:07  0a40b57  james — fix: 底部关闭按钮selector补冒号——unrecognized selector的真正根因
2026-09-14 22:18  0d681f0  james — fix: 奖励动画后蜜蜂归位 + 编辑页高度修正 + 时段图平滑过渡
2026-09-15 09:06  c4de27a  james — fix: 补editDayTimeVC场景storyboardIdentifier——修复点击行闪退
2026-09-15 09:38  66379cf  james — feat: 保存打卡位置后智能引导启用围栏（补齐设置后围栏立即生效链路）
2026-09-15 09:55  40c482e  james — feat: 围栏属性调整后立即执行围栏内匹配检查——自动打卡即时生效
2026-09-15 10:21  d15ad15  james — fix: 补hasCheckedInToday实现——修复围栏检查闪退
2026-09-15 14:10  583a306  james — chore: 清理BeeAnimationView.h两个无实现死声明（flyBee系列）
2026-09-15 17:19  51a181c  james — fix: 主界面汇总区布局适配——高度62→130、底部间距60→14
2026-09-15 18:00  0c266c2  james — fix: 时段图节流防双触发 + 打卡区大时钟小屏适配
2026-09-16 09:01  0cdff42  james — feat: 时段图补淡入过渡——完整的淡入→停留→放大淡出链路
2026-09-16 21:40  a6847a8  james — feat: 组件自适应改造第一批——卡片最小高度+动态字体
2026-09-17 09:32  53b50b2  james — feat: DayTVCell七label接入自适应字体（Tool.adaptiveFontWithSize）
2026-09-18 10:19  8894444  james — feat: 月明细页防误拉空白+底部关闭按钮，设置页共用图标说明
2026-09-18 10:19  7d46f55  james — feat: 主界面汇总区布局适配——卡片间距20、表头字体12接入自适应
2026-09-18 10:58  7df37db  james — feat: 月明细页面板高度自适应内容——custom detent 消除下方空白
2026-09-20 08:46  ebf2994  james — feat: 首启分步向导——欢迎轮播+三步设置替代单页首启
2026-09-20 08:47  db0d361  james — fix: CurMonthSumVC 刷新回主线程，修复后台保存触发布局崩溃
2026-09-20 08:47  9d6deef  james — fix: 首启向导进行中跳过时段过渡图
2026-09-20 08:47  06b6441  james — fix: 蜂窝动画飞行条幅钳制在蜂巢上沿之上
2026-09-20 11:26  194c7b8  james — fix: 首启向导步骤页类别标题与副标题居中显示
2026-09-20 11:26  b37c187  james — fix: 缺卡记录显示造假——列表假工时、编辑页假17:45下班卡
2026-09-20 14:37  339f212  james — chore: 版本号升至 1.1.0（build 2）
2026-09-20 14:37  f1b8e8e  james — docs: App Store材料更新至1.1.0——重截5张截图、新增版本更新说明与向导审核备注
2026-09-20 22:17  6659027  james — fix: 体检P0/P1修复——通知深链补卡、缺卡显示造假链、地址搜索命中外地、键盘遮挡
2026-09-20 22:18  fc5f6cc  james — chore: 清理死代码与无用资源
2026-09-20 22:18  4a74538  james — docs: 审核备注节假日数据来源改为 timor.tech
2026-09-21 08:56  dc3097b  james — fix: LocationSetVC 底部重排为双卡——位置信息卡+保存卡
2026-09-21 08:56  fc34f0b  james — fix: 时段过渡图只在主界面正在显示时播放
2026-09-21 21:25  25b9463  james — feat: 设置页新增工休日历——月历查看/强制刷新/哨兵校验/失败红点
2026-09-21 21:25  e13c8aa  james — fix: 时段过渡图统一显示比例 + 白天图换双图轮转
2026-09-21 21:25  33e5ca3  james — docs: AppStore 材料同步更新——隐私政策数据源纠正+语种切换
2026-09-22 11:11  7863463  james — feat: 加班时长全口径统一——打卡区/记录表/周月汇总同源计算
2026-09-22 11:11  0808df4  james — fix: 周月汇总区底部死空白——容器高度与内容精确吻合
2026-09-22 11:11  b997cd9  james — feat: 时段过渡图统一悬浮卡片化——圆角+投影+呼吸边
2026-09-22 11:11  35d0eb0  james — chore: Release 配置静音 NSLog——新增 PrefixHeader.pch
2026-09-22 11:11  ad2ae0d  james — docs: App Store 主截图更新为上班中状态
2026-09-22 16:45  fc5ff2d  james — fix: 设置页cell复用手势串扰与围栏清零存nil——回归测试揪出的两个遗留bug
2026-09-22 16:46  0a2c6fb  james — chore: 编译警告清零——89个唯一警告降至7个storyboard/IB提示
2026-09-23 14:59  db5999f  james — feat: 国际化节假日映射层（Nager.Date）——海外自动选区、1请求/年
2026-09-23 15:57  330813f  james — fix: 月详情面板跳变与 push 关闭失效修复——残余未用变量警告清零
2026-09-23 16:47  67d313c  james — feat: UI 多语种（中/英）——中文原文作 key 的轻量本地化层
2026-09-23 17:11  ddb3198  james — feat: 白天时段图换无文字新图——郁金香/蓝天白云
2026-09-23 17:17  d1c7101  james — feat: 打卡按钮图标文字换英文——上班卡/下班卡 → Check In/Check Out
2026-09-23 17:31  ee66a31  james — fix: 打卡按钮图标按语言路由——中文恢复上班卡/下班卡，其他语言 Check In/Out
2026-09-23 17:48  5a48787  james — fix: btn_work_on_active Contents.json 被 Xcode 回写旧 lproj 状态致警告
2026-09-23 17:49  3bdd9ef  james — chore: 撤销 Xcode 自动加的 beefly2l/r 空 2x/3x 槽位噪音
2026-09-23 17:50  76e6bd1  james — chore: 移除被跟踪的 .DS_Store（Finder 噪音，.gitignore 已有规则）
2026-09-23 22:12  947d4a7  james — fix: UI多语种v2——storyboard静态文案本地化+英文排版4处bug修复
2026-09-24 21:59  0148a24  james — fix: 围栏幽灵事件连环误打卡——进出事件GPS实测复核+下班防抖
2026-09-25 16:52  2c24674  james — fix: 蜜蜂首帧闪烁两处——布局函数不再动蜜蜂约束+飞行动画弃用启动快照
2026-09-25 20:31  531cacf  james — feat: 设置页新增隐私政策入口——github.io主源4s超时自动切阿里云备源
2026-09-25 21:28  29949f5  james — chore: App Store 元数据联系邮箱换为 jameshys@outlook.com
2026-09-27 21:08  3ab5d71  james — fix: 悬空记录弹窗时序与补卡落库修复
2026-09-27 21:36  c4cde82  james — feat: 商业模式落地——免费下载+7天全功能试用+¥12一次性买断
2026-09-29 09:40  8e70c03  james — feat: 主界面围栏状态胶囊——切前台实时刷新+定位健壮性
2026-09-29 11:29  14b7ae5  james — fix: 提醒胶囊落点改道设置页开关行+试用胶囊移到按钮行中间改淡绿配色
2026-10-02 21:42  f30e9c5  james — fix: 假日胶囊首启缺位——打卡后补渲染+每分钟零阻塞补查
2026-10-03 19:24  e05ddd6  james — fix: 欢迎页「到点自动打卡」改「到达自动打卡」消歧义
2026-10-03 19:26  078625e  james — fix: 欢迎页标题改「到达离开自动打卡」补齐离开方向
2026-10-03 20:19  93067bd  james — fix: 商品加载通知切主线程发——修TestFlight后台线程碰AutoLayout崩溃
2026-10-03 20:31  8598229  james — fix: 商品请求失败自动重试+进购买页兜底重拉——修首装购买页必失败
2026-10-05 19:59  2fbdb99  james — fix: 向导期自动打卡延后到向导完成+保存位置requestLocation崩溃@try兜底+build8批次(部署目标15.0/向导返回键改完成钮/付费墙文案与素材遗留/ASC材料)
2026-10-05 20:08  da91b0e  james — fix: 测试钩子包#ifdef DEBUG——Release二进制9处钩子签名清零(2.3.1隐藏功能风险清理)
2026-10-09 16:33  f4cff20  james — fix: 10-8真机三修复+10-9围栏漂移防乒乓——向导复用页底部完成钮/恢复购买错误文案/立即启用后segment补刷/自动下班连续二次确认+入口10分钟防抖

---

## Continuity note (added October 10, 2026)

The historical branches above were originally preserved separately. On
October 10, 2026 they were joined, merge-only, into one continuous branch
(master) in the private repository "worktime": the 2019 prototype
(Phase 1), the 2020 continued prototype (Phase 1.5, branch "syncday"),
and the current app line (Phase 2) are now a single lineage in which the
earliest commits appear as direct ancestors of the latest ones.

The join used `git merge -s ours --allow-unrelated-histories` twice: it
only creates two merge commits that point at the existing histories. No
commit was rewritten, rebased, or re-dated; every historical SHA, author,
date, and message is unchanged, and the resulting tree is identical to
the current app's tree. The full graph (375 commits: 373 unique + 2
merge commits) can be verified with `git log --graph` in the private
repository.
