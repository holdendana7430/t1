代发 wailian999

[U99] JS：事件监听
来源：http://rr.huixiangedu.cn

el.addEventListener("click", e => {})
来源：http://qm.jctech888.com.cn

[U100] JS：DOM 查询
来源：http://yd.muxihuayi.cn

document.querySelector(".item")
来源：http://ug.szxytkj.cn

[U101] JS：classList 操作
来源：http://fd.haigaiapp.cn

el.classList.toggle("active")
来源：http://az.jctech888.com.cn

[U102] JS：本地存储
来源：http://bz.gzmigu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wi.bjjhwx.cn

[U103] JS：定时器
来源：http://ar.jianghongdianzi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://aa.hnjuh.cn

[U104] JS：防抖
来源：http://fg.wgjwhj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ck.huixiangedu.cn

[U105] JS：节流
来源：http://fk.jctech888.com.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fx.hahajie.cn

[U106] JS：日期格式化
来源：http://gl.bookmarksfly.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uc.yuntaijiaju.cn

[U107] JS：数字千分位
来源：http://wh.yuexingan06.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zp.shxzskj.cn

[U108] JS：随机整数
来源：http://nu.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.chemitech.net.cn

[U109] JS：数组分组
来源：http://cd.shtwfgs.cn

Object.groupBy(arr, x => x.type)
来源：http://jx.jctech888.com.cn

[U110] JS：数组分块
来源：http://rp.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ib.jianghongdianzi.cn

[U111] JS：对象转 Map
来源：http://ol.nicolike.cn

new Map(Object.entries(obj))
来源：http://mg.asd995.cn

[U112] JS：字符串补位
来源：http://jp.szxytkj.cn

"7".padStart(3, "0")
来源：http://yy.shxzukj.cn

[U113] JS：正则替换全部
来源：http://ja.bookmarksfly.cn

s.replaceAll("a", "b")
来源：http://ui.asd995.cn

[U114] JS：JSON 深比较
来源：http://dl.yuexingan06.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vh.hnjuh.cn

[U115] JS：生成 UUID
来源：http://rv.muxihuayi.cn

crypto.randomUUID()
来源：http://sd.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://qd.yuexingan06.cn

/** @param {string} name */ function f(name) {}
来源：http://ke.bjjhwx.cn

[U117] JS：单元测试
来源：http://pa.nicolike.cn

npm i -D vitest;  npx vitest
来源：http://jv.haigaiapp.cn

[U118] JS：开发服务器
来源：http://ft.asd995.cn

npm i -D vite;  npx vite
来源：http://hf.yuexingan06.cn

[U119] JS：生产构建
来源：http://rn.newstarts.cn

npx vite build
来源：http://yp.hahajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://wx.huixinmuqiang.cn

import.meta.env.VITE_API_URL
来源：http://jd.huixiangedu.cn

================================================================================
来源：http://jx.nszjky.cn

统计汇总
来源：http://it.szsharing.cn

================================================================================
来源：http://bf.lnxyls.cn

按语言统计（条）：
来源：http://ko.wgjwhj.cn

Python ......... 252
来源：http://fy.colortex.cn

PHP ............ 252
来源：http://kj.chemitech.net.cn

JavaScript ..... 252
来源：http://kl.521024.cn

TypeScript ..... 212
来源：http://th.panjiajie.cn

Java ........... 212
来源：http://ss.shxzukj.cn

Go ............. 212
来源：http://pu.bjjhwx.cn

Ruby ........... 212
来源：http://kl.bookmarksfly.cn

C# ............. 212
来源：http://zf.jctech888.com.cn

C .............. 30
来源：http://wo.chemitech.net.cn

C++ ............ 30
来源：http://gs.shxzskj.cn

SQL ............ 90
来源：http://ig.nicolike.cn

Bash ........... 80
来源：http://nn.szxytkj.cn

Kotlin ......... 15
来源：http://po.szxytkj.cn

