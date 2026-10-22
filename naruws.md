代发 wailian999

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2khekpdgt.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rckxvxek.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2yaznhgdh.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ooccexxf.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2dmcdtfrm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ffuicwxg.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gowyrgaq.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2omlqmryf.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2lctwxfui.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2kqotesyt.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2kzzpipkf.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2igzrnfim.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2iiikfcvo.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2kqhvfywb.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2traarmmd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2rxbjrvfh.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2kocukbnm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ppvhyjds.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2jgjtnrzn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ansqetdg.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2sleommiw.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2qdrqadpv.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2epquesfy.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2oyfuuttq.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2kedymojd.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2jvotdezx.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2pxrbqkwx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2xocijlms.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2nggsjqng.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2vlrivrgf.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2yqqzrliu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xokusnsk.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2tqlgumyc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2rhfaroal.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2rbyqgzaj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2zwiolywc.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ewpdsmtn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2yrcpgpqi.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2zpmghbkb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ybgjjnwn.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2yemxybmg.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2mramydkj.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2bzrebjia.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2erypdaqn.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2qivvlaru.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2hezdprte.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2zcckcrqm.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2azvzhupz.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2hqyawtgv.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zyllfpwf.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2kytkpmhs.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2froufjie.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2pnypudwn.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zuggfaao.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2uwdexcub.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2svyppjpw.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2eaprmxaf.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2jfqbhpbm.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2xvgpgxzx.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2igljnzrs.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2nhxzztwa.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2ytdxweqj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2nthcckgs.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2fxgvvyry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rgninull.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2gfvjfbnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2irhmbbcu.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2axqtpvgx.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2zyuocvmu.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2uhqpcerz.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2eszjgivc.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gxificml.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2bcfzipxw.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ckpmybou.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2nyzruzxk.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2iogneqgc.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2lqbtjlir.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2kwbcewce.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2tfyehcjg.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2mybofmge.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2pxvobpms.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2nqpojrme.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2fxduajnw.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2vnrowznu.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2kzofdujz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rasrqtqn.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2lxsjypnp.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2qlxwwhwb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2guzwlxem.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2hwonkosy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2sukqjsde.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2uevvwaou.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2mqkbgkgp.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2vwoyudjx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2flozlaur.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2zkdvvpdo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qqkytiwd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2cnhyrojq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mswmaigz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ciurjqay.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ddxyiawd.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2krcqzvgu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2nsjurcna.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2egwayfya.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2msorrjxf.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2zgofjtyd.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2cyheudou.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2typrruea.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2qmlqcaol.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tfiufyuz.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2syezoyrn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vbczmjco.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2rdufwckx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hmlrjstu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2jlriiakf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2zhihmrer.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2yjnjjvpy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2dijqzxda.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2ltlqhlcp.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2uysortsl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ayskdftc.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2hrpstqdc.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2olzcpitk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dbiqnbyq.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2gnnyywbe.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2boxwlacu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2tpsgqjrw.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2hopglbrg.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2rbqklmaq.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2kevxghmc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2kikkghex.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2cuqvuhka.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2yigkwkty.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2upmzzpeg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2otufidjc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2ggpsirzm.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2fovivalh.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2vjpdxoop.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2zlxbiaqd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2vctzhcym.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2dlvkirxl.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2mlgskdxl.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2difawvou.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2hosuhkbg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ljrwbzmg.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2ekacpkrq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rfpbnmuv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2shgzifuu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2fdihngbh.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2vbgwhkvs.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iqphtlml.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2pnuosyvn.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zazuxkek.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yyfdtrum.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mxyzfgdd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kdzlacle.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qttmkmrc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2zowkgppy.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ylpmhnwb.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jthumjzl.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2gegqzkue.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eceydrtl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ykfmsfqt.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2jeoqoxsy.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2iubbueux.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2ucxyecpk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2vnvqcwpd.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2jluejcjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2udnaqxov.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2gudnwmla.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nafybqbu.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bwhwckoz.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ernacoaa.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2uxruougi.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2umjbelnp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2reliaobp.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2patsuejo.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2gxuyzegh.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2mulzprji.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ocderojo.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2vzhktgtv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2whddweiz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vghwngmj.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ryfdshvq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ztdxlmqm.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2qmvvbsvw.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2ykrvxpva.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2spirsenu.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xddjgeaw.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2wjwoogdk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2juhreqpe.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cffzoves.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fwxrattl.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2migcaebc.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cxrtriqv.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2cbocotxl.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2jipuhnfx.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vhjifoht.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2muhjzvaa.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2sglibkjj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2fzpdfggw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2roemgwey.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2ajhycdun.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2nkbadxhd.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2himrzbvk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2aawxsocj.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2ebwzchni.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2pmgzfvpb.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2zpflnvqp.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2sdecvcax.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bzvhxlec.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bzbqqwki.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2uupxoyki.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rqqbpjyt.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2txbafxqg.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2yudalxjn.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2buuhhngr.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ngffucvu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ejbvrcwj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2amuwydqj.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2aghilpkk.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2wqripukx.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2onzkwwdh.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2xatlebki.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2geznonns.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2wjgpblbm.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2piajrjjy.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2kirvpdkb.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ofycpdvd.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xkurmxow.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tbjouzyq.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fimlytie.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2bxkkrvgi.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2szsaokbw.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2lcuibkfx.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2dhqnwuwz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2siaqngro.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dniskfbr.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2nizcmgji.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2suodsrao.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2decuwlmc.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2nisrazgl.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pksmixeq.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2rfrlixht.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vhsdrvec.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fkchiixq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fsuwquym.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ehfmlbra.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lgpmbouy.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2fmbgamjz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2eodszwkm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2joqgnskf.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2dstfnbqt.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2zwbpdphu.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2cmvdeebn.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2coadhvge.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2fwzprwnl.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2gqpzendi.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2fjujotnu.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2kqkslaei.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2qnmfzqtd.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2crqycnun.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bbcuglkg.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fdxbviab.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vtlswmwl.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qcjujnbq.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2slddmegp.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2oikbafuq.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qhblpqjr.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hrtpqapz.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2kmxijagi.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2xowidjtx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2sdzkdfex.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2lwofsbui.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2bdboymak.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2srwrbwwf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2quanwsxs.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ensrkwom.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2burnkzbk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2wrcogsip.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hjybjifh.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2anccsgnn.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2scehmsrj.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gqoxhwex.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2iiqprlrw.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2swdmczpm.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yogmntsh.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qpthqfgz.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2wpjtwhom.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2owvgzzym.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tcpagewf.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fhvljtmi.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fwcrymlx.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2gvgyvvxx.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xpwcavzh.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2mxeuhgow.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qrnwzzmp.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2zfjnjzos.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2owibxkdo.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ibablndp.html


<!-- 参考信息 -->