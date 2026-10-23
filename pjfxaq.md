代发 wailian999

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3kekbvvzv.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ylyltvei.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3yhfmatwf.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3lchnoorc.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3zmrrbpdc.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3mmaiihzw.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3gqmcccfs.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3ynyuikay.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3siurelru.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3rxzctlcl.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3mnnwsyhz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jntqrxse.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3rokxykon.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3oebliczm.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3clitgbgj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3sbizgyoz.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3pveatkgn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3fhrguutg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3iygpkugt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3yukblhbo.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3arudoots.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3anqzzupv.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3jmmcixhj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3mdkiqpji.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3cewgpzjv.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3iwvevzfo.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3sijnqcoa.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wconxvnn.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3aemjfhks.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uudtpbzl.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3goxuzntj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dgjhwtml.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3mdxkvvpy.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zqcqmcaw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3xucaqfux.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3layenimz.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3yrcphtxs.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3ushikinm.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3zxprdjyu.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3duzpksgv.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3rwbldihs.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3hmdlvfac.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3apouvcqm.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3iknjlmsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3livijiiq.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3popqugnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vhbiujxr.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3klsiscgx.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3vsafanps.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3ghdlhewg.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3azecjzto.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3tfbipxql.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3fdtmsesa.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ulzojybp.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xwraiuod.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3nlpldiha.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3dnpfzsrn.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3hipomocs.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3hbdhutyc.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3tnsjotid.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3iuuwcfse.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3erlqzjny.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3boziglrt.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3rcmpuids.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3ltgyatvz.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fatgzcqb.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3kiklvmsp.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3suulypoe.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3fzcvidug.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3kkbvmazv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3fpsyhcbm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ticzcaqd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3afglmddj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3salposfv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ghuwtrno.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3caarosua.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3lqexfxpu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3aymojwyp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3cflsapfy.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rizzbena.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ywmceihc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3wlsysscw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3dququeks.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3opffpwca.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3tsaqcsec.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3ptnmyzip.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3riryqcsi.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3egsplqml.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3zhqeggzs.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zopvzvlo.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3xltxwdcu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3agzbeqch.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3bsartmbe.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cqumafhg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3ghmbluus.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3dggyqhat.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3sevunxqm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3sofejaaq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3elvgkafq.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3qsgamlsx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hcxahwpf.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3ulsihouc.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3gpehhlif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3onktiyok.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3xsuolyzg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3wtbqrgla.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3kbrfhlzt.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3dhlvcjoq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3zhrrzxwr.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3wrycskeb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3pwuopzip.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3cptbykyl.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3fnyrpgjs.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3hflrevyg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3cdkselet.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3ggczucqz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3vnjfxvzp.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3bbfezakr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3vgyskceq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3xvankpcx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3gqvdudrs.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3qelrftck.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3eppgajdy.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3jxthxjmw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dodjvfrc.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3tgqyswbm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bilkxtxv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xudssdzb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fyxbdceq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3xvwbvdne.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ovkjluxk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kvbnuhgj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3sbyeejac.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vhucaujj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3dsvbfjud.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vrnczoty.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dtjrqidw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lztcphbv.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3angoevqf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ptfetshk.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ufhqrafx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mndegpdh.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rwkyvdme.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nltkbjfe.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ghanbpha.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3dvptmfvx.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ejgjdlwo.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kduhhxsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kwqbybex.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3eighonaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gnzoeylm.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3povzbvih.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3rmrxabpn.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3gbfyfrnq.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3rtqdonuf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3gnoepzse.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3xaahrebe.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3wnzhhwii.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3zaepitzj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3zixmtjtp.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3punwmnkn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3rjszajac.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3bzmpdidt.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3odsyqjox.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3tqwudila.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3iegvlpzf.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3kikxbjtb.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3awqhljsl.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vvdxuogg.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3kqvmawxz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3mibliyxx.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rlcutudk.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vdlraqhh.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ihjmkdlt.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fcegnvhl.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3gpmavefc.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3xuwezqzh.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tjfhwdui.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3pnhnmmdr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3ovfnavie.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3segjvfgf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3lqlpclqa.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3axabmjms.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3hzxnqcsi.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3ztwnfbbk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3bvuzcavc.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3rjwrbujo.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3tbfxnqnl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3tbcevqmm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vusachsg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zpxdxivw.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3menmijgf.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hrleetho.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3liffziwe.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3auweaszk.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fbjccars.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3lmgznzdh.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3kkyvsnwd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3mrbbnpvs.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3xbbzbaxx.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3xvtgziou.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3inzpsipk.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3yjuclteb.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3tkdhtifu.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3wkxrcecs.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3kpbxzbqt.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bgbijvrs.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jfzxksqh.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3rmtxnvtk.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3cbxnkrcr.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vhevxeat.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3wvtewbuf.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3vwjlrtxh.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3mqfezfvr.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3afycviru.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jdxngydi.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3vprylgsi.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jvhwdgyl.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3lqwvqxbl.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ihckvbqi.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3fiuontma.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3ortpdowu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gomhpcdn.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3sbiqegjt.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dqvaoiod.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fcdxxwfd.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bwzgftlb.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xisdrjfm.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lwuttylp.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3xgyszgdx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3rlxrnrmn.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jzwsprxq.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3tnazckag.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3stwkvxxr.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3ewagcqkr.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3rvyyzogn.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3mygrlugx.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3binhzype.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3llqusggi.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3ixdxsdrh.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3djalnlfh.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3qkwlulbp.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3pbsufhrc.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3vihfghdm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3snbdizjb.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3npgdgclv.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xuogoxac.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3nnunkxhb.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ktsqxffm.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bzbvjjky.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3hajhutpq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3hvbkwdxq.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3jmkqtskd.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3wgihhbee.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3zdbjnvqz.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3ssyxoqkq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hiyeazdg.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3exsudonq.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3oipbpqmd.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3hhmzftwz.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yhhrqgfy.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dhvxoagr.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qznsxmiu.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wclodcvv.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qzxnqvpe.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bjoticsp.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3frqyhcfk.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ozzgqetl.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3wmpkixtf.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3lztojwmg.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ynahnzyb.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hzzhkwxi.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lrhkcnhi.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3qugdbmfg.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qusieybh.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3mssfuste.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3spkhfoei.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ltgkbudp.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ogfovsyw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3zujzpnhr.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3eojjxrjp.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3keqyupum.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3bhlhzukv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3cqwzvbiz.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3eiacwscb.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3uhclbdjg.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3xyvtbqla.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3srhrcxds.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3sfqgmqgr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3oftckdjj.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dwdxagai.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nkvphdnt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3ltgrtnek.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3jdfushax.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3upidhuzj.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3iycdzhve.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lwkwtwyt.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fxhfkavx.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3oliiebie.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mlmkhyji.html


<!-- 参考信息 -->