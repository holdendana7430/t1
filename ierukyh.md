代发 wailian999

[U103] JS：定时器
来源：http://tu.lnxyls.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tz.521024.cn

[U104] JS：防抖
来源：http://nh.huixinmuqiang.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xb.muxihuayi.cn

[U105] JS：节流
来源：http://pa.yuexingan06.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ag.gzmigu.cn

[U106] JS：日期格式化
来源：http://av.hahajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jg.shxzukj.cn

[U107] JS：数字千分位
来源：http://sd.9csxet.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://oj.shxzukj.cn

[U108] JS：随机整数
来源：http://um.nicolike.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pb.hnjuh.cn

[U109] JS：数组分组
来源：http://av.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://so.shxzukj.cn

[U110] JS：数组分块
来源：http://je.lnxyls.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zl.shxzukj.cn

[U111] JS：对象转 Map
来源：http://jh.yuexingan06.cn

new Map(Object.entries(obj))
来源：http://zi.9csxet.cn

[U112] JS：字符串补位
来源：http://sy.muxihuayi.cn

"7".padStart(3, "0")
来源：http://yv.shtwfgs.cn

[U113] JS：正则替换全部
来源：http://hr.hahajie.cn

s.replaceAll("a", "b")
来源：http://ub.yuntaijiaju.cn

[U114] JS：JSON 深比较
来源：http://ei.muxihuayi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xn.jctech888.com.cn

[U115] JS：生成 UUID
来源：http://xt.colortex.cn

crypto.randomUUID()
来源：http://sl.gzmigu.cn

[U116] JS：类型检查（JSDoc）
来源：http://kg.hnjuh.cn

/** @param {string} name */ function f(name) {}
来源：http://zc.huixiangedu.cn

[U117] JS：单元测试
来源：http://ke.shxzukj.cn

npm i -D vitest;  npx vitest
来源：http://rp.jctech888.com.cn

[U118] JS：开发服务器
来源：http://nb.shxzukj.cn

npm i -D vite;  npx vite
来源：http://dm.haigaiapp.cn

[U119] JS：生产构建
来源：http://rb.yuntaijiaju.cn

npx vite build
来源：http://oc.yuexingan06.cn

[U120] JS：读取环境变量（Vite）
来源：http://dt.panjiajie.cn

import.meta.env.VITE_API_URL
来源：http://yo.521024.cn

================================================================================
来源：http://iv.jctech888.com.cn

统计汇总
来源：http://ao.nicolike.cn

================================================================================
来源：http://la.yuexingan06.cn

按语言统计（条）：
来源：http://fz.asd995.cn

Python ......... 252
来源：http://jc.huanxung.cn

PHP ............ 252
来源：http://vi.jctech888.com.cn

JavaScript ..... 252
来源：http://oa.szsharing.cn

TypeScript ..... 212
来源：http://ml.muxihuayi.cn

Java ........... 212
来源：http://ti.chemitech.net.cn

Go ............. 212
来源：http://cp.asd995.cn

Ruby ........... 212
来源：http://jt.jctech888.com.cn

C# ............. 212
来源：http://ub.newstarts.cn

C .............. 30
来源：http://cc.shxzukj.cn

C++ ............ 30
来源：http://kh.huixiangedu.cn

SQL ............ 90
来源：http://wz.nicolike.cn

Bash ........... 80
来源：http://pd.jianghongdianzi.cn

Kotlin ......... 15
来源：http://nu.9csxet.cn

Swift .......... 15
来源：http://gn.szsharing.cn

Lua ............ 10
来源：http://rd.newstarts.cn

Perl ........... 10
来源：http://fq.nszjky.cn

Scala .......... 10
来源：http://av.hnjuh.cn

------------------------------------
来源：http://fe.shxzukj.cn

合计 ........... 2106 条
来源：http://xa.yuntaijiaju.cn

