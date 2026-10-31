代发 wailian999

[U103] JS：定时器
来源：http://jj.muxihuayi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qj.shxzukj.cn

[U104] JS：防抖
来源：http://jz.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qb.hnjuh.cn

[U105] JS：节流
来源：http://ny.9csxet.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ac.jianghongdianzi.cn

[U106] JS：日期格式化
来源：http://bj.newstarts.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sr.huixinmuqiang.cn

[U107] JS：数字千分位
来源：http://da.hahajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ol.bookmarksfly.cn

[U108] JS：随机整数
来源：http://es.haigaiapp.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://is.shxzukj.cn

[U109] JS：数组分组
来源：http://kv.huixiangedu.cn

Object.groupBy(arr, x => x.type)
来源：http://ih.haigaiapp.cn

[U110] JS：数组分块
来源：http://ts.colortex.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mx.huixiangedu.cn

[U111] JS：对象转 Map
来源：http://mw.hahajie.cn

new Map(Object.entries(obj))
来源：http://vl.jianghongdianzi.cn

[U112] JS：字符串补位
来源：http://ng.newstarts.cn

"7".padStart(3, "0")
来源：http://ce.521024.cn

[U113] JS：正则替换全部
来源：http://mk.hahajie.cn

s.replaceAll("a", "b")
来源：http://nw.hnjuh.cn

[U114] JS：JSON 深比较
来源：http://za.panjiajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pb.huanxung.cn

[U115] JS：生成 UUID
来源：http://wn.asd995.cn

crypto.randomUUID()
来源：http://rg.asd995.cn

[U116] JS：类型检查（JSDoc）
来源：http://ol.szsharing.cn

/** @param {string} name */ function f(name) {}
来源：http://dx.bjjhwx.cn

[U117] JS：单元测试
来源：http://df.hahajie.cn

npm i -D vitest;  npx vitest
来源：http://qb.bjjhwx.cn

[U118] JS：开发服务器
来源：http://sh.yuntaijiaju.cn

npm i -D vite;  npx vite
来源：http://eh.colortex.cn

[U119] JS：生产构建
来源：http://ao.szxytkj.cn

npx vite build
来源：http://qf.colortex.cn

[U120] JS：读取环境变量（Vite）
来源：http://ax.jianghongdianzi.cn

import.meta.env.VITE_API_URL
来源：http://gp.szsharing.cn

================================================================================
来源：http://hd.huanxung.cn

统计汇总
来源：http://nl.haigaiapp.cn

================================================================================
来源：http://bg.9csxet.cn

按语言统计（条）：
来源：http://ke.colortex.cn

Python ......... 252
来源：http://pb.bookmarksfly.cn

PHP ............ 252
来源：http://cy.nicolike.cn

JavaScript ..... 252
来源：http://nb.szsharing.cn

TypeScript ..... 212
来源：http://qw.bjjhwx.cn

Java ........... 212
来源：http://pa.haigaiapp.cn

Go ............. 212
来源：http://pk.chemitech.net.cn

Ruby ........... 212
来源：http://dm.bookmarksfly.cn

C# ............. 212
来源：http://ea.wgjwhj.cn

C .............. 30
来源：http://vq.9csxet.cn

C++ ............ 30
来源：http://pz.hnjuh.cn

SQL ............ 90
来源：http://kp.jctech888.com.cn

Bash ........... 80
来源：http://bw.colortex.cn

Kotlin ......... 15
来源：http://ab.haigaiapp.cn

Swift .......... 15
来源：http://qm.wgjwhj.cn

Lua ............ 10
来源：http://vs.hahajie.cn

Perl ........... 10
来源：http://re.panjiajie.cn

Scala .......... 10
来源：http://ti.jctech888.com.cn

------------------------------------
来源：http://ko.521024.cn

合计 ........... 2106 条
来源：http://dp.colortex.cn