Swift .......... 15
来源：http://ml.yuntaijiaju.cn

Lua ............ 10
来源：http://if.panjiajie.cn

Perl ........... 10
来源：http://dk.nszjky.cn

Scala .......... 10
来源：http://wf.9csxet.cn

------------------------------------
来源：http://vy.huanxung.cn

合计 ........... 2106 条
来源：http://mw.nicolike.cn

按章节统计：
来源：http://sn.521024.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ss.hahajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nh.haigaiapp.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cf.shxzskj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ft.wgjwhj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wy.nicolike.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mr.521024.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://co.nicolike.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://oj.asd995.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tf.colortex.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ck.wgjwhj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gn.muxihuayi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qh.huixinmuqiang.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bd.szsharing.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://en.nszjky.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ym.jctech888.com.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mj.newstarts.cn

Q SQL 专题                              90
来源：http://cw.yuntaijiaju.cn

R Bash 专题                             80
来源：http://gj.shtwfgs.cn

S C / C++ 专题                          60
来源：http://oh.jianghongdianzi.cn

T 其他语言补充                          60
来源：http://ow.hahajie.cn

U 高频实用片段                         120
来源：http://mi.szsharing.cn

------------------------------------
来源：http://wp.haigaiapp.cn

合计                                  2106 条
来源：http://ou.huanxung.cn

--------------------------------------------------------------------------------
来源：http://gc.shxzukj.cn

使用提醒
来源：http://bg.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://ys.muxihuayi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yj.huixiangedu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://st.bookmarksfly.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ff.shtwfgs.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ln.bjjhwx.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://oy.huixinmuqiang.cn

—— 文件结束 ——
来源：http://rz.szxytkj.cn

================================================================================
来源：http://iq.hahajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://jb.chemitech.net.cn

Common Programming Examples Cheat Book
来源：http://am.huixinmuqiang.cn

================================================================================
来源：http://pb.chemitech.net.cn

【收录内容】
来源：http://ax.jctech888.com.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ne.asd995.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bq.szxytkj.cn

SQL · Bash · C · C++
来源：http://wz.muxihuayi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rs.szsharing.cn

【使用说明】
来源：http://zu.muxihuayi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xx.panjiajie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yh.lnxyls.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bf.wgjwhj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rc.hnjuh.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wp.jianghongdianzi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sn.wgjwhj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qf.szxytkj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pg.shtwfgs.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cw.bookmarksfly.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jp.521024.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ta.jctech888.com.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mt.chemitech.net.cn

【文件统计】
来源：http://am.huanxung.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cw.nicolike.cn

--------------------------------------------------------------------------------
来源：http://ac.haigaiapp.cn

目  录
来源：http://dx.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://tq.colortex.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ui.gzmigu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gp.yuntaijiaju.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://li.shtwfgs.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zg.shxzskj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ds.muxihuayi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wi.huixiangedu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gj.shtwfgs.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tv.muxihuayi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qp.huanxung.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wz.9csxet.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qw.yuntaijiaju.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rb.jctech888.com.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wm.szxytkj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://oj.haigaiapp.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pk.bookmarksfly.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ed.wgjwhj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bc.szxytkj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://lo.521024.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bc.shtwfgs.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cb.gzmigu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://sj.bookmarksfly.cn

================================================================================
来源：http://mh.muxihuayi.cn

A. 基础语法与类型
来源：http://kp.panjiajie.cn

================================================================================
来源：http://ro.muxihuayi.cn

[A01] Hello World
来源：http://vh.nicolike.cn

Py:   print("Hello, World!")
来源：http://ho.shtwfgs.cn

PHP:  echo "Hello, World!";
来源：http://ps.nicolike.cn

JS:   console.log("Hello, World!");
来源：http://ok.panjiajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pw.huanxung.cn

Java: System.out.println("Hello, World!");
来源：http://ts.szsharing.cn

