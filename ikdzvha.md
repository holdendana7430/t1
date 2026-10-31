代发 wailian999

[U101] JS：classList 操作
来源：http://mw.huixinmuqiang.cn

el.classList.toggle("active")
来源：http://oa.hnjuh.cn

[U102] JS：本地存储
来源：http://uf.newstarts.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ry.bookmarksfly.cn

[U103] JS：定时器
来源：http://dq.szxytkj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zq.nicolike.cn

[U104] JS：防抖
来源：http://cg.huixiangedu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ab.hnjuh.cn

[U105] JS：节流
来源：http://uj.muxihuayi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://um.bookmarksfly.cn

[U106] JS：日期格式化
来源：http://ek.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gk.huanxung.cn

[U107] JS：数字千分位
来源：http://lo.huanxung.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://oe.jianghongdianzi.cn

[U108] JS：随机整数
来源：http://ex.jctech888.com.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wd.bjjhwx.cn

[U109] JS：数组分组
来源：http://nv.521024.cn

Object.groupBy(arr, x => x.type)
来源：http://ta.haigaiapp.cn

[U110] JS：数组分块
来源：http://zb.wgjwhj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://at.panjiajie.cn

[U111] JS：对象转 Map
来源：http://mn.gzmigu.cn

new Map(Object.entries(obj))
来源：http://ck.huixiangedu.cn

[U112] JS：字符串补位
来源：http://yx.colortex.cn

"7".padStart(3, "0")
来源：http://qp.huixinmuqiang.cn

[U113] JS：正则替换全部
来源：http://kd.hnjuh.cn

s.replaceAll("a", "b")
来源：http://yf.huixiangedu.cn

[U114] JS：JSON 深比较
来源：http://ko.yuexingan06.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://oj.haigaiapp.cn

[U115] JS：生成 UUID
来源：http://gg.shtwfgs.cn

crypto.randomUUID()
来源：http://mi.yuntaijiaju.cn

[U116] JS：类型检查（JSDoc）
来源：http://zl.hnjuh.cn

/** @param {string} name */ function f(name) {}
来源：http://cy.bookmarksfly.cn

[U117] JS：单元测试
来源：http://pd.yuntaijiaju.cn

npm i -D vitest;  npx vitest
来源：http://rk.huanxung.cn

[U118] JS：开发服务器
来源：http://js.huanxung.cn

npm i -D vite;  npx vite
来源：http://pw.hahajie.cn

[U119] JS：生产构建
来源：http://cw.colortex.cn

npx vite build
来源：http://dw.panjiajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://on.muxihuayi.cn

import.meta.env.VITE_API_URL
来源：http://kf.yuntaijiaju.cn

================================================================================
来源：http://my.huanxung.cn

统计汇总
来源：http://zq.huixinmuqiang.cn

================================================================================
来源：http://mc.lnxyls.cn

按语言统计（条）：
来源：http://vh.shxzskj.cn

Python ......... 252
来源：http://rp.shxzukj.cn

PHP ............ 252
来源：http://do.jianghongdianzi.cn

JavaScript ..... 252
来源：http://lb.bjjhwx.cn

TypeScript ..... 212
来源：http://hd.szsharing.cn

Java ........... 212
来源：http://oi.9csxet.cn

Go ............. 212
来源：http://uz.chemitech.net.cn

Ruby ........... 212
来源：http://tu.wgjwhj.cn

C# ............. 212
来源：http://vs.panjiajie.cn

C .............. 30
来源：http://ci.huixiangedu.cn

C++ ............ 30
来源：http://md.lnxyls.cn

SQL ............ 90
来源：http://lq.lnxyls.cn

Bash ........... 80
来源：http://tl.shtwfgs.cn

Kotlin ......... 15
来源：http://uh.newstarts.cn

Swift .......... 15
来源：http://sy.panjiajie.cn

Lua ............ 10
来源：http://tj.szsharing.cn

