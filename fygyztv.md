代发 wailian999

[U99] JS：事件监听
来源：http://tp.haigaiapp.cn

el.addEventListener("click", e => {})
来源：http://is.chemitech.net.cn

[U100] JS：DOM 查询
来源：http://nn.lnxyls.cn

document.querySelector(".item")
来源：http://qd.huixinmuqiang.cn

[U101] JS：classList 操作
来源：http://eh.huixinmuqiang.cn

el.classList.toggle("active")
来源：http://rr.jctech888.com.cn

[U102] JS：本地存储
来源：http://uo.panjiajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rz.wgjwhj.cn

[U103] JS：定时器
来源：http://du.chemitech.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yl.huixiangedu.cn

[U104] JS：防抖
来源：http://ou.yuexingan06.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qn.szsharing.cn

[U105] JS：节流
来源：http://cy.hahajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gg.521024.cn

[U106] JS：日期格式化
来源：http://ge.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hp.huixinmuqiang.cn

[U107] JS：数字千分位
来源：http://ic.jianghongdianzi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lc.muxihuayi.cn

[U108] JS：随机整数
来源：http://xa.lnxyls.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jm.hahajie.cn

[U109] JS：数组分组
来源：http://wh.nszjky.cn

Object.groupBy(arr, x => x.type)
来源：http://mm.jctech888.com.cn

[U110] JS：数组分块
来源：http://uo.szsharing.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qn.huixiangedu.cn

[U111] JS：对象转 Map
来源：http://bn.yuntaijiaju.cn

new Map(Object.entries(obj))
来源：http://rf.gzmigu.cn

[U112] JS：字符串补位
来源：http://cd.jctech888.com.cn

"7".padStart(3, "0")
来源：http://vm.shxzskj.cn

[U113] JS：正则替换全部
来源：http://ax.hahajie.cn

s.replaceAll("a", "b")
来源：http://ys.chemitech.net.cn

[U114] JS：JSON 深比较
来源：http://ep.hahajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ee.chemitech.net.cn

[U115] JS：生成 UUID
来源：http://qg.haigaiapp.cn

crypto.randomUUID()
来源：http://un.hnjuh.cn

[U116] JS：类型检查（JSDoc）
来源：http://wd.newstarts.cn

/** @param {string} name */ function f(name) {}
来源：http://js.bjjhwx.cn

[U117] JS：单元测试
来源：http://rn.bjjhwx.cn

npm i -D vitest;  npx vitest
来源：http://cw.shxzskj.cn

[U118] JS：开发服务器
来源：http://xn.huixiangedu.cn

npm i -D vite;  npx vite
来源：http://en.newstarts.cn

[U119] JS：生产构建
来源：http://hb.yuntaijiaju.cn

npx vite build
来源：http://ua.bookmarksfly.cn

[U120] JS：读取环境变量（Vite）
来源：http://xm.huanxung.cn

import.meta.env.VITE_API_URL
来源：http://nv.jianghongdianzi.cn

================================================================================
来源：http://so.szxytkj.cn

统计汇总
来源：http://ud.chemitech.net.cn

================================================================================
来源：http://uz.colortex.cn

按语言统计（条）：
来源：http://zu.yuntaijiaju.cn

Python ......... 252
来源：http://qu.hahajie.cn

PHP ............ 252
来源：http://ys.hnjuh.cn

JavaScript ..... 252
来源：http://yf.yuexingan06.cn

TypeScript ..... 212
来源：http://vm.nicolike.cn

Java ........... 212
来源：http://gh.colortex.cn

Go ............. 212
来源：http://lr.newstarts.cn

Ruby ........... 212
来源：http://jv.bjjhwx.cn

C# ............. 212
来源：http://gz.colortex.cn

C .............. 30
来源：http://do.shxzskj.cn

C++ ............ 30
来源：http://jo.huixinmuqiang.cn

SQL ............ 90
来源：http://vy.muxihuayi.cn

Bash ........... 80
来源：http://no.shxzskj.cn

