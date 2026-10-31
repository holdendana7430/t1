代发 wailian999

[U101] JS：classList 操作
来源：http://vn.nicolike.cn

el.classList.toggle("active")
来源：http://za.shtwfgs.cn

[U102] JS：本地存储
来源：http://sw.hnjuh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ls.huixinmuqiang.cn

[U103] JS：定时器
来源：http://sp.wgjwhj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ez.jctech888.com.cn

[U104] JS：防抖
来源：http://kb.asd995.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ea.shxzskj.cn

[U105] JS：节流
来源：http://ga.hahajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ye.9csxet.cn

[U106] JS：日期格式化
来源：http://ot.9csxet.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qf.hnjuh.cn

[U107] JS：数字千分位
来源：http://hw.newstarts.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lo.nicolike.cn

[U108] JS：随机整数
来源：http://yt.shxzukj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vk.shxzskj.cn

[U109] JS：数组分组
来源：http://ya.szxytkj.cn

Object.groupBy(arr, x => x.type)
来源：http://ld.colortex.cn

[U110] JS：数组分块
来源：http://qh.lnxyls.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pj.521024.cn

[U111] JS：对象转 Map
来源：http://kj.szsharing.cn

new Map(Object.entries(obj))
来源：http://sk.gzmigu.cn

[U112] JS：字符串补位
来源：http://zy.asd995.cn

"7".padStart(3, "0")
来源：http://vy.gzmigu.cn

[U113] JS：正则替换全部
来源：http://kl.asd995.cn

s.replaceAll("a", "b")
来源：http://eo.hnjuh.cn

[U114] JS：JSON 深比较
来源：http://yg.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ly.szxytkj.cn

[U115] JS：生成 UUID
来源：http://mm.shxzskj.cn

crypto.randomUUID()
来源：http://gm.muxihuayi.cn

[U116] JS：类型检查（JSDoc）
来源：http://il.bjjhwx.cn

/** @param {string} name */ function f(name) {}
来源：http://uh.gzmigu.cn

[U117] JS：单元测试
来源：http://ez.huixinmuqiang.cn

npm i -D vitest;  npx vitest
来源：http://lm.colortex.cn

[U118] JS：开发服务器
来源：http://pf.bjjhwx.cn

npm i -D vite;  npx vite
来源：http://cq.muxihuayi.cn

[U119] JS：生产构建
来源：http://at.yuntaijiaju.cn

npx vite build
来源：http://ae.521024.cn

[U120] JS：读取环境变量（Vite）
来源：http://op.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://bi.bjjhwx.cn

================================================================================
来源：http://xi.lnxyls.cn

统计汇总
来源：http://gj.jianghongdianzi.cn

================================================================================
来源：http://ry.9csxet.cn

按语言统计（条）：
来源：http://ho.muxihuayi.cn

Python ......... 252
来源：http://px.muxihuayi.cn

PHP ............ 252
来源：http://fj.yuntaijiaju.cn

JavaScript ..... 252
来源：http://dk.haigaiapp.cn

TypeScript ..... 212
来源：http://hs.huanxung.cn

Java ........... 212
来源：http://bc.nicolike.cn

Go ............. 212
来源：http://di.lnxyls.cn

Ruby ........... 212
来源：http://ar.lnxyls.cn

C# ............. 212
来源：http://uk.yuntaijiaju.cn

C .............. 30
来源：http://rk.nicolike.cn

C++ ............ 30
来源：http://av.shxzskj.cn

SQL ............ 90
来源：http://up.521024.cn

Bash ........... 80
来源：http://qh.newstarts.cn

Kotlin ......... 15
来源：http://ks.jctech888.com.cn

Swift .......... 15
来源：http://ss.bookmarksfly.cn

Lua ............ 10
来源：http://sz.newstarts.cn

Perl ........... 10
来源：http://zo.jianghongdianzi.cn

Scala .......... 10
来源：http://dh.szxytkj.cn

