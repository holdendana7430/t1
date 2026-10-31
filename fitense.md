代发 wailian999

[U105] JS：节流
来源：http://xj.haigaiapp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lm.yuexingan06.cn

[U106] JS：日期格式化
来源：http://kp.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ql.haigaiapp.cn

[U107] JS：数字千分位
来源：http://nm.nszjky.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zd.bjjhwx.cn

[U108] JS：随机整数
来源：http://vb.newstarts.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wf.chemitech.net.cn

[U109] JS：数组分组
来源：http://oz.hahajie.cn

Object.groupBy(arr, x => x.type)
来源：http://pp.yuexingan06.cn

[U110] JS：数组分块
来源：http://pq.huixinmuqiang.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pm.shxzukj.cn

[U111] JS：对象转 Map
来源：http://jg.muxihuayi.cn

new Map(Object.entries(obj))
来源：http://si.muxihuayi.cn

[U112] JS：字符串补位
来源：http://su.shxzskj.cn

"7".padStart(3, "0")
来源：http://iz.muxihuayi.cn

[U113] JS：正则替换全部
来源：http://zx.wgjwhj.cn

s.replaceAll("a", "b")
来源：http://cc.jianghongdianzi.cn

[U114] JS：JSON 深比较
来源：http://iq.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://bq.huanxung.cn

[U115] JS：生成 UUID
来源：http://lj.hnjuh.cn

crypto.randomUUID()
来源：http://pg.9csxet.cn

[U116] JS：类型检查（JSDoc）
来源：http://ko.szsharing.cn

/** @param {string} name */ function f(name) {}
来源：http://of.panjiajie.cn

[U117] JS：单元测试
来源：http://pu.shxzukj.cn

npm i -D vitest;  npx vitest
来源：http://dj.asd995.cn

[U118] JS：开发服务器
来源：http://uk.9csxet.cn

npm i -D vite;  npx vite
来源：http://fz.yuntaijiaju.cn

[U119] JS：生产构建
来源：http://zq.shtwfgs.cn

npx vite build
来源：http://fc.nszjky.cn

[U120] JS：读取环境变量（Vite）
来源：http://zu.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://mc.hahajie.cn

================================================================================
来源：http://hv.haigaiapp.cn

统计汇总
来源：http://mx.shtwfgs.cn

================================================================================
来源：http://if.chemitech.net.cn

按语言统计（条）：
来源：http://yq.szsharing.cn

Python ......... 252
来源：http://vj.9csxet.cn

PHP ............ 252
来源：http://gh.szsharing.cn

JavaScript ..... 252
来源：http://rr.szxytkj.cn

TypeScript ..... 212
来源：http://ku.bookmarksfly.cn

Java ........... 212
来源：http://xw.hnjuh.cn

Go ............. 212
来源：http://ep.shxzukj.cn

Ruby ........... 212
来源：http://ux.bjjhwx.cn

C# ............. 212
来源：http://uv.chemitech.net.cn

C .............. 30
来源：http://dj.521024.cn

C++ ............ 30
来源：http://em.nszjky.cn

SQL ............ 90
来源：http://sa.nicolike.cn

Bash ........... 80
来源：http://bo.newstarts.cn

Kotlin ......... 15
来源：http://cu.yuntaijiaju.cn

Swift .......... 15
来源：http://hw.bjjhwx.cn

Lua ............ 10
来源：http://lj.newstarts.cn

Perl ........... 10
来源：http://xe.panjiajie.cn

Scala .......... 10
来源：http://sk.bookmarksfly.cn

------------------------------------
来源：http://dl.shxzskj.cn

合计 ........... 2106 条
来源：http://wf.huixiangedu.cn

按章节统计：
来源：http://fb.bjjhwx.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sn.bookmarksfly.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fh.bjjhwx.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://np.lnxyls.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ue.huixinmuqiang.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dg.gzmigu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ug.shtwfgs.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ru.bjjhwx.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kl.shxzukj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kc.haigaiapp.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rq.szsharing.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cp.bookmarksfly.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ka.lnxyls.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qx.nicolike.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pp.lnxyls.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lm.yuexingan06.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://to.521024.cn