Kotlin ......... 15
来源：http://od.asd995.cn

Swift .......... 15
来源：http://re.shxzskj.cn

Lua ............ 10
来源：http://el.szsharing.cn

Perl ........... 10
来源：http://za.panjiajie.cn

Scala .......... 10
来源：http://jv.bjjhwx.cn

------------------------------------
来源：http://nu.chemitech.net.cn

合计 ........... 2106 条
来源：http://wl.haigaiapp.cn

按章节统计：
来源：http://en.szsharing.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dt.jianghongdianzi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://em.asd995.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://eg.szxytkj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kd.hahajie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rg.521024.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ky.yuntaijiaju.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qe.haigaiapp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://km.hnjuh.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wm.nszjky.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://li.bookmarksfly.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ur.haigaiapp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ke.huixinmuqiang.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zs.panjiajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vy.asd995.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fa.jctech888.com.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://om.panjiajie.cn

Q SQL 专题                              90
来源：http://np.szxytkj.cn

R Bash 专题                             80
来源：http://mw.nicolike.cn

S C / C++ 专题                          60
来源：http://fs.wgjwhj.cn

T 其他语言补充                          60
来源：http://mc.haigaiapp.cn

U 高频实用片段                         120
来源：http://jq.521024.cn

------------------------------------
来源：http://uf.colortex.cn

合计                                  2106 条
来源：http://qi.colortex.cn

--------------------------------------------------------------------------------
来源：http://hd.gzmigu.cn

使用提醒
来源：http://js.9csxet.cn

--------------------------------------------------------------------------------
来源：http://cm.bookmarksfly.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hf.lnxyls.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yd.lnxyls.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kj.asd995.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://li.shxzskj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ws.jctech888.com.cn

—— 文件结束 ——
来源：http://fa.jianghongdianzi.cn

================================================================================
来源：http://dl.haigaiapp.cn

程序语言常见例子速查手册（2024 版）
来源：http://br.shxzskj.cn

Common Programming Examples Cheat Book
来源：http://vo.lnxyls.cn

================================================================================
来源：http://nv.huixiangedu.cn

【收录内容】
来源：http://px.wgjwhj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ja.shtwfgs.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tw.nszjky.cn

SQL · Bash · C · C++
来源：http://ul.jianghongdianzi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ll.yuexingan06.cn

【使用说明】
来源：http://nr.jctech888.com.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fi.panjiajie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nr.jctech888.com.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yk.huixinmuqiang.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gf.shxzskj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://hk.szxytkj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vz.wgjwhj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jr.shtwfgs.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://st.panjiajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ag.colortex.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ic.nszjky.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ks.shxzukj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://sa.yuntaijiaju.cn

【文件统计】
来源：http://mg.nicolike.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://du.9csxet.cn

--------------------------------------------------------------------------------
来源：http://or.huixinmuqiang.cn

目  录
来源：http://gc.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://ox.huixinmuqiang.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ub.newstarts.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ak.szxytkj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ds.jctech888.com.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yk.lnxyls.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mh.9csxet.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fr.hnjuh.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qn.shxzskj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zc.yuntaijiaju.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://uk.haigaiapp.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://po.haigaiapp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wo.chemitech.net.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kf.gzmigu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wq.newstarts.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nv.newstarts.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://er.szxytkj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kh.yuexingan06.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pn.shtwfgs.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://zr.chemitech.net.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jp.jianghongdianzi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cl.huixiangedu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://li.shxzskj.cn

================================================================================
来源：http://re.shxzskj.cn

A. 基础语法与类型
来源：http://sv.yuexingan06.cn

================================================================================
来源：http://ks.9csxet.cn

[A01] Hello World
来源：http://tf.nszjky.cn

Py:   print("Hello, World!")
来源：http://se.hnjuh.cn

PHP:  echo "Hello, World!";
来源：http://up.huixiangedu.cn

JS:   console.log("Hello, World!");
来源：http://xl.haigaiapp.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hy.nszjky.cn

