代发 wailian999

[U103] JS：定时器
来源：http://jr.newstarts.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wu.chemitech.net.cn

[U104] JS：防抖
来源：http://po.yuexingan06.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xk.bjjhwx.cn

[U105] JS：节流
来源：http://ds.jianghongdianzi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qp.shxzskj.cn

[U106] JS：日期格式化
来源：http://gn.nicolike.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wn.nszjky.cn

[U107] JS：数字千分位
来源：http://vq.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qa.bookmarksfly.cn

[U108] JS：随机整数
来源：http://st.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zx.nicolike.cn

[U109] JS：数组分组
来源：http://bd.shtwfgs.cn

Object.groupBy(arr, x => x.type)
来源：http://ar.bookmarksfly.cn

[U110] JS：数组分块
来源：http://uo.yuexingan06.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ya.lnxyls.cn

[U111] JS：对象转 Map
来源：http://in.newstarts.cn

new Map(Object.entries(obj))
来源：http://jt.asd995.cn

[U112] JS：字符串补位
来源：http://ci.huixiangedu.cn

"7".padStart(3, "0")
来源：http://cp.521024.cn

[U113] JS：正则替换全部
来源：http://rw.colortex.cn

s.replaceAll("a", "b")
来源：http://ty.hahajie.cn

[U114] JS：JSON 深比较
来源：http://eg.panjiajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fj.yuexingan06.cn

[U115] JS：生成 UUID
来源：http://dn.szsharing.cn

crypto.randomUUID()
来源：http://nk.yuexingan06.cn

[U116] JS：类型检查（JSDoc）
来源：http://am.huixiangedu.cn

/** @param {string} name */ function f(name) {}
来源：http://kz.521024.cn

[U117] JS：单元测试
来源：http://tb.hnjuh.cn

npm i -D vitest;  npx vitest
来源：http://tg.huixinmuqiang.cn

[U118] JS：开发服务器
来源：http://ow.hahajie.cn

npm i -D vite;  npx vite
来源：http://fz.shxzskj.cn

[U119] JS：生产构建
来源：http://hx.yuexingan06.cn

npx vite build
来源：http://py.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://jq.shxzskj.cn

import.meta.env.VITE_API_URL
来源：http://nw.shtwfgs.cn

================================================================================
来源：http://bb.jctech888.com.cn

统计汇总
来源：http://ff.asd995.cn

================================================================================
来源：http://il.yuexingan06.cn

按语言统计（条）：
来源：http://jr.huanxung.cn

Python ......... 252
来源：http://tg.yuexingan06.cn

PHP ............ 252
来源：http://sk.yuntaijiaju.cn

JavaScript ..... 252
来源：http://cp.huixiangedu.cn

TypeScript ..... 212
来源：http://mg.hnjuh.cn

Java ........... 212
来源：http://mb.huixiangedu.cn

Go ............. 212
来源：http://sj.hahajie.cn

Ruby ........... 212
来源：http://xo.bookmarksfly.cn

C# ............. 212
来源：http://sh.shtwfgs.cn

C .............. 30
来源：http://ii.nicolike.cn

C++ ............ 30
来源：http://rr.yuexingan06.cn

SQL ............ 90
来源：http://ml.9csxet.cn

Bash ........... 80
来源：http://bl.muxihuayi.cn

Kotlin ......... 15
来源：http://xz.bookmarksfly.cn

Swift .......... 15
来源：http://yg.bookmarksfly.cn

Lua ............ 10
来源：http://pl.colortex.cn

Perl ........... 10
来源：http://bf.yuexingan06.cn

Scala .......... 10
来源：http://bp.bookmarksfly.cn

------------------------------------
来源：http://fj.shtwfgs.cn

合计 ........... 2106 条
来源：http://rn.hnjuh.cn