Q SQL 专题                              90
来源：http://xb.lnxyls.cn

R Bash 专题                             80
来源：http://ug.shxzukj.cn

S C / C++ 专题                          60
来源：http://ge.bjjhwx.cn

T 其他语言补充                          60
来源：http://nl.asd995.cn

U 高频实用片段                         120
来源：http://bd.jctech888.com.cn

------------------------------------
来源：http://zz.shxzukj.cn

合计                                  2106 条
来源：http://vi.nicolike.cn

--------------------------------------------------------------------------------
来源：http://sk.panjiajie.cn

使用提醒
来源：http://nj.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://pj.chemitech.net.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jt.9csxet.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gf.nicolike.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cu.lnxyls.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://hd.yuntaijiaju.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ht.gzmigu.cn

—— 文件结束 ——
来源：http://jk.nszjky.cn

================================================================================
来源：http://rg.yuntaijiaju.cn

程序语言常见例子速查手册（2024 版）
来源：http://wy.shxzukj.cn

Common Programming Examples Cheat Book
来源：http://mc.szsharing.cn

================================================================================
来源：http://zu.gzmigu.cn

【收录内容】
来源：http://ge.gzmigu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://la.shxzskj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sz.yuntaijiaju.cn

SQL · Bash · C · C++
来源：http://er.yuexingan06.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uf.jianghongdianzi.cn

【使用说明】
来源：http://wo.jctech888.com.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sp.yuexingan06.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rj.shxzukj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ok.521024.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://up.yuexingan06.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://bn.szxytkj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nm.shxzskj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://oh.hnjuh.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xt.hahajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ox.hahajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lu.colortex.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bn.jianghongdianzi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://db.yuntaijiaju.cn

【文件统计】
来源：http://az.gzmigu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pe.9csxet.cn

--------------------------------------------------------------------------------
来源：http://mo.szxytkj.cn

目  录
来源：http://tx.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://sf.bjjhwx.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gs.nszjky.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bl.shxzskj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fy.jctech888.com.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xp.huixinmuqiang.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mb.panjiajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yc.szxytkj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://no.szsharing.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xf.shxzukj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sd.huanxung.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ax.shtwfgs.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fi.yuexingan06.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://le.szxytkj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://co.hnjuh.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tx.shxzukj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zh.haigaiapp.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yb.9csxet.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pj.szsharing.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ql.gzmigu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ag.shxzukj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qm.lnxyls.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://av.shxzukj.cn

================================================================================
来源：http://yy.nszjky.cn

A. 基础语法与类型
来源：http://qt.newstarts.cn

================================================================================
来源：http://wv.shxzukj.cn

[A01] Hello World
来源：http://xr.shtwfgs.cn

Py:   print("Hello, World!")
来源：http://kc.panjiajie.cn

PHP:  echo "Hello, World!";
来源：http://el.newstarts.cn

JS:   console.log("Hello, World!");
来源：http://lg.bjjhwx.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qb.muxihuayi.cn

Java: System.out.println("Hello, World!");
来源：http://dz.yuntaijiaju.cn

Go:   fmt.Println("Hello, World!")
来源：http://gc.9csxet.cn

Ruby: puts "Hello, World!"
来源：http://ki.bookmarksfly.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://bg.szsharing.cn

[A02] 变量声明与赋值
来源：http://nu.shxzskj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://eb.lnxyls.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ts.shtwfgs.cn

JS:   let name = "Alex"; const age = 20;
来源：http://gg.bjjhwx.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sj.bjjhwx.cn

Java: String name = "Alex"; int age = 20;
来源：http://sv.huixiangedu.cn

Go:   name := "Alex"; age := 20
来源：http://ev.colortex.cn