------------------------------------
来源：http://pm.lnxyls.cn

合计 ........... 2106 条
来源：http://up.newstarts.cn

按章节统计：
来源：http://uz.haigaiapp.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kn.hahajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dh.jctech888.com.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://iy.jianghongdianzi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://th.jctech888.com.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uo.9csxet.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ap.huanxung.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pu.521024.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kj.gzmigu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mh.jianghongdianzi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sd.haigaiapp.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dz.huixinmuqiang.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fv.panjiajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pw.bjjhwx.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://og.haigaiapp.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ir.yuntaijiaju.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://eo.yuntaijiaju.cn

Q SQL 专题                              90
来源：http://xh.bjjhwx.cn

R Bash 专题                             80
来源：http://ja.shxzukj.cn

S C / C++ 专题                          60
来源：http://hh.panjiajie.cn

T 其他语言补充                          60
来源：http://je.shxzukj.cn

U 高频实用片段                         120
来源：http://wi.wgjwhj.cn

------------------------------------
来源：http://bz.wgjwhj.cn

合计                                  2106 条
来源：http://vf.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://pm.newstarts.cn

使用提醒
来源：http://qe.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://yf.jianghongdianzi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://br.nicolike.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cl.colortex.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jq.521024.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://np.wgjwhj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nw.yuntaijiaju.cn

—— 文件结束 ——
来源：http://hk.asd995.cn

================================================================================
来源：http://zz.haigaiapp.cn

程序语言常见例子速查手册（2024 版）
来源：http://qh.shxzskj.cn

Common Programming Examples Cheat Book
来源：http://mb.bjjhwx.cn

================================================================================
来源：http://ot.gzmigu.cn

【收录内容】
来源：http://ga.szxytkj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ba.chemitech.net.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xt.nicolike.cn

SQL · Bash · C · C++
来源：http://ua.szsharing.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://aw.9csxet.cn

【使用说明】
来源：http://qq.gzmigu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://uh.jctech888.com.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hl.shxzskj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pu.newstarts.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jh.bjjhwx.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qj.muxihuayi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mm.nicolike.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xd.huixinmuqiang.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gm.9csxet.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uo.jianghongdianzi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vh.muxihuayi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vv.bookmarksfly.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hh.haigaiapp.cn

【文件统计】
来源：http://tw.jctech888.com.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gu.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://dc.haigaiapp.cn

目  录
来源：http://iv.nicolike.cn

--------------------------------------------------------------------------------
来源：http://dc.chemitech.net.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ok.nicolike.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zm.lnxyls.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uo.nszjky.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xr.huixinmuqiang.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://em.nicolike.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pa.hahajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cl.hnjuh.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xr.huixinmuqiang.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://un.yuexingan06.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ra.yuntaijiaju.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ym.colortex.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sp.muxihuayi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gk.jianghongdianzi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://iw.szxytkj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://na.shxzukj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ft.asd995.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ol.hnjuh.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bg.jctech888.com.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://js.huixiangedu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nj.szxytkj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vc.szsharing.cn

================================================================================
来源：http://gi.hnjuh.cn

A. 基础语法与类型
来源：http://av.jctech888.com.cn

================================================================================
来源：http://am.haigaiapp.cn

[A01] Hello World
来源：http://wg.panjiajie.cn

Py:   print("Hello, World!")
来源：http://or.gzmigu.cn

PHP:  echo "Hello, World!";
来源：http://mq.panjiajie.cn

JS:   console.log("Hello, World!");
来源：http://io.jctech888.com.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fs.jianghongdianzi.cn

Java: System.out.println("Hello, World!");
来源：http://ri.szxytkj.cn

Go:   fmt.Println("Hello, World!")
来源：http://uz.jctech888.com.cn

Ruby: puts "Hello, World!"
来源：http://rs.szxytkj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ea.shxzskj.cn