Perl ........... 10
来源：http://dk.yuexingan06.cn

Scala .......... 10
来源：http://wl.521024.cn

------------------------------------
来源：http://aw.shtwfgs.cn

合计 ........... 2106 条
来源：http://yu.shxzskj.cn

按章节统计：
来源：http://qi.huixinmuqiang.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://he.huixiangedu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://em.hnjuh.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ve.hahajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lr.lnxyls.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://st.lnxyls.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dd.colortex.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fa.jianghongdianzi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jh.huixiangedu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fj.wgjwhj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gm.huixinmuqiang.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zv.chemitech.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hy.jianghongdianzi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://eq.lnxyls.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mi.jianghongdianzi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dp.colortex.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mv.colortex.cn

Q SQL 专题                              90
来源：http://lr.bjjhwx.cn

R Bash 专题                             80
来源：http://cq.hahajie.cn

S C / C++ 专题                          60
来源：http://lj.panjiajie.cn

T 其他语言补充                          60
来源：http://ai.yuntaijiaju.cn

U 高频实用片段                         120
来源：http://dp.yuexingan06.cn

------------------------------------
来源：http://gz.lnxyls.cn

合计                                  2106 条
来源：http://mx.szsharing.cn

--------------------------------------------------------------------------------
来源：http://kb.gzmigu.cn

使用提醒
来源：http://sk.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://dj.jctech888.com.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mk.hahajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hc.wgjwhj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wi.colortex.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ae.szxytkj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vx.hahajie.cn

—— 文件结束 ——
来源：http://uk.chemitech.net.cn

================================================================================
来源：http://hy.panjiajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://js.panjiajie.cn

Common Programming Examples Cheat Book
来源：http://vi.panjiajie.cn

================================================================================
来源：http://qk.chemitech.net.cn

【收录内容】
来源：http://in.gzmigu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://gd.szxytkj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kw.muxihuayi.cn

SQL · Bash · C · C++
来源：http://dt.bookmarksfly.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vk.newstarts.cn

【使用说明】
来源：http://tx.shxzukj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tv.huixinmuqiang.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yw.panjiajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://oq.newstarts.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gh.huanxung.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ud.bookmarksfly.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ie.chemitech.net.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ya.haigaiapp.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fz.huixinmuqiang.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vx.bjjhwx.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://is.bookmarksfly.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ve.huixiangedu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pi.lnxyls.cn

【文件统计】
来源：http://zk.colortex.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sn.szsharing.cn

--------------------------------------------------------------------------------
来源：http://ot.yuexingan06.cn

目  录
来源：http://cz.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://oh.shxzukj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wu.szsharing.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ru.wgjwhj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ic.wgjwhj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://my.yuntaijiaju.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lc.yuexingan06.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://em.nicolike.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ug.jctech888.com.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ou.wgjwhj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lg.wgjwhj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cw.lnxyls.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ft.bookmarksfly.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cl.bjjhwx.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vo.shxzukj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hs.lnxyls.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hc.bookmarksfly.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gh.gzmigu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ou.nszjky.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wp.asd995.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tp.panjiajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://iz.nicolike.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kg.huanxung.cn

================================================================================
来源：http://lz.colortex.cn

A. 基础语法与类型
来源：http://el.huanxung.cn

================================================================================
来源：http://jw.jianghongdianzi.cn

[A01] Hello World
来源：http://hs.huixiangedu.cn

Py:   print("Hello, World!")
来源：http://ap.szxytkj.cn

PHP:  echo "Hello, World!";
来源：http://dp.szxytkj.cn

JS:   console.log("Hello, World!");
来源：http://xi.521024.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fq.hahajie.cn

Java: System.out.println("Hello, World!");
来源：http://xw.bjjhwx.cn

Go:   fmt.Println("Hello, World!")
来源：http://wz.gzmigu.cn