Java: System.out.println("Hello, World!");
来源：http://cj.yuexingan06.cn

Go:   fmt.Println("Hello, World!")
来源：http://ss.shxzskj.cn

Ruby: puts "Hello, World!"
来源：http://pv.chemitech.net.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://nj.jctech888.com.cn

[A02] 变量声明与赋值
来源：http://tr.shtwfgs.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yr.521024.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rt.nicolike.cn

JS:   let name = "Alex"; const age = 20;
来源：http://pj.huixinmuqiang.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mm.hahajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://vj.asd995.cn

Go:   name := "Alex"; age := 20
来源：http://ft.nszjky.cn

Ruby: name = "Alex"; age = 20
来源：http://dn.newstarts.cn

C#:   string name = "Alex"; int age = 20;
来源：http://qf.asd995.cn

[A03] 常量定义
来源：http://bo.haigaiapp.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jo.newstarts.cn

PHP:  const PI = 3.14159;
来源：http://wb.lnxyls.cn

JS:   const PI = 3.14159;
来源：http://bt.nicolike.cn

TS:   const PI: number = 3.14159;
来源：http://ve.521024.cn

Java: static final double PI = 3.14159;
来源：http://kx.jianghongdianzi.cn

Go:   const PI = 3.14159
来源：http://tl.haigaiapp.cn

Ruby: PI = 3.14159
来源：http://ax.muxihuayi.cn

C#:   const double PI = 3.14159;
来源：http://cm.haigaiapp.cn

[A04] 判断变量类型
来源：http://uc.shxzskj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://fd.9csxet.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vv.szxytkj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wj.newstarts.cn

TS:   typeof x; x instanceof Date
来源：http://op.yuntaijiaju.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://my.nszjky.cn

Go:   reflect.TypeOf(x).Name()
来源：http://yj.huanxung.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://rt.szsharing.cn

C#:   x.GetType().Name; x is int
来源：http://zx.521024.cn

[A05] 整数除法与取模
来源：http://oo.jctech888.com.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://eo.newstarts.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ak.szsharing.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vy.szsharing.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bu.bookmarksfly.cn

Java: 7 / 2; 7 % 2
来源：http://ho.yuexingan06.cn

Go:   7 / 2; 7 % 2
来源：http://lf.shtwfgs.cn

Ruby: 7 / 2; 7 % 2
来源：http://ru.yuexingan06.cn

C#:   7 / 2; 7 % 2
来源：http://qk.huanxung.cn

[A06] 字符串转数字
来源：http://my.521024.cn

Py:   int("42"); float("3.14")
来源：http://aq.hnjuh.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wo.yuntaijiaju.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xi.haigaiapp.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ba.asd995.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://by.asd995.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://um.huixinmuqiang.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fq.haigaiapp.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rm.yuexingan06.cn

[A07] 数字转字符串
来源：http://wf.shxzukj.cn

Py:   str(42)
来源：http://px.szsharing.cn

PHP:  (string) 42; strval(42)
来源：http://qx.huanxung.cn

JS:   String(42); (42).toString()
来源：http://iw.shtwfgs.cn

TS:   String(42)
来源：http://ac.bjjhwx.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://dc.shxzskj.cn

Go:   strconv.Itoa(42)
来源：http://hn.shtwfgs.cn

Ruby: 42.to_s
来源：http://dz.lnxyls.cn

C#:   42.ToString()
来源：http://om.jctech888.com.cn

[A08] 取整与四舍五入
来源：http://ra.nszjky.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ab.yuexingan06.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xd.newstarts.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ag.nszjky.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ev.huanxung.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qy.szxytkj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://sw.hahajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ef.shxzukj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://og.newstarts.cn

[A09] 绝对值与最大最小值
来源：http://tf.nszjky.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yk.lnxyls.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fg.nicolike.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yo.panjiajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ni.muxihuayi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ic.muxihuayi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ht.gzmigu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pu.lnxyls.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fg.gzmigu.cn

[A10] 生成随机数
来源：http://hg.bookmarksfly.cn