按章节统计：
来源：http://dz.wgjwhj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://de.yuexingan06.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://oh.huixinmuqiang.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jn.huixiangedu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ha.jianghongdianzi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://iy.hahajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gn.colortex.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qk.nszjky.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dt.szxytkj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mk.yuntaijiaju.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kf.panjiajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://av.nicolike.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://el.shtwfgs.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zo.szxytkj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gh.chemitech.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://if.lnxyls.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://id.chemitech.net.cn

Q SQL 专题                              90
来源：http://qv.panjiajie.cn

R Bash 专题                             80
来源：http://by.huixinmuqiang.cn

S C / C++ 专题                          60
来源：http://gk.szxytkj.cn

T 其他语言补充                          60
来源：http://nm.wgjwhj.cn

U 高频实用片段                         120
来源：http://ul.wgjwhj.cn

------------------------------------
来源：http://st.yuexingan06.cn

合计                                  2106 条
来源：http://sk.nicolike.cn

--------------------------------------------------------------------------------
来源：http://mi.szxytkj.cn

使用提醒
来源：http://db.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://dp.nszjky.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kh.shtwfgs.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ed.haigaiapp.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nl.asd995.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qm.lnxyls.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hp.bookmarksfly.cn

—— 文件结束 ——
来源：http://io.newstarts.cn

================================================================================
来源：http://no.lnxyls.cn

程序语言常见例子速查手册（2024 版）
来源：http://ij.huixiangedu.cn

Common Programming Examples Cheat Book
来源：http://oi.yuntaijiaju.cn

================================================================================
来源：http://us.szsharing.cn

【收录内容】
来源：http://xr.shxzskj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://lg.9csxet.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xj.panjiajie.cn

SQL · Bash · C · C++
来源：http://kb.yuntaijiaju.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fb.newstarts.cn

【使用说明】
来源：http://mk.wgjwhj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://je.colortex.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ub.hahajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ph.gzmigu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mj.lnxyls.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ex.haigaiapp.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rd.szsharing.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ne.szsharing.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pv.asd995.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vq.lnxyls.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wt.wgjwhj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kz.huanxung.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ho.newstarts.cn

【文件统计】
来源：http://cr.hnjuh.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xy.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://vd.newstarts.cn

目  录
来源：http://ne.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://vf.chemitech.net.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ho.hahajie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bl.hnjuh.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vn.521024.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kz.chemitech.net.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dd.yuexingan06.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://go.shxzskj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yb.521024.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qk.nszjky.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sv.nicolike.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ds.szxytkj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fn.shtwfgs.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lo.lnxyls.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wm.wgjwhj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://js.huanxung.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ts.shxzukj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sn.wgjwhj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pl.gzmigu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://yy.muxihuayi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://aq.bookmarksfly.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ey.huixiangedu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://js.panjiajie.cn

================================================================================
来源：http://pb.521024.cn

A. 基础语法与类型
来源：http://pk.jctech888.com.cn

================================================================================
来源：http://xs.hnjuh.cn

[A01] Hello World
来源：http://tw.9csxet.cn

Py:   print("Hello, World!")
来源：http://vx.hnjuh.cn

PHP:  echo "Hello, World!";
来源：http://nn.colortex.cn

JS:   console.log("Hello, World!");
来源：http://vx.huanxung.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://na.huanxung.cn

Java: System.out.println("Hello, World!");
来源：http://ps.muxihuayi.cn

Go:   fmt.Println("Hello, World!")
来源：http://xc.panjiajie.cn

Ruby: puts "Hello, World!"
来源：http://iv.huixiangedu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fi.lnxyls.cn

[A02] 变量声明与赋值
来源：http://ql.hnjuh.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kq.bjjhwx.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://sa.chemitech.net.cn

JS:   let name = "Alex"; const age = 20;
来源：http://na.asd995.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vx.szsharing.cn

Java: String name = "Alex"; int age = 20;
来源：http://yz.huixinmuqiang.cn

Go:   name := "Alex"; age := 20
来源：http://ee.asd995.cn