Ruby: puts "Hello, World!"
来源：http://lm.lnxyls.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://th.panjiajie.cn

[A02] 变量声明与赋值
来源：http://gr.muxihuayi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bz.newstarts.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://uy.bjjhwx.cn

JS:   let name = "Alex"; const age = 20;
来源：http://cy.nszjky.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ca.nicolike.cn

Java: String name = "Alex"; int age = 20;
来源：http://lw.newstarts.cn

Go:   name := "Alex"; age := 20
来源：http://ep.lnxyls.cn

Ruby: name = "Alex"; age = 20
来源：http://ez.nszjky.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ad.colortex.cn

[A03] 常量定义
来源：http://am.panjiajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mn.huixinmuqiang.cn

PHP:  const PI = 3.14159;
来源：http://jz.haigaiapp.cn

JS:   const PI = 3.14159;
来源：http://he.szxytkj.cn

TS:   const PI: number = 3.14159;
来源：http://dk.newstarts.cn

Java: static final double PI = 3.14159;
来源：http://js.huixiangedu.cn

Go:   const PI = 3.14159
来源：http://cz.newstarts.cn

Ruby: PI = 3.14159
来源：http://ux.szsharing.cn

C#:   const double PI = 3.14159;
来源：http://mk.bookmarksfly.cn

[A04] 判断变量类型
来源：http://mk.jianghongdianzi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ic.huixiangedu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jm.panjiajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bj.jianghongdianzi.cn

TS:   typeof x; x instanceof Date
来源：http://gc.yuexingan06.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://in.lnxyls.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ja.nszjky.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ot.hahajie.cn

C#:   x.GetType().Name; x is int
来源：http://yh.shxzskj.cn

[A05] 整数除法与取模
来源：http://oi.yuntaijiaju.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gs.shxzukj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://tx.wgjwhj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rm.muxihuayi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fr.wgjwhj.cn

Java: 7 / 2; 7 % 2
来源：http://ko.shxzukj.cn

Go:   7 / 2; 7 % 2
来源：http://zy.huixiangedu.cn

Ruby: 7 / 2; 7 % 2
来源：http://xx.szxytkj.cn

C#:   7 / 2; 7 % 2
来源：http://pq.shxzukj.cn

[A06] 字符串转数字
来源：http://wq.chemitech.net.cn

Py:   int("42"); float("3.14")
来源：http://de.521024.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gh.yuexingan06.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vv.haigaiapp.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wi.shxzskj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://su.hnjuh.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://eb.shxzukj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://gn.9csxet.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cz.chemitech.net.cn

[A07] 数字转字符串
来源：http://bw.nszjky.cn

Py:   str(42)
来源：http://qm.lnxyls.cn

PHP:  (string) 42; strval(42)
来源：http://py.9csxet.cn

JS:   String(42); (42).toString()
来源：http://ud.yuexingan06.cn

TS:   String(42)
来源：http://gl.szxytkj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ue.hnjuh.cn

Go:   strconv.Itoa(42)
来源：http://wr.gzmigu.cn

Ruby: 42.to_s
来源：http://sq.szsharing.cn

C#:   42.ToString()
来源：http://aa.shxzukj.cn

[A08] 取整与四舍五入
来源：http://in.panjiajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vp.bjjhwx.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mk.521024.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ku.jianghongdianzi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wb.nszjky.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://uz.newstarts.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ur.gzmigu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://tw.shxzukj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://re.huixiangedu.cn

[A09] 绝对值与最大最小值
来源：http://kp.panjiajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://sy.nicolike.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xu.jianghongdianzi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://il.lnxyls.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gn.jctech888.com.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dq.hnjuh.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wm.9csxet.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://sh.wgjwhj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mb.521024.cn

[A10] 生成随机数
来源：http://gm.huixiangedu.cn

Py:   import random; random.randint(1, 100)
来源：http://br.yuexingan06.cn

