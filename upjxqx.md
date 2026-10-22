代发 wailian999

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2tknrwlvh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pwlpxuac.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2ibehrbrj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2daqfgtmq.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2vnuypcir.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2escrcpgy.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2xrfvnomu.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2gdgsfujs.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2uocqeinj.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2iwtvemdb.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2uklbwrbb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2eixtishd.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2ltaghxws.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2bdgukvqy.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2dcldfgog.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2evlbtbra.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2qmoyasih.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2esncjpbu.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xnkcsjms.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2mgtumplg.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2qlpusngg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2lymymjbr.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2vaeinphs.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2wbrshfio.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2dbtjkydf.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ghglhqkd.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2upbfaipa.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2hbmcmluq.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2dlxyltlw.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2twukwdfn.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2lddyenvz.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2uzmvtjds.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2cxjamxlh.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uikaxquw.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2pfbomony.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vdovkbij.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2gjmvdaip.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2rlqulyka.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2cpgsiqnc.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bcqkedxv.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2oyyfwqgz.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2rtmudsxt.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2krofizfx.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2nqssrshq.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2zyfdmpxr.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2seutygjt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2nhofteex.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2mqdrtmrq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cfejnqim.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2xkctfgkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cqvxxupm.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2wqdbbczw.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2drmsfvbq.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2fkyfmvsb.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2asohxdwr.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2lvsadcxi.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wwgsylgp.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2qbugnnix.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2frqvwuyr.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2gygwiils.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2xntdrrtt.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2iukrwaep.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2emigrtzo.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ciehvhst.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2gvnthdxw.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2mssgvvwh.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2wdfdcgrn.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2itwvcgxz.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2wuvumezu.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tkdrvzxj.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2wqbelxsg.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2obttcuff.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2jytkmzwk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2fpjpwwra.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2frgwwtdw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ukrjwlbl.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2invrjvvv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2uwyipyii.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jrozngcp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2vlvmitzu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2yqhjxovv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2oxgxpsaj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ljradvfo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2cpwjgtlx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2avwwxsmh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2lrrkykce.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2sbjjoruz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fpcreglh.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2kjxwaoby.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2bsoafldo.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2jdrvvldf.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2scpxoyha.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2jppydpek.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2eebjhqps.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ipezwkxw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qhhvorbr.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2qfrbykii.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ffiybhkf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2xvjwslmp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2wmrnxygj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2znknwzbi.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2ralabcyq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2tecgipmn.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2rpccpypa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nlocxtve.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2gkmzhyom.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2kuuscdtc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2arqadszd.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2xijrldhe.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2uhwijdgf.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2bdqwskvj.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2txhzvcts.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2gqtcpzzi.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2nzegkmkl.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2kyeqiyrr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2zsnsyoth.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2cvahnmjw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2mjrudsmv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2iofbqdih.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2fjgcicvp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2tmceixqv.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2zozbovpl.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2qenvxgxe.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2yyupiunh.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2kvxyhajf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2xwjxmdgo.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2orwrpxpf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2vryeyrkm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ipvdywvk.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2lswbwgjw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bxkvbacl.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2gtnhcbfp.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2tieypvlq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2wfgmefso.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zgnnjtjw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zcdalktc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2yukcdste.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2shwvwsmb.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2dweeineu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gnfoshef.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2grcxihwz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vwnpdoec.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2pkrdtpxe.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ismzpptp.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ynmnskux.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qonxjrnp.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lnjjgoyp.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2kobyhtdt.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hcadnwrw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2osfxbedq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2njhboivx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2gltbwlvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rbjfnive.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2vltpfkxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2crvetsbj.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2acjirbam.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2wfmwzina.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2blhktdvd.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ojbxmsur.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2yobnupwl.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2zagnylmi.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2tprpdfmd.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2ivcsbxuj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ucqomvcu.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2abtaylvu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2ryolvfqx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2lnknghip.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xxnsxlfa.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2izicfdqk.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2qnkqwqiv.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2gaqwksxb.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2tiqssugt.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2sadttgyo.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2prczbgdd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2fbamldqt.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fmihlumm.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cizrlolp.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ofrkynsm.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zwxxglvi.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2eagdjoys.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2izoyklpg.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uqdtkaza.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2bnfhcwjp.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2acgqlitn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2qwxtorht.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2avpldxqc.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2hgszaxop.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2iqajqclg.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2wutmwdzu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2ydtlskkh.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2pzkxvfml.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2gvqyrndo.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2wptjfjqw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gggtxrqq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2irddsvka.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zbrstxuk.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2yqcupdaj.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dxfubzbd.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lnaiafaq.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ldewojpq.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2fqcuwygg.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ctmynitn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2iekktdwj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2omrmykfx.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2twrynbps.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2rynofetz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2cgnghghs.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2mwmjgnbb.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2cofunpjf.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aedambtl.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2qwjckwnz.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2zdifdbnp.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2axlwozus.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2glnpviuo.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2mzcjfmka.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2grxxfjgr.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2chxestdy.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2crayvuxo.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2lmyltmrz.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2shmqshqv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2fqntqshw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2akvegzei.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2kesfdwtj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2hdkcfbox.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2wuuhmxlm.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2pkjcllfo.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2cfmvchwe.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2mrgnjqtc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pytbjdlo.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2llipxcui.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lfxdmmho.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rncsvgtm.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ugfaojci.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2xqkgfqfg.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2doberipa.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vskohujq.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2agubzldn.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2nvgtdozc.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2wtxnshzm.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2dmptjldf.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2zqnkxdpn.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2hyssbolp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2cgplhbvi.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2fvzejgmh.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2jgatpuib.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2qbqbnfxx.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2sqvotves.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xdbudbxk.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gzoxdjpn.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bxuhlgly.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hhmesjal.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2vocxbifk.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2agpxtrky.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zmmeqohy.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dszrlgef.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2tgmtiuat.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2ktxoqqbx.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2igqkubzx.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2fkxjhuht.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2rsbrtwfe.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fsolctkw.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2uesqeceo.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2xldhtvla.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2qkoofqjv.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vtloqlai.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lvbjhelx.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cgjvydgg.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uozpizvt.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gdblsdct.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jimbgxxn.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2aeqyiknj.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jpyaljjr.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2bogwydpv.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2uoydozza.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2weuuwxad.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zynumdml.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2oejckbav.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2qmuithsa.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hjmfjiri.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2tntaibbu.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2hsiuzaya.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2mhemkzwm.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2fpilruhp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hssggqyt.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qxkiqajf.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2lkecgfrt.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2qgqrpgth.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2xbgpjrwu.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2kjjyxdac.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2bfzpyokd.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2gkzkdioq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2vayfqcbp.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2frrnpydg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2efkrpxmk.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rdkqurhe.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tljqosfi.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2uvvhcigu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2fmstjoxo.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2bmmersmv.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2czjczkvp.html


<!-- 参考信息 -->