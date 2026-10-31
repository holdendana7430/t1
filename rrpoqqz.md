代发 wailian999

[U97] JS：并发请求
来源：http://eb.jctech888.com.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://wr.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://zb.9csxet.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rs.huixinmuqiang.cn

[U99] JS：事件监听
来源：http://oi.muxihuayi.cn

el.addEventListener("click", e => {})
来源：http://hv.9csxet.cn

[U100] JS：DOM 查询
来源：http://gs.yuexingan06.cn

document.querySelector(".item")
来源：http://cu.jianghongdianzi.cn

[U101] JS：classList 操作
来源：http://yu.yuntaijiaju.cn

el.classList.toggle("active")
来源：http://kd.nszjky.cn

[U102] JS：本地存储
来源：http://jh.asd995.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wf.newstarts.cn

[U103] JS：定时器
来源：http://ro.haigaiapp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ka.shxzukj.cn

[U104] JS：防抖
来源：http://pk.lnxyls.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qj.szsharing.cn

[U105] JS：节流
来源：http://vb.panjiajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jw.shxzskj.cn

[U106] JS：日期格式化
来源：http://rk.hahajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jf.nszjky.cn

[U107] JS：数字千分位
来源：http://hi.shxzskj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hx.muxihuayi.cn

[U108] JS：随机整数
来源：http://ve.wgjwhj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qy.hnjuh.cn

[U109] JS：数组分组
来源：http://ak.bjjhwx.cn

Object.groupBy(arr, x => x.type)
来源：http://hs.muxihuayi.cn

[U110] JS：数组分块
来源：http://hr.wgjwhj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uw.szsharing.cn

[U111] JS：对象转 Map
来源：http://mq.jianghongdianzi.cn

new Map(Object.entries(obj))
来源：http://od.chemitech.net.cn

[U112] JS：字符串补位
来源：http://xj.9csxet.cn

"7".padStart(3, "0")
来源：http://xy.gzmigu.cn

[U113] JS：正则替换全部
来源：http://ig.colortex.cn

s.replaceAll("a", "b")
来源：http://vs.huanxung.cn

[U114] JS：JSON 深比较
来源：http://hy.huixiangedu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://is.nszjky.cn

[U115] JS：生成 UUID
来源：http://du.huixinmuqiang.cn

crypto.randomUUID()
来源：http://or.chemitech.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://hz.jianghongdianzi.cn

/** @param {string} name */ function f(name) {}
来源：http://cm.9csxet.cn

[U117] JS：单元测试
来源：http://pj.bjjhwx.cn

npm i -D vitest;  npx vitest
来源：http://dm.jianghongdianzi.cn

[U118] JS：开发服务器
来源：http://rt.nicolike.cn

npm i -D vite;  npx vite
来源：http://oz.nicolike.cn

[U119] JS：生产构建
来源：http://vw.huixiangedu.cn

npx vite build
来源：http://at.shxzskj.cn

[U120] JS：读取环境变量（Vite）
来源：http://up.huixinmuqiang.cn

import.meta.env.VITE_API_URL
来源：http://mi.huixiangedu.cn

================================================================================
来源：http://pw.nicolike.cn

统计汇总
来源：http://wn.nszjky.cn

================================================================================
来源：http://vs.yuexingan06.cn

按语言统计（条）：
来源：http://vt.shxzukj.cn

Python ......... 252
来源：http://vs.muxihuayi.cn

PHP ............ 252
来源：http://mj.bjjhwx.cn

JavaScript ..... 252
来源：http://on.yuntaijiaju.cn

TypeScript ..... 212
来源：http://fv.jctech888.com.cn

Java ........... 212
来源：http://wq.asd995.cn

Go ............. 212
来源：http://lg.szsharing.cn

Ruby ........... 212
来源：http://zb.szxytkj.cn

C# ............. 212
来源：http://ad.yuntaijiaju.cn

C .............. 30
来源：http://sr.asd995.cn

C++ ............ 30
来源：http://fn.shxzukj.cn