按章节统计：
来源：http://rd.szxytkj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ek.colortex.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dj.shxzskj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zf.szsharing.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nm.shtwfgs.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ko.huanxung.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sx.muxihuayi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jw.521024.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sk.521024.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cr.yuexingan06.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vl.nicolike.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ut.colortex.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gg.hnjuh.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nb.yuexingan06.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xf.wgjwhj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nb.asd995.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qa.lnxyls.cn

Q SQL 专题                              90
来源：http://wm.shxzukj.cn

R Bash 专题                             80
来源：http://ds.nicolike.cn

S C / C++ 专题                          60
来源：http://cj.bookmarksfly.cn

T 其他语言补充                          60
来源：http://ia.shxzukj.cn

U 高频实用片段                         120
来源：http://og.szsharing.cn

------------------------------------
来源：http://fn.bjjhwx.cn

合计                                  2106 条
来源：http://jn.9csxet.cn

--------------------------------------------------------------------------------
来源：http://em.bjjhwx.cn

使用提醒
来源：http://hd.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://da.wgjwhj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vv.yuexingan06.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tt.huixiangedu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qq.jianghongdianzi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ac.chemitech.net.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://on.nicolike.cn

—— 文件结束 ——
来源：http://ge.chemitech.net.cn

================================================================================
来源：http://qv.huanxung.cn

程序语言常见例子速查手册（2024 版）
来源：http://dk.wgjwhj.cn

Common Programming Examples Cheat Book
来源：http://xz.huixinmuqiang.cn

================================================================================
来源：http://zp.huixinmuqiang.cn

【收录内容】
来源：http://is.huanxung.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://fj.nicolike.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ui.colortex.cn

SQL · Bash · C · C++
来源：http://gd.panjiajie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gm.asd995.cn

【使用说明】
来源：http://eb.shtwfgs.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bu.newstarts.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ea.szsharing.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://be.hahajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://aj.wgjwhj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://tg.shxzukj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://td.shxzukj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hs.newstarts.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mr.yuntaijiaju.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wk.jianghongdianzi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xd.yuexingan06.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lh.panjiajie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nq.newstarts.cn

【文件统计】
来源：http://zi.chemitech.net.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://di.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://jf.shtwfgs.cn

目  录
来源：http://oi.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://qn.nszjky.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kr.gzmigu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://iq.panjiajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://au.newstarts.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zx.szsharing.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qq.521024.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yb.huixinmuqiang.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gb.bjjhwx.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vv.nicolike.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vk.huanxung.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bw.szsharing.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gw.bjjhwx.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fg.9csxet.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fw.szxytkj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gi.wgjwhj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lp.nicolike.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qq.huanxung.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hw.szxytkj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://if.bjjhwx.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ck.chemitech.net.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mj.hnjuh.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fv.yuexingan06.cn

================================================================================
来源：http://bq.bjjhwx.cn

A. 基础语法与类型
来源：http://zx.yuntaijiaju.cn

================================================================================
来源：http://nt.jianghongdianzi.cn

[A01] Hello World
来源：http://bp.hahajie.cn

Py:   print("Hello, World!")
来源：http://fp.nszjky.cn

PHP:  echo "Hello, World!";
来源：http://mv.haigaiapp.cn

JS:   console.log("Hello, World!");
来源：http://ac.muxihuayi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lg.nicolike.cn

Java: System.out.println("Hello, World!");
来源：http://ke.colortex.cn

Go:   fmt.Println("Hello, World!")
来源：http://jt.wgjwhj.cn

Ruby: puts "Hello, World!"
来源：http://yp.bookmarksfly.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zv.bookmarksfly.cn

[A02] 变量声明与赋值
来源：http://sb.panjiajie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zk.chemitech.net.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://lz.nszjky.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ct.jctech888.com.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ga.muxihuayi.cn

Java: String name = "Alex"; int age = 20;
来源：http://qk.huanxung.cn

Go:   name := "Alex"; age := 20
来源：http://hx.521024.cn

Ruby: name = "Alex"; age = 20
来源：http://xd.yuntaijiaju.cn

