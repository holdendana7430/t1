代发 wailian999

[U105] JS：节流
来源：http://ss.bookmarksfly.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://un.jctech888.com.cn

[U106] JS：日期格式化
来源：http://rf.9csxet.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://af.yuexingan06.cn

[U107] JS：数字千分位
来源：http://di.9csxet.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bi.9csxet.cn

[U108] JS：随机整数
来源：http://kc.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ja.muxihuayi.cn

[U109] JS：数组分组
来源：http://rq.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://jr.521024.cn

[U110] JS：数组分块
来源：http://sv.521024.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zy.gzmigu.cn

[U111] JS：对象转 Map
来源：http://ij.jianghongdianzi.cn

new Map(Object.entries(obj))
来源：http://dd.jctech888.com.cn

[U112] JS：字符串补位
来源：http://iv.huixiangedu.cn

"7".padStart(3, "0")
来源：http://ur.gzmigu.cn

[U113] JS：正则替换全部
来源：http://xy.lnxyls.cn

s.replaceAll("a", "b")
来源：http://oy.bookmarksfly.cn

[U114] JS：JSON 深比较
来源：http://bu.wgjwhj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xf.bookmarksfly.cn

[U115] JS：生成 UUID
来源：http://zt.muxihuayi.cn

crypto.randomUUID()
来源：http://vw.hahajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://dx.huanxung.cn

/** @param {string} name */ function f(name) {}
来源：http://ud.panjiajie.cn

[U117] JS：单元测试
来源：http://ov.shtwfgs.cn

npm i -D vitest;  npx vitest
来源：http://nd.panjiajie.cn

[U118] JS：开发服务器
来源：http://mq.colortex.cn

npm i -D vite;  npx vite
来源：http://uv.chemitech.net.cn

[U119] JS：生产构建
来源：http://kv.asd995.cn

npx vite build
来源：http://dl.chemitech.net.cn

[U120] JS：读取环境变量（Vite）
来源：http://wt.bjjhwx.cn

import.meta.env.VITE_API_URL
来源：http://zx.jctech888.com.cn

================================================================================
来源：http://pr.gzmigu.cn

统计汇总
来源：http://dx.hahajie.cn

================================================================================
来源：http://bc.shxzskj.cn

按语言统计（条）：
来源：http://yq.haigaiapp.cn

Python ......... 252
来源：http://un.huanxung.cn

PHP ............ 252
来源：http://mc.newstarts.cn

JavaScript ..... 252
来源：http://ce.asd995.cn

TypeScript ..... 212
来源：http://hu.nicolike.cn

Java ........... 212
来源：http://kl.muxihuayi.cn

Go ............. 212
来源：http://vh.colortex.cn

Ruby ........... 212
来源：http://vo.hahajie.cn

C# ............. 212
来源：http://ez.lnxyls.cn

C .............. 30
来源：http://mt.yuexingan06.cn

C++ ............ 30
来源：http://av.muxihuayi.cn

SQL ............ 90
来源：http://kz.colortex.cn

Bash ........... 80
来源：http://yd.bookmarksfly.cn

Kotlin ......... 15
来源：http://im.newstarts.cn

Swift .......... 15
来源：http://ct.jianghongdianzi.cn

Lua ............ 10
来源：http://cc.shxzskj.cn

Perl ........... 10
来源：http://fe.nicolike.cn

Scala .......... 10
来源：http://or.jianghongdianzi.cn

------------------------------------
来源：http://cs.yuntaijiaju.cn

合计 ........... 2106 条
来源：http://jy.9csxet.cn

按章节统计：
来源：http://ta.colortex.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.nicolike.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dt.wgjwhj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mh.shxzskj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yt.gzmigu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jp.wgjwhj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mh.szxytkj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sc.asd995.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yc.wgjwhj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qu.shxzukj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xx.bjjhwx.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://am.colortex.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sd.nszjky.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wf.huixiangedu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nq.haigaiapp.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bb.521024.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wc.yuntaijiaju.cn

