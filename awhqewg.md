代发 wailian999

[U105] JS：节流
来源：http://kh.shxzskj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fi.hnjuh.cn

[U106] JS：日期格式化
来源：http://pu.szsharing.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://db.jctech888.com.cn

[U107] JS：数字千分位
来源：http://et.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://iv.colortex.cn

[U108] JS：随机整数
来源：http://kz.gzmigu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ql.huixiangedu.cn

[U109] JS：数组分组
来源：http://qc.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://tw.szsharing.cn

[U110] JS：数组分块
来源：http://kt.shxzukj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dm.panjiajie.cn

[U111] JS：对象转 Map
来源：http://ox.hahajie.cn

new Map(Object.entries(obj))
来源：http://ur.wgjwhj.cn

[U112] JS：字符串补位
来源：http://em.wgjwhj.cn

"7".padStart(3, "0")
来源：http://gq.shxzukj.cn

[U113] JS：正则替换全部
来源：http://ro.colortex.cn

s.replaceAll("a", "b")
来源：http://ju.shtwfgs.cn

[U114] JS：JSON 深比较
来源：http://cm.9csxet.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ub.yuntaijiaju.cn

[U115] JS：生成 UUID
来源：http://hq.shtwfgs.cn

crypto.randomUUID()
来源：http://rw.haigaiapp.cn

[U116] JS：类型检查（JSDoc）
来源：http://kv.haigaiapp.cn

/** @param {string} name */ function f(name) {}
来源：http://it.nicolike.cn

[U117] JS：单元测试
来源：http://di.9csxet.cn

npm i -D vitest;  npx vitest
来源：http://ea.colortex.cn

[U118] JS：开发服务器
来源：http://bd.yuntaijiaju.cn

npm i -D vite;  npx vite
来源：http://rc.huixinmuqiang.cn

[U119] JS：生产构建
来源：http://pu.nszjky.cn

npx vite build
来源：http://pa.chemitech.net.cn

[U120] JS：读取环境变量（Vite）
来源：http://wa.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://us.jctech888.com.cn

================================================================================
来源：http://xg.shxzskj.cn

统计汇总
来源：http://tw.szsharing.cn

================================================================================
来源：http://hk.huixiangedu.cn

按语言统计（条）：
来源：http://eg.newstarts.cn

Python ......... 252
来源：http://bc.szxytkj.cn

PHP ............ 252
来源：http://iw.wgjwhj.cn

JavaScript ..... 252
来源：http://vf.shxzukj.cn

TypeScript ..... 212
来源：http://ro.haigaiapp.cn

Java ........... 212
来源：http://wk.asd995.cn

Go ............. 212
来源：http://mz.gzmigu.cn

Ruby ........... 212
来源：http://po.shxzukj.cn

C# ............. 212
来源：http://ea.shxzukj.cn

C .............. 30
来源：http://zj.huixinmuqiang.cn

C++ ............ 30
来源：http://bl.szsharing.cn

SQL ............ 90
来源：http://uv.bjjhwx.cn

Bash ........... 80
来源：http://lm.jianghongdianzi.cn

Kotlin ......... 15
来源：http://vq.haigaiapp.cn

Swift .......... 15
来源：http://un.bookmarksfly.cn

Lua ............ 10
来源：http://qg.hahajie.cn

Perl ........... 10
来源：http://js.panjiajie.cn

Scala .......... 10
来源：http://sa.colortex.cn

------------------------------------
来源：http://tj.nicolike.cn

合计 ........... 2106 条
来源：http://tk.bjjhwx.cn

按章节统计：
来源：http://ou.huixiangedu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://te.bookmarksfly.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://em.9csxet.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sn.bjjhwx.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lr.muxihuayi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jq.nszjky.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://er.hnjuh.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://da.yuntaijiaju.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wn.jianghongdianzi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rv.colortex.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://iq.colortex.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pg.hahajie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mf.9csxet.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kc.bjjhwx.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ft.gzmigu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sa.nicolike.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tx.bjjhwx.cn