PHP:  random_int(1, 100);
来源：http://dc.bookmarksfly.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ti.nicolike.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dm.shxzskj.cn

Java: new Random().nextInt(100) + 1
来源：http://ks.nicolike.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vt.szsharing.cn

Ruby: rand(1..100)
来源：http://ip.yuntaijiaju.cn

C#:   new Random().Next(1, 101)
来源：http://vr.panjiajie.cn

[A11] 条件表达式（三元）
来源：http://jq.gzmigu.cn

Py:   "yes" if x > 0 else "no"
来源：http://cb.huanxung.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://wi.hahajie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pv.nszjky.cn

TS:   x > 0 ? "yes" : "no"
来源：http://fr.chemitech.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://zd.nszjky.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ko.shxzskj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://zi.huixinmuqiang.cn

C#:   x > 0 ? "yes" : "no"
来源：http://wh.szxytkj.cn

[A12] 字符串插值 / 格式化
来源：http://qu.shxzskj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nu.panjiajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gf.huixiangedu.cn

JS:   `Hello, ${name}!`
来源：http://kv.jianghongdianzi.cn

TS:   `Hello, ${name}!`
来源：http://or.asd995.cn

Java: "Hello, %s!".formatted(name)
来源：http://td.hahajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ri.haigaiapp.cn

Ruby: "Hello, #{name}!"
来源：http://ga.haigaiapp.cn

C#:   $"Hello, {name}!"
来源：http://oi.szsharing.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ws.nicolike.cn

Py:   "第一行\n第二行"
来源：http://mt.szsharing.cn

PHP:  "第一行\n第二行"
来源：http://cr.colortex.cn

JS:   "第一行\n第二行"
来源：http://oo.jianghongdianzi.cn

TS:   "第一行\n第二行"
来源：http://ou.szsharing.cn

Java: "第一行\n第二行"
来源：http://ic.szsharing.cn

Go:   "第一行\n第二行"
来源：http://vl.wgjwhj.cn

Ruby: "第一行\n第二行"
来源：http://mz.colortex.cn

C#:   "第一行\n第二行"
来源：http://zi.colortex.cn

[A14] 注释写法
来源：http://qu.szsharing.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://yo.newstarts.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://jh.jctech888.com.cn

JS:   // 单行；/* 多行 */
来源：http://sf.asd995.cn

TS:   // 单行；/* 多行 */
来源：http://ju.huixiangedu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tt.bookmarksfly.cn

Go:   // 单行；/* 多行 */
来源：http://cn.panjiajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://jb.shxzukj.cn

C#:   // 单行；/* 多行 */
来源：http://yg.colortex.cn

[A15] 空值判断与默认值
来源：http://rj.panjiajie.cn

Py:   value = data or "默认值"
来源：http://zd.newstarts.cn

PHP:  $value = $data ?? "默认值";
来源：http://mq.hahajie.cn

JS:   const value = data ?? "默认值";
来源：http://ic.huixinmuqiang.cn

TS:   const value = data ?? "默认值";
来源：http://fv.yuexingan06.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pk.yuexingan06.cn

Go:   if data == "" { data = "默认值" }
来源：http://ee.szsharing.cn

Ruby: value = data || "默认值"
来源：http://xo.huixinmuqiang.cn

C#:   var value = data ?? "默认值";
来源：http://pj.9csxet.cn

[A16] 真假值判断规则
来源：http://ud.yuexingan06.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kf.bookmarksfly.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wm.9csxet.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fh.bjjhwx.cn

TS:   if (!x) {}
来源：http://pr.521024.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nb.asd995.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jk.szxytkj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ub.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://np.shxzskj.cn

[A17] 位运算
来源：http://hn.szxytkj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ys.gzmigu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kz.bookmarksfly.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pr.jctech888.com.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bo.asd995.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gi.yuexingan06.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fs.nicolike.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ma.panjiajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://az.nicolike.cn


<!-- 参考信息 -->