Ruby: name = "Alex"; age = 20
来源：http://nz.nicolike.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ig.huixinmuqiang.cn

[A03] 常量定义
来源：http://zz.haigaiapp.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fi.panjiajie.cn

PHP:  const PI = 3.14159;
来源：http://kh.yuexingan06.cn

JS:   const PI = 3.14159;
来源：http://kz.shtwfgs.cn

TS:   const PI: number = 3.14159;
来源：http://ok.newstarts.cn

Java: static final double PI = 3.14159;
来源：http://pe.shtwfgs.cn

Go:   const PI = 3.14159
来源：http://ek.521024.cn

Ruby: PI = 3.14159
来源：http://ot.yuntaijiaju.cn

C#:   const double PI = 3.14159;
来源：http://zm.shxzukj.cn

[A04] 判断变量类型
来源：http://js.newstarts.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hx.chemitech.net.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lz.shxzukj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xr.jianghongdianzi.cn

TS:   typeof x; x instanceof Date
来源：http://pw.wgjwhj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bu.bjjhwx.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ln.wgjwhj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://dm.gzmigu.cn

C#:   x.GetType().Name; x is int
来源：http://tm.chemitech.net.cn

[A05] 整数除法与取模
来源：http://wu.yuntaijiaju.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rr.asd995.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ji.panjiajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://we.huixiangedu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ho.bjjhwx.cn

Java: 7 / 2; 7 % 2
来源：http://sk.9csxet.cn

Go:   7 / 2; 7 % 2
来源：http://cf.gzmigu.cn

Ruby: 7 / 2; 7 % 2
来源：http://oe.hahajie.cn

C#:   7 / 2; 7 % 2
来源：http://be.haigaiapp.cn

[A06] 字符串转数字
来源：http://dg.asd995.cn

Py:   int("42"); float("3.14")
来源：http://fv.jianghongdianzi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nt.haigaiapp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bg.newstarts.cn

TS:   parseInt("42", 10); Number("42")
来源：http://bo.bjjhwx.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hj.haigaiapp.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uq.521024.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://iw.huixinmuqiang.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yg.shxzukj.cn

[A07] 数字转字符串
来源：http://cv.gzmigu.cn

Py:   str(42)
来源：http://eh.bjjhwx.cn

PHP:  (string) 42; strval(42)
来源：http://ym.nszjky.cn

JS:   String(42); (42).toString()
来源：http://ty.lnxyls.cn

TS:   String(42)
来源：http://xb.jctech888.com.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://yk.asd995.cn

Go:   strconv.Itoa(42)
来源：http://ez.nszjky.cn

Ruby: 42.to_s
来源：http://pg.shxzukj.cn

C#:   42.ToString()
来源：http://sl.newstarts.cn

[A08] 取整与四舍五入
来源：http://de.yuntaijiaju.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://du.hnjuh.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fq.shxzukj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kp.shxzukj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vi.newstarts.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rp.521024.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://no.yuntaijiaju.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mw.newstarts.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ph.gzmigu.cn

[A09] 绝对值与最大最小值
来源：http://pz.muxihuayi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ep.muxihuayi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zg.shxzukj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tv.szsharing.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://dz.521024.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hg.szxytkj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cb.szxytkj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lh.colortex.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ev.521024.cn

[A10] 生成随机数
来源：http://af.chemitech.net.cn

Py:   import random; random.randint(1, 100)
来源：http://un.nicolike.cn

PHP:  random_int(1, 100);
来源：http://il.haigaiapp.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://to.yuexingan06.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://uv.bjjhwx.cn

Java: new Random().nextInt(100) + 1
来源：http://wg.shtwfgs.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xd.yuexingan06.cn

Ruby: rand(1..100)
来源：http://ab.gzmigu.cn

C#:   new Random().Next(1, 101)
来源：http://gw.wgjwhj.cn

[A11] 条件表达式（三元）
来源：http://xk.nicolike.cn

