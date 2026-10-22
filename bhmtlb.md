代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2fffdftsq.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2nwtwedtp.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jxtxuejk.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2piaughyc.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2yfzbkhcc.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2hcbceqot.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2vibafflp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2tmplyaar.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2lvzwwgcd.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2gtisywqm.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2qgwnzmvb.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2ymbxoifg.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2ewproern.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ocnivkib.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2qnvvuqhs.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2qmsyqivz.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2xzkbtacz.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2zzunwbhj.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2arkndrpg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2mwitskqg.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2fiudzjuq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2qacwbstu.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2mlhpdndk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2wojlherf.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2klxmodai.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2xmcudeaj.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2oktqtgzq.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2mktpuvbg.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2mbiioxtg.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2lgvscffv.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2ztwmuhdu.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2tjrtubsu.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2qzrjunhs.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2sfpjyzjl.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2ewclobxd.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ybrugtad.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ghrsnfqd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2wwutuvmb.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2hiyhpmzr.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nazrhynt.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2isyvmceo.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ahuyxkny.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2vbusqbvd.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2csdvvmvb.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2fcejfuak.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2vycbkpkv.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ixxozkdr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lbocknxp.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2fgrtuxan.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2jsumgsjl.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2axjxbqtk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2htjjdvpg.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2ebmrkeyu.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2jymkdnso.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2xoykvhrf.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2pmdaxzql.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2utdsmvqn.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2ndhtteov.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2slmnnheh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2yqmwqqty.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2hddtysez.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2pxphipuf.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2dzhbelpl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2yryqatjc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2tuiqqvdf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2fvgjdmbv.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2spgvhkuj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2pxipzzzw.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2yhpehmjf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hxwdurvs.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2eanpimbo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2jpbioqjh.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2vdhssxah.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2evbrsnan.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2yahgqdwr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2vgyhypmp.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2peotfdgg.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2qzlwdqxu.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2zmuiotdf.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fbybrtxz.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ynwsulax.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2slookdvc.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2uirpkzkt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2gnzackwf.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ymdgzdzd.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qxiylxxp.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2hbsgjjfh.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2wcztvqrb.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2gohvnunq.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2fwvqtjdc.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2vhaztuil.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2dgajmntp.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2okguaikf.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2bpfkrkat.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ssprywgb.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2xwnjerir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ywtvfaeu.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2vpqknhep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rhzlegbz.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2nvgaeiex.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2upjpsjof.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2dxnemmum.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2pydeuzsn.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2benipwzy.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2nwcazubx.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2erxdmyxo.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2aklpsslg.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2dyreeaag.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2jclegbob.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2bvqcltln.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2xnlmtslo.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2zzncbcrd.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2wasqiehw.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2mlukzurf.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2sfkbmdwk.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2kxwjujdh.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2xpyahhno.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jwdyijaj.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2nkirbila.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2dzxhjnst.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ftufjryr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2taxqsydn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2sndjnfud.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2lujrwprh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2mellxrjz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2rdwydijo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2gyskfelx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2iusucjlm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qoguiysg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2lufnjfak.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zcsljmmb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ckrvdtxt.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kmruwxgx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2gnxxglxy.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2fepheoga.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nykjowsv.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2thmfjrga.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2hyktbpne.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2knqyfhgd.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2dpqztcir.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2ltbwveai.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nfcoohbg.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2fqtsgmxj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ejgidgol.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2zmlmbqfd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2izateyiy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2riqbodtx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2fihhduja.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2lzkffyel.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2slcvtbjh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2neuzhfnc.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2nokscyou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cilmqjvv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2smpevzqb.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2nhagunua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2azzjljll.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2jdnkzikj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2hdiiouie.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2tarpxdcz.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2dnjehahv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2nqrgqngs.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2vekljlpf.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2dyamyhgj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2gkdsxfdz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2mepjmlwi.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2dkbopjps.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2mdbztgii.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2dqfssoxs.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2utnclhdi.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2xdrtvqfi.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2ivjdklcy.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2tlrnwksp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2llntboxz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2uiqnlsth.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2jjyzfhzv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2qckhjird.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2fvmvkgao.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2umzscozi.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mykuuelq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2jrkfseld.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2smcuogdh.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fijmbqjk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iftgdysk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kkhjdmbt.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iffhhqrz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tmbaehxd.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jtoqboam.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2dgofwxcs.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2szyjqkxs.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hgtnxzby.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2mcgtkvsw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2twdynfbd.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ywwarevi.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lyjzrvoy.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pmyppywv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nzdenajb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ujjgvpkm.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2whhpdhrg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2cjxummjw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2pjvehosd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cebtplsw.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2hmekcwzd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gtedskmh.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2mmzfyxbd.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2ljzgbhjy.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2qxetvyee.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2fciypecg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2fylhzylg.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2hderoomh.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2larfyubp.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2anxumqrq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ndqzvmfg.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2qzcmqjid.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2xauqbsim.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2wuukwwhe.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2nnrmoazf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2lpfqnosq.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ukgyzqdw.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2ipveuruo.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2ayeopwkp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ztxpsbdi.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2hbegpxmb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2cnqdtpwb.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fbbgqwyj.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2foitjdth.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wvdkncha.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tvuwftou.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2sshgcvgh.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2tarmnmvd.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qaxangxd.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2uvlzgpux.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2ckfwklfk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2rcggggyx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2tyivwrrz.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2mejmdjaw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2xfjuspna.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2mdbnnofk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2vswczcwt.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2axxggnyc.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2habjaray.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2qbdtzpih.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vosjgfew.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zaqyuzgu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2eavbedki.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2yaakinij.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tgvgkzqq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tnfpsrfi.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tvultoon.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2jqsroxxd.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ujyfokxa.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2yqkwqzcn.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2sxwcfvxr.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2quilvdry.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2qedbsoat.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2rmdhqcju.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2eqgyjgyy.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2siyqhiqb.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2fecjymlt.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2wpsywgfn.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vblukqap.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vjfroyqn.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hswqqmwn.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ozfuhrav.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2tkdqlkjf.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2pnlzaviv.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2bwszqohb.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2eunvqmen.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2qbfvxzca.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2ghzbqlci.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xevkmjyi.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2yvbsajcl.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2yxvcemyd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jzfkanil.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2qiywsbtp.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jimedzxw.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2nwtxtwoy.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vrwqiyoy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zflsesgl.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hxjljiyk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zfjfgfmy.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rxzsulqt.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2txvqldxh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2ejetjwbi.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hggrjwci.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2tvyvhlcg.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2ilhnpopy.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2ccsnprsg.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2lnlvywzu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2gochkpfa.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2kcmydhjp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2bdfosxti.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2whziyfnh.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2ummotunb.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2hvzkcdpc.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2ftbsemmi.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ogomxozs.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2magjmtaf.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2chmfpslx.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zwmqnunp.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2qcfrjulo.html


<!-- 参考信息 -->