[A02] 变量声明与赋值
来源：http://an.colortex.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://el.muxihuayi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://dz.gzmigu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://pk.bookmarksfly.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ha.bjjhwx.cn

Java: String name = "Alex"; int age = 20;
来源：http://nk.521024.cn

Go:   name := "Alex"; age := 20
来源：http://sp.szxytkj.cn

Ruby: name = "Alex"; age = 20
来源：http://ia.szsharing.cn

C#:   string name = "Alex"; int age = 20;
来源：http://on.nicolike.cn

[A03] 常量定义
来源：http://kb.huixinmuqiang.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://uc.shxzskj.cn

PHP:  const PI = 3.14159;
来源：http://ds.huixiangedu.cn

JS:   const PI = 3.14159;
来源：http://hd.bjjhwx.cn

TS:   const PI: number = 3.14159;
来源：http://ss.jianghongdianzi.cn

Java: static final double PI = 3.14159;
来源：http://my.huixiangedu.cn

Go:   const PI = 3.14159
来源：http://fn.wgjwhj.cn

Ruby: PI = 3.14159
来源：http://pz.colortex.cn

C#:   const double PI = 3.14159;
来源：http://uv.lnxyls.cn

[A04] 判断变量类型
来源：http://xc.asd995.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ig.jianghongdianzi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zd.yuexingan06.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ky.yuntaijiaju.cn

TS:   typeof x; x instanceof Date
来源：http://vm.panjiajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pi.521024.cn

Go:   reflect.TypeOf(x).Name()
来源：http://mg.9csxet.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://jf.nszjky.cn

C#:   x.GetType().Name; x is int
来源：http://cv.szsharing.cn

[A05] 整数除法与取模
来源：http://jf.newstarts.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zx.521024.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://dv.nicolike.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://on.huixinmuqiang.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://in.shtwfgs.cn

Java: 7 / 2; 7 % 2
来源：http://wo.wgjwhj.cn

Go:   7 / 2; 7 % 2
来源：http://sd.nicolike.cn

Ruby: 7 / 2; 7 % 2
来源：http://bt.nszjky.cn

C#:   7 / 2; 7 % 2
来源：http://wa.huixinmuqiang.cn

[A06] 字符串转数字
来源：http://qo.haigaiapp.cn

Py:   int("42"); float("3.14")
来源：http://hw.wgjwhj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zg.hahajie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lh.chemitech.net.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ki.nicolike.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cz.colortex.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mu.huixiangedu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://np.shxzskj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kq.yuntaijiaju.cn

[A07] 数字转字符串
来源：http://lq.9csxet.cn

Py:   str(42)
来源：http://ib.bookmarksfly.cn

PHP:  (string) 42; strval(42)
来源：http://ek.bjjhwx.cn

JS:   String(42); (42).toString()
来源：http://dj.yuexingan06.cn

TS:   String(42)
来源：http://at.gzmigu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://qr.huixiangedu.cn

Go:   strconv.Itoa(42)
来源：http://qv.521024.cn

Ruby: 42.to_s
来源：http://lw.lnxyls.cn

C#:   42.ToString()
来源：http://ah.huixiangedu.cn

[A08] 取整与四舍五入
来源：http://dw.shxzskj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rz.hahajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tk.newstarts.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jv.nszjky.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ku.jianghongdianzi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gn.lnxyls.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://cu.521024.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://cc.shtwfgs.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ie.nszjky.cn

[A09] 绝对值与最大最小值
来源：http://mb.yuntaijiaju.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yy.shxzukj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qz.panjiajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://po.szxytkj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yo.lnxyls.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mf.hnjuh.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hm.huixiangedu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zi.huanxung.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qm.bjjhwx.cn

[A10] 生成随机数
来源：http://wz.colortex.cn

Py:   import random; random.randint(1, 100)
来源：http://qb.jctech888.com.cn

PHP:  random_int(1, 100);
来源：http://vv.jctech888.com.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ib.nszjky.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://za.muxihuayi.cn