按章节统计：
来源：http://bb.jctech888.com.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mw.521024.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sf.newstarts.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://el.shxzskj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vy.yuntaijiaju.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://en.yuexingan06.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ax.shtwfgs.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ie.huanxung.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bi.yuntaijiaju.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://am.jctech888.com.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tt.huixiangedu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zc.muxihuayi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fr.521024.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kp.huixinmuqiang.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://we.chemitech.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pv.lnxyls.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rb.hnjuh.cn

Q SQL 专题                              90
来源：http://jb.9csxet.cn

R Bash 专题                             80
来源：http://uv.wgjwhj.cn

S C / C++ 专题                          60
来源：http://sv.lnxyls.cn

T 其他语言补充                          60
来源：http://qk.521024.cn

U 高频实用片段                         120
来源：http://hr.shxzskj.cn

------------------------------------
来源：http://od.panjiajie.cn

合计                                  2106 条
来源：http://fu.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://sj.hnjuh.cn

使用提醒
来源：http://jn.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://is.szxytkj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xc.muxihuayi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bx.yuexingan06.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ap.wgjwhj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://xy.muxihuayi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ik.huanxung.cn

—— 文件结束 ——
来源：http://hq.shxzskj.cn

================================================================================
来源：http://wj.huixinmuqiang.cn

程序语言常见例子速查手册（2024 版）
来源：http://lq.nicolike.cn

Common Programming Examples Cheat Book
来源：http://qb.colortex.cn

================================================================================
来源：http://ep.szxytkj.cn

【收录内容】
来源：http://ud.huanxung.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zq.huanxung.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ka.chemitech.net.cn

SQL · Bash · C · C++
来源：http://xo.nicolike.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dw.gzmigu.cn

【使用说明】
来源：http://cy.colortex.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wm.chemitech.net.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qy.shtwfgs.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://an.yuexingan06.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zy.jianghongdianzi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ix.nszjky.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qc.jianghongdianzi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gt.lnxyls.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vb.nicolike.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dy.huanxung.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wf.hnjuh.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dd.muxihuayi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://he.newstarts.cn

【文件统计】
来源：http://yj.wgjwhj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rd.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://ca.shxzukj.cn

目  录
来源：http://kz.huanxung.cn

--------------------------------------------------------------------------------
来源：http://at.haigaiapp.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xe.lnxyls.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://eo.panjiajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hh.szxytkj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rt.huixinmuqiang.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xr.jctech888.com.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kt.nicolike.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uj.nszjky.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wc.bookmarksfly.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sd.szsharing.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lt.hnjuh.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bw.szxytkj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://oj.asd995.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lr.bookmarksfly.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vk.hahajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://me.bookmarksfly.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yq.muxihuayi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lk.szsharing.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gh.yuexingan06.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pk.panjiajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://od.bookmarksfly.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hg.bookmarksfly.cn

================================================================================
来源：http://dq.bjjhwx.cn

A. 基础语法与类型
来源：http://vb.jctech888.com.cn

================================================================================
来源：http://nq.panjiajie.cn

[A01] Hello World
来源：http://zx.newstarts.cn

Py:   print("Hello, World!")
来源：http://kn.yuntaijiaju.cn

PHP:  echo "Hello, World!";
来源：http://rw.wgjwhj.cn

JS:   console.log("Hello, World!");
来源：http://ha.shxzukj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://uq.nszjky.cn

Java: System.out.println("Hello, World!");
来源：http://dp.521024.cn

Go:   fmt.Println("Hello, World!")
来源：http://lp.szsharing.cn

Ruby: puts "Hello, World!"
来源：http://ga.haigaiapp.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://he.hnjuh.cn

[A02] 变量声明与赋值
来源：http://we.gzmigu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ne.panjiajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rc.chemitech.net.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hn.panjiajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nc.huixinmuqiang.cn

Java: String name = "Alex"; int age = 20;
来源：http://yk.huixiangedu.cn