SQL ............ 90
来源：http://kg.hnjuh.cn

Bash ........... 80
来源：http://wg.jianghongdianzi.cn

Kotlin ......... 15
来源：http://fm.haigaiapp.cn

Swift .......... 15
来源：http://dc.gzmigu.cn

Lua ............ 10
来源：http://rf.hnjuh.cn

Perl ........... 10
来源：http://im.gzmigu.cn

Scala .......... 10
来源：http://fj.haigaiapp.cn

------------------------------------
来源：http://cc.yuntaijiaju.cn

合计 ........... 2106 条
来源：http://ah.newstarts.cn

按章节统计：
来源：http://xp.yuntaijiaju.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fb.shxzukj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://an.huanxung.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uv.muxihuayi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ur.shxzukj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ua.colortex.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kg.wgjwhj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jy.colortex.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rn.huixinmuqiang.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ov.521024.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ve.huixinmuqiang.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ww.szsharing.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ly.jctech888.com.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sx.chemitech.net.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fn.shxzukj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hj.hnjuh.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fb.wgjwhj.cn

Q SQL 专题                              90
来源：http://cd.huixinmuqiang.cn

R Bash 专题                             80
来源：http://ep.bookmarksfly.cn

S C / C++ 专题                          60
来源：http://vf.huanxung.cn

T 其他语言补充                          60
来源：http://th.haigaiapp.cn

U 高频实用片段                         120
来源：http://os.huixiangedu.cn

------------------------------------
来源：http://zq.shxzskj.cn

合计                                  2106 条
来源：http://xt.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://cq.bjjhwx.cn

使用提醒
来源：http://tt.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://oy.muxihuayi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mz.hnjuh.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://us.haigaiapp.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://av.szxytkj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://au.wgjwhj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ve.chemitech.net.cn

—— 文件结束 ——
来源：http://gw.jctech888.com.cn

================================================================================
来源：http://ei.yuexingan06.cn

程序语言常见例子速查手册（2024 版）
来源：http://ss.yuntaijiaju.cn

Common Programming Examples Cheat Book
来源：http://bh.jianghongdianzi.cn

================================================================================
来源：http://it.huixinmuqiang.cn

【收录内容】
来源：http://mu.jctech888.com.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://yo.huanxung.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hi.haigaiapp.cn

SQL · Bash · C · C++
来源：http://mn.colortex.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qj.bookmarksfly.cn

【使用说明】
来源：http://fz.shxzukj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ba.panjiajie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://av.bookmarksfly.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://no.bookmarksfly.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://os.bookmarksfly.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://pk.huixinmuqiang.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ne.haigaiapp.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mj.shxzskj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fs.nicolike.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jc.9csxet.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ql.gzmigu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wi.szsharing.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://oc.bookmarksfly.cn

【文件统计】
来源：http://cu.huixinmuqiang.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rh.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://xq.hahajie.cn

目  录
来源：http://uv.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://sv.muxihuayi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gv.shtwfgs.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sz.colortex.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ud.wgjwhj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rx.bjjhwx.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wz.jctech888.com.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vv.muxihuayi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gm.asd995.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ed.shtwfgs.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tq.lnxyls.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://iq.bjjhwx.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dx.shtwfgs.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rp.nicolike.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://uu.chemitech.net.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cz.wgjwhj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sp.lnxyls.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ga.wgjwhj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://th.shtwfgs.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ti.huixinmuqiang.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ln.lnxyls.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mi.colortex.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rz.huanxung.cn

================================================================================
来源：http://as.panjiajie.cn

A. 基础语法与类型
来源：http://lf.shxzukj.cn

================================================================================
来源：http://fx.lnxyls.cn

[A01] Hello World
来源：http://dr.9csxet.cn

Py:   print("Hello, World!")
来源：http://wi.yuntaijiaju.cn

PHP:  echo "Hello, World!";
来源：http://wq.szsharing.cn

JS:   console.log("Hello, World!");
来源：http://hq.yuntaijiaju.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ej.shtwfgs.cn

