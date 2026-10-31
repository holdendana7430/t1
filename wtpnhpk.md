代发 wailian999

[U103] JS：定时器
来源：http://vl.521024.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ec.szsharing.cn

[U104] JS：防抖
来源：http://jg.hnjuh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sv.hahajie.cn

[U105] JS：节流
来源：http://to.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cd.nszjky.cn

[U106] JS：日期格式化
来源：http://fg.wgjwhj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ws.bjjhwx.cn

[U107] JS：数字千分位
来源：http://bb.lnxyls.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ex.shxzskj.cn

[U108] JS：随机整数
来源：http://vb.hahajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yh.panjiajie.cn

[U109] JS：数组分组
来源：http://um.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://tr.shtwfgs.cn

[U110] JS：数组分块
来源：http://tz.hahajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nx.huixiangedu.cn

[U111] JS：对象转 Map
来源：http://rr.huixiangedu.cn

new Map(Object.entries(obj))
来源：http://sj.bjjhwx.cn

[U112] JS：字符串补位
来源：http://xc.shxzukj.cn

"7".padStart(3, "0")
来源：http://lr.yuntaijiaju.cn

[U113] JS：正则替换全部
来源：http://bu.szxytkj.cn

s.replaceAll("a", "b")
来源：http://lw.shxzukj.cn

[U114] JS：JSON 深比较
来源：http://wv.lnxyls.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lg.gzmigu.cn

[U115] JS：生成 UUID
来源：http://rj.521024.cn

crypto.randomUUID()
来源：http://nj.newstarts.cn

[U116] JS：类型检查（JSDoc）
来源：http://mn.nicolike.cn

/** @param {string} name */ function f(name) {}
来源：http://oj.shtwfgs.cn

[U117] JS：单元测试
来源：http://mo.jianghongdianzi.cn

npm i -D vitest;  npx vitest
来源：http://ud.nicolike.cn

[U118] JS：开发服务器
来源：http://ss.hnjuh.cn

npm i -D vite;  npx vite
来源：http://fp.nicolike.cn

[U119] JS：生产构建
来源：http://fv.asd995.cn

npx vite build
来源：http://hn.jianghongdianzi.cn

[U120] JS：读取环境变量（Vite）
来源：http://yo.asd995.cn

import.meta.env.VITE_API_URL
来源：http://yo.hnjuh.cn

================================================================================
来源：http://jh.shtwfgs.cn

统计汇总
来源：http://ir.bookmarksfly.cn

================================================================================
来源：http://gf.colortex.cn

按语言统计（条）：
来源：http://cy.521024.cn

Python ......... 252
来源：http://un.colortex.cn

PHP ............ 252
来源：http://uv.nicolike.cn

JavaScript ..... 252
来源：http://uh.colortex.cn

TypeScript ..... 212
来源：http://gz.szsharing.cn

Java ........... 212
来源：http://zq.nszjky.cn

Go ............. 212
来源：http://zr.jianghongdianzi.cn

Ruby ........... 212
来源：http://iq.lnxyls.cn

C# ............. 212
来源：http://ar.panjiajie.cn

C .............. 30
来源：http://st.shxzskj.cn

C++ ............ 30
来源：http://oe.bookmarksfly.cn

SQL ............ 90
来源：http://vl.yuexingan06.cn

Bash ........... 80
来源：http://gv.nszjky.cn

Kotlin ......... 15
来源：http://aq.jianghongdianzi.cn

Swift .......... 15
来源：http://tr.chemitech.net.cn

Lua ............ 10
来源：http://be.jctech888.com.cn

Perl ........... 10
来源：http://fx.huixinmuqiang.cn

Scala .......... 10
来源：http://tw.bookmarksfly.cn

------------------------------------
来源：http://ul.huixiangedu.cn

合计 ........... 2106 条
来源：http://fc.521024.cn

按章节统计：
来源：http://xy.huanxung.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fu.nszjky.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ra.haigaiapp.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://up.lnxyls.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gi.lnxyls.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yo.yuexingan06.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qq.bjjhwx.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pp.colortex.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yk.newstarts.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uu.chemitech.net.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ar.huixinmuqiang.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cu.wgjwhj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ii.asd995.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fk.muxihuayi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://af.yuntaijiaju.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lr.hnjuh.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://oh.shxzskj.cn

Q SQL 专题                              90
来源：http://wl.521024.cn

R Bash 专题                             80
来源：http://ew.jctech888.com.cn

S C / C++ 专题                          60
来源：http://os.wgjwhj.cn

T 其他语言补充                          60
来源：http://wt.yuexingan06.cn

U 高频实用片段                         120
来源：http://sp.shxzskj.cn

------------------------------------
来源：http://rq.muxihuayi.cn

合计                                  2106 条
来源：http://wd.hahajie.cn

--------------------------------------------------------------------------------
来源：http://ja.colortex.cn

使用提醒
来源：http://zu.newstarts.cn

--------------------------------------------------------------------------------
来源：http://wt.hahajie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ep.jianghongdianzi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lj.yuexingan06.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://le.shxzskj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://by.panjiajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vb.bjjhwx.cn

