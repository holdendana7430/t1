代发 wailian999

[U99] JS：事件监听
来源：http://uv.chemitech.net.cn

el.addEventListener("click", e => {})
来源：http://ad.gzmigu.cn

[U100] JS：DOM 查询
来源：http://dh.huanxung.cn

document.querySelector(".item")
来源：http://dq.shxzskj.cn

[U101] JS：classList 操作
来源：http://nk.hahajie.cn

el.classList.toggle("active")
来源：http://wf.szsharing.cn

[U102] JS：本地存储
来源：http://et.chemitech.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hm.huixinmuqiang.cn

[U103] JS：定时器
来源：http://fd.shtwfgs.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tu.szsharing.cn

[U104] JS：防抖
来源：http://uc.jctech888.com.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ya.nszjky.cn

[U105] JS：节流
来源：http://is.huanxung.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gd.yuntaijiaju.cn

[U106] JS：日期格式化
来源：http://nx.jianghongdianzi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nk.wgjwhj.cn

[U107] JS：数字千分位
来源：http://po.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gc.panjiajie.cn

[U108] JS：随机整数
来源：http://lp.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://iw.9csxet.cn

[U109] JS：数组分组
来源：http://dc.huixiangedu.cn

Object.groupBy(arr, x => x.type)
来源：http://ym.nszjky.cn

[U110] JS：数组分块
来源：http://au.chemitech.net.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ca.shxzskj.cn

[U111] JS：对象转 Map
来源：http://vw.nszjky.cn

new Map(Object.entries(obj))
来源：http://ur.yuntaijiaju.cn

[U112] JS：字符串补位
来源：http://gu.nicolike.cn

"7".padStart(3, "0")
来源：http://qd.shxzskj.cn

[U113] JS：正则替换全部
来源：http://fs.newstarts.cn

s.replaceAll("a", "b")
来源：http://kj.wgjwhj.cn

[U114] JS：JSON 深比较
来源：http://lz.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tk.muxihuayi.cn

[U115] JS：生成 UUID
来源：http://lh.asd995.cn

crypto.randomUUID()
来源：http://ko.bookmarksfly.cn

[U116] JS：类型检查（JSDoc）
来源：http://wm.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://wj.panjiajie.cn

[U117] JS：单元测试
来源：http://pt.nszjky.cn

npm i -D vitest;  npx vitest
来源：http://il.9csxet.cn

[U118] JS：开发服务器
来源：http://eh.huixinmuqiang.cn

npm i -D vite;  npx vite
来源：http://hq.huixinmuqiang.cn

[U119] JS：生产构建
来源：http://pz.yuexingan06.cn

npx vite build
来源：http://na.haigaiapp.cn

[U120] JS：读取环境变量（Vite）
来源：http://wg.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://jk.gzmigu.cn

================================================================================
来源：http://jo.szsharing.cn

统计汇总
来源：http://lq.gzmigu.cn

================================================================================
来源：http://sh.shxzskj.cn

按语言统计（条）：
来源：http://ha.szsharing.cn

Python ......... 252
来源：http://xs.hnjuh.cn

PHP ............ 252
来源：http://wo.lnxyls.cn

JavaScript ..... 252
来源：http://jg.szsharing.cn

TypeScript ..... 212
来源：http://ju.panjiajie.cn

Java ........... 212
来源：http://hm.asd995.cn

Go ............. 212
来源：http://gu.nszjky.cn

Ruby ........... 212
来源：http://xi.nicolike.cn

C# ............. 212
来源：http://ae.nicolike.cn

C .............. 30
来源：http://by.chemitech.net.cn

C++ ............ 30
来源：http://hz.gzmigu.cn

SQL ............ 90
来源：http://rm.huixinmuqiang.cn

Bash ........... 80
来源：http://cq.shtwfgs.cn

Kotlin ......... 15
来源：http://gw.nszjky.cn

Swift .......... 15
来源：http://vc.newstarts.cn