Ruby: name = "Alex"; age = 20
来源：http://nv.yuntaijiaju.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ej.colortex.cn

[A03] 常量定义
来源：http://ti.shxzskj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://di.nicolike.cn

PHP:  const PI = 3.14159;
来源：http://fe.gzmigu.cn

JS:   const PI = 3.14159;
来源：http://de.shxzukj.cn

TS:   const PI: number = 3.14159;
来源：http://vu.shtwfgs.cn

Java: static final double PI = 3.14159;
来源：http://xu.szxytkj.cn

Go:   const PI = 3.14159
来源：http://sk.521024.cn

Ruby: PI = 3.14159
来源：http://hs.szxytkj.cn

C#:   const double PI = 3.14159;
来源：http://lc.lnxyls.cn

[A04] 判断变量类型
来源：http://rk.yuexingan06.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vd.bjjhwx.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nq.wgjwhj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kd.hnjuh.cn

TS:   typeof x; x instanceof Date
来源：http://au.yuexingan06.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jv.bjjhwx.cn

Go:   reflect.TypeOf(x).Name()
来源：http://uh.szxytkj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://hh.colortex.cn

C#:   x.GetType().Name; x is int
来源：http://nr.shxzskj.cn

[A05] 整数除法与取模
来源：http://ic.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://by.yuntaijiaju.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://wm.muxihuayi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://sw.huixinmuqiang.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qh.huanxung.cn

Java: 7 / 2; 7 % 2
来源：http://uv.newstarts.cn

Go:   7 / 2; 7 % 2
来源：http://ud.yuexingan06.cn

Ruby: 7 / 2; 7 % 2
来源：http://ne.panjiajie.cn

C#:   7 / 2; 7 % 2
来源：http://od.yuntaijiaju.cn

[A06] 字符串转数字
来源：http://ee.shtwfgs.cn

Py:   int("42"); float("3.14")
来源：http://ak.bookmarksfly.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ic.yuexingan06.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ng.nicolike.cn

TS:   parseInt("42", 10); Number("42")
来源：http://sl.nicolike.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gs.bjjhwx.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://li.hahajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ae.szxytkj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nj.shtwfgs.cn

[A07] 数字转字符串
来源：http://va.bjjhwx.cn

Py:   str(42)
来源：http://bc.lnxyls.cn

PHP:  (string) 42; strval(42)
来源：http://hq.shxzskj.cn

JS:   String(42); (42).toString()
来源：http://vk.shxzukj.cn

TS:   String(42)
来源：http://ws.bookmarksfly.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://sd.yuntaijiaju.cn

Go:   strconv.Itoa(42)
来源：http://bj.shtwfgs.cn

Ruby: 42.to_s
来源：http://qa.wgjwhj.cn

C#:   42.ToString()
来源：http://hp.jianghongdianzi.cn

[A08] 取整与四舍五入
来源：http://uv.haigaiapp.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://oa.bjjhwx.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kl.bookmarksfly.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xj.wgjwhj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ht.nicolike.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qw.newstarts.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ca.9csxet.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://cd.colortex.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lj.newstarts.cn

[A09] 绝对值与最大最小值
来源：http://hh.hahajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pd.hnjuh.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://sg.szxytkj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sb.bookmarksfly.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vk.haigaiapp.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bn.huixiangedu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zx.huixinmuqiang.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qf.huixiangedu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pi.gzmigu.cn

[A10] 生成随机数
来源：http://rj.haigaiapp.cn

Py:   import random; random.randint(1, 100)
来源：http://ba.huixinmuqiang.cn

PHP:  random_int(1, 100);
来源：http://pn.nicolike.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gd.huanxung.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vp.bjjhwx.cn

Java: new Random().nextInt(100) + 1
来源：http://fr.yuexingan06.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hm.jctech888.com.cn

Ruby: rand(1..100)
来源：http://dw.lnxyls.cn