—— 文件结束 ——
来源：http://vb.huixinmuqiang.cn

================================================================================
来源：http://dv.panjiajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://ph.bjjhwx.cn

Common Programming Examples Cheat Book
来源：http://qi.hahajie.cn

================================================================================
来源：http://cq.panjiajie.cn

【收录内容】
来源：http://ae.jctech888.com.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ir.asd995.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ip.haigaiapp.cn

SQL · Bash · C · C++
来源：http://cw.chemitech.net.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mr.huixinmuqiang.cn

【使用说明】
来源：http://te.jctech888.com.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qx.haigaiapp.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hr.jctech888.com.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ig.huixinmuqiang.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ek.yuexingan06.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://sb.nicolike.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cm.nicolike.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yd.521024.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ii.shtwfgs.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://li.wgjwhj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://iz.shtwfgs.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ir.colortex.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://sx.yuntaijiaju.cn

【文件统计】
来源：http://ry.haigaiapp.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cw.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://sn.huixinmuqiang.cn

目  录
来源：http://je.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://zf.asd995.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hh.huixiangedu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wx.shtwfgs.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://be.szxytkj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rk.hnjuh.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zh.szsharing.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pt.shxzukj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zj.jctech888.com.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fk.yuntaijiaju.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bz.hahajie.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://tb.nicolike.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tr.szxytkj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wh.szxytkj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cc.hnjuh.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://do.bjjhwx.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ww.colortex.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vt.muxihuayi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fj.yuexingan06.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bt.521024.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xt.chemitech.net.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://df.newstarts.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bo.jianghongdianzi.cn

================================================================================
来源：http://jj.hahajie.cn

A. 基础语法与类型
来源：http://ah.lnxyls.cn

================================================================================
来源：http://mb.jctech888.com.cn

[A01] Hello World
来源：http://gv.yuexingan06.cn

Py:   print("Hello, World!")
来源：http://qu.bookmarksfly.cn

PHP:  echo "Hello, World!";
来源：http://yo.yuexingan06.cn

JS:   console.log("Hello, World!");
来源：http://jh.chemitech.net.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wb.haigaiapp.cn

Java: System.out.println("Hello, World!");
来源：http://vj.nszjky.cn

Go:   fmt.Println("Hello, World!")
来源：http://ks.huanxung.cn

Ruby: puts "Hello, World!"
来源：http://fb.panjiajie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ot.szsharing.cn

[A02] 变量声明与赋值
来源：http://al.bjjhwx.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pd.huixinmuqiang.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://pr.szxytkj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://sh.bookmarksfly.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qv.huixiangedu.cn

Java: String name = "Alex"; int age = 20;
来源：http://rj.szxytkj.cn

Go:   name := "Alex"; age := 20
来源：http://jz.muxihuayi.cn

Ruby: name = "Alex"; age = 20
来源：http://bd.hahajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://xa.szxytkj.cn

[A03] 常量定义
来源：http://gj.huixinmuqiang.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wc.huixinmuqiang.cn

PHP:  const PI = 3.14159;
来源：http://nk.huixiangedu.cn

JS:   const PI = 3.14159;
来源：http://af.muxihuayi.cn

TS:   const PI: number = 3.14159;
来源：http://fp.wgjwhj.cn

Java: static final double PI = 3.14159;
来源：http://md.muxihuayi.cn

Go:   const PI = 3.14159
来源：http://md.yuexingan06.cn

Ruby: PI = 3.14159
来源：http://ol.shxzskj.cn

C#:   const double PI = 3.14159;
来源：http://iv.asd995.cn

[A04] 判断变量类型
来源：http://bx.huanxung.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://zm.newstarts.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zj.muxihuayi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qf.newstarts.cn

TS:   typeof x; x instanceof Date
来源：http://jq.hahajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vj.yuntaijiaju.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ko.huixiangedu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ve.nszjky.cn

C#:   x.GetType().Name; x is int
来源：http://kk.wgjwhj.cn

[A05] 整数除法与取模
来源：http://ed.gzmigu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vo.colortex.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ze.newstarts.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ff.shxzskj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dp.huanxung.cn

Java: 7 / 2; 7 % 2
来源：http://on.jctech888.com.cn

Go:   7 / 2; 7 % 2
来源：http://cz.hnjuh.cn

Ruby: 7 / 2; 7 % 2
来源：http://ba.szsharing.cn

C#:   7 / 2; 7 % 2
来源：http://pg.szxytkj.cn

[A06] 字符串转数字
来源：http://yh.gzmigu.cn

Py:   int("42"); float("3.14")
来源：http://sb.newstarts.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qw.hnjuh.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vy.huanxung.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ii.521024.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ak.wgjwhj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ad.newstarts.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ip.9csxet.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mm.nszjky.cn

[A07] 数字转字符串
来源：http://mu.colortex.cn

Py:   str(42)
来源：http://ag.colortex.cn

PHP:  (string) 42; strval(42)
来源：http://cg.hnjuh.cn

JS:   String(42); (42).toString()
来源：http://jy.muxihuayi.cn

TS:   String(42)
来源：http://tf.shxzukj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ot.hnjuh.cn