Go:   name := "Alex"; age := 20
来源：http://mu.newstarts.cn

Ruby: name = "Alex"; age = 20
来源：http://kk.huixinmuqiang.cn

C#:   string name = "Alex"; int age = 20;
来源：http://kn.yuntaijiaju.cn

[A03] 常量定义
来源：http://vb.chemitech.net.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mq.colortex.cn

PHP:  const PI = 3.14159;
来源：http://la.shxzukj.cn

JS:   const PI = 3.14159;
来源：http://qx.gzmigu.cn

TS:   const PI: number = 3.14159;
来源：http://mj.bjjhwx.cn

Java: static final double PI = 3.14159;
来源：http://vx.bookmarksfly.cn

Go:   const PI = 3.14159
来源：http://bf.asd995.cn

Ruby: PI = 3.14159
来源：http://sb.shxzskj.cn

C#:   const double PI = 3.14159;
来源：http://vw.huixiangedu.cn

[A04] 判断变量类型
来源：http://qo.panjiajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://xs.521024.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ai.gzmigu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://sc.huanxung.cn

TS:   typeof x; x instanceof Date
来源：http://vm.hahajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ta.shtwfgs.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rx.muxihuayi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ay.hahajie.cn

C#:   x.GetType().Name; x is int
来源：http://sc.521024.cn

[A05] 整数除法与取模
来源：http://xx.jctech888.com.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ah.nicolike.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://bf.muxihuayi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tt.bjjhwx.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dh.nicolike.cn

Java: 7 / 2; 7 % 2
来源：http://vb.huixinmuqiang.cn

Go:   7 / 2; 7 % 2
来源：http://io.yuexingan06.cn

Ruby: 7 / 2; 7 % 2
来源：http://fh.nicolike.cn

C#:   7 / 2; 7 % 2
来源：http://tm.jctech888.com.cn

[A06] 字符串转数字
来源：http://mj.shxzskj.cn

Py:   int("42"); float("3.14")
来源：http://pb.hahajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ml.wgjwhj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://sr.9csxet.cn

TS:   parseInt("42", 10); Number("42")
来源：http://dd.bookmarksfly.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mb.bookmarksfly.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://io.huixiangedu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://dh.panjiajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://md.muxihuayi.cn

[A07] 数字转字符串
来源：http://as.yuexingan06.cn

Py:   str(42)
来源：http://zf.nszjky.cn

PHP:  (string) 42; strval(42)
来源：http://ca.huanxung.cn

JS:   String(42); (42).toString()
来源：http://py.szxytkj.cn

TS:   String(42)
来源：http://xt.yuntaijiaju.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bn.huanxung.cn

Go:   strconv.Itoa(42)
来源：http://jw.shxzukj.cn

Ruby: 42.to_s
来源：http://jp.bjjhwx.cn

C#:   42.ToString()
来源：http://nf.yuntaijiaju.cn

[A08] 取整与四舍五入
来源：http://xc.newstarts.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hg.nicolike.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mn.muxihuayi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xu.chemitech.net.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yd.shxzukj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qg.haigaiapp.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pr.lnxyls.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://iy.huanxung.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jj.521024.cn

[A09] 绝对值与最大最小值
来源：http://su.szxytkj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://sc.shxzukj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lp.newstarts.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hs.huixinmuqiang.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ja.asd995.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vc.gzmigu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ca.wgjwhj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ee.hahajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ew.chemitech.net.cn

[A10] 生成随机数
来源：http://fc.szxytkj.cn

Py:   import random; random.randint(1, 100)
来源：http://nt.newstarts.cn

PHP:  random_int(1, 100);
来源：http://uz.szsharing.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://et.bjjhwx.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ca.colortex.cn

Java: new Random().nextInt(100) + 1
来源：http://gd.nicolike.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jd.jctech888.com.cn

Ruby: rand(1..100)
来源：http://kb.chemitech.net.cn