Py:   "yes" if x > 0 else "no"
来源：http://fy.huixinmuqiang.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://et.szxytkj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://jt.nicolike.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dl.colortex.cn

Java: x > 0 ? "yes" : "no"
来源：http://hg.bjjhwx.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zl.szxytkj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://oj.shtwfgs.cn

C#:   x > 0 ? "yes" : "no"
来源：http://mf.bjjhwx.cn

[A12] 字符串插值 / 格式化
来源：http://pn.szsharing.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jc.hahajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://il.haigaiapp.cn

JS:   `Hello, ${name}!`
来源：http://bk.chemitech.net.cn

TS:   `Hello, ${name}!`
来源：http://qc.newstarts.cn

Java: "Hello, %s!".formatted(name)
来源：http://ul.panjiajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://by.chemitech.net.cn

Ruby: "Hello, #{name}!"
来源：http://rh.huixinmuqiang.cn

C#:   $"Hello, {name}!"
来源：http://ly.newstarts.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hi.muxihuayi.cn

Py:   "第一行\n第二行"
来源：http://rg.521024.cn

PHP:  "第一行\n第二行"
来源：http://bg.nicolike.cn

JS:   "第一行\n第二行"
来源：http://kw.huixiangedu.cn

TS:   "第一行\n第二行"
来源：http://mb.bookmarksfly.cn

Java: "第一行\n第二行"
来源：http://wg.jctech888.com.cn

Go:   "第一行\n第二行"
来源：http://dr.panjiajie.cn

Ruby: "第一行\n第二行"
来源：http://fs.521024.cn

C#:   "第一行\n第二行"
来源：http://xi.chemitech.net.cn

[A14] 注释写法
来源：http://xz.chemitech.net.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ev.nicolike.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://nv.asd995.cn

JS:   // 单行；/* 多行 */
来源：http://rc.huanxung.cn

TS:   // 单行；/* 多行 */
来源：http://ln.szxytkj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zs.panjiajie.cn

Go:   // 单行；/* 多行 */
来源：http://sf.hahajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wp.muxihuayi.cn

C#:   // 单行；/* 多行 */
来源：http://to.shxzukj.cn

[A15] 空值判断与默认值
来源：http://si.huixinmuqiang.cn

Py:   value = data or "默认值"
来源：http://ek.huanxung.cn

PHP:  $value = $data ?? "默认值";
来源：http://tn.muxihuayi.cn

JS:   const value = data ?? "默认值";
来源：http://eu.jctech888.com.cn

TS:   const value = data ?? "默认值";
来源：http://vr.nicolike.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vz.gzmigu.cn

Go:   if data == "" { data = "默认值" }
来源：http://bs.bookmarksfly.cn

Ruby: value = data || "默认值"
来源：http://yi.nszjky.cn

C#:   var value = data ?? "默认值";
来源：http://lv.gzmigu.cn

[A16] 真假值判断规则
来源：http://pz.huanxung.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://sa.shxzskj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ns.521024.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sd.newstarts.cn

TS:   if (!x) {}
来源：http://gf.shtwfgs.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kr.huanxung.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zm.yuexingan06.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ty.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://or.yuntaijiaju.cn

[A17] 位运算
来源：http://qs.521024.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ek.bookmarksfly.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rr.huixiangedu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oz.shtwfgs.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pp.gzmigu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ez.szsharing.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ow.nicolike.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lr.jctech888.com.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yd.jianghongdianzi.cn

[A18] 字符与 ASCII 码互转
来源：http://jp.muxihuayi.cn

Py:   ord("A"); chr(65)
来源：http://zh.chemitech.net.cn

PHP:  ord("A"); chr(65)
来源：http://mh.haigaiapp.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lo.521024.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kl.wgjwhj.cn

Java: (int) 'A'; (char) 65
来源：http://vp.nicolike.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jk.colortex.cn

Ruby: "A".ord; 65.chr
来源：http://vv.huixiangedu.cn


<!-- 参考信息 -->