Java: System.out.println("Hello, World!");
来源：http://bj.shtwfgs.cn

Go:   fmt.Println("Hello, World!")
来源：http://ab.wgjwhj.cn

Ruby: puts "Hello, World!"
来源：http://jj.nicolike.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ul.hahajie.cn

[A02] 变量声明与赋值
来源：http://as.chemitech.net.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zh.asd995.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://sg.hnjuh.cn

JS:   let name = "Alex"; const age = 20;
来源：http://zx.chemitech.net.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hh.szxytkj.cn

Java: String name = "Alex"; int age = 20;
来源：http://ti.panjiajie.cn

Go:   name := "Alex"; age := 20
来源：http://tb.yuexingan06.cn

Ruby: name = "Alex"; age = 20
来源：http://ag.shxzukj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://dv.wgjwhj.cn

[A03] 常量定义
来源：http://hx.jianghongdianzi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ik.colortex.cn

PHP:  const PI = 3.14159;
来源：http://ah.hnjuh.cn

JS:   const PI = 3.14159;
来源：http://iq.gzmigu.cn

TS:   const PI: number = 3.14159;
来源：http://ah.szxytkj.cn

Java: static final double PI = 3.14159;
来源：http://sh.jianghongdianzi.cn

Go:   const PI = 3.14159
来源：http://lo.szxytkj.cn

Ruby: PI = 3.14159
来源：http://gy.yuexingan06.cn

C#:   const double PI = 3.14159;
来源：http://rq.bookmarksfly.cn

[A04] 判断变量类型
来源：http://qk.wgjwhj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vj.shxzukj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tl.9csxet.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lh.9csxet.cn

TS:   typeof x; x instanceof Date
来源：http://wq.9csxet.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xc.9csxet.cn

Go:   reflect.TypeOf(x).Name()
来源：http://xp.lnxyls.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://jw.hnjuh.cn

C#:   x.GetType().Name; x is int
来源：http://be.jianghongdianzi.cn

[A05] 整数除法与取模
来源：http://fs.yuexingan06.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hl.muxihuayi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ha.yuntaijiaju.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nv.colortex.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://iu.chemitech.net.cn

Java: 7 / 2; 7 % 2
来源：http://jd.jctech888.com.cn

Go:   7 / 2; 7 % 2
来源：http://pq.yuntaijiaju.cn

Ruby: 7 / 2; 7 % 2
来源：http://xm.yuntaijiaju.cn

C#:   7 / 2; 7 % 2
来源：http://ag.shtwfgs.cn

[A06] 字符串转数字
来源：http://mb.newstarts.cn

Py:   int("42"); float("3.14")
来源：http://of.lnxyls.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gt.shxzskj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ma.szxytkj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://he.panjiajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gh.szxytkj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vw.jianghongdianzi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://xi.huixinmuqiang.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hs.9csxet.cn

[A07] 数字转字符串
来源：http://in.hnjuh.cn

Py:   str(42)
来源：http://xm.huanxung.cn

PHP:  (string) 42; strval(42)
来源：http://sx.bookmarksfly.cn

JS:   String(42); (42).toString()
来源：http://cd.yuntaijiaju.cn

TS:   String(42)
来源：http://xn.shxzukj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://am.colortex.cn

Go:   strconv.Itoa(42)
来源：http://qo.wgjwhj.cn

Ruby: 42.to_s
来源：http://gy.huanxung.cn

C#:   42.ToString()
来源：http://dh.colortex.cn

[A08] 取整与四舍五入
来源：http://uf.nszjky.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pq.521024.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xs.wgjwhj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fb.shxzskj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sd.hahajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yz.lnxyls.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jq.bjjhwx.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://jy.9csxet.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jg.521024.cn

[A09] 绝对值与最大最小值
来源：http://pm.shtwfgs.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mi.muxihuayi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jo.jianghongdianzi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hj.9csxet.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ee.shxzskj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mh.shxzskj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pb.chemitech.net.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ja.jctech888.com.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://di.nszjky.cn

[A10] 生成随机数
来源：http://og.jctech888.com.cn