Go:   strconv.Itoa(42)
来源：http://bg.9csxet.cn

Ruby: 42.to_s
来源：http://dy.chemitech.net.cn

C#:   42.ToString()
来源：http://dw.asd995.cn

[A08] 取整与四舍五入
来源：http://xv.nszjky.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vy.newstarts.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://px.shtwfgs.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ee.shxzskj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ba.huixiangedu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ra.nicolike.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://sb.nicolike.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pm.colortex.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wd.panjiajie.cn

[A09] 绝对值与最大最小值
来源：http://yz.bookmarksfly.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jo.chemitech.net.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://uy.nicolike.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ns.huixiangedu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://am.huixinmuqiang.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yf.muxihuayi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lk.shxzskj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vk.yuexingan06.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hx.szxytkj.cn

[A10] 生成随机数
来源：http://bh.hnjuh.cn

Py:   import random; random.randint(1, 100)
来源：http://tp.yuntaijiaju.cn

PHP:  random_int(1, 100);
来源：http://pf.hahajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ni.panjiajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://sa.haigaiapp.cn

Java: new Random().nextInt(100) + 1
来源：http://xy.521024.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hq.szsharing.cn

Ruby: rand(1..100)
来源：http://bu.chemitech.net.cn

C#:   new Random().Next(1, 101)
来源：http://ek.huixinmuqiang.cn

[A11] 条件表达式（三元）
来源：http://ec.chemitech.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://jc.9csxet.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rx.huanxung.cn

JS:   x > 0 ? "yes" : "no"
来源：http://kt.bookmarksfly.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ib.colortex.cn

Java: x > 0 ? "yes" : "no"
来源：http://ub.hahajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://vo.nicolike.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qc.huixinmuqiang.cn

C#:   x > 0 ? "yes" : "no"
来源：http://un.colortex.cn

[A12] 字符串插值 / 格式化
来源：http://ul.szsharing.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bd.hahajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://oc.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://qx.nszjky.cn

TS:   `Hello, ${name}!`
来源：http://oq.jctech888.com.cn

Java: "Hello, %s!".formatted(name)
来源：http://up.chemitech.net.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hv.colortex.cn

Ruby: "Hello, #{name}!"
来源：http://wa.yuexingan06.cn

C#:   $"Hello, {name}!"
来源：http://td.colortex.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hc.nicolike.cn

Py:   "第一行\n第二行"
来源：http://hp.newstarts.cn

PHP:  "第一行\n第二行"
来源：http://wu.nicolike.cn

JS:   "第一行\n第二行"
来源：http://kp.muxihuayi.cn

TS:   "第一行\n第二行"
来源：http://hb.huixiangedu.cn

Java: "第一行\n第二行"
来源：http://to.huixinmuqiang.cn

Go:   "第一行\n第二行"
来源：http://ga.asd995.cn

Ruby: "第一行\n第二行"
来源：http://fc.colortex.cn

C#:   "第一行\n第二行"
来源：http://zw.huanxung.cn

[A14] 注释写法
来源：http://mx.haigaiapp.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://cv.szsharing.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wt.shtwfgs.cn

JS:   // 单行；/* 多行 */
来源：http://de.panjiajie.cn

TS:   // 单行；/* 多行 */
来源：http://id.panjiajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kh.huanxung.cn

Go:   // 单行；/* 多行 */
来源：http://lc.shxzskj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://co.panjiajie.cn

C#:   // 单行；/* 多行 */
来源：http://ii.chemitech.net.cn

[A15] 空值判断与默认值
来源：http://sr.szsharing.cn

Py:   value = data or "默认值"
来源：http://jh.hnjuh.cn

PHP:  $value = $data ?? "默认值";
来源：http://ny.9csxet.cn

JS:   const value = data ?? "默认值";
来源：http://zt.bookmarksfly.cn

TS:   const value = data ?? "默认值";
来源：http://ri.lnxyls.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ym.szxytkj.cn

Go:   if data == "" { data = "默认值" }
来源：http://hw.9csxet.cn

Ruby: value = data || "默认值"
来源：http://yj.shxzskj.cn

C#:   var value = data ?? "默认值";
来源：http://xq.huanxung.cn

[A16] 真假值判断规则
来源：http://zy.szsharing.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://om.bjjhwx.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ld.lnxyls.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rz.shxzukj.cn

TS:   if (!x) {}
来源：http://fy.bjjhwx.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://im.panjiajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hd.jianghongdianzi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ib.szxytkj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nv.chemitech.net.cn

[A17] 位运算
来源：http://vs.yuntaijiaju.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ef.hnjuh.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sg.yuexingan06.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cb.szsharing.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://li.9csxet.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vk.jianghongdianzi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wi.9csxet.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vt.hnjuh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eb.haigaiapp.cn

[A18] 字符与 ASCII 码互转
来源：http://az.bookmarksfly.cn

Py:   ord("A"); chr(65)
来源：http://sf.jianghongdianzi.cn

PHP:  ord("A"); chr(65)
来源：http://he.haigaiapp.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jt.huixinmuqiang.cn


<!-- 参考信息 -->