C#:   string name = "Alex"; int age = 20;
来源：http://bt.wgjwhj.cn

[A03] 常量定义
来源：http://ue.szxytkj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jm.yuntaijiaju.cn

PHP:  const PI = 3.14159;
来源：http://ur.asd995.cn

JS:   const PI = 3.14159;
来源：http://en.muxihuayi.cn

TS:   const PI: number = 3.14159;
来源：http://gm.colortex.cn

Java: static final double PI = 3.14159;
来源：http://oa.lnxyls.cn

Go:   const PI = 3.14159
来源：http://cm.newstarts.cn

Ruby: PI = 3.14159
来源：http://bm.521024.cn

C#:   const double PI = 3.14159;
来源：http://ic.szxytkj.cn

[A04] 判断变量类型
来源：http://uc.shxzukj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://jt.jctech888.com.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mg.nicolike.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://es.chemitech.net.cn

TS:   typeof x; x instanceof Date
来源：http://ev.bjjhwx.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bd.shtwfgs.cn

Go:   reflect.TypeOf(x).Name()
来源：http://en.yuntaijiaju.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xx.9csxet.cn

C#:   x.GetType().Name; x is int
来源：http://nk.shtwfgs.cn

[A05] 整数除法与取模
来源：http://wg.hahajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qq.yuntaijiaju.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ad.szsharing.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pu.gzmigu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://uf.bjjhwx.cn

Java: 7 / 2; 7 % 2
来源：http://cp.bjjhwx.cn

Go:   7 / 2; 7 % 2
来源：http://uz.shtwfgs.cn

Ruby: 7 / 2; 7 % 2
来源：http://gu.shtwfgs.cn

C#:   7 / 2; 7 % 2
来源：http://yd.hahajie.cn

[A06] 字符串转数字
来源：http://md.asd995.cn

Py:   int("42"); float("3.14")
来源：http://it.huanxung.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bk.lnxyls.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xq.muxihuayi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://tq.shxzskj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://or.huixinmuqiang.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nd.huixinmuqiang.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://mu.huixinmuqiang.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fn.huanxung.cn

[A07] 数字转字符串
来源：http://du.hnjuh.cn

Py:   str(42)
来源：http://fo.yuexingan06.cn

PHP:  (string) 42; strval(42)
来源：http://qq.shtwfgs.cn

JS:   String(42); (42).toString()
来源：http://xb.szxytkj.cn

TS:   String(42)
来源：http://dz.bookmarksfly.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://fy.panjiajie.cn

Go:   strconv.Itoa(42)
来源：http://er.huixiangedu.cn

Ruby: 42.to_s
来源：http://cw.nicolike.cn

C#:   42.ToString()
来源：http://em.colortex.cn

[A08] 取整与四舍五入
来源：http://zz.newstarts.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hq.haigaiapp.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bc.szsharing.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cc.shxzskj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sy.9csxet.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tk.panjiajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://oy.yuexingan06.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://cr.521024.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://nd.panjiajie.cn

[A09] 绝对值与最大最小值
来源：http://pk.szsharing.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bs.wgjwhj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://im.yuntaijiaju.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ls.haigaiapp.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rt.newstarts.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yd.shtwfgs.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ka.newstarts.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zu.muxihuayi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://id.gzmigu.cn

[A10] 生成随机数
来源：http://se.haigaiapp.cn

Py:   import random; random.randint(1, 100)
来源：http://by.huixinmuqiang.cn

PHP:  random_int(1, 100);
来源：http://pk.bookmarksfly.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yy.9csxet.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nk.shtwfgs.cn

Java: new Random().nextInt(100) + 1
来源：http://gw.yuntaijiaju.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ge.yuntaijiaju.cn

Ruby: rand(1..100)
来源：http://op.lnxyls.cn

C#:   new Random().Next(1, 101)
来源：http://ok.yuexingan06.cn