Lua ............ 10
来源：http://fb.colortex.cn

Perl ........... 10
来源：http://we.szsharing.cn

Scala .......... 10
来源：http://vl.muxihuayi.cn

------------------------------------
来源：http://ma.lnxyls.cn

合计 ........... 2106 条
来源：http://wt.shxzskj.cn

按章节统计：
来源：http://xx.jctech888.com.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fl.haigaiapp.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ab.521024.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qa.9csxet.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fp.huixinmuqiang.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rn.huanxung.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ya.lnxyls.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qx.jianghongdianzi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sq.gzmigu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ve.nicolike.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://se.bookmarksfly.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zr.shxzukj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kh.huanxung.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cf.lnxyls.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wx.jianghongdianzi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bi.521024.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://sk.521024.cn

Q SQL 专题                              90
来源：http://ez.shxzskj.cn

R Bash 专题                             80
来源：http://bg.colortex.cn

S C / C++ 专题                          60
来源：http://rv.muxihuayi.cn

T 其他语言补充                          60
来源：http://nv.shxzskj.cn

U 高频实用片段                         120
来源：http://fs.521024.cn

------------------------------------
来源：http://er.yuexingan06.cn

合计                                  2106 条
来源：http://nl.colortex.cn

--------------------------------------------------------------------------------
来源：http://tp.9csxet.cn

使用提醒
来源：http://bz.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://zq.szsharing.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bj.521024.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cv.lnxyls.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tb.jctech888.com.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ui.shxzskj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://po.jctech888.com.cn

—— 文件结束 ——
来源：http://dv.huanxung.cn

================================================================================
来源：http://gb.asd995.cn

程序语言常见例子速查手册（2024 版）
来源：http://os.9csxet.cn

Common Programming Examples Cheat Book
来源：http://ig.shtwfgs.cn

================================================================================
来源：http://gc.nicolike.cn

【收录内容】
来源：http://gs.nszjky.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://pv.yuntaijiaju.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://os.huixiangedu.cn

SQL · Bash · C · C++
来源：http://sn.gzmigu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://iq.huanxung.cn

【使用说明】
来源：http://gt.hnjuh.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lz.jianghongdianzi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vj.huanxung.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hi.huanxung.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ha.nszjky.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://tz.jctech888.com.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://iz.huixinmuqiang.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://if.9csxet.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kd.asd995.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ds.asd995.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://iy.panjiajie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bf.nicolike.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ka.muxihuayi.cn

【文件统计】
来源：http://ik.colortex.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rh.nicolike.cn

--------------------------------------------------------------------------------
来源：http://bd.nszjky.cn

目  录
来源：http://ev.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://lk.521024.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jp.huixiangedu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tb.colortex.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yg.chemitech.net.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vm.huixiangedu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qi.haigaiapp.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://sd.nicolike.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ru.szsharing.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ly.hahajie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rt.chemitech.net.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pm.szsharing.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wq.9csxet.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ac.shxzukj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kq.wgjwhj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://li.szxytkj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lr.hahajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rh.szsharing.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sj.szsharing.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://nt.huanxung.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ou.shtwfgs.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yo.9csxet.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zy.shxzskj.cn

================================================================================
来源：http://ll.shxzukj.cn

A. 基础语法与类型
来源：http://zw.gzmigu.cn

================================================================================
来源：http://jc.colortex.cn

[A01] Hello World
来源：http://ko.lnxyls.cn

Py:   print("Hello, World!")
来源：http://tj.521024.cn

PHP:  echo "Hello, World!";
来源：http://ei.haigaiapp.cn

JS:   console.log("Hello, World!");
来源：http://cj.panjiajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xd.haigaiapp.cn

Java: System.out.println("Hello, World!");
来源：http://jh.shtwfgs.cn

Go:   fmt.Println("Hello, World!")
来源：http://nr.shxzukj.cn

Ruby: puts "Hello, World!"
来源：http://yc.shxzukj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fh.521024.cn

