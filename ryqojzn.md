代发 wailian999

[U91] JS：对象键值遍历
来源：http://ut.jctech888.com.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xs.haigaiapp.cn

[U92] JS：深拷贝
来源：http://gk.nszjky.cn

structuredClone(obj)
来源：http://pr.colortex.cn

[U93] JS：模板字符串
来源：http://go.hahajie.cn

`共 ${n} 条`
来源：http://ns.wgjwhj.cn

[U94] JS：箭头函数
来源：http://ql.jctech888.com.cn

const double = x => x * 2;
来源：http://ee.bjjhwx.cn

[U95] JS：Promise 包装
来源：http://hh.nszjky.cn

new Promise((resolve, reject) => {})
来源：http://ra.yuntaijiaju.cn

[U96] JS：async/await 与异常
来源：http://rg.colortex.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cw.shtwfgs.cn

[U97] JS：并发请求
来源：http://gy.newstarts.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://nw.yuntaijiaju.cn

[U98] JS：fetch 带 JSON
来源：http://lo.gzmigu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nb.shtwfgs.cn

[U99] JS：事件监听
来源：http://ss.colortex.cn

el.addEventListener("click", e => {})
来源：http://pp.szsharing.cn

[U100] JS：DOM 查询
来源：http://pm.hnjuh.cn

document.querySelector(".item")
来源：http://pb.jctech888.com.cn

[U101] JS：classList 操作
来源：http://fx.jianghongdianzi.cn

el.classList.toggle("active")
来源：http://he.jctech888.com.cn

[U102] JS：本地存储
来源：http://fu.nicolike.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zu.shxzukj.cn

[U103] JS：定时器
来源：http://mx.colortex.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yf.521024.cn

[U104] JS：防抖
来源：http://li.nicolike.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ve.jianghongdianzi.cn

[U105] JS：节流
来源：http://nc.szxytkj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ln.shxzskj.cn

[U106] JS：日期格式化
来源：http://yx.yuexingan06.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://so.nszjky.cn

[U107] JS：数字千分位
来源：http://lf.521024.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mx.muxihuayi.cn

[U108] JS：随机整数
来源：http://tz.colortex.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zk.shtwfgs.cn

[U109] JS：数组分组
来源：http://nv.szxytkj.cn

Object.groupBy(arr, x => x.type)
来源：http://jx.asd995.cn

[U110] JS：数组分块
来源：http://pc.szxytkj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://os.jctech888.com.cn

[U111] JS：对象转 Map
来源：http://pw.jctech888.com.cn

new Map(Object.entries(obj))
来源：http://mi.colortex.cn

[U112] JS：字符串补位
来源：http://rf.jctech888.com.cn

"7".padStart(3, "0")
来源：http://lb.colortex.cn

[U113] JS：正则替换全部
来源：http://aj.shxzukj.cn

s.replaceAll("a", "b")
来源：http://en.shxzukj.cn

[U114] JS：JSON 深比较
来源：http://kg.nicolike.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mn.wgjwhj.cn

[U115] JS：生成 UUID
来源：http://ym.shxzskj.cn

crypto.randomUUID()
来源：http://hg.shtwfgs.cn

[U116] JS：类型检查（JSDoc）
来源：http://lp.huanxung.cn

/** @param {string} name */ function f(name) {}
来源：http://wd.lnxyls.cn

[U117] JS：单元测试
来源：http://rq.bjjhwx.cn

npm i -D vitest;  npx vitest
来源：http://df.nszjky.cn

[U118] JS：开发服务器
来源：http://ho.newstarts.cn

npm i -D vite;  npx vite
来源：http://lg.jianghongdianzi.cn

[U119] JS：生产构建
来源：http://dl.bookmarksfly.cn

npx vite build
来源：http://cm.colortex.cn

[U120] JS：读取环境变量（Vite）
来源：http://oo.huixiangedu.cn

import.meta.env.VITE_API_URL
来源：http://qv.szsharing.cn

================================================================================
来源：http://rk.huanxung.cn