Q SQL 专题                              90
来源：http://pf.521024.cn

R Bash 专题                             80
来源：http://vp.gzmigu.cn

S C / C++ 专题                          60
来源：http://rq.lnxyls.cn

T 其他语言补充                          60
来源：http://mp.jianghongdianzi.cn

U 高频实用片段                         120
来源：http://bs.szxytkj.cn

------------------------------------
来源：http://fv.asd995.cn

合计                                  2106 条
来源：http://if.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://ta.szsharing.cn

使用提醒
来源：http://ay.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://pv.yuntaijiaju.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://al.newstarts.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mx.panjiajie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sb.yuntaijiaju.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ej.jctech888.com.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vw.nszjky.cn

—— 文件结束 ——
来源：http://ha.huanxung.cn

================================================================================
来源：http://ap.hahajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://ap.hnjuh.cn

Common Programming Examples Cheat Book
来源：http://cb.colortex.cn

================================================================================
来源：http://po.bookmarksfly.cn

【收录内容】
来源：http://qv.huanxung.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://fs.wgjwhj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vx.newstarts.cn

SQL · Bash · C · C++
来源：http://ue.wgjwhj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xe.jctech888.com.cn

【使用说明】
来源：http://fp.yuexingan06.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rb.asd995.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xf.huixiangedu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pb.yuntaijiaju.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zx.szsharing.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://gj.wgjwhj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rk.jianghongdianzi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://as.yuntaijiaju.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cj.shxzukj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zc.chemitech.net.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pf.wgjwhj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nq.lnxyls.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nd.9csxet.cn

【文件统计】
来源：http://wy.bjjhwx.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fv.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://rj.huanxung.cn

目  录
来源：http://he.newstarts.cn

--------------------------------------------------------------------------------
来源：http://bm.521024.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ss.huixinmuqiang.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ex.nszjky.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mu.shxzukj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qm.bookmarksfly.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ex.huixinmuqiang.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pb.shxzukj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xh.huixinmuqiang.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fq.nszjky.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fx.hnjuh.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lj.huanxung.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://be.shxzukj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zb.haigaiapp.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://sr.szsharing.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gl.521024.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uj.nicolike.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vm.lnxyls.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vf.colortex.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hd.hahajie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ao.shtwfgs.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ge.chemitech.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kl.nicolike.cn

================================================================================
来源：http://aa.nszjky.cn

A. 基础语法与类型
来源：http://ek.521024.cn

================================================================================
来源：http://kp.nszjky.cn

[A01] Hello World
来源：http://zb.huixiangedu.cn

Py:   print("Hello, World!")
来源：http://fw.yuntaijiaju.cn

PHP:  echo "Hello, World!";
来源：http://ln.jctech888.com.cn

JS:   console.log("Hello, World!");
来源：http://nm.shxzukj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zx.huanxung.cn

Java: System.out.println("Hello, World!");
来源：http://ep.newstarts.cn

Go:   fmt.Println("Hello, World!")
来源：http://tp.jianghongdianzi.cn

Ruby: puts "Hello, World!"
来源：http://ei.521024.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gw.jctech888.com.cn

[A02] 变量声明与赋值
来源：http://cz.nszjky.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hu.yuexingan06.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ln.haigaiapp.cn

JS:   let name = "Alex"; const age = 20;
来源：http://sa.jctech888.com.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gb.yuexingan06.cn

Java: String name = "Alex"; int age = 20;
来源：http://sd.jianghongdianzi.cn

Go:   name := "Alex"; age := 20
来源：http://ki.bjjhwx.cn

Ruby: name = "Alex"; age = 20
来源：http://yi.szsharing.cn

C#:   string name = "Alex"; int age = 20;
来源：http://eq.hahajie.cn