C#:   new Random().Next(1, 101)
来源：http://bw.shxzukj.cn

[A11] 条件表达式（三元）
来源：http://in.asd995.cn

Py:   "yes" if x > 0 else "no"
来源：http://ol.chemitech.net.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cn.asd995.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ns.panjiajie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://as.huixiangedu.cn

Java: x > 0 ? "yes" : "no"
来源：http://jx.hnjuh.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://we.hnjuh.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ow.wgjwhj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://dx.gzmigu.cn

[A12] 字符串插值 / 格式化
来源：http://hn.jianghongdianzi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lx.asd995.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://td.gzmigu.cn

JS:   `Hello, ${name}!`
来源：http://rw.nicolike.cn

TS:   `Hello, ${name}!`
来源：http://to.lnxyls.cn

Java: "Hello, %s!".formatted(name)
来源：http://xd.shxzskj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://la.shxzukj.cn

Ruby: "Hello, #{name}!"
来源：http://dw.shxzskj.cn

C#:   $"Hello, {name}!"
来源：http://ls.yuexingan06.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://aq.shxzskj.cn

Py:   "第一行\n第二行"
来源：http://jc.nicolike.cn

PHP:  "第一行\n第二行"
来源：http://nr.huanxung.cn

JS:   "第一行\n第二行"
来源：http://hv.muxihuayi.cn

TS:   "第一行\n第二行"
来源：http://tb.asd995.cn

Java: "第一行\n第二行"
来源：http://pt.nszjky.cn

Go:   "第一行\n第二行"
来源：http://bl.shxzskj.cn

Ruby: "第一行\n第二行"
来源：http://vp.lnxyls.cn

C#:   "第一行\n第二行"
来源：http://bb.hahajie.cn

[A14] 注释写法
来源：http://rj.jianghongdianzi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://zh.huixinmuqiang.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://zr.shxzskj.cn

JS:   // 单行；/* 多行 */
来源：http://co.9csxet.cn

TS:   // 单行；/* 多行 */
来源：http://la.szxytkj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://id.szxytkj.cn

Go:   // 单行；/* 多行 */
来源：http://yx.lnxyls.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rf.nicolike.cn

C#:   // 单行；/* 多行 */
来源：http://np.szxytkj.cn

[A15] 空值判断与默认值
来源：http://no.chemitech.net.cn

Py:   value = data or "默认值"
来源：http://pm.shxzukj.cn

PHP:  $value = $data ?? "默认值";
来源：http://so.bookmarksfly.cn

JS:   const value = data ?? "默认值";
来源：http://sq.9csxet.cn

TS:   const value = data ?? "默认值";
来源：http://ns.huixinmuqiang.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tn.hnjuh.cn

Go:   if data == "" { data = "默认值" }
来源：http://hu.chemitech.net.cn

Ruby: value = data || "默认值"
来源：http://jk.huixiangedu.cn

C#:   var value = data ?? "默认值";
来源：http://he.wgjwhj.cn

[A16] 真假值判断规则
来源：http://we.shtwfgs.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jr.huixiangedu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kf.hahajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://us.chemitech.net.cn

TS:   if (!x) {}
来源：http://pr.szsharing.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qf.yuntaijiaju.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://th.szsharing.cn

Ruby: unless x            # nil 与 false 为假
来源：http://nc.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hq.jctech888.com.cn

[A17] 位运算
来源：http://fx.lnxyls.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ne.panjiajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jd.wgjwhj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lb.haigaiapp.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://se.huixiangedu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hh.muxihuayi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://so.hnjuh.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ke.szsharing.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xn.bjjhwx.cn

[A18] 字符与 ASCII 码互转
来源：http://mw.bookmarksfly.cn

Py:   ord("A"); chr(65)
来源：http://lm.gzmigu.cn

PHP:  ord("A"); chr(65)
来源：http://bk.jianghongdianzi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dt.yuntaijiaju.cn


<!-- 参考信息 -->