Py:   import random; random.randint(1, 100)
来源：http://zl.jctech888.com.cn

PHP:  random_int(1, 100);
来源：http://vw.shxzukj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://uj.lnxyls.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://aq.asd995.cn

Java: new Random().nextInt(100) + 1
来源：http://lr.gzmigu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kx.colortex.cn

Ruby: rand(1..100)
来源：http://rw.chemitech.net.cn

C#:   new Random().Next(1, 101)
来源：http://wj.shxzskj.cn

[A11] 条件表达式（三元）
来源：http://tj.colortex.cn

Py:   "yes" if x > 0 else "no"
来源：http://id.shtwfgs.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ms.haigaiapp.cn

JS:   x > 0 ? "yes" : "no"
来源：http://gm.newstarts.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ff.huixinmuqiang.cn

Java: x > 0 ? "yes" : "no"
来源：http://mp.chemitech.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ti.shxzskj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://bo.lnxyls.cn

C#:   x > 0 ? "yes" : "no"
来源：http://hq.shxzukj.cn

[A12] 字符串插值 / 格式化
来源：http://pn.bookmarksfly.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wm.521024.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zs.shxzukj.cn

JS:   `Hello, ${name}!`
来源：http://pu.huixiangedu.cn

TS:   `Hello, ${name}!`
来源：http://lb.shxzskj.cn

Java: "Hello, %s!".formatted(name)
来源：http://yw.huanxung.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dm.asd995.cn

Ruby: "Hello, #{name}!"
来源：http://dc.jianghongdianzi.cn

C#:   $"Hello, {name}!"
来源：http://td.huanxung.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hl.gzmigu.cn

Py:   "第一行\n第二行"
来源：http://oi.szsharing.cn

PHP:  "第一行\n第二行"
来源：http://gh.shtwfgs.cn

JS:   "第一行\n第二行"
来源：http://pf.szxytkj.cn

TS:   "第一行\n第二行"
来源：http://ft.jianghongdianzi.cn

Java: "第一行\n第二行"
来源：http://en.shxzukj.cn

Go:   "第一行\n第二行"
来源：http://kk.wgjwhj.cn

Ruby: "第一行\n第二行"
来源：http://uy.bookmarksfly.cn

C#:   "第一行\n第二行"
来源：http://jm.nszjky.cn

[A14] 注释写法
来源：http://cl.hahajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://lr.jctech888.com.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tr.huixiangedu.cn

JS:   // 单行；/* 多行 */
来源：http://sl.shxzskj.cn

TS:   // 单行；/* 多行 */
来源：http://rt.newstarts.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ht.colortex.cn

Go:   // 单行；/* 多行 */
来源：http://zy.asd995.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ak.gzmigu.cn

C#:   // 单行；/* 多行 */
来源：http://dr.yuexingan06.cn

[A15] 空值判断与默认值
来源：http://dk.shxzskj.cn

Py:   value = data or "默认值"
来源：http://db.lnxyls.cn

PHP:  $value = $data ?? "默认值";
来源：http://qd.lnxyls.cn

JS:   const value = data ?? "默认值";
来源：http://gt.szxytkj.cn

TS:   const value = data ?? "默认值";
来源：http://vr.nicolike.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ac.hnjuh.cn

Go:   if data == "" { data = "默认值" }
来源：http://tx.muxihuayi.cn

Ruby: value = data || "默认值"
来源：http://jc.asd995.cn

C#:   var value = data ?? "默认值";
来源：http://bi.yuexingan06.cn

[A16] 真假值判断规则
来源：http://tf.muxihuayi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kf.jianghongdianzi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kj.gzmigu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jo.haigaiapp.cn

TS:   if (!x) {}
来源：http://vh.jctech888.com.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uh.wgjwhj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://om.yuexingan06.cn

Ruby: unless x            # nil 与 false 为假
来源：http://nq.szsharing.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qa.jianghongdianzi.cn

[A17] 位运算
来源：http://lv.9csxet.cn


<!-- 参考信息 -->