统计汇总
来源：http://gb.521024.cn

================================================================================
来源：http://tn.bookmarksfly.cn

按语言统计（条）：
来源：http://mp.gzmigu.cn

Python ......... 252
来源：http://to.huanxung.cn

PHP ............ 252
来源：http://dc.jctech888.com.cn

JavaScript ..... 252
来源：http://vm.yuexingan06.cn

TypeScript ..... 212
来源：http://dx.wgjwhj.cn

Java ........... 212
来源：http://mw.colortex.cn

Go ............. 212
来源：http://va.hnjuh.cn

Ruby ........... 212
来源：http://bg.gzmigu.cn

C# ............. 212
来源：http://il.asd995.cn

C .............. 30
来源：http://ql.yuexingan06.cn

C++ ............ 30
来源：http://xy.szsharing.cn

SQL ............ 90
来源：http://eb.hahajie.cn

Bash ........... 80
来源：http://ep.muxihuayi.cn

Kotlin ......... 15
来源：http://nn.yuntaijiaju.cn

Swift .......... 15
来源：http://dp.hnjuh.cn

Lua ............ 10
来源：http://tp.huixiangedu.cn

Perl ........... 10
来源：http://es.lnxyls.cn

Scala .......... 10
来源：http://hv.bookmarksfly.cn

------------------------------------
来源：http://ks.bjjhwx.cn

合计 ........... 2106 条
来源：http://ff.bjjhwx.cn

按章节统计：
来源：http://sc.colortex.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wd.haigaiapp.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cw.521024.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cf.newstarts.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://th.yuntaijiaju.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kq.yuntaijiaju.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ph.szsharing.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xm.521024.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xu.shxzskj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zz.hnjuh.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rb.hahajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ke.hnjuh.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cd.shxzskj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zd.hahajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ko.huixiangedu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gr.nicolike.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ld.shxzukj.cn

Q SQL 专题                              90
来源：http://mf.shxzukj.cn

R Bash 专题                             80
来源：http://ug.colortex.cn

S C / C++ 专题                          60
来源：http://wh.nicolike.cn

T 其他语言补充                          60
来源：http://jt.newstarts.cn

U 高频实用片段                         120
来源：http://yk.521024.cn

------------------------------------
来源：http://dc.muxihuayi.cn

合计                                  2106 条
来源：http://gt.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://fs.nicolike.cn

使用提醒
来源：http://kt.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://wf.newstarts.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yc.shxzukj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ge.hahajie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ap.wgjwhj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://lq.shxzskj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ot.bookmarksfly.cn

—— 文件结束 ——
来源：http://gc.szsharing.cn

================================================================================
来源：http://qz.huanxung.cn

程序语言常见例子速查手册（2024 版）
来源：http://wc.yuntaijiaju.cn

Common Programming Examples Cheat Book
来源：http://uz.wgjwhj.cn

================================================================================
来源：http://rk.colortex.cn

【收录内容】
来源：http://wa.hnjuh.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://sv.521024.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gc.szxytkj.cn

SQL · Bash · C · C++
来源：http://td.szsharing.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://st.yuntaijiaju.cn

【使用说明】
来源：http://vv.jctech888.com.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://px.bjjhwx.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tt.chemitech.net.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ir.muxihuayi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gx.gzmigu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://sf.gzmigu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jt.bjjhwx.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nq.yuexingan06.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gw.chemitech.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mq.bjjhwx.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gw.szsharing.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://up.nicolike.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ks.chemitech.net.cn

【文件统计】
来源：http://dl.muxihuayi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zn.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://zu.yuexingan06.cn

目  录
来源：http://eb.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://cg.521024.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dv.521024.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ri.haigaiapp.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vo.huanxung.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ov.gzmigu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://al.hahajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wh.lnxyls.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mh.9csxet.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qi.shtwfgs.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tl.lnxyls.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lo.lnxyls.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://uo.lnxyls.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ot.haigaiapp.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hy.yuexingan06.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pe.jianghongdianzi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hb.asd995.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mi.szsharing.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pt.bjjhwx.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bb.newstarts.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tu.9csxet.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nr.szxytkj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dk.huixiangedu.cn

