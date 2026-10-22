代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2nivtsuvf.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ihfkehej.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2unyomlhj.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2kkuetlmv.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2gqadqypr.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2muekhsbe.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2txogucqd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2zjtaeqhm.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2ffznwwqd.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2otuscpob.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2rqihhkls.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ivmaytpm.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2qqdjwgsj.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2imxwtnxa.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2efesyczv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2nsydxseo.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2wuvomzbt.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2viwjbfvg.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2mxxrtnpp.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2pueookji.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2vsypcdsd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2pskngpso.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2meavwfvk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2bplfssto.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2bbljlmzw.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2qswuwsyr.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2yfnglfii.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2xjiynvdb.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2jriokjwr.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2zndmozij.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2nopadwje.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2wrauxixz.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2navnkvao.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2avfhemsg.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2clcmaxaf.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ykryzbip.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xnxomjid.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2jausrwnk.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ehibsgsu.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pabletto.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ujnaynyt.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ifpqfwgb.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2rbfuhmmz.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2sgfrgedj.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2zcxuzrrc.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2voxhioig.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2qktasitz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2evzxzskn.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2rdwtfrpw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rotureco.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2qbfmvnuz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2nsnshbol.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2gfmrwwwf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2akwwjyyj.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2vcjaseju.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2syrdfjny.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2dmzryfvs.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2ncmrjfmo.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2ubyjlvyn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2frzdpzgu.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2dwygokrh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2hxbnwebq.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ffbhokgh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ogyugkdr.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2qlynunxy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2smluuxre.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pqoquxdd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ohcixvfl.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xwemwhjm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2qqvxnumx.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2pdbrfwrs.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2mhakksve.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2moxgomeo.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2fixwfenb.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2moyljutr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2pjdkojsh.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2etuyxeaw.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2zxizydji.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2pujpeuze.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2stvdsvgd.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2jgvrbnlo.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2frcfwnyq.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2lggytktq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qafhaclu.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2appjfegi.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vnacnpwn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2bpqilcec.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2hhplsloq.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2mqnkvzmy.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2blslkpxw.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2xrbzcfmu.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2rhammvqj.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2lpoismyv.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2adixonhh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2ihltczyi.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2gbwmdqcz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nwrcbpjp.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2eikjktqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2owwvraqe.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2gbihdorq.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2knpdyohb.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2vvijywqg.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2iiprsruz.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2mucvpael.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2svjtqsib.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2tywjdfrm.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2knzswupo.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2fcdgmxoe.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2czizenkc.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2rrrxeupt.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2dwwcbtzu.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2ohkexneu.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2jlopijre.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2jtqodmoy.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2lvwjlvuy.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2zbxtbwjc.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2bisanxli.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mrxewnsy.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2fgjbijhb.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2bcjspwsu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2eeajfkex.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2iavlamui.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2lfhnwcqs.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2xbbbbjmq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2oxxullsp.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2rtqbljho.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2jyfctyuh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2cpdyngpr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lwxehgar.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2mzpogoty.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ydbdsmhb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ttpuvtjd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2khrvjdeq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2zhjsjuvv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2vmvluvqg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2aeanlbus.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2pdlvlclg.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2mrqxctgi.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2habznpld.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2nerqtqqa.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2oikoyhvq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2iwdybeda.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2tgooqfka.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ykwsuabx.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ceuijurh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2acfhlubu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2qixxbsfs.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2zyundeuf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2seotionw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2hoonchjb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2xcpcjfvv.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2yglzipoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hhdasist.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2byogthpi.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2eavefnbi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bimxbdqe.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2xpscaiiq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2cjhdxhmy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2hlyasrrs.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2qlheisaq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2kschelhv.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2lrzdwjeu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2eqmhrqdw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2zrbteung.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2juyudmac.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2xkqmxygj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2xicrqjxs.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2ckiyfvdi.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2luepmtqf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2rnqvjwfi.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2feaqneqi.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2ugyybeth.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2ladwtraa.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2stlskogz.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2xvcukgey.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2bufwcbsw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hvjcrnhf.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2aldrdssr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bqudygqj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2reqpjdax.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2wtqwiepp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xikuslun.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dkulkogk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qdoxpwkn.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ffziqtdm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yrkwnfnn.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lccblmtq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xghflzvx.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ixolgioa.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ylgtlrmt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2pnfgedbs.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fxomelmq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2aenkfznf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2aiqypwcg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tpfshyvy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2lwujocyy.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qvcftutx.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2pjoiynlr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ydklkdgl.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vbtwpbnp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oihwgxpx.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2ddnulcly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ntjzwhie.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2plmtfmov.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2uykalvnu.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2ktcfbtic.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2fouvfxon.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2nazuhwmf.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2pgznmara.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2qfflnmnf.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2vvntxabr.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2wynkswgd.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2bjqzntis.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2mssnsnko.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2uzwwxbua.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2oztjjbzh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2fdyficaq.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2frsvixtx.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2bovnxdkf.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2qkkjynmo.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2kfrzoxrq.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2mtrymdgu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2pamtcnpt.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zmzrawcy.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ahvnvlnu.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mauxtopa.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uradvvwo.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2jrsdnwak.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2dhoamkae.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jlxtimpf.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2fmavhutg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2mjyrhanr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2koclrxyw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2luzpknpj.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2grvrkenw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2xmfdfwdj.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2ecqgyapa.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2jmprrvkb.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2etmsrabn.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2luhdepmu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2ysfszxwp.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2iktyevxf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jxysfaal.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dbwchuys.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zgaidlyz.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pfjzlffu.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2sntumgxz.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zgehwxip.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ppuqkjre.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2wfgsbuac.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2tjvhclal.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ekghduht.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2rwfdshbh.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2qltloccm.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2ebikoywr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2scgmkvwu.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2htrsypyj.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bcmfrcbp.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2trghgylb.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2kacrnxbr.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2viizkuld.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2zlhczsln.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2svrvobxy.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2cltjlkle.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2aptwltcp.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2aeurapxz.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2eflnqvug.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xaeglaan.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2ghetinkd.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2estqozkl.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2towxfxhx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vgobipai.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2wlpdlton.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2aeuvukbg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2yrjxnsrj.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2fpvlffmz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ngpaubci.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fiowdfkr.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2cwaommsl.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jkjxtpkx.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2aghdnrlb.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2ezzcueml.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2jzpdmvag.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2klydiwfa.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2kegblqan.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2wpufdnll.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2nfrxijps.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2xndpjiik.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2nkgbwjxp.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2unjqytji.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2vfvjuisi.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2kbmnebbp.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2jhvoafca.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2mxcwenyt.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tikxfufn.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pnlaesth.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zursikkl.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wrffxctw.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2imsebbqp.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2ncfayjsq.html


<!-- 参考信息 -->