Q SQL 专题                              90
来源：http://ld.nicolike.cn

R Bash 专题                             80
来源：http://fh.521024.cn

S C / C++ 专题                          60
来源：http://ap.jctech888.com.cn

T 其他语言补充                          60
来源：http://tx.hnjuh.cn

U 高频实用片段                         120
来源：http://hz.chemitech.net.cn

------------------------------------
来源：http://cn.yuexingan06.cn

合计                                  2106 条
来源：http://qx.521024.cn

--------------------------------------------------------------------------------
来源：http://zp.newstarts.cn

使用提醒
来源：http://iw.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://zl.chemitech.net.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ii.nicolike.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nu.lnxyls.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kp.haigaiapp.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ld.hahajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ov.shtwfgs.cn

—— 文件结束 ——
来源：http://np.jianghongdianzi.cn

================================================================================
来源：http://tf.newstarts.cn

程序语言常见例子速查手册（2024 版）
来源：http://qp.huanxung.cn

Common Programming Examples Cheat Book
来源：http://nb.wgjwhj.cn

================================================================================
来源：http://gx.szsharing.cn

【收录内容】
来源：http://se.newstarts.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://hb.yuntaijiaju.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jm.nszjky.cn

SQL · Bash · C · C++
来源：http://vz.lnxyls.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://df.asd995.cn

【使用说明】
来源：http://uo.jianghongdianzi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gw.wgjwhj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ym.chemitech.net.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tm.szxytkj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zr.huixiangedu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://yy.colortex.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pz.szsharing.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vk.shxzskj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xw.bjjhwx.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jv.jianghongdianzi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://he.szsharing.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dv.huixiangedu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://iv.newstarts.cn

【文件统计】
来源：http://bf.9csxet.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cv.newstarts.cn

--------------------------------------------------------------------------------
来源：http://ez.shxzukj.cn

目  录
来源：http://fq.nszjky.cn

--------------------------------------------------------------------------------
来源：http://le.521024.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cm.bookmarksfly.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zb.hnjuh.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://oj.szsharing.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pp.lnxyls.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qc.asd995.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pv.shxzukj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ef.szxytkj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jg.muxihuayi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pe.newstarts.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jl.9csxet.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tx.huixinmuqiang.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://tt.huixiangedu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zr.bookmarksfly.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lm.hahajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jh.newstarts.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zr.huixiangedu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wm.nszjky.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vz.lnxyls.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rn.huanxung.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lg.szxytkj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vt.521024.cn

================================================================================
来源：http://an.yuexingan06.cn

A. 基础语法与类型
来源：http://lu.colortex.cn

================================================================================
来源：http://mf.chemitech.net.cn

[A01] Hello World
来源：http://bn.shtwfgs.cn

Py:   print("Hello, World!")
来源：http://cn.shxzukj.cn

PHP:  echo "Hello, World!";
来源：http://rz.huanxung.cn

JS:   console.log("Hello, World!");
来源：http://qc.gzmigu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://uw.hahajie.cn

Java: System.out.println("Hello, World!");
来源：http://fu.nicolike.cn

Go:   fmt.Println("Hello, World!")
来源：http://ls.panjiajie.cn

Ruby: puts "Hello, World!"
来源：http://iv.huixinmuqiang.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://hg.bjjhwx.cn

[A02] 变量声明与赋值
来源：http://vj.yuexingan06.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hs.shxzskj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://jo.yuexingan06.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ck.jianghongdianzi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lf.huanxung.cn

Java: String name = "Alex"; int age = 20;
来源：http://de.haigaiapp.cn

Go:   name := "Alex"; age := 20
来源：http://yn.colortex.cn

Ruby: name = "Alex"; age = 20
来源：http://qw.jianghongdianzi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://vo.9csxet.cn

[A03] 常量定义
来源：http://fu.szxytkj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rq.nszjky.cn

PHP:  const PI = 3.14159;
来源：http://ub.hnjuh.cn

JS:   const PI = 3.14159;
来源：http://yx.lnxyls.cn

TS:   const PI: number = 3.14159;
来源：http://ij.panjiajie.cn

Java: static final double PI = 3.14159;
来源：http://px.asd995.cn

Go:   const PI = 3.14159
来源：http://bz.szsharing.cn

Ruby: PI = 3.14159
来源：http://lp.9csxet.cn

C#:   const double PI = 3.14159;
来源：http://bl.muxihuayi.cn

[A04] 判断变量类型
来源：http://aa.bjjhwx.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://wx.szsharing.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://me.nszjky.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nb.colortex.cn

TS:   typeof x; x instanceof Date
来源：http://ul.bjjhwx.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fu.muxihuayi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://dp.nszjky.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://rt.521024.cn

C#:   x.GetType().Name; x is int
来源：http://cz.yuntaijiaju.cn

[A05] 整数除法与取模
来源：http://mg.lnxyls.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vd.huanxung.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gf.szsharing.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bj.nicolike.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gf.huixinmuqiang.cn

Java: 7 / 2; 7 % 2
来源：http://vr.9csxet.cn

Go:   7 / 2; 7 % 2
来源：http://ma.lnxyls.cn

Ruby: 7 / 2; 7 % 2
来源：http://ev.yuexingan06.cn

C#:   7 / 2; 7 % 2
来源：http://ww.asd995.cn

[A06] 字符串转数字
来源：http://jx.hnjuh.cn

Py:   int("42"); float("3.14")
来源：http://sk.lnxyls.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jx.huanxung.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://py.nszjky.cn

TS:   parseInt("42", 10); Number("42")
来源：http://tq.huanxung.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ag.gzmigu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zv.jctech888.com.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wo.lnxyls.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sl.yuntaijiaju.cn

[A07] 数字转字符串
来源：http://vj.colortex.cn

Py:   str(42)
来源：http://rs.bjjhwx.cn

PHP:  (string) 42; strval(42)
来源：http://re.wgjwhj.cn

JS:   String(42); (42).toString()
来源：http://wf.szxytkj.cn

TS:   String(42)
来源：http://gk.shxzukj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bf.9csxet.cn

Go:   strconv.Itoa(42)
来源：http://gq.yuexingan06.cn

Ruby: 42.to_s
来源：http://df.asd995.cn

C#:   42.ToString()
来源：http://dh.521024.cn

[A08] 取整与四舍五入
来源：http://iw.panjiajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tv.chemitech.net.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kj.wgjwhj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wh.panjiajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sg.muxihuayi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kh.gzmigu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://be.wgjwhj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://sv.muxihuayi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wq.huixinmuqiang.cn

[A09] 绝对值与最大最小值
来源：http://ux.hahajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://or.szxytkj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mq.bjjhwx.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sd.huanxung.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tq.szxytkj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rb.shxzskj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gu.nszjky.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ec.jianghongdianzi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qe.shxzskj.cn

[A10] 生成随机数
来源：http://cs.newstarts.cn

Py:   import random; random.randint(1, 100)
来源：http://ad.shxzskj.cn

PHP:  random_int(1, 100);
来源：http://tu.muxihuayi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nx.shxzukj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zo.huanxung.cn

Java: new Random().nextInt(100) + 1
来源：http://wn.haigaiapp.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ug.wgjwhj.cn

Ruby: rand(1..100)
来源：http://ve.gzmigu.cn

C#:   new Random().Next(1, 101)
来源：http://qe.nszjky.cn

[A11] 条件表达式（三元）
来源：http://yw.bjjhwx.cn

Py:   "yes" if x > 0 else "no"
来源：http://uc.muxihuayi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://jy.chemitech.net.cn

JS:   x > 0 ? "yes" : "no"
来源：http://oe.chemitech.net.cn

TS:   x > 0 ? "yes" : "no"
来源：http://nb.huixinmuqiang.cn

Java: x > 0 ? "yes" : "no"
来源：http://am.huixiangedu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://bn.szxytkj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://em.haigaiapp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://cu.hnjuh.cn

[A12] 字符串插值 / 格式化
来源：http://or.gzmigu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rs.wgjwhj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hd.huixinmuqiang.cn

JS:   `Hello, ${name}!`
来源：http://lx.newstarts.cn

TS:   `Hello, ${name}!`
来源：http://dd.szsharing.cn

Java: "Hello, %s!".formatted(name)
来源：http://tg.bjjhwx.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wp.huixiangedu.cn

Ruby: "Hello, #{name}!"
来源：http://ca.hahajie.cn

C#:   $"Hello, {name}!"
来源：http://yr.521024.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://up.521024.cn

Py:   "第一行\n第二行"
来源：http://cr.shxzskj.cn

PHP:  "第一行\n第二行"
来源：http://gq.panjiajie.cn

JS:   "第一行\n第二行"
来源：http://tk.asd995.cn

TS:   "第一行\n第二行"
来源：http://gb.521024.cn

Java: "第一行\n第二行"
来源：http://ga.gzmigu.cn

Go:   "第一行\n第二行"
来源：http://hx.yuntaijiaju.cn

Ruby: "第一行\n第二行"
来源：http://wz.shxzskj.cn

C#:   "第一行\n第二行"
来源：http://gk.bookmarksfly.cn

[A14] 注释写法
来源：http://tl.wgjwhj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://hr.hnjuh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://gp.wgjwhj.cn

JS:   // 单行；/* 多行 */
来源：http://xr.jctech888.com.cn

TS:   // 单行；/* 多行 */
来源：http://xw.chemitech.net.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ll.9csxet.cn

Go:   // 单行；/* 多行 */
来源：http://zy.muxihuayi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://mi.gzmigu.cn

C#:   // 单行；/* 多行 */
来源：http://rj.colortex.cn

[A15] 空值判断与默认值
来源：http://ok.shxzukj.cn

Py:   value = data or "默认值"
来源：http://ek.nszjky.cn

PHP:  $value = $data ?? "默认值";
来源：http://lp.wgjwhj.cn

JS:   const value = data ?? "默认值";
来源：http://bg.hahajie.cn

TS:   const value = data ?? "默认值";
来源：http://vg.lnxyls.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fd.shxzskj.cn

Go:   if data == "" { data = "默认值" }
来源：http://oo.hnjuh.cn

Ruby: value = data || "默认值"
来源：http://hf.colortex.cn

C#:   var value = data ?? "默认值";
来源：http://zd.szxytkj.cn

[A16] 真假值判断规则
来源：http://ig.hahajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ir.wgjwhj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ih.huanxung.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ay.shxzukj.cn

TS:   if (!x) {}
来源：http://yk.colortex.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wo.yuexingan06.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wk.yuexingan06.cn

Ruby: unless x            # nil 与 false 为假
来源：http://yj.szsharing.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fi.szsharing.cn

[A17] 位运算
来源：http://ab.muxihuayi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dy.huixinmuqiang.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://of.huixinmuqiang.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://go.bookmarksfly.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pg.szsharing.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gy.huixinmuqiang.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tf.nszjky.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oo.bookmarksfly.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://se.chemitech.net.cn

[A18] 字符与 ASCII 码互转
来源：http://bq.asd995.cn

Py:   ord("A"); chr(65)
来源：http://ld.nicolike.cn

PHP:  ord("A"); chr(65)
来源：http://fo.nszjky.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lf.szxytkj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ip.shxzskj.cn

Java: (int) 'A'; (char) 65
来源：http://ct.nicolike.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rp.yuexingan06.cn

Ruby: "A".ord; 65.chr
来源：http://xy.nicolike.cn


<!-- 参考信息 -->