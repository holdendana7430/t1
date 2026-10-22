代发 wailian999

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ytlfvtjk.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2heqrokag.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2pojnfket.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ykpvlwjq.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2jwzitlsy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2skgahrdz.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2stdzvbaq.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2bflqtrhc.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2elgcvncv.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2jxbcznmn.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2vemahncr.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2yyakgjjr.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2wntobuau.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2pcjasvdw.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ustfmyiq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2fauqidob.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2gdgmotcv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2utarnvvf.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rxknzxcd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2bhyhwpsz.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2unvtbdog.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ajsqfdbo.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2uoljfduk.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2jklqcbck.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2rjsnbalg.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2gtjpivpv.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2jayszzcn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2vfzbcngb.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2dpzxiedq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2sdnhpgta.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ypkssjru.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fpuzavbq.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2jsrmodxa.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nejmcqye.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ckrmrhli.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2vkmvbrqc.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2vcotswno.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2rvzwtpvx.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2gzlgiyib.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2sjcnitvg.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2erfhywpv.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2vlujeycg.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2niolosrs.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2hiviubnn.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2tdwaszuh.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2curxczqf.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2bxsgmnsg.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2epzsftjj.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2zxpygkjm.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2obycovog.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2kniqpcqy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qbpdijjx.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2vrxzxxfm.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2opkpyrli.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2vzreafsh.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dfkjpibd.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2kdphibms.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2zvorxtjt.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2keuafmzg.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2aytaqqbe.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2lwacqcbh.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2bowwpemm.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2pvsgnnqx.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2khzcljsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ezsqsicz.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2vaopzzkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2smwrmtuw.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2npdbnmbt.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2fkgsrauu.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2adhvmhzm.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2xnvvjiko.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2fsyqghrw.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ssxfkswk.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2nipcngpy.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2yenitexj.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2nfurbxdx.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2leokbxno.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2igiacqef.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2zepxfcsg.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2mpfkvang.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2uognhhys.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2zdcgmoub.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2fdwcjaar.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2giiswoqr.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2afndfhkj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2onemfjci.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2yszgkims.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ocpjtvwk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ueleppoa.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2kzllesmq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2obbbixap.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2apszldkh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2dtbeppve.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ozmfgexo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2yitxpfal.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2adtnisxr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2yarasjzo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2eikzmcrg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2iwfrlega.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hdtcvzyl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2tbzmjfsh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2tjlrzrph.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2jctzikdf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ktgmczhf.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2ndooqodp.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2geuqurpq.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2aloczits.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2awfwkoqb.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2jxnqrrny.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vddpikcr.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2hwxoctiy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qwfjfmml.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ekmmjyqn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qwqwzkxt.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2dcvsjwxc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2tatgndfm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2djvpslmi.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2swpjywpl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2zltmiyuu.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2fcmitygb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rrswxhif.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2uypiruea.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2royvsqkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xnsxpdac.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2wpvefpbw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2bymbcoom.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2ncqyshgk.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2wrzbnrsf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2hazkgvfv.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2dumnijiw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2fvfliinl.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2pzfmisvq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2gisjewqr.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2oiymqwnc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2zzlyvbbi.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2bifulxia.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2vkscfaco.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2okrgecdl.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2eqddtzhl.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2bsdmvjcv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2rtvmxfrr.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2flappncc.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2teuwbqaj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2plgydgio.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cwlaqczw.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2vqyxohcb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2svvcfnff.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2xekzglsb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oexabzmz.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2jotqzgti.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fefqvzbw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2hvrrabtt.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tzxjzqmn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2bgrjwhwo.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ackprlzo.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lillkqev.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2xobgyrwx.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2axcuxqvj.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fawophdi.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jnbumwln.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mbwjilxw.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2muyxgbok.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2stufooam.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2dyayayhh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vdiggvuc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cccgdtwx.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2xstgirqp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2zpvtjdqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jymtbcqa.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2ezwmuipi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xjsxocmg.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2ghthvdbw.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2odkgfeoi.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2sssneshb.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2bzttsqti.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2jfsqluxw.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2gfcieqwg.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2vtnmgodb.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2hdagydkv.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2plvhslqe.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2tddnwezu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2pozchisq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rtpkoglm.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2uyabkpmi.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2axmmzglw.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tpqokqez.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2sfkmhkjw.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2fazyldzo.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2mtafusxx.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2vxohtvkm.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2sshgndqi.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yvanhjfe.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2amlprcoa.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jzmovxhg.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pdidgbyf.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2oxxrxuuo.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2dowqloqw.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gpvsmujm.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2obgobsme.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2feyriuax.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2dpsigzpb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2emkwivza.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2kuuiguil.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2uoimplwy.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2lrwrajvu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2eniaxfvh.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2jxxmgkiu.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2ksqfuvan.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2fnnbyrjf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mzloyevg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2afwrcull.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qqdvzvbf.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hnlhgdfa.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ehlfgzkk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2koxbmxaj.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2csoikqsp.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2kwcsgajo.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2mzqmpjba.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2pcydpwgi.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2czkyanzh.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2xpqdnvmh.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2viltgofn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2ainqkivg.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2dxfmpnph.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2hqnvrsms.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2hhowqjlv.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2afaohgfx.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2yxgckeyz.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zharypeg.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2zxhsudro.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2ssjkaxlf.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2ktfdnnoz.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2mctvmajb.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2mclwmcxu.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2mmckntzm.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ouezokwj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2nekkbyuq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2iysowedj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2nbtlcprd.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2smovznme.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qfqzlahb.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2ddjnojrr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vkcpdvlu.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fsurwjtn.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ubifslrg.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lwcoluxq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lygdmeth.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xoizslig.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lozpmuux.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2qhifvvop.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2sdbnqzzp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nmjtrole.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2cuxypygt.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2fvymbjtv.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2fojrbiil.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2cuqksoug.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2olbbobyr.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2fiisgvfi.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2invvjzse.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2jlsxessi.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2zrvqictc.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2napgwgkz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2abevxyft.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2cdinyquo.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wepgueue.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2byjiwljo.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lrntsgew.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2hqmqwjfn.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2onucztkm.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vfnspqmp.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2fdorylsy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2xkdnhbhf.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2jmvemkhn.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2dncmdhbt.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2oqkdfhxv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2lcjefcgu.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xvwdqfpt.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2nbdvezws.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2obfrfwad.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2ilqqujup.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qceilcup.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tyekbkwz.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pnmrljsw.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fganzzax.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dbhxkmzh.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pidgzegu.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2udpqpfhn.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2opwnoeyi.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2decxxwgr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2qyhriwsh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xsvwyjrl.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2hzmqkxzw.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2awbyabqb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2ddjobzkq.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mvnmvdbi.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2ykqyqwpa.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2spmfjxns.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2bpgfdhsr.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ybncqyib.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xxnrxphy.html


<!-- 参考信息 -->