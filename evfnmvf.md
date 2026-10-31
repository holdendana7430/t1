代发 wailian999

[U99] JS：事件监听
来源：http://aw.newstarts.cn

el.addEventListener("click", e => {})
来源：http://ru.huixiangedu.cn

[U100] JS：DOM 查询
来源：http://do.gzmigu.cn

document.querySelector(".item")
来源：http://fp.nicolike.cn

[U101] JS：classList 操作
来源：http://id.huixiangedu.cn

el.classList.toggle("active")
来源：http://ku.jctech888.com.cn

[U102] JS：本地存储
来源：http://le.gzmigu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qf.chemitech.net.cn

[U103] JS：定时器
来源：http://vt.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qz.lnxyls.cn

[U104] JS：防抖
来源：http://ee.jctech888.com.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nk.huixinmuqiang.cn

[U105] JS：节流
来源：http://uw.shxzukj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hn.nicolike.cn

[U106] JS：日期格式化
来源：http://jn.hahajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://za.huanxung.cn

[U107] JS：数字千分位
来源：http://yr.jianghongdianzi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fc.jctech888.com.cn

[U108] JS：随机整数
来源：http://pe.shxzukj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rq.huixinmuqiang.cn

[U109] JS：数组分组
来源：http://uu.9csxet.cn

Object.groupBy(arr, x => x.type)
来源：http://tt.9csxet.cn

[U110] JS：数组分块
来源：http://qn.lnxyls.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wh.szxytkj.cn

[U111] JS：对象转 Map
来源：http://gk.huixinmuqiang.cn

new Map(Object.entries(obj))
来源：http://hm.huixinmuqiang.cn

[U112] JS：字符串补位
来源：http://qg.shxzskj.cn

"7".padStart(3, "0")
来源：http://uf.colortex.cn

[U113] JS：正则替换全部
来源：http://bs.colortex.cn

s.replaceAll("a", "b")
来源：http://tc.huixinmuqiang.cn

[U114] JS：JSON 深比较
来源：http://fv.muxihuayi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tj.lnxyls.cn

[U115] JS：生成 UUID
来源：http://nz.panjiajie.cn

crypto.randomUUID()
来源：http://iv.jctech888.com.cn

[U116] JS：类型检查（JSDoc）
来源：http://db.colortex.cn

/** @param {string} name */ function f(name) {}
来源：http://zu.haigaiapp.cn

[U117] JS：单元测试
来源：http://co.newstarts.cn

npm i -D vitest;  npx vitest
来源：http://lt.colortex.cn

[U118] JS：开发服务器
来源：http://aa.muxihuayi.cn

npm i -D vite;  npx vite
来源：http://xb.nszjky.cn

[U119] JS：生产构建
来源：http://nt.jctech888.com.cn

npx vite build
来源：http://hm.huanxung.cn

[U120] JS：读取环境变量（Vite）
来源：http://ar.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://wn.nszjky.cn

================================================================================
来源：http://ri.asd995.cn

统计汇总
来源：http://mb.huanxung.cn

================================================================================
来源：http://uz.nszjky.cn

按语言统计（条）：
来源：http://ic.huixinmuqiang.cn

Python ......... 252
来源：http://ba.521024.cn

PHP ............ 252
来源：http://xi.haigaiapp.cn

JavaScript ..... 252
来源：http://hh.haigaiapp.cn

TypeScript ..... 212
来源：http://dq.nszjky.cn

Java ........... 212
来源：http://xs.521024.cn

Go ............. 212
来源：http://wx.nicolike.cn

Ruby ........... 212
来源：http://gf.panjiajie.cn

C# ............. 212
来源：http://vj.chemitech.net.cn

C .............. 30
来源：http://gj.shxzskj.cn

C++ ............ 30
来源：http://se.huanxung.cn

SQL ............ 90
来源：http://bd.szxytkj.cn

Bash ........... 80
来源：http://pj.bookmarksfly.cn

Kotlin ......... 15
来源：http://pd.huixiangedu.cn