C#:   new Random().Next(1, 101)
来源：http://oz.panjiajie.cn

[A11] 条件表达式（三元）
来源：http://pp.chemitech.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://ia.wgjwhj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://yi.szsharing.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rg.9csxet.cn

TS:   x > 0 ? "yes" : "no"
来源：http://gr.huixinmuqiang.cn

Java: x > 0 ? "yes" : "no"
来源：http://ul.panjiajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://eh.yuexingan06.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://dd.shtwfgs.cn

C#:   x > 0 ? "yes" : "no"
来源：http://kj.panjiajie.cn

[A12] 字符串插值 / 格式化
来源：http://lo.newstarts.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ke.muxihuayi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uh.yuexingan06.cn

JS:   `Hello, ${name}!`
来源：http://gk.asd995.cn

TS:   `Hello, ${name}!`
来源：http://ve.nszjky.cn

Java: "Hello, %s!".formatted(name)
来源：http://mn.521024.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rv.shxzskj.cn

Ruby: "Hello, #{name}!"
来源：http://if.gzmigu.cn

C#:   $"Hello, {name}!"
来源：http://gg.gzmigu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://by.shxzskj.cn

Py:   "第一行\n第二行"
来源：http://qc.shxzskj.cn

PHP:  "第一行\n第二行"
来源：http://pp.nszjky.cn

JS:   "第一行\n第二行"
来源：http://va.muxihuayi.cn

TS:   "第一行\n第二行"
来源：http://tz.nszjky.cn

Java: "第一行\n第二行"
来源：http://kr.nszjky.cn

Go:   "第一行\n第二行"
来源：http://pn.asd995.cn

Ruby: "第一行\n第二行"
来源：http://sz.chemitech.net.cn

C#:   "第一行\n第二行"
来源：http://cc.huanxung.cn

[A14] 注释写法
来源：http://zx.9csxet.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ah.newstarts.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://jm.jctech888.com.cn

JS:   // 单行；/* 多行 */
来源：http://sd.nicolike.cn

TS:   // 单行；/* 多行 */
来源：http://fg.jianghongdianzi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://go.lnxyls.cn

Go:   // 单行；/* 多行 */
来源：http://bz.muxihuayi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ma.szxytkj.cn

C#:   // 单行；/* 多行 */
来源：http://jx.nszjky.cn

[A15] 空值判断与默认值
来源：http://pf.9csxet.cn

Py:   value = data or "默认值"
来源：http://dw.bookmarksfly.cn

PHP:  $value = $data ?? "默认值";
来源：http://xy.gzmigu.cn

JS:   const value = data ?? "默认值";
来源：http://rp.shtwfgs.cn

TS:   const value = data ?? "默认值";
来源：http://hs.chemitech.net.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fv.jianghongdianzi.cn

Go:   if data == "" { data = "默认值" }
来源：http://ej.huanxung.cn

Ruby: value = data || "默认值"
来源：http://cu.haigaiapp.cn

C#:   var value = data ?? "默认值";
来源：http://yx.newstarts.cn

[A16] 真假值判断规则
来源：http://ik.9csxet.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vn.jianghongdianzi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ip.shxzskj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pb.szxytkj.cn

TS:   if (!x) {}
来源：http://rg.hnjuh.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://px.nicolike.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wp.shxzskj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://rt.hnjuh.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jy.yuntaijiaju.cn

[A17] 位运算
来源：http://xe.lnxyls.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iq.haigaiapp.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wr.yuexingan06.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vx.chemitech.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zm.9csxet.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ue.huixiangedu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gi.hnjuh.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://da.shxzskj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lo.nicolike.cn

[A18] 字符与 ASCII 码互转
来源：http://eq.shxzukj.cn

Py:   ord("A"); chr(65)
来源：http://kd.newstarts.cn

PHP:  ord("A"); chr(65)
来源：http://nm.haigaiapp.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yb.colortex.cn


<!-- 参考信息 -->