Java: new Random().nextInt(100) + 1
来源：http://kq.shtwfgs.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ix.jctech888.com.cn

Ruby: rand(1..100)
来源：http://kt.nicolike.cn

C#:   new Random().Next(1, 101)
来源：http://qn.panjiajie.cn

[A11] 条件表达式（三元）
来源：http://wq.nszjky.cn

Py:   "yes" if x > 0 else "no"
来源：http://nc.521024.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fk.lnxyls.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ga.muxihuayi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qc.shxzskj.cn

Java: x > 0 ? "yes" : "no"
来源：http://mk.wgjwhj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://kg.shxzukj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://kg.jctech888.com.cn

C#:   x > 0 ? "yes" : "no"
来源：http://lp.yuntaijiaju.cn

[A12] 字符串插值 / 格式化
来源：http://os.szxytkj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://om.szxytkj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ss.521024.cn

JS:   `Hello, ${name}!`
来源：http://ts.newstarts.cn

TS:   `Hello, ${name}!`
来源：http://ap.colortex.cn

Java: "Hello, %s!".formatted(name)
来源：http://cb.yuntaijiaju.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://iu.shxzukj.cn

Ruby: "Hello, #{name}!"
来源：http://wc.shxzskj.cn

C#:   $"Hello, {name}!"
来源：http://ph.yuexingan06.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://xo.chemitech.net.cn

Py:   "第一行\n第二行"
来源：http://at.nszjky.cn

PHP:  "第一行\n第二行"
来源：http://uk.jctech888.com.cn

JS:   "第一行\n第二行"
来源：http://is.nszjky.cn

TS:   "第一行\n第二行"
来源：http://hl.huixinmuqiang.cn

Java: "第一行\n第二行"
来源：http://gy.huixinmuqiang.cn

Go:   "第一行\n第二行"
来源：http://fv.shxzukj.cn

Ruby: "第一行\n第二行"
来源：http://ai.nicolike.cn

C#:   "第一行\n第二行"
来源：http://oh.huixinmuqiang.cn

[A14] 注释写法
来源：http://ta.9csxet.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://iw.nicolike.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://me.asd995.cn

JS:   // 单行；/* 多行 */
来源：http://yz.lnxyls.cn

TS:   // 单行；/* 多行 */
来源：http://ot.huixiangedu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ov.huixinmuqiang.cn

Go:   // 单行；/* 多行 */
来源：http://hh.yuntaijiaju.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wn.jianghongdianzi.cn

C#:   // 单行；/* 多行 */
来源：http://ir.nicolike.cn

[A15] 空值判断与默认值
来源：http://lo.gzmigu.cn

Py:   value = data or "默认值"
来源：http://qo.shxzskj.cn

PHP:  $value = $data ?? "默认值";
来源：http://hc.szsharing.cn

JS:   const value = data ?? "默认值";
来源：http://aq.szxytkj.cn

TS:   const value = data ?? "默认值";
来源：http://wg.haigaiapp.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pd.panjiajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://uz.huanxung.cn

Ruby: value = data || "默认值"
来源：http://oj.huixiangedu.cn

C#:   var value = data ?? "默认值";
来源：http://hb.hahajie.cn

[A16] 真假值判断规则
来源：http://zy.shtwfgs.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fi.521024.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://st.lnxyls.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://od.newstarts.cn

TS:   if (!x) {}
来源：http://gf.newstarts.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pt.huixinmuqiang.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fv.yuntaijiaju.cn

Ruby: unless x            # nil 与 false 为假
来源：http://cv.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qq.muxihuayi.cn

[A17] 位运算
来源：http://il.nszjky.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pk.hahajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://if.yuexingan06.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lz.shxzskj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://oh.hahajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zw.shxzskj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gg.haigaiapp.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dw.jianghongdianzi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ib.jianghongdianzi.cn


<!-- 参考信息 -->