Swift .......... 15
来源：http://la.521024.cn

Lua ............ 10
来源：http://df.yuntaijiaju.cn

Perl ........... 10
来源：http://pa.asd995.cn

Scala .......... 10
来源：http://qr.asd995.cn

------------------------------------
来源：http://au.jctech888.com.cn

合计 ........... 2106 条
来源：http://xg.colortex.cn

按章节统计：
来源：http://pz.szxytkj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jt.huixiangedu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nn.huixinmuqiang.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://of.panjiajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fy.bjjhwx.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fy.shxzukj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://my.panjiajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wd.asd995.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tb.nicolike.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lr.wgjwhj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ow.muxihuayi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hc.colortex.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://on.bjjhwx.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ii.9csxet.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nm.yuntaijiaju.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sr.nszjky.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zk.newstarts.cn

Q SQL 专题                              90
来源：http://et.hnjuh.cn

R Bash 专题                             80
来源：http://yb.asd995.cn

S C / C++ 专题                          60
来源：http://tv.nicolike.cn

T 其他语言补充                          60
来源：http://lm.chemitech.net.cn

U 高频实用片段                         120
来源：http://sq.panjiajie.cn

------------------------------------
来源：http://ic.shxzukj.cn

合计                                  2106 条
来源：http://cn.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://zs.jctech888.com.cn

使用提醒
来源：http://oe.hahajie.cn

--------------------------------------------------------------------------------
来源：http://el.chemitech.net.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://oj.wgjwhj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yb.huanxung.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://no.asd995.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://un.chemitech.net.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://np.lnxyls.cn

—— 文件结束 ——
来源：http://dw.huanxung.cn

================================================================================
来源：http://jc.newstarts.cn

程序语言常见例子速查手册（2024 版）
来源：http://aj.hnjuh.cn

Common Programming Examples Cheat Book
来源：http://mc.panjiajie.cn

================================================================================
来源：http://bb.shxzukj.cn

【收录内容】
来源：http://dv.yuexingan06.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qy.jianghongdianzi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hn.shxzskj.cn

SQL · Bash · C · C++
来源：http://dd.9csxet.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rd.lnxyls.cn

【使用说明】
来源：http://gr.szsharing.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lu.hnjuh.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ze.haigaiapp.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qx.chemitech.net.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://io.colortex.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://pk.colortex.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ue.chemitech.net.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xe.hahajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ip.muxihuayi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vi.nszjky.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yc.shxzskj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://an.nszjky.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ev.colortex.cn

【文件统计】
来源：http://cj.huixiangedu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kn.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://yw.jianghongdianzi.cn

目  录
来源：http://rl.colortex.cn

--------------------------------------------------------------------------------
来源：http://od.muxihuayi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pl.shxzukj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ec.shtwfgs.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vs.bookmarksfly.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ke.szsharing.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://oc.bjjhwx.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ey.newstarts.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ro.yuexingan06.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rc.bookmarksfly.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fl.szxytkj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fr.panjiajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sn.szsharing.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jh.nszjky.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dd.shtwfgs.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://of.gzmigu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vj.shtwfgs.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bc.shxzukj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pg.nszjky.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://aa.nicolike.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lg.shtwfgs.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mp.hnjuh.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cc.hnjuh.cn

================================================================================
来源：http://zb.gzmigu.cn

A. 基础语法与类型
来源：http://yq.huanxung.cn

================================================================================
来源：http://dr.yuntaijiaju.cn

[A01] Hello World
来源：http://ln.jianghongdianzi.cn

Py:   print("Hello, World!")
来源：http://gg.hahajie.cn

PHP:  echo "Hello, World!";
来源：http://tq.jianghongdianzi.cn

JS:   console.log("Hello, World!");
来源：http://wg.jianghongdianzi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hv.chemitech.net.cn

Java: System.out.println("Hello, World!");
来源：http://eu.szxytkj.cn

Go:   fmt.Println("Hello, World!")
来源：http://le.haigaiapp.cn