[A03] 常量定义
来源：http://ae.bjjhwx.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ie.newstarts.cn

PHP:  const PI = 3.14159;
来源：http://on.lnxyls.cn

JS:   const PI = 3.14159;
来源：http://ps.nszjky.cn

TS:   const PI: number = 3.14159;
来源：http://oi.bookmarksfly.cn

Java: static final double PI = 3.14159;
来源：http://ug.shxzukj.cn

Go:   const PI = 3.14159
来源：http://vo.muxihuayi.cn

Ruby: PI = 3.14159
来源：http://aq.shtwfgs.cn

C#:   const double PI = 3.14159;
来源：http://jb.nszjky.cn

[A04] 判断变量类型
来源：http://tp.nicolike.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://nm.huixiangedu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ea.hnjuh.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ut.haigaiapp.cn

TS:   typeof x; x instanceof Date
来源：http://ew.bookmarksfly.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dk.9csxet.cn

Go:   reflect.TypeOf(x).Name()
来源：http://py.gzmigu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gp.wgjwhj.cn

C#:   x.GetType().Name; x is int
来源：http://fd.nicolike.cn

[A05] 整数除法与取模
来源：http://gu.9csxet.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ag.chemitech.net.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://of.szxytkj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wj.nicolike.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nt.chemitech.net.cn

Java: 7 / 2; 7 % 2
来源：http://qz.szxytkj.cn

Go:   7 / 2; 7 % 2
来源：http://ew.yuntaijiaju.cn

Ruby: 7 / 2; 7 % 2
来源：http://nu.asd995.cn

C#:   7 / 2; 7 % 2
来源：http://tx.chemitech.net.cn

[A06] 字符串转数字
来源：http://gj.asd995.cn

Py:   int("42"); float("3.14")
来源：http://oq.shxzskj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ss.haigaiapp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mt.panjiajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://sf.nszjky.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rl.shxzukj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ml.colortex.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zp.shxzskj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mf.bookmarksfly.cn

[A07] 数字转字符串
来源：http://gh.yuntaijiaju.cn

Py:   str(42)
来源：http://pe.asd995.cn

PHP:  (string) 42; strval(42)
来源：http://wt.asd995.cn

JS:   String(42); (42).toString()
来源：http://pq.gzmigu.cn

TS:   String(42)
来源：http://li.wgjwhj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://kq.asd995.cn

Go:   strconv.Itoa(42)
来源：http://zd.jctech888.com.cn

Ruby: 42.to_s
来源：http://ez.haigaiapp.cn

C#:   42.ToString()
来源：http://xk.shxzukj.cn

[A08] 取整与四舍五入
来源：http://gx.nicolike.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rj.521024.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://me.asd995.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ec.shtwfgs.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bx.huixinmuqiang.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dn.huanxung.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://im.shxzskj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qg.9csxet.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.szxytkj.cn

[A09] 绝对值与最大最小值
来源：http://cn.asd995.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://co.521024.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fa.wgjwhj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://da.huixinmuqiang.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ff.shxzskj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://sm.shxzukj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dn.hahajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://un.huixinmuqiang.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fv.chemitech.net.cn

[A10] 生成随机数
来源：http://zq.lnxyls.cn

Py:   import random; random.randint(1, 100)
来源：http://ob.szsharing.cn

PHP:  random_int(1, 100);
来源：http://ci.muxihuayi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ug.nszjky.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://sj.huanxung.cn

Java: new Random().nextInt(100) + 1
来源：http://wx.haigaiapp.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kg.shtwfgs.cn

Ruby: rand(1..100)
来源：http://xy.jctech888.com.cn

C#:   new Random().Next(1, 101)
来源：http://il.bjjhwx.cn

[A11] 条件表达式（三元）
来源：http://ny.9csxet.cn

Py:   "yes" if x > 0 else "no"
来源：http://nh.bookmarksfly.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://to.bookmarksfly.cn