================================================================================
来源：http://vq.nszjky.cn

A. 基础语法与类型
来源：http://ue.nicolike.cn

================================================================================
来源：http://dy.wgjwhj.cn

[A01] Hello World
来源：http://sz.panjiajie.cn

Py:   print("Hello, World!")
来源：http://it.huixinmuqiang.cn

PHP:  echo "Hello, World!";
来源：http://pi.huanxung.cn

JS:   console.log("Hello, World!");
来源：http://mq.9csxet.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://it.chemitech.net.cn

Java: System.out.println("Hello, World!");
来源：http://xe.haigaiapp.cn

Go:   fmt.Println("Hello, World!")
来源：http://ue.jctech888.com.cn

Ruby: puts "Hello, World!"
来源：http://mx.yuntaijiaju.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vr.shxzukj.cn

[A02] 变量声明与赋值
来源：http://up.shtwfgs.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nf.shtwfgs.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://cr.shxzskj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vq.wgjwhj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lg.gzmigu.cn

Java: String name = "Alex"; int age = 20;
来源：http://nx.muxihuayi.cn

Go:   name := "Alex"; age := 20
来源：http://xz.nszjky.cn

Ruby: name = "Alex"; age = 20
来源：http://iq.haigaiapp.cn

C#:   string name = "Alex"; int age = 20;
来源：http://gp.huixinmuqiang.cn

[A03] 常量定义
来源：http://nr.nszjky.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tg.bjjhwx.cn

PHP:  const PI = 3.14159;
来源：http://xu.shxzukj.cn

JS:   const PI = 3.14159;
来源：http://cw.hnjuh.cn

TS:   const PI: number = 3.14159;
来源：http://yh.panjiajie.cn

Java: static final double PI = 3.14159;
来源：http://hr.9csxet.cn

Go:   const PI = 3.14159
来源：http://ep.nszjky.cn

Ruby: PI = 3.14159
来源：http://ov.huixinmuqiang.cn

C#:   const double PI = 3.14159;
来源：http://ev.521024.cn

[A04] 判断变量类型
来源：http://mj.gzmigu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://uv.colortex.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fg.shtwfgs.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bj.colortex.cn

TS:   typeof x; x instanceof Date
来源：http://nv.jctech888.com.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cd.szsharing.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ax.colortex.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vk.jctech888.com.cn

C#:   x.GetType().Name; x is int
来源：http://ad.shtwfgs.cn

[A05] 整数除法与取模
来源：http://mm.lnxyls.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://th.shxzskj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://bl.shxzskj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ps.shtwfgs.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mf.panjiajie.cn

Java: 7 / 2; 7 % 2
来源：http://jq.yuexingan06.cn

Go:   7 / 2; 7 % 2
来源：http://oq.shtwfgs.cn

Ruby: 7 / 2; 7 % 2
来源：http://wh.lnxyls.cn

C#:   7 / 2; 7 % 2
来源：http://wo.shxzukj.cn

[A06] 字符串转数字
来源：http://yk.hahajie.cn

Py:   int("42"); float("3.14")
来源：http://fw.huixinmuqiang.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gq.jctech888.com.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://sy.lnxyls.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ec.muxihuayi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hg.shtwfgs.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jc.chemitech.net.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ok.haigaiapp.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xd.wgjwhj.cn

[A07] 数字转字符串
来源：http://iw.shtwfgs.cn

Py:   str(42)
来源：http://qu.bjjhwx.cn

PHP:  (string) 42; strval(42)
来源：http://jz.jianghongdianzi.cn

JS:   String(42); (42).toString()
来源：http://kn.jianghongdianzi.cn

TS:   String(42)
来源：http://bk.newstarts.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ok.yuntaijiaju.cn

Go:   strconv.Itoa(42)
来源：http://ys.521024.cn

Ruby: 42.to_s
来源：http://jp.shxzukj.cn

