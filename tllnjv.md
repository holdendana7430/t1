代发 wailian999

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3wubenhfr.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3erxilygm.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3crirygvo.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3usboystj.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3mmfipyzp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3cgpbolrl.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3aqffnvgu.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3uexnoebk.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3ceudsdli.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3fqjbtedu.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3nicckmyg.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3bxzzbcrv.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3tgtpaknj.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3lulviofo.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3jgqafaha.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jeoycimq.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3clypgnir.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gymumpwu.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3hlwqopus.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3eavbxkui.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3fcmgtobu.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3zlpebkgb.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3rbbysxay.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3mrqdodnn.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3frdxxvtn.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ehujxuef.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3gzjpxxcy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3sgyamlzf.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3yphmhded.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3lkmnzivf.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3rrfxscqs.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jfqosalq.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3dpgeorct.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rdoprqrk.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3edzdocqv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3ofdklwga.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3pilbanbk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3mvurahqs.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3ibzebvkz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3xrezhgtz.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3xpmqwttd.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ylwlopqs.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3wvdszdzl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3guagpooi.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3mqijsedq.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3wnlqrlnt.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3scpyofsp.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kmhnennw.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3yqejzajd.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qeqiaqgp.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3tiqnqoqf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nujcjgyj.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3tiiwozkd.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ecaflltr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3seqpktqs.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tgyehwfx.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3lrjllzvf.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3erqimebu.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3flyxfndj.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3xvdhmgru.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3qagezzgc.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3bsrwpzok.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3fbnobtfd.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3grtxolsx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lvhcqial.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3tyyqiyav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kqlasiud.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3nenvdphz.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3fnctappt.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3dytqnaon.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3kulkmdin.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3luuyvnup.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ikzcdjwj.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3brhwndqi.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3cdvkhima.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3nqtckoyz.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3vlqczstz.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3dbakvumx.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3vqfvilwo.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3enygzqug.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3sitnrwpy.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3xpgjwjdl.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3ekgesyxz.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ezusaiaa.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3twtvbqdc.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3yohwbfbx.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3exwxcqay.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3curxizob.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3hwiyyvzn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3quzajrra.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3llajqvfs.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ynigsdrt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3cabibqgt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3pgpphgef.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3lbavnqeb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3xrlqzkrb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xburjfje.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3xozatxxb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fauuoyln.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3udpqwnvg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3dcvzswuq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3lnrpmiku.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3pzokqaoa.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wqehndte.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3lmmidkzr.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3gvtwmkzb.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3snmuhxvh.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3btxzoafw.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3byrwnokn.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ccxbfdef.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3ieyiqlgh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qceyzdoj.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3llwiadvv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rxtytfei.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3fvzknagg.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3fxdifdxr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3pdnqyasa.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3ukczhstz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3icnfewvv.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3nwqhduno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xtbwihvf.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3zyjnrong.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3rfjlhqgv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3grxsyzkx.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3jwbihwwq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3onrotfwj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3acrjancy.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3dpauluey.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3ggasydrs.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3nfsvabmp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3iiwyvzcq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3jirrvant.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3ilfcuwid.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3xbkbixve.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3xolebxkb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3kidigzun.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3wxihloiz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3xpbblewo.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3bqgshqzy.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3bbmekwax.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3akxrlvrv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3czgewcfp.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3heqmcrvz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3tkubojvm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ynfmexrz.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3vlljsdpj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wgwucphn.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3myacnsjm.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fyrvzurd.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3nlpgrvvg.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3hustmzuh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3upiqgpgy.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3guzmkmpj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3avdkpjvp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3totpfidd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nkbnnecy.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uclbgdnu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3acziynnf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vlbhaphg.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jlhxvsrn.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3grtqorfk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3yfregysu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oamqfnne.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3ruiwstoh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rvjctvzs.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3nopzyjvd.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3letqcvdr.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mdgakaeq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xwsvtsgd.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3ujjirwhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ipqcqznd.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3ajfzkhxx.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ufigoefl.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3pzolarjm.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3tegkaiwu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3qinnswcq.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3oqbhtrnp.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3bxgzobyv.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3lrjfgpsi.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3hwaoadze.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3kdbealul.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3qxkfoemc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xpfyfagd.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3hpbylioi.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3sjxdalwt.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3szbyvoce.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3xcsesiig.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3qgvlilmv.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3fkwwbrjp.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3szavzubu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3ujqoguhh.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bvbxtgik.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3aqgqfuzt.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xkutzael.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3sgcoxqin.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ouhdzkjv.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3atpdaapc.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yyrobvjl.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3jszcicpd.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3recmdrfm.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3iptnjwmx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3fxqinmlp.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3kphoqpxr.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3xmpxobkm.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3jomiuvlc.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3xcrctdfs.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3zbneqqgn.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3bfrtexvw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3qxqbjvcb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hkgsdlus.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wyytkpxc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cpqnfnpc.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dneyhaum.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yxaguwok.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ixmahccf.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ehibauoq.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3icdxytpx.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3mxdorlre.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3drcjehcq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3eriwbksn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3uotrahpv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3vomvnumx.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3dlrltklz.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3zohnmlhl.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3wlfjxhby.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ucmzpnnx.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zgluuaqa.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3vxvqqwjc.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wdcawxmp.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3xdrcvfbn.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3qfnyixax.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3ydmayrdz.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3pbuvrizp.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3epgdobua.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3zmjjgtkf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3rspfqeyb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3bglusqwz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zzrqmdky.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3shdoiupy.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3kvkbqpyg.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3eplxuxtq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3vjebrgyl.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ejiphwye.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3sdpqccrg.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ztvknphf.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dkfnrxmu.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3uatxgmpj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3smrfkhje.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3veegsaxp.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3kpfzbcpd.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3rjcwrods.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jsnwsdrg.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3ypyolidm.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3brztujsl.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3qakzazey.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3gfziduhr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3thxjqnxg.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3uygbzlpm.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3cdwxujyw.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3jjkzjvxv.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3nbfpxlou.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3xonueeug.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3luvmjdnw.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3avqylxoy.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3yudygskq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xrmzwgup.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zeleqfhu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3whnkajnv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tqaxmser.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dgulhqnq.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3edlophjf.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3iwtsqkrc.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3pppntdao.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3gmewefts.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3tdvhrocw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3khfikbmn.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wpdfuoig.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3pjgdknpj.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3tajoukra.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3ruiwtjls.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wlrokjpi.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dzvbkzmr.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3seeskbqz.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qbwvuadj.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zttwzwyg.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nddasguv.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dfeunqsh.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lukpshan.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3qgsafshi.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3gamkbrjd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3eoxhvtwx.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zyxikalc.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3aydqpcqp.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3bgtxvsjm.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tmmypiad.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3lyouwigk.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3olzbqkml.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3sapwvdce.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3iqnbjbbv.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3cyhdzekv.html


<!-- 参考信息 -->