[A02] 变量声明与赋值
来源：http://oi.yuntaijiaju.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xu.asd995.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hd.bjjhwx.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hp.bjjhwx.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qk.chemitech.net.cn

Java: String name = "Alex"; int age = 20;
来源：http://xk.gzmigu.cn

Go:   name := "Alex"; age := 20
来源：http://bc.hahajie.cn

Ruby: name = "Alex"; age = 20
来源：http://qr.chemitech.net.cn

C#:   string name = "Alex"; int age = 20;
来源：http://yi.wgjwhj.cn

[A03] 常量定义
来源：http://qs.jianghongdianzi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dl.asd995.cn

PHP:  const PI = 3.14159;
来源：http://mw.muxihuayi.cn

JS:   const PI = 3.14159;
来源：http://gd.hahajie.cn

TS:   const PI: number = 3.14159;
来源：http://pc.haigaiapp.cn

Java: static final double PI = 3.14159;
来源：http://lb.huanxung.cn

Go:   const PI = 3.14159
来源：http://jw.asd995.cn

Ruby: PI = 3.14159
来源：http://lb.521024.cn

C#:   const double PI = 3.14159;
来源：http://kx.jctech888.com.cn

[A04] 判断变量类型
来源：http://wo.hnjuh.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vs.chemitech.net.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://iu.jctech888.com.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qi.shtwfgs.cn

TS:   typeof x; x instanceof Date
来源：http://zg.haigaiapp.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tq.nicolike.cn

Go:   reflect.TypeOf(x).Name()
来源：http://qi.huanxung.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gk.panjiajie.cn

C#:   x.GetType().Name; x is int
来源：http://ns.yuntaijiaju.cn

[A05] 整数除法与取模
来源：http://fv.nicolike.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gs.huixiangedu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://he.shxzskj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://im.shtwfgs.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zy.jianghongdianzi.cn

Java: 7 / 2; 7 % 2
来源：http://sq.hnjuh.cn

Go:   7 / 2; 7 % 2
来源：http://av.newstarts.cn

Ruby: 7 / 2; 7 % 2
来源：http://lx.hahajie.cn

C#:   7 / 2; 7 % 2
来源：http://oc.panjiajie.cn

[A06] 字符串转数字
来源：http://hu.haigaiapp.cn

Py:   int("42"); float("3.14")
来源：http://lh.jctech888.com.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zl.huixiangedu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://sg.jctech888.com.cn

TS:   parseInt("42", 10); Number("42")
来源：http://tw.wgjwhj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://og.wgjwhj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uk.bookmarksfly.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://or.bjjhwx.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mq.yuntaijiaju.cn

[A07] 数字转字符串
来源：http://vo.colortex.cn

Py:   str(42)
来源：http://gw.chemitech.net.cn

PHP:  (string) 42; strval(42)
来源：http://og.9csxet.cn

JS:   String(42); (42).toString()
来源：http://no.szxytkj.cn

TS:   String(42)
来源：http://bq.yuexingan06.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://if.jctech888.com.cn

Go:   strconv.Itoa(42)
来源：http://wk.asd995.cn

Ruby: 42.to_s
来源：http://rg.gzmigu.cn

C#:   42.ToString()
来源：http://cm.521024.cn

[A08] 取整与四舍五入
来源：http://nh.bjjhwx.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://er.jianghongdianzi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yn.nicolike.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rj.huixiangedu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xi.huixinmuqiang.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mt.hahajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bu.huixiangedu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pm.wgjwhj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cw.asd995.cn

[A09] 绝对值与最大最小值
来源：http://tv.shtwfgs.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xm.bookmarksfly.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gk.nszjky.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sk.hnjuh.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mv.bjjhwx.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bk.chemitech.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ex.521024.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wo.yuntaijiaju.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gu.haigaiapp.cn

[A10] 生成随机数
来源：http://iu.nszjky.cn