Ruby: puts "Hello, World!"
来源：http://ey.9csxet.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vq.shxzskj.cn

[A02] 变量声明与赋值
来源：http://tb.haigaiapp.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yk.hnjuh.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qw.yuexingan06.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ar.nicolike.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kh.lnxyls.cn

Java: String name = "Alex"; int age = 20;
来源：http://gl.szsharing.cn

Go:   name := "Alex"; age := 20
来源：http://xl.szxytkj.cn

Ruby: name = "Alex"; age = 20
来源：http://tc.jianghongdianzi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://rg.nicolike.cn

[A03] 常量定义
来源：http://kb.shtwfgs.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jo.colortex.cn

PHP:  const PI = 3.14159;
来源：http://or.muxihuayi.cn

JS:   const PI = 3.14159;
来源：http://kz.jianghongdianzi.cn

TS:   const PI: number = 3.14159;
来源：http://ql.szsharing.cn

Java: static final double PI = 3.14159;
来源：http://yw.panjiajie.cn

Go:   const PI = 3.14159
来源：http://au.shxzukj.cn

Ruby: PI = 3.14159
来源：http://fm.gzmigu.cn

C#:   const double PI = 3.14159;
来源：http://wq.huixiangedu.cn

[A04] 判断变量类型
来源：http://uf.haigaiapp.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ss.muxihuayi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://sd.huixinmuqiang.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yr.newstarts.cn

TS:   typeof x; x instanceof Date
来源：http://lj.huixinmuqiang.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://am.nszjky.cn

Go:   reflect.TypeOf(x).Name()
来源：http://zk.bookmarksfly.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://wp.yuexingan06.cn

C#:   x.GetType().Name; x is int
来源：http://no.jctech888.com.cn

[A05] 整数除法与取模
来源：http://ga.szxytkj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fj.haigaiapp.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vv.shtwfgs.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jn.szxytkj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ej.colortex.cn

Java: 7 / 2; 7 % 2
来源：http://sb.9csxet.cn

Go:   7 / 2; 7 % 2
来源：http://jn.asd995.cn

Ruby: 7 / 2; 7 % 2
来源：http://pe.muxihuayi.cn

C#:   7 / 2; 7 % 2
来源：http://di.chemitech.net.cn

[A06] 字符串转数字
来源：http://qd.shxzukj.cn

Py:   int("42"); float("3.14")
来源：http://sw.yuntaijiaju.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kw.wgjwhj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://te.shtwfgs.cn

TS:   parseInt("42", 10); Number("42")
来源：http://sq.jctech888.com.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://en.bjjhwx.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ic.szsharing.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://il.nszjky.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sa.nszjky.cn

[A07] 数字转字符串
来源：http://cz.huixinmuqiang.cn

Py:   str(42)
来源：http://ey.panjiajie.cn

PHP:  (string) 42; strval(42)
来源：http://pr.chemitech.net.cn

JS:   String(42); (42).toString()
来源：http://vi.nicolike.cn

TS:   String(42)
来源：http://gd.szxytkj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://hg.newstarts.cn

Go:   strconv.Itoa(42)
来源：http://yt.huixinmuqiang.cn

Ruby: 42.to_s
来源：http://os.hahajie.cn

C#:   42.ToString()
来源：http://jj.jctech888.com.cn

[A08] 取整与四舍五入
来源：http://kd.nszjky.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ij.hnjuh.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fn.shxzskj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gw.hahajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ud.newstarts.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tt.haigaiapp.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gs.muxihuayi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://jk.haigaiapp.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hb.chemitech.net.cn

[A09] 绝对值与最大最小值
来源：http://mv.gzmigu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://sq.shxzskj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gu.szsharing.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://op.shxzukj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nh.hahajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://il.shtwfgs.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gp.haigaiapp.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yg.yuntaijiaju.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qj.chemitech.net.cn

[A10] 生成随机数
来源：http://rf.panjiajie.cn