JS:   x > 0 ? "yes" : "no"
来源：http://me.jianghongdianzi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://mi.hnjuh.cn

Java: x > 0 ? "yes" : "no"
来源：http://pv.panjiajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://js.chemitech.net.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://yv.panjiajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xp.panjiajie.cn

[A12] 字符串插值 / 格式化
来源：http://pz.yuexingan06.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kw.szsharing.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://in.wgjwhj.cn

JS:   `Hello, ${name}!`
来源：http://be.huixiangedu.cn

TS:   `Hello, ${name}!`
来源：http://gj.yuntaijiaju.cn

Java: "Hello, %s!".formatted(name)
来源：http://op.asd995.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tz.panjiajie.cn

Ruby: "Hello, #{name}!"
来源：http://bt.lnxyls.cn

C#:   $"Hello, {name}!"
来源：http://qk.jctech888.com.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://yz.shtwfgs.cn

Py:   "第一行\n第二行"
来源：http://sj.jianghongdianzi.cn

PHP:  "第一行\n第二行"
来源：http://sx.shxzukj.cn

JS:   "第一行\n第二行"
来源：http://oh.bjjhwx.cn

TS:   "第一行\n第二行"
来源：http://ti.jctech888.com.cn

Java: "第一行\n第二行"
来源：http://vw.huanxung.cn

Go:   "第一行\n第二行"
来源：http://rc.lnxyls.cn

Ruby: "第一行\n第二行"
来源：http://dz.bookmarksfly.cn

C#:   "第一行\n第二行"
来源：http://ft.gzmigu.cn

[A14] 注释写法
来源：http://bv.9csxet.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://tp.yuexingan06.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wg.newstarts.cn

JS:   // 单行；/* 多行 */
来源：http://vo.hnjuh.cn

TS:   // 单行；/* 多行 */
来源：http://tm.colortex.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bn.wgjwhj.cn

Go:   // 单行；/* 多行 */
来源：http://ex.shxzukj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://lr.yuexingan06.cn

C#:   // 单行；/* 多行 */
来源：http://ic.colortex.cn

[A15] 空值判断与默认值
来源：http://zj.yuntaijiaju.cn

Py:   value = data or "默认值"
来源：http://fw.muxihuayi.cn

PHP:  $value = $data ?? "默认值";
来源：http://fg.hahajie.cn

JS:   const value = data ?? "默认值";
来源：http://cn.haigaiapp.cn

TS:   const value = data ?? "默认值";
来源：http://tj.chemitech.net.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://je.haigaiapp.cn

Go:   if data == "" { data = "默认值" }
来源：http://ch.huixinmuqiang.cn

Ruby: value = data || "默认值"
来源：http://ke.9csxet.cn

C#:   var value = data ?? "默认值";
来源：http://ci.9csxet.cn

[A16] 真假值判断规则
来源：http://hj.hnjuh.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rs.colortex.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nj.bjjhwx.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nu.bookmarksfly.cn

TS:   if (!x) {}
来源：http://qz.wgjwhj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wz.asd995.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://oe.521024.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ae.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ig.hahajie.cn

[A17] 位运算
来源：http://yg.wgjwhj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ao.shtwfgs.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hv.huixiangedu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gu.shxzskj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cn.lnxyls.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fw.hnjuh.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jm.jctech888.com.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://na.shxzukj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://me.yuntaijiaju.cn

[A18] 字符与 ASCII 码互转
来源：http://vl.asd995.cn

Py:   ord("A"); chr(65)
来源：http://db.gzmigu.cn

PHP:  ord("A"); chr(65)
来源：http://ie.9csxet.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ve.hahajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zy.colortex.cn

Java: (int) 'A'; (char) 65
来源：http://wr.wgjwhj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://iz.wgjwhj.cn

Ruby: "A".ord; 65.chr
来源：http://kq.nicolike.cn


<!-- 参考信息 -->