C#:   42.ToString()
来源：http://ip.muxihuayi.cn

[A08] 取整与四舍五入
来源：http://mo.jianghongdianzi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cf.huixinmuqiang.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ce.shxzukj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lv.lnxyls.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nv.shxzskj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wc.jctech888.com.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vk.huixinmuqiang.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://hx.haigaiapp.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jr.haigaiapp.cn

[A09] 绝对值与最大最小值
来源：http://py.yuexingan06.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yu.lnxyls.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yl.szsharing.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zt.szxytkj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cb.panjiajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ru.asd995.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ij.bookmarksfly.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hy.shxzskj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ek.asd995.cn

[A10] 生成随机数
来源：http://hr.nszjky.cn

Py:   import random; random.randint(1, 100)
来源：http://ni.panjiajie.cn

PHP:  random_int(1, 100);
来源：http://zj.yuexingan06.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gk.9csxet.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bb.haigaiapp.cn

Java: new Random().nextInt(100) + 1
来源：http://ju.huixinmuqiang.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wr.asd995.cn

Ruby: rand(1..100)
来源：http://te.chemitech.net.cn

C#:   new Random().Next(1, 101)
来源：http://uk.yuntaijiaju.cn

[A11] 条件表达式（三元）
来源：http://yv.chemitech.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://md.chemitech.net.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://wa.huixiangedu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rb.huixinmuqiang.cn

TS:   x > 0 ? "yes" : "no"
来源：http://lb.wgjwhj.cn

Java: x > 0 ? "yes" : "no"
来源：http://vw.colortex.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://gc.yuntaijiaju.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://tl.panjiajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ny.hahajie.cn

[A12] 字符串插值 / 格式化
来源：http://dl.nszjky.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nf.9csxet.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://oh.shtwfgs.cn

JS:   `Hello, ${name}!`
来源：http://zx.haigaiapp.cn

TS:   `Hello, ${name}!`
来源：http://pz.szsharing.cn

Java: "Hello, %s!".formatted(name)
来源：http://rx.shxzukj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vo.chemitech.net.cn

Ruby: "Hello, #{name}!"
来源：http://ty.lnxyls.cn

C#:   $"Hello, {name}!"
来源：http://tg.gzmigu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://uv.haigaiapp.cn

Py:   "第一行\n第二行"
来源：http://wc.521024.cn

PHP:  "第一行\n第二行"
来源：http://nz.asd995.cn

JS:   "第一行\n第二行"
来源：http://kw.bjjhwx.cn

TS:   "第一行\n第二行"
来源：http://cr.panjiajie.cn

Java: "第一行\n第二行"
来源：http://yg.shxzskj.cn

Go:   "第一行\n第二行"
来源：http://hy.hahajie.cn

Ruby: "第一行\n第二行"
来源：http://gq.asd995.cn

C#:   "第一行\n第二行"
来源：http://iq.yuntaijiaju.cn

[A14] 注释写法
来源：http://bq.nszjky.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://kc.hahajie.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://na.521024.cn

JS:   // 单行；/* 多行 */
来源：http://rr.9csxet.cn

TS:   // 单行；/* 多行 */
来源：http://zb.bjjhwx.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mu.521024.cn

Go:   // 单行；/* 多行 */
来源：http://rr.huixinmuqiang.cn

Ruby: # 单行；=begin 多行 =end
来源：http://mt.bookmarksfly.cn

C#:   // 单行；/* 多行 */
来源：http://db.huixinmuqiang.cn

[A15] 空值判断与默认值
来源：http://mg.muxihuayi.cn

Py:   value = data or "默认值"
来源：http://tm.shxzukj.cn

PHP:  $value = $data ?? "默认值";
来源：http://ym.colortex.cn

JS:   const value = data ?? "默认值";
来源：http://vo.muxihuayi.cn

TS:   const value = data ?? "默认值";
来源：http://zl.huixinmuqiang.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vx.521024.cn

Go:   if data == "" { data = "默认值" }
来源：http://nc.521024.cn


<!-- 参考信息 -->