[A11] 条件表达式（三元）
来源：http://il.colortex.cn

Py:   "yes" if x > 0 else "no"
来源：http://hj.newstarts.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ez.huixinmuqiang.cn

JS:   x > 0 ? "yes" : "no"
来源：http://tw.huixinmuqiang.cn

TS:   x > 0 ? "yes" : "no"
来源：http://gt.lnxyls.cn

Java: x > 0 ? "yes" : "no"
来源：http://hf.nicolike.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://gy.gzmigu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://gf.bookmarksfly.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ay.bookmarksfly.cn

[A12] 字符串插值 / 格式化
来源：http://ex.shtwfgs.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bq.haigaiapp.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://oc.bookmarksfly.cn

JS:   `Hello, ${name}!`
来源：http://qd.yuexingan06.cn

TS:   `Hello, ${name}!`
来源：http://nx.nicolike.cn

Java: "Hello, %s!".formatted(name)
来源：http://ur.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wd.yuexingan06.cn

Ruby: "Hello, #{name}!"
来源：http://eh.szxytkj.cn

C#:   $"Hello, {name}!"
来源：http://pq.huixiangedu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://eb.hnjuh.cn

Py:   "第一行\n第二行"
来源：http://eo.asd995.cn

PHP:  "第一行\n第二行"
来源：http://ri.jianghongdianzi.cn

JS:   "第一行\n第二行"
来源：http://nc.lnxyls.cn

TS:   "第一行\n第二行"
来源：http://un.9csxet.cn

Java: "第一行\n第二行"
来源：http://sl.nszjky.cn

Go:   "第一行\n第二行"
来源：http://mb.lnxyls.cn

Ruby: "第一行\n第二行"
来源：http://pe.shxzukj.cn

C#:   "第一行\n第二行"
来源：http://gn.nicolike.cn

[A14] 注释写法
来源：http://kf.jctech888.com.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ew.panjiajie.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://po.gzmigu.cn

JS:   // 单行；/* 多行 */
来源：http://cx.shxzukj.cn

TS:   // 单行；/* 多行 */
来源：http://fo.hahajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://le.huixinmuqiang.cn

Go:   // 单行；/* 多行 */
来源：http://pr.shxzukj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://dd.newstarts.cn

C#:   // 单行；/* 多行 */
来源：http://ws.9csxet.cn

[A15] 空值判断与默认值
来源：http://cf.chemitech.net.cn

Py:   value = data or "默认值"
来源：http://ic.gzmigu.cn

PHP:  $value = $data ?? "默认值";
来源：http://rl.asd995.cn

JS:   const value = data ?? "默认值";
来源：http://qb.gzmigu.cn

TS:   const value = data ?? "默认值";
来源：http://sj.szsharing.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rm.bjjhwx.cn

Go:   if data == "" { data = "默认值" }
来源：http://jm.jianghongdianzi.cn

Ruby: value = data || "默认值"
来源：http://ez.shtwfgs.cn

C#:   var value = data ?? "默认值";
来源：http://wf.9csxet.cn

[A16] 真假值判断规则
来源：http://et.shxzskj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fz.jianghongdianzi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cr.chemitech.net.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wj.nszjky.cn

TS:   if (!x) {}
来源：http://nn.colortex.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rz.hnjuh.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wq.muxihuayi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://wi.shxzukj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qg.nicolike.cn

[A17] 位运算
来源：http://mv.huixiangedu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ei.yuntaijiaju.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://im.jctech888.com.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wb.yuexingan06.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://sa.yuntaijiaju.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sw.shxzskj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xi.asd995.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zq.shtwfgs.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ss.nicolike.cn

[A18] 字符与 ASCII 码互转
来源：http://cm.shxzukj.cn

Py:   ord("A"); chr(65)
来源：http://nc.asd995.cn

PHP:  ord("A"); chr(65)
来源：http://mz.shtwfgs.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ar.szxytkj.cn


<!-- 参考信息 -->