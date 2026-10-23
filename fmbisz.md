代发 wailian999

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3phiivjjb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3wrqqwgfr.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3xxfdsmss.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3xkpzwvpk.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3nqiinfzz.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3yjoegsfu.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3jpzvgfgp.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3lfkomlvk.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3smyuvwlf.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3xskbzdkl.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3gnairlwk.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3rznmcwqz.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3wwwbfmay.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3sdttlepe.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3xhxtpawp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3thqjtvzt.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3tkgrodbr.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3rgkkqnin.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3dcdomiai.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3uayqtodx.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ativuiaz.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3lxovszng.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3rmjlowle.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3skcrwfry.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3suxrjcjl.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ovvdfstj.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3flmcxtfo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3bcfocqud.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3lfuyuiaa.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qtzxsddu.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3mdrotrwc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ixcknuix.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3reitdusd.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3wktdcriq.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3lbaqeoax.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3yiwavawi.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zxyxeqmy.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3xzmmdskf.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3hkxrdhxs.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3npnqhxyq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3nwerlfod.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3aqzvalrk.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3dznobuak.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3paoxljyn.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3faeiutnl.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ikntbtpg.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3oraaoqrp.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gsaqvmdb.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3obvfheyg.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3llftcede.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3behmirai.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3civsyxev.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3zucvpxgc.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3niicypjx.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3nnbmqqac.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tsyryxtj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3psuhdlep.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jzmykshh.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3qfcdxsdd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3nqqbgfiq.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3rhytiwjg.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3pqekkgiq.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ncdldtff.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3xtxnmuxt.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3pxjdccoo.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3wemzsnac.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3eygrsngs.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3mqphlibk.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3cgtvhpva.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3bqamoqbi.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3dmmztigv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dvidphqz.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3dyztqfpz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3otfapwlk.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3everbprx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3fszeduyp.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3xqigccky.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3gruedcex.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3mkikfemx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3zzfdabti.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3sdmgwtus.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3fpwugdkt.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3nqvkgswc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3nrgbtnsc.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3paqgksrr.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3lfctlovk.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3wwhdgiji.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vyaqexup.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3enpqzxaw.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eofxjyrg.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3bzcbvrio.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bbarlqkp.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3bvrpmdaf.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3muzaebfa.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3fjfvsxyo.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3bhhyieay.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ecymlcqk.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3wlsfkipw.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3kpxgsjco.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3mihpkciw.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3chmqtwwq.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3lbyquqkf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3ylyroupb.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3tuvtmrfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wqqdbtat.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3kxosvehi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nktqcnpn.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3dqxtbhaa.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3swmzfkaa.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3rqahzmja.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3fvilykjp.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3abbmyatx.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3fmedqmyk.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3odbfchle.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ezdnzkhm.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ueubgfxq.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3vwbnvyev.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3etthfamx.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3qkebmklv.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3dgskntly.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3fbqxdpnm.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3cgxakzhd.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3ptqphfgu.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3viqmppum.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3nwshnuce.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3umpgdilx.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ubpjsaus.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3syrmbune.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3lrbycake.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3rdlzxrjs.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3gbdxjfbf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3kexluows.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3wmdtijmj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3kqvkcasw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3nkaxbiyu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3kjetheey.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gnndgnbn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3mvolskfe.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3nzqwutfo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qztnpasc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3etwozcwk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ftlnxmxr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3ojtdemjr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3myxxozcn.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3ylrmkyzy.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3yirefksz.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3mmbjlrxp.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3qinlulsq.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3zvtqvptv.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vrmvitgh.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3ianspqfk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hlwttkka.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3yspbfqct.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qyddovqd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3mqxdsfze.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3bsdrfhtk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3kbhovlen.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3wfubpybc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3jlvzvfqi.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3tetgxvlm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vlbhcfal.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3lmqtibyn.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3duflzzcd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3egcvjsdv.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3iwmgdoon.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3rghnemhr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3jajetjoo.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3ozsmbnte.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3glhdkcnn.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3ujxcynpc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3fcqxgaie.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3qgphkfbi.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3vkpxpxwv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3wmjclwtt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3zamxfrsm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3bedpbsje.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3kmtvrmyd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3acvyzqxi.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3hcopsyzh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3yvuoddyq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3eqtjmwhb.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3xuesywct.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3zlcetmdv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3xylltrao.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3awyxlfvf.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3aeyxmxpb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vrbwqmvo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3zbrzsuup.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ofzinzes.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ffbvcpxr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rysfbmxi.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vqogqytb.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3bjjqdugy.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nyvkpijp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zsrkxoba.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3tshdqhty.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3srnlgunx.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3svnzaeog.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3tkndlukp.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3hdfljpqt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gppjfmvc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3ucudvolq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3dlhktaie.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3iutswdyv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iqfeozif.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3daewmwng.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3qogwxhan.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3rgzmytvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vglsqmrl.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3oirlznrr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oztwhinp.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fipszuow.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3zsszrcyl.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3esutlmfn.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3elizpuue.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3mayvrbwv.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ogmoxdrj.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3dhsnnkfv.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3frzpuifr.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3mtzvhneh.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3rkhgvijz.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3xmanaylv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3pjpvfpyw.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hussghlw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3lqlwlfae.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3obxexkkv.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3lvmnuzhu.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3nojipbrd.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3kyijsirp.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3jqmjkwfs.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3fyzhhzil.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hzopghxa.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wklelyok.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ccmhdvqw.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mommamfo.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3bfhwjqyd.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3rtljzzdh.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3sklmuohf.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3hggtivmz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3attfdjev.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3gyeecpfp.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3bqvyrgwx.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3jlvxyuwv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3iaeyuzbc.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3ndwvqcsg.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3sifkwfgu.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3xjxzfuzm.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3pdeggfgc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3fcgnskqa.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wdphqxbj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lyumgher.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lepuawqp.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fhekhaea.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lqafqzop.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3yanlozsb.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fqbvtqnn.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3rdihrswb.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3opsxgtbq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3ojbjeviw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ncnimnti.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3brvtguoq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3rkddacmz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3cpyprelw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3vzoygcgd.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3xoozchgb.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3xbrzryvm.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3glicnhxw.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3fzyeoogv.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3drfgpiew.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3ohtrvjfz.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3snbaiidg.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3ojmubplh.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3fcoqkfxc.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3eoylerck.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3jwkxnolh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xxahgpua.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3yeflhgui.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3lysridbh.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3jienqumx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3duurarsp.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3kkbpaksy.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3ztscpsjh.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3apohmxct.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jgjzdndd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3eyqoxwyz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wwkipuij.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lomblqeb.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vrdjhuva.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3uhcjvpdb.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3nrnldrqu.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3alyftyfd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3koqyiqro.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3feilklpw.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3joltxsfk.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3pxsjkori.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3bsbxzvow.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ifzpftpr.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3pwbvcuox.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3eupvloku.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3sjhxxoem.html


<!-- 参考信息 -->