Py:   import random; random.randint(1, 100)
来源：http://fh.lnxyls.cn

PHP:  random_int(1, 100);
来源：http://pz.bjjhwx.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jf.yuexingan06.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ms.panjiajie.cn

Java: new Random().nextInt(100) + 1
来源：http://kl.hahajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ab.wgjwhj.cn

Ruby: rand(1..100)
来源：http://zt.gzmigu.cn

C#:   new Random().Next(1, 101)
来源：http://jo.szsharing.cn

[A11] 条件表达式（三元）
来源：http://cs.bjjhwx.cn

Py:   "yes" if x > 0 else "no"
来源：http://jf.shtwfgs.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://kv.gzmigu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://jy.jianghongdianzi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://mu.huanxung.cn

Java: x > 0 ? "yes" : "no"
来源：http://jb.bookmarksfly.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://dt.jctech888.com.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://xv.panjiajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://mb.asd995.cn

[A12] 字符串插值 / 格式化
来源：http://qc.haigaiapp.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vf.panjiajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ev.colortex.cn

JS:   `Hello, ${name}!`
来源：http://vb.nicolike.cn

TS:   `Hello, ${name}!`
来源：http://xj.szsharing.cn

Java: "Hello, %s!".formatted(name)
来源：http://oq.szxytkj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rh.huanxung.cn

Ruby: "Hello, #{name}!"
来源：http://nf.muxihuayi.cn

C#:   $"Hello, {name}!"
来源：http://wl.wgjwhj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ym.gzmigu.cn

Py:   "第一行\n第二行"
来源：http://yr.panjiajie.cn

PHP:  "第一行\n第二行"
来源：http://tl.huixiangedu.cn

JS:   "第一行\n第二行"
来源：http://el.haigaiapp.cn

TS:   "第一行\n第二行"
来源：http://rg.szsharing.cn

Java: "第一行\n第二行"
来源：http://zr.yuntaijiaju.cn

Go:   "第一行\n第二行"
来源：http://vu.huixiangedu.cn

Ruby: "第一行\n第二行"
来源：http://kq.wgjwhj.cn

C#:   "第一行\n第二行"
来源：http://em.jctech888.com.cn

[A14] 注释写法
来源：http://vp.jctech888.com.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://de.colortex.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://dl.gzmigu.cn

JS:   // 单行；/* 多行 */
来源：http://yz.hahajie.cn

TS:   // 单行；/* 多行 */
来源：http://fz.wgjwhj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wc.lnxyls.cn

Go:   // 单行；/* 多行 */
来源：http://uz.bookmarksfly.cn

Ruby: # 单行；=begin 多行 =end
来源：http://gl.colortex.cn

C#:   // 单行；/* 多行 */
来源：http://qd.gzmigu.cn

[A15] 空值判断与默认值
来源：http://ie.chemitech.net.cn

Py:   value = data or "默认值"
来源：http://ud.bookmarksfly.cn

PHP:  $value = $data ?? "默认值";
来源：http://cv.szxytkj.cn

JS:   const value = data ?? "默认值";
来源：http://us.newstarts.cn

TS:   const value = data ?? "默认值";
来源：http://et.chemitech.net.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yt.huanxung.cn

Go:   if data == "" { data = "默认值" }
来源：http://vb.colortex.cn

Ruby: value = data || "默认值"
来源：http://xr.nicolike.cn

C#:   var value = data ?? "默认值";
来源：http://bi.jianghongdianzi.cn

[A16] 真假值判断规则
来源：http://as.szsharing.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zn.gzmigu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bq.yuexingan06.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rs.hnjuh.cn

TS:   if (!x) {}
来源：http://sr.yuntaijiaju.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cm.shxzskj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fr.newstarts.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ax.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sz.newstarts.cn

[A17] 位运算
来源：http://eo.bjjhwx.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rr.shtwfgs.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://le.shxzskj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wa.9csxet.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vn.hnjuh.cn


<!-- 参考信息 -->