Py:   import random; random.randint(1, 100)
来源：http://ar.huixiangedu.cn

PHP:  random_int(1, 100);
来源：http://pm.wgjwhj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jq.asd995.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gd.panjiajie.cn

Java: new Random().nextInt(100) + 1
来源：http://tg.hahajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://df.chemitech.net.cn

Ruby: rand(1..100)
来源：http://va.huixiangedu.cn

C#:   new Random().Next(1, 101)
来源：http://og.shxzukj.cn

[A11] 条件表达式（三元）
来源：http://xu.hahajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://bh.huixiangedu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://tp.nicolike.cn

JS:   x > 0 ? "yes" : "no"
来源：http://td.colortex.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qd.asd995.cn

Java: x > 0 ? "yes" : "no"
来源：http://dm.jctech888.com.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zu.bookmarksfly.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://nl.newstarts.cn

C#:   x > 0 ? "yes" : "no"
来源：http://zm.shtwfgs.cn

[A12] 字符串插值 / 格式化
来源：http://he.shtwfgs.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://an.huanxung.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://oc.nicolike.cn

JS:   `Hello, ${name}!`
来源：http://xl.huixiangedu.cn

TS:   `Hello, ${name}!`
来源：http://hx.jianghongdianzi.cn

Java: "Hello, %s!".formatted(name)
来源：http://lc.521024.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nj.hahajie.cn

Ruby: "Hello, #{name}!"
来源：http://ep.gzmigu.cn

C#:   $"Hello, {name}!"
来源：http://jv.hnjuh.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vf.shxzukj.cn

Py:   "第一行\n第二行"
来源：http://jx.newstarts.cn

PHP:  "第一行\n第二行"
来源：http://ma.bookmarksfly.cn

JS:   "第一行\n第二行"
来源：http://os.hnjuh.cn

TS:   "第一行\n第二行"
来源：http://ki.yuntaijiaju.cn

Java: "第一行\n第二行"
来源：http://ay.asd995.cn

Go:   "第一行\n第二行"
来源：http://gn.bjjhwx.cn

Ruby: "第一行\n第二行"
来源：http://cc.lnxyls.cn

C#:   "第一行\n第二行"
来源：http://sx.bjjhwx.cn

[A14] 注释写法
来源：http://gk.chemitech.net.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://lk.lnxyls.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xl.newstarts.cn

JS:   // 单行；/* 多行 */
来源：http://si.shxzskj.cn

TS:   // 单行；/* 多行 */
来源：http://iw.lnxyls.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://we.huixiangedu.cn

Go:   // 单行；/* 多行 */
来源：http://ph.huixinmuqiang.cn

Ruby: # 单行；=begin 多行 =end
来源：http://cd.chemitech.net.cn

C#:   // 单行；/* 多行 */
来源：http://cv.panjiajie.cn

[A15] 空值判断与默认值
来源：http://js.colortex.cn

Py:   value = data or "默认值"
来源：http://vl.szxytkj.cn

PHP:  $value = $data ?? "默认值";
来源：http://ll.bookmarksfly.cn

JS:   const value = data ?? "默认值";
来源：http://el.panjiajie.cn

TS:   const value = data ?? "默认值";
来源：http://ma.nicolike.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ti.huixiangedu.cn

Go:   if data == "" { data = "默认值" }
来源：http://ih.haigaiapp.cn

Ruby: value = data || "默认值"
来源：http://zj.nicolike.cn

C#:   var value = data ?? "默认值";
来源：http://lr.shtwfgs.cn

[A16] 真假值判断规则
来源：http://nc.shtwfgs.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://su.shtwfgs.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://an.nicolike.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uq.521024.cn

TS:   if (!x) {}
来源：http://jw.shxzukj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uv.huixinmuqiang.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dn.hahajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ij.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tz.panjiajie.cn

[A17] 位运算
来源：http://nx.9csxet.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://np.gzmigu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hm.chemitech.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ap.jctech888.com.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fq.yuexingan06.cn


<!-- 参考信息 -->