Py:   import random; random.randint(1, 100)
来源：http://bs.huixinmuqiang.cn

PHP:  random_int(1, 100);
来源：http://id.nicolike.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bq.shtwfgs.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://id.muxihuayi.cn

Java: new Random().nextInt(100) + 1
来源：http://vc.haigaiapp.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dm.huanxung.cn

Ruby: rand(1..100)
来源：http://bn.huanxung.cn

C#:   new Random().Next(1, 101)
来源：http://qu.huixiangedu.cn

[A11] 条件表达式（三元）
来源：http://qs.bjjhwx.cn

Py:   "yes" if x > 0 else "no"
来源：http://ni.jctech888.com.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://tr.nicolike.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rb.hnjuh.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ng.yuntaijiaju.cn

Java: x > 0 ? "yes" : "no"
来源：http://ef.chemitech.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hj.bookmarksfly.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://bu.bjjhwx.cn

C#:   x > 0 ? "yes" : "no"
来源：http://lx.bjjhwx.cn

[A12] 字符串插值 / 格式化
来源：http://hl.panjiajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ce.newstarts.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kb.lnxyls.cn

JS:   `Hello, ${name}!`
来源：http://yw.yuexingan06.cn

TS:   `Hello, ${name}!`
来源：http://sg.hnjuh.cn

Java: "Hello, %s!".formatted(name)
来源：http://oy.huixiangedu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://es.wgjwhj.cn

Ruby: "Hello, #{name}!"
来源：http://rt.shxzukj.cn

C#:   $"Hello, {name}!"
来源：http://dh.hahajie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://in.bookmarksfly.cn

Py:   "第一行\n第二行"
来源：http://fy.colortex.cn

PHP:  "第一行\n第二行"
来源：http://vn.shtwfgs.cn

JS:   "第一行\n第二行"
来源：http://fd.hahajie.cn

TS:   "第一行\n第二行"
来源：http://qz.shxzskj.cn

Java: "第一行\n第二行"
来源：http://um.shxzukj.cn

Go:   "第一行\n第二行"
来源：http://ed.chemitech.net.cn

Ruby: "第一行\n第二行"
来源：http://hk.huixinmuqiang.cn

C#:   "第一行\n第二行"
来源：http://li.muxihuayi.cn

[A14] 注释写法
来源：http://kz.jctech888.com.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://hh.colortex.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://cb.yuntaijiaju.cn

JS:   // 单行；/* 多行 */
来源：http://qf.nicolike.cn

TS:   // 单行；/* 多行 */
来源：http://lg.panjiajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qx.szsharing.cn

Go:   // 单行；/* 多行 */
来源：http://ze.asd995.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ep.shtwfgs.cn

C#:   // 单行；/* 多行 */
来源：http://xs.colortex.cn

[A15] 空值判断与默认值
来源：http://ys.huixinmuqiang.cn

Py:   value = data or "默认值"
来源：http://ax.huanxung.cn

PHP:  $value = $data ?? "默认值";
来源：http://ok.jctech888.com.cn

JS:   const value = data ?? "默认值";
来源：http://zd.hnjuh.cn

TS:   const value = data ?? "默认值";
来源：http://dd.haigaiapp.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rg.shxzskj.cn

Go:   if data == "" { data = "默认值" }
来源：http://vl.shxzukj.cn

Ruby: value = data || "默认值"
来源：http://ul.hnjuh.cn

C#:   var value = data ?? "默认值";
来源：http://db.asd995.cn

[A16] 真假值判断规则
来源：http://am.szxytkj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yg.muxihuayi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ak.nszjky.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bc.huixinmuqiang.cn

TS:   if (!x) {}
来源：http://pd.yuntaijiaju.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bn.huixiangedu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lf.haigaiapp.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xs.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wz.gzmigu.cn

[A17] 位运算
来源：http://hm.huixiangedu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lj.panjiajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ox.wgjwhj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ax.shtwfgs.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kw.bookmarksfly.cn


<!-- 参考信息 -->