Go:   fmt.Println("Hello, World!")
来源：http://ha.szxytkj.cn

Ruby: puts "Hello, World!"
来源：http://uj.szxytkj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://tr.hnjuh.cn

[A02] 变量声明与赋值
来源：http://zd.panjiajie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fy.panjiajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://im.szsharing.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ww.panjiajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://oh.szsharing.cn

Java: String name = "Alex"; int age = 20;
来源：http://us.nicolike.cn

Go:   name := "Alex"; age := 20
来源：http://mm.9csxet.cn

Ruby: name = "Alex"; age = 20
来源：http://od.asd995.cn

C#:   string name = "Alex"; int age = 20;
来源：http://cp.yuexingan06.cn

[A03] 常量定义
来源：http://iy.szsharing.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tp.shxzskj.cn

PHP:  const PI = 3.14159;
来源：http://qp.colortex.cn

JS:   const PI = 3.14159;
来源：http://fi.muxihuayi.cn

TS:   const PI: number = 3.14159;
来源：http://fc.huanxung.cn

Java: static final double PI = 3.14159;
来源：http://am.huanxung.cn

Go:   const PI = 3.14159
来源：http://lb.jctech888.com.cn

Ruby: PI = 3.14159
来源：http://yl.nicolike.cn

C#:   const double PI = 3.14159;
来源：http://to.wgjwhj.cn

[A04] 判断变量类型
来源：http://nv.colortex.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://fw.shxzskj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qo.bookmarksfly.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vc.chemitech.net.cn

TS:   typeof x; x instanceof Date
来源：http://kv.shtwfgs.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dq.muxihuayi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://db.bjjhwx.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://dc.haigaiapp.cn

C#:   x.GetType().Name; x is int
来源：http://lu.hnjuh.cn

[A05] 整数除法与取模
来源：http://ap.yuexingan06.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bi.panjiajie.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gi.szsharing.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hh.huanxung.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://iz.shtwfgs.cn

Java: 7 / 2; 7 % 2
来源：http://ru.shxzskj.cn

Go:   7 / 2; 7 % 2
来源：http://jy.yuexingan06.cn

Ruby: 7 / 2; 7 % 2
来源：http://kp.hahajie.cn

C#:   7 / 2; 7 % 2
来源：http://vm.szxytkj.cn

[A06] 字符串转数字
来源：http://op.bjjhwx.cn

Py:   int("42"); float("3.14")
来源：http://yz.newstarts.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hh.colortex.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gr.colortex.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vp.shxzskj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://na.hahajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fq.yuntaijiaju.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ju.lnxyls.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sh.jianghongdianzi.cn

[A07] 数字转字符串
来源：http://as.521024.cn

Py:   str(42)
来源：http://dk.shxzukj.cn

PHP:  (string) 42; strval(42)
来源：http://bh.newstarts.cn

JS:   String(42); (42).toString()
来源：http://ds.9csxet.cn

TS:   String(42)
来源：http://qg.panjiajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xp.jctech888.com.cn

Go:   strconv.Itoa(42)
来源：http://ns.yuexingan06.cn

Ruby: 42.to_s
来源：http://mr.szsharing.cn

C#:   42.ToString()
来源：http://zy.shtwfgs.cn

[A08] 取整与四舍五入
来源：http://ot.nszjky.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://im.yuntaijiaju.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xr.nszjky.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://eo.huixinmuqiang.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sn.hahajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wx.huixinmuqiang.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://re.nicolike.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://oy.asd995.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ut.szsharing.cn

[A09] 绝对值与最大最小值
来源：http://uv.huixinmuqiang.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hd.szsharing.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hi.haigaiapp.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ut.chemitech.net.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zn.nszjky.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://of.huixiangedu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gj.jctech888.com.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qc.colortex.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kb.newstarts.cn

[A10] 生成随机数
来源：http://sh.muxihuayi.cn

Py:   import random; random.randint(1, 100)
来源：http://pt.huanxung.cn

PHP:  random_int(1, 100);
来源：http://bs.shxzskj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://as.jianghongdianzi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lu.shxzukj.cn

Java: new Random().nextInt(100) + 1
来源：http://rg.huixinmuqiang.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rk.chemitech.net.cn

Ruby: rand(1..100)
来源：http://fw.jianghongdianzi.cn

C#:   new Random().Next(1, 101)
来源：http://ov.huixinmuqiang.cn

[A11] 条件表达式（三元）
来源：http://nh.newstarts.cn

Py:   "yes" if x > 0 else "no"
来源：http://mw.chemitech.net.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rg.nszjky.cn

JS:   x > 0 ? "yes" : "no"
来源：http://uz.shxzskj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://su.szsharing.cn

Java: x > 0 ? "yes" : "no"
来源：http://en.huanxung.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ye.shxzukj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://go.hnjuh.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ng.newstarts.cn

[A12] 字符串插值 / 格式化
来源：http://xc.yuntaijiaju.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jj.jianghongdianzi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ry.jctech888.com.cn

JS:   `Hello, ${name}!`
来源：http://ul.hahajie.cn

TS:   `Hello, ${name}!`
来源：http://pj.hahajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://dl.panjiajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ax.szsharing.cn

Ruby: "Hello, #{name}!"
来源：http://pi.szxytkj.cn

C#:   $"Hello, {name}!"
来源：http://jd.haigaiapp.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ne.9csxet.cn

Py:   "第一行\n第二行"
来源：http://ma.jianghongdianzi.cn

PHP:  "第一行\n第二行"
来源：http://hk.chemitech.net.cn

JS:   "第一行\n第二行"
来源：http://mj.yuexingan06.cn

TS:   "第一行\n第二行"
来源：http://ys.newstarts.cn

Java: "第一行\n第二行"
来源：http://jv.wgjwhj.cn

Go:   "第一行\n第二行"
来源：http://md.muxihuayi.cn

Ruby: "第一行\n第二行"
来源：http://nd.nicolike.cn

C#:   "第一行\n第二行"
来源：http://vt.nszjky.cn

[A14] 注释写法
来源：http://qg.jctech888.com.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://zl.asd995.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ff.shxzukj.cn

JS:   // 单行；/* 多行 */
来源：http://qa.huixiangedu.cn

TS:   // 单行；/* 多行 */
来源：http://nz.bjjhwx.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dv.bookmarksfly.cn

Go:   // 单行；/* 多行 */
来源：http://xq.huixiangedu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://on.huixiangedu.cn

C#:   // 单行；/* 多行 */
来源：http://wl.szxytkj.cn

[A15] 空值判断与默认值
来源：http://ml.nszjky.cn

Py:   value = data or "默认值"
来源：http://ty.yuntaijiaju.cn

PHP:  $value = $data ?? "默认值";
来源：http://ro.jctech888.com.cn

JS:   const value = data ?? "默认值";
来源：http://zx.panjiajie.cn

TS:   const value = data ?? "默认值";
来源：http://lk.szsharing.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://or.bookmarksfly.cn

Go:   if data == "" { data = "默认值" }
来源：http://wl.jctech888.com.cn

Ruby: value = data || "默认值"
来源：http://fj.shtwfgs.cn

C#:   var value = data ?? "默认值";
来源：http://cu.nszjky.cn

[A16] 真假值判断规则
来源：http://ru.lnxyls.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xo.colortex.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fh.panjiajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wg.panjiajie.cn

TS:   if (!x) {}
来源：http://za.huixinmuqiang.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kn.shtwfgs.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ex.jctech888.com.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qr.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mr.szsharing.cn

[A17] 位运算
来源：http://na.chemitech.net.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nb.yuntaijiaju.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://yc.lnxyls.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://on.huixinmuqiang.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jt.gzmigu.cn


<!-- 参考信息 -->