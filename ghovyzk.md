代发 wailian999

[U103] JS：定时器
来源：http://ej.9csxet.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://za.haigaiapp.cn

[U104] JS：防抖
来源：http://dq.521024.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qa.gzmigu.cn

[U105] JS：节流
来源：http://gs.colortex.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zt.shxzskj.cn

[U106] JS：日期格式化
来源：http://hn.colortex.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wi.huanxung.cn

[U107] JS：数字千分位
来源：http://mi.huanxung.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hx.9csxet.cn

[U108] JS：随机整数
来源：http://sd.jctech888.com.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yw.nicolike.cn

[U109] JS：数组分组
来源：http://bv.yuntaijiaju.cn

Object.groupBy(arr, x => x.type)
来源：http://tp.szsharing.cn

[U110] JS：数组分块
来源：http://dz.shxzukj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kk.haigaiapp.cn

[U111] JS：对象转 Map
来源：http://xe.9csxet.cn

new Map(Object.entries(obj))
来源：http://uj.yuexingan06.cn

[U112] JS：字符串补位
来源：http://zt.muxihuayi.cn

"7".padStart(3, "0")
来源：http://zg.colortex.cn

[U113] JS：正则替换全部
来源：http://my.muxihuayi.cn

s.replaceAll("a", "b")
来源：http://yw.muxihuayi.cn

[U114] JS：JSON 深比较
来源：http://qo.huixiangedu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rd.chemitech.net.cn

[U115] JS：生成 UUID
来源：http://cz.jctech888.com.cn

crypto.randomUUID()
来源：http://bx.hahajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://bn.yuntaijiaju.cn

/** @param {string} name */ function f(name) {}
来源：http://ho.hnjuh.cn

[U117] JS：单元测试
来源：http://bi.szxytkj.cn

npm i -D vitest;  npx vitest
来源：http://br.asd995.cn

[U118] JS：开发服务器
来源：http://ec.huixiangedu.cn

npm i -D vite;  npx vite
来源：http://nc.nszjky.cn

[U119] JS：生产构建
来源：http://rv.jianghongdianzi.cn

npx vite build
来源：http://zn.szsharing.cn

[U120] JS：读取环境变量（Vite）
来源：http://eq.bookmarksfly.cn

import.meta.env.VITE_API_URL
来源：http://wz.shxzukj.cn

================================================================================
来源：http://wi.yuexingan06.cn

统计汇总
来源：http://rb.521024.cn

================================================================================
来源：http://im.muxihuayi.cn

按语言统计（条）：
来源：http://en.shtwfgs.cn

Python ......... 252
来源：http://xt.lnxyls.cn

PHP ............ 252
来源：http://su.chemitech.net.cn

JavaScript ..... 252
来源：http://ih.9csxet.cn

TypeScript ..... 212
来源：http://fh.wgjwhj.cn

Java ........... 212
来源：http://ax.nicolike.cn

Go ............. 212
来源：http://sh.bookmarksfly.cn

Ruby ........... 212
来源：http://pn.shtwfgs.cn

C# ............. 212
来源：http://lh.yuexingan06.cn

C .............. 30
来源：http://hh.huixinmuqiang.cn

C++ ............ 30
来源：http://ra.szxytkj.cn

SQL ............ 90
来源：http://kg.huixiangedu.cn

Bash ........... 80
来源：http://kq.yuntaijiaju.cn

Kotlin ......... 15
来源：http://mx.szsharing.cn

Swift .......... 15
来源：http://ue.lnxyls.cn

Lua ............ 10
来源：http://vi.521024.cn

Perl ........... 10
来源：http://uv.hahajie.cn

Scala .......... 10
来源：http://yx.huixinmuqiang.cn

------------------------------------
来源：http://mt.haigaiapp.cn

合计 ........... 2106 条
来源：http://sm.521024.cn

按章节统计：
来源：http://xq.hahajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pt.muxihuayi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yi.szsharing.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ou.shxzskj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ns.panjiajie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hy.bjjhwx.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kd.shxzukj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pk.hahajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mn.szsharing.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ec.newstarts.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wu.szxytkj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://up.521024.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fk.chemitech.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ja.colortex.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jy.wgjwhj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nq.jianghongdianzi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ef.wgjwhj.cn

Q SQL 专题                              90
来源：http://ix.shxzukj.cn

R Bash 专题                             80
来源：http://ml.yuntaijiaju.cn

S C / C++ 专题                          60
来源：http://fi.shxzukj.cn

T 其他语言补充                          60
来源：http://hm.chemitech.net.cn

U 高频实用片段                         120
来源：http://jh.shxzukj.cn

------------------------------------
来源：http://hm.szsharing.cn

合计                                  2106 条
来源：http://ye.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://qk.newstarts.cn

使用提醒
来源：http://bp.hahajie.cn

--------------------------------------------------------------------------------
来源：http://vv.wgjwhj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sd.muxihuayi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nf.nicolike.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://en.haigaiapp.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ze.asd995.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://sm.bookmarksfly.cn

—— 文件结束 ——
来源：http://ke.gzmigu.cn

================================================================================
来源：http://jl.newstarts.cn

程序语言常见例子速查手册（2024 版）
来源：http://gi.yuexingan06.cn

Common Programming Examples Cheat Book
来源：http://ek.asd995.cn

================================================================================
来源：http://yu.newstarts.cn

【收录内容】
来源：http://gm.wgjwhj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://mv.asd995.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jm.hahajie.cn

SQL · Bash · C · C++
来源：http://id.yuexingan06.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yf.newstarts.cn

【使用说明】
来源：http://fo.shxzskj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ue.muxihuayi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://px.newstarts.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vh.szsharing.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cu.asd995.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ni.hnjuh.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zb.huixinmuqiang.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pn.nicolike.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://os.colortex.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fj.521024.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ne.chemitech.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xf.shxzukj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ex.colortex.cn

【文件统计】
来源：http://wv.521024.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://db.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://oq.szxytkj.cn

目  录
来源：http://hn.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://mu.jianghongdianzi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ue.hnjuh.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rf.muxihuayi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xd.szxytkj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zw.shtwfgs.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tr.huixinmuqiang.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rr.newstarts.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jj.newstarts.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sv.huanxung.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ji.yuexingan06.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://po.shtwfgs.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://es.chemitech.net.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dg.jctech888.com.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ck.jianghongdianzi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://so.shxzskj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nn.muxihuayi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://db.lnxyls.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cm.nicolike.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ho.gzmigu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://up.nszjky.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://om.chemitech.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cx.haigaiapp.cn

================================================================================
来源：http://ho.nicolike.cn

A. 基础语法与类型
来源：http://kb.521024.cn

================================================================================
来源：http://jp.szsharing.cn

[A01] Hello World
来源：http://ls.newstarts.cn

Py:   print("Hello, World!")
来源：http://hu.nicolike.cn

PHP:  echo "Hello, World!";
来源：http://yr.yuntaijiaju.cn

JS:   console.log("Hello, World!");
来源：http://zu.shxzukj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://um.521024.cn

Java: System.out.println("Hello, World!");
来源：http://eq.wgjwhj.cn

Go:   fmt.Println("Hello, World!")
来源：http://cr.jianghongdianzi.cn

Ruby: puts "Hello, World!"
来源：http://ko.huixinmuqiang.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://pm.gzmigu.cn

[A02] 变量声明与赋值
来源：http://ro.nszjky.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tx.nicolike.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://jb.muxihuayi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://nv.bjjhwx.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ei.wgjwhj.cn

Java: String name = "Alex"; int age = 20;
来源：http://eq.521024.cn

Go:   name := "Alex"; age := 20
来源：http://up.wgjwhj.cn

Ruby: name = "Alex"; age = 20
来源：http://fm.shxzskj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://at.asd995.cn

[A03] 常量定义
来源：http://kn.yuntaijiaju.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mo.nszjky.cn

PHP:  const PI = 3.14159;
来源：http://ym.yuntaijiaju.cn

JS:   const PI = 3.14159;
来源：http://yg.huanxung.cn

TS:   const PI: number = 3.14159;
来源：http://dp.jianghongdianzi.cn

Java: static final double PI = 3.14159;
来源：http://lu.yuntaijiaju.cn

Go:   const PI = 3.14159
来源：http://nm.bjjhwx.cn

Ruby: PI = 3.14159
来源：http://fv.szsharing.cn

C#:   const double PI = 3.14159;
来源：http://jl.jctech888.com.cn

[A04] 判断变量类型
来源：http://ow.huixinmuqiang.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://pp.muxihuayi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://be.huixinmuqiang.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://iu.nszjky.cn

TS:   typeof x; x instanceof Date
来源：http://hq.wgjwhj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vk.huanxung.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ay.wgjwhj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://si.shxzskj.cn

C#:   x.GetType().Name; x is int
来源：http://qz.huixiangedu.cn

[A05] 整数除法与取模
来源：http://px.szxytkj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gw.lnxyls.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gp.shtwfgs.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://py.gzmigu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rl.newstarts.cn

Java: 7 / 2; 7 % 2
来源：http://db.haigaiapp.cn

Go:   7 / 2; 7 % 2
来源：http://ri.jctech888.com.cn

Ruby: 7 / 2; 7 % 2
来源：http://xc.shxzukj.cn

C#:   7 / 2; 7 % 2
来源：http://kb.shxzukj.cn

[A06] 字符串转数字
来源：http://yt.muxihuayi.cn

Py:   int("42"); float("3.14")
来源：http://df.521024.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wf.lnxyls.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://oo.colortex.cn

TS:   parseInt("42", 10); Number("42")
来源：http://qb.lnxyls.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wu.wgjwhj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xf.asd995.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ma.shtwfgs.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cd.szxytkj.cn

[A07] 数字转字符串
来源：http://si.newstarts.cn

Py:   str(42)
来源：http://lp.shtwfgs.cn

PHP:  (string) 42; strval(42)
来源：http://dv.chemitech.net.cn

JS:   String(42); (42).toString()
来源：http://dj.panjiajie.cn

TS:   String(42)
来源：http://wy.huixinmuqiang.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://dc.521024.cn

Go:   strconv.Itoa(42)
来源：http://xz.huanxung.cn

Ruby: 42.to_s
来源：http://oy.huixiangedu.cn

C#:   42.ToString()
来源：http://ox.huixiangedu.cn

[A08] 取整与四舍五入
来源：http://oz.panjiajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mt.shxzukj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://eu.colortex.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ff.nicolike.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jq.chemitech.net.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xt.newstarts.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://eg.asd995.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://jf.bjjhwx.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://en.huixiangedu.cn

[A09] 绝对值与最大最小值
来源：http://xp.bookmarksfly.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vw.bjjhwx.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://li.haigaiapp.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ru.huixiangedu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://os.hahajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ak.521024.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rs.yuexingan06.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://so.panjiajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gy.panjiajie.cn

[A10] 生成随机数
来源：http://fu.panjiajie.cn

Py:   import random; random.randint(1, 100)
来源：http://sa.bjjhwx.cn

PHP:  random_int(1, 100);
来源：http://ho.muxihuayi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gd.panjiajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://sh.jianghongdianzi.cn

Java: new Random().nextInt(100) + 1
来源：http://en.panjiajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rx.szsharing.cn

Ruby: rand(1..100)
来源：http://os.nicolike.cn

C#:   new Random().Next(1, 101)
来源：http://kp.wgjwhj.cn

[A11] 条件表达式（三元）
来源：http://kh.nicolike.cn

Py:   "yes" if x > 0 else "no"
来源：http://sk.muxihuayi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ds.521024.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rr.newstarts.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xg.gzmigu.cn

Java: x > 0 ? "yes" : "no"
来源：http://bb.lnxyls.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wf.521024.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://xu.shxzskj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://dr.bjjhwx.cn

[A12] 字符串插值 / 格式化
来源：http://ya.szsharing.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://em.lnxyls.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ji.szsharing.cn

JS:   `Hello, ${name}!`
来源：http://qq.nszjky.cn

TS:   `Hello, ${name}!`
来源：http://dh.szxytkj.cn

Java: "Hello, %s!".formatted(name)
来源：http://rr.jctech888.com.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gm.bjjhwx.cn

Ruby: "Hello, #{name}!"
来源：http://lg.521024.cn

C#:   $"Hello, {name}!"
来源：http://wp.521024.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://uh.nszjky.cn

Py:   "第一行\n第二行"
来源：http://jx.nszjky.cn

PHP:  "第一行\n第二行"
来源：http://pa.haigaiapp.cn

JS:   "第一行\n第二行"
来源：http://dx.asd995.cn

TS:   "第一行\n第二行"
来源：http://jf.521024.cn

Java: "第一行\n第二行"
来源：http://po.shxzukj.cn

Go:   "第一行\n第二行"
来源：http://cl.hnjuh.cn

Ruby: "第一行\n第二行"
来源：http://yn.jianghongdianzi.cn

C#:   "第一行\n第二行"
来源：http://ix.jianghongdianzi.cn

[A14] 注释写法
来源：http://cv.huixiangedu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://sq.yuntaijiaju.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tb.shxzskj.cn

JS:   // 单行；/* 多行 */
来源：http://mh.hahajie.cn

TS:   // 单行；/* 多行 */
来源：http://fb.521024.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nk.huixinmuqiang.cn

Go:   // 单行；/* 多行 */
来源：http://uq.yuexingan06.cn

Ruby: # 单行；=begin 多行 =end
来源：http://du.jctech888.com.cn

C#:   // 单行；/* 多行 */
来源：http://xc.shxzskj.cn

[A15] 空值判断与默认值
来源：http://vd.shxzskj.cn

Py:   value = data or "默认值"
来源：http://ao.shxzskj.cn

PHP:  $value = $data ?? "默认值";
来源：http://ta.colortex.cn

JS:   const value = data ?? "默认值";
来源：http://dw.9csxet.cn

TS:   const value = data ?? "默认值";
来源：http://rg.szxytkj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ov.chemitech.net.cn

Go:   if data == "" { data = "默认值" }
来源：http://ej.shxzukj.cn

Ruby: value = data || "默认值"
来源：http://it.yuntaijiaju.cn

C#:   var value = data ?? "默认值";
来源：http://tm.chemitech.net.cn

[A16] 真假值判断规则
来源：http://kv.jctech888.com.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zg.gzmigu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ip.colortex.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ft.huixinmuqiang.cn

TS:   if (!x) {}
来源：http://db.asd995.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://by.yuexingan06.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xr.muxihuayi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://kt.nszjky.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rd.521024.cn

[A17] 位运算
来源：http://mu.panjiajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bt.huixinmuqiang.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lm.yuntaijiaju.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ee.lnxyls.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hf.huixinmuqiang.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://at.nicolike.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lg.hahajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fs.haigaiapp.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://um.yuntaijiaju.cn

[A18] 字符与 ASCII 码互转
来源：http://oq.chemitech.net.cn

Py:   ord("A"); chr(65)
来源：http://ak.szxytkj.cn

PHP:  ord("A"); chr(65)
来源：http://ni.huixinmuqiang.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zn.shxzskj.cn


<!-- 参考信息 -->