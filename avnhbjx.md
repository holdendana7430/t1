代发 wailian999

[U89] JS：数组去重
来源：http://qu.szxytkj.cn

[...new Set(arr)]
来源：http://yk.bjjhwx.cn

[U90] JS：数字数组排序
来源：http://bg.newstarts.cn

[...arr].sort((a, b) => a - b)
来源：http://wf.muxihuayi.cn

[U91] JS：对象键值遍历
来源：http://gn.gzmigu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yp.jctech888.com.cn

[U92] JS：深拷贝
来源：http://ee.9csxet.cn

structuredClone(obj)
来源：http://wb.lnxyls.cn

[U93] JS：模板字符串
来源：http://xd.colortex.cn

`共 ${n} 条`
来源：http://cb.szxytkj.cn

[U94] JS：箭头函数
来源：http://gk.asd995.cn

const double = x => x * 2;
来源：http://gd.szsharing.cn

[U95] JS：Promise 包装
来源：http://yi.colortex.cn

new Promise((resolve, reject) => {})
来源：http://nh.gzmigu.cn

[U96] JS：async/await 与异常
来源：http://dq.jianghongdianzi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ur.huixinmuqiang.cn

[U97] JS：并发请求
来源：http://cw.jctech888.com.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zw.shxzukj.cn

[U98] JS：fetch 带 JSON
来源：http://na.bjjhwx.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xz.shtwfgs.cn

[U99] JS：事件监听
来源：http://vc.wgjwhj.cn

el.addEventListener("click", e => {})
来源：http://pg.9csxet.cn

[U100] JS：DOM 查询
来源：http://ak.yuexingan06.cn

document.querySelector(".item")
来源：http://kf.yuexingan06.cn

[U101] JS：classList 操作
来源：http://rt.yuexingan06.cn

el.classList.toggle("active")
来源：http://bh.shxzskj.cn

[U102] JS：本地存储
来源：http://zq.shxzskj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://aw.bookmarksfly.cn

[U103] JS：定时器
来源：http://yg.gzmigu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cg.bjjhwx.cn

[U104] JS：防抖
来源：http://bx.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ca.bjjhwx.cn

[U105] JS：节流
来源：http://oc.newstarts.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yx.huixiangedu.cn

[U106] JS：日期格式化
来源：http://em.bjjhwx.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ss.nicolike.cn

[U107] JS：数字千分位
来源：http://ek.shxzukj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ze.haigaiapp.cn

[U108] JS：随机整数
来源：http://zz.9csxet.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gn.muxihuayi.cn

[U109] JS：数组分组
来源：http://bp.panjiajie.cn

Object.groupBy(arr, x => x.type)
来源：http://zj.szsharing.cn

[U110] JS：数组分块
来源：http://re.521024.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gf.wgjwhj.cn

[U111] JS：对象转 Map
来源：http://ne.szsharing.cn

new Map(Object.entries(obj))
来源：http://os.chemitech.net.cn

[U112] JS：字符串补位
来源：http://hz.521024.cn

"7".padStart(3, "0")
来源：http://ro.chemitech.net.cn

[U113] JS：正则替换全部
来源：http://wi.lnxyls.cn

s.replaceAll("a", "b")
来源：http://hy.colortex.cn

[U114] JS：JSON 深比较
来源：http://iw.yuexingan06.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mx.nszjky.cn

[U115] JS：生成 UUID
来源：http://et.shxzukj.cn

crypto.randomUUID()
来源：http://nx.gzmigu.cn

[U116] JS：类型检查（JSDoc）
来源：http://hm.lnxyls.cn

/** @param {string} name */ function f(name) {}
来源：http://di.haigaiapp.cn

[U117] JS：单元测试
来源：http://hz.yuexingan06.cn

npm i -D vitest;  npx vitest
来源：http://tx.nszjky.cn

[U118] JS：开发服务器
来源：http://yx.colortex.cn

npm i -D vite;  npx vite
来源：http://vs.wgjwhj.cn

[U119] JS：生产构建
来源：http://pf.shtwfgs.cn

npx vite build
来源：http://to.haigaiapp.cn

[U120] JS：读取环境变量（Vite）
来源：http://dd.huixiangedu.cn

import.meta.env.VITE_API_URL
来源：http://jp.hnjuh.cn

================================================================================
来源：http://ef.haigaiapp.cn

统计汇总
来源：http://rw.shxzskj.cn

================================================================================
来源：http://os.hahajie.cn

按语言统计（条）：
来源：http://qm.muxihuayi.cn

Python ......... 252
来源：http://hz.huixiangedu.cn

PHP ............ 252
来源：http://rv.asd995.cn

JavaScript ..... 252
来源：http://ec.muxihuayi.cn

TypeScript ..... 212
来源：http://bw.huixinmuqiang.cn

Java ........... 212
来源：http://qm.yuntaijiaju.cn

Go ............. 212
来源：http://im.hahajie.cn

Ruby ........... 212
来源：http://mb.nszjky.cn

C# ............. 212
来源：http://ad.521024.cn

C .............. 30
来源：http://cc.huixinmuqiang.cn

C++ ............ 30
来源：http://sx.521024.cn

SQL ............ 90
来源：http://wv.jianghongdianzi.cn

Bash ........... 80
来源：http://sy.bjjhwx.cn

Kotlin ......... 15
来源：http://jc.gzmigu.cn

Swift .......... 15
来源：http://ss.szxytkj.cn

Lua ............ 10
来源：http://ll.chemitech.net.cn

Perl ........... 10
来源：http://yn.huanxung.cn

Scala .......... 10
来源：http://nf.shxzukj.cn

------------------------------------
来源：http://lq.shxzskj.cn

合计 ........... 2106 条
来源：http://pp.shxzskj.cn

按章节统计：
来源：http://dx.shxzukj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sv.huanxung.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://py.haigaiapp.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sr.huixinmuqiang.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uz.chemitech.net.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mm.panjiajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kk.haigaiapp.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dh.shtwfgs.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kf.shxzskj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nn.huixinmuqiang.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://iq.yuntaijiaju.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wj.bjjhwx.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ft.yuntaijiaju.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qy.gzmigu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jc.yuexingan06.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bl.haigaiapp.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nv.yuntaijiaju.cn

Q SQL 专题                              90
来源：http://je.shxzukj.cn

R Bash 专题                             80
来源：http://cq.muxihuayi.cn

S C / C++ 专题                          60
来源：http://io.nszjky.cn

T 其他语言补充                          60
来源：http://pu.jctech888.com.cn

U 高频实用片段                         120
来源：http://vu.shtwfgs.cn

------------------------------------
来源：http://tb.jianghongdianzi.cn

合计                                  2106 条
来源：http://kw.nicolike.cn

--------------------------------------------------------------------------------
来源：http://iv.colortex.cn

使用提醒
来源：http://rh.nszjky.cn

--------------------------------------------------------------------------------
来源：http://km.asd995.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fm.gzmigu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lq.shxzskj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://av.wgjwhj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qa.newstarts.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zz.nszjky.cn

—— 文件结束 ——
来源：http://tn.szxytkj.cn

================================================================================
来源：http://ea.panjiajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://id.9csxet.cn

Common Programming Examples Cheat Book
来源：http://cr.shxzskj.cn

================================================================================
来源：http://mh.nicolike.cn

【收录内容】
来源：http://jc.hahajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qb.shtwfgs.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dt.wgjwhj.cn

SQL · Bash · C · C++
来源：http://wl.chemitech.net.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://go.jctech888.com.cn

【使用说明】
来源：http://dv.yuexingan06.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sv.shtwfgs.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ke.wgjwhj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ef.jctech888.com.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zu.521024.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://kh.colortex.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zs.shxzskj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ug.szsharing.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://je.muxihuayi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xc.haigaiapp.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ci.newstarts.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pm.huixiangedu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://sw.shtwfgs.cn

【文件统计】
来源：http://bj.huixinmuqiang.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://eh.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://mj.jianghongdianzi.cn

目  录
来源：http://gs.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://ss.hnjuh.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ut.wgjwhj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mq.nicolike.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xt.colortex.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ud.panjiajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ad.panjiajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ku.hahajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kb.yuntaijiaju.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ug.bjjhwx.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://yx.chemitech.net.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vl.hahajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vr.9csxet.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zp.yuexingan06.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vg.lnxyls.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qk.gzmigu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yf.nszjky.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ov.yuntaijiaju.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ix.chemitech.net.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://lj.yuntaijiaju.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hr.newstarts.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fi.szsharing.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nf.jctech888.com.cn

================================================================================
来源：http://rw.nicolike.cn

A. 基础语法与类型
来源：http://ee.yuexingan06.cn

================================================================================
来源：http://mw.521024.cn

[A01] Hello World
来源：http://xy.lnxyls.cn

Py:   print("Hello, World!")
来源：http://xa.nicolike.cn

PHP:  echo "Hello, World!";
来源：http://zs.nicolike.cn

JS:   console.log("Hello, World!");
来源：http://tg.nszjky.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tq.shxzukj.cn

Java: System.out.println("Hello, World!");
来源：http://jn.szsharing.cn

Go:   fmt.Println("Hello, World!")
来源：http://ms.yuexingan06.cn

Ruby: puts "Hello, World!"
来源：http://pi.yuntaijiaju.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fc.asd995.cn

[A02] 变量声明与赋值
来源：http://uq.shtwfgs.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jk.shxzukj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://nf.newstarts.cn

JS:   let name = "Alex"; const age = 20;
来源：http://tz.nicolike.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ma.haigaiapp.cn

Java: String name = "Alex"; int age = 20;
来源：http://ap.colortex.cn

Go:   name := "Alex"; age := 20
来源：http://qz.shxzskj.cn

Ruby: name = "Alex"; age = 20
来源：http://az.jianghongdianzi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://tq.hahajie.cn

[A03] 常量定义
来源：http://kd.panjiajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://es.shxzukj.cn

PHP:  const PI = 3.14159;
来源：http://yk.muxihuayi.cn

JS:   const PI = 3.14159;
来源：http://nn.gzmigu.cn

TS:   const PI: number = 3.14159;
来源：http://ho.chemitech.net.cn

Java: static final double PI = 3.14159;
来源：http://qw.yuntaijiaju.cn

Go:   const PI = 3.14159
来源：http://ao.colortex.cn

Ruby: PI = 3.14159
来源：http://cq.jianghongdianzi.cn

C#:   const double PI = 3.14159;
来源：http://yq.chemitech.net.cn

[A04] 判断变量类型
来源：http://ky.lnxyls.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://me.shxzskj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rr.wgjwhj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ya.hahajie.cn

TS:   typeof x; x instanceof Date
来源：http://dt.shtwfgs.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ts.bookmarksfly.cn

Go:   reflect.TypeOf(x).Name()
来源：http://uw.lnxyls.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://qi.huixinmuqiang.cn

C#:   x.GetType().Name; x is int
来源：http://rv.jianghongdianzi.cn

[A05] 整数除法与取模
来源：http://fl.szsharing.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ip.yuexingan06.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://an.lnxyls.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vx.newstarts.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ta.asd995.cn

Java: 7 / 2; 7 % 2
来源：http://sl.hahajie.cn

Go:   7 / 2; 7 % 2
来源：http://ce.panjiajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://xu.hnjuh.cn

C#:   7 / 2; 7 % 2
来源：http://es.wgjwhj.cn

[A06] 字符串转数字
来源：http://cm.9csxet.cn

Py:   int("42"); float("3.14")
来源：http://zo.shxzukj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://eu.szsharing.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pq.jianghongdianzi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://jo.jctech888.com.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://az.shxzukj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tu.panjiajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://el.yuntaijiaju.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hc.lnxyls.cn

[A07] 数字转字符串
来源：http://zd.shtwfgs.cn

Py:   str(42)
来源：http://ou.gzmigu.cn

PHP:  (string) 42; strval(42)
来源：http://fp.szsharing.cn

JS:   String(42); (42).toString()
来源：http://xk.gzmigu.cn

TS:   String(42)
来源：http://rf.haigaiapp.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zn.nicolike.cn

Go:   strconv.Itoa(42)
来源：http://kc.szsharing.cn

Ruby: 42.to_s
来源：http://va.szsharing.cn

C#:   42.ToString()
来源：http://eg.jianghongdianzi.cn

[A08] 取整与四舍五入
来源：http://yq.nicolike.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fk.huixinmuqiang.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ke.haigaiapp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xg.panjiajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ol.huixinmuqiang.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ho.hnjuh.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dj.jianghongdianzi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pt.panjiajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xk.nicolike.cn

[A09] 绝对值与最大最小值
来源：http://iq.szxytkj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cb.hahajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tj.asd995.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pm.szxytkj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cz.gzmigu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ue.asd995.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wv.chemitech.net.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qg.newstarts.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lk.chemitech.net.cn

[A10] 生成随机数
来源：http://su.yuexingan06.cn

Py:   import random; random.randint(1, 100)
来源：http://vk.chemitech.net.cn

PHP:  random_int(1, 100);
来源：http://qc.wgjwhj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pz.shxzskj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qc.huixiangedu.cn

Java: new Random().nextInt(100) + 1
来源：http://ik.yuntaijiaju.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://do.muxihuayi.cn

Ruby: rand(1..100)
来源：http://rb.jctech888.com.cn

C#:   new Random().Next(1, 101)
来源：http://xw.hnjuh.cn

[A11] 条件表达式（三元）
来源：http://vg.nszjky.cn

Py:   "yes" if x > 0 else "no"
来源：http://tz.lnxyls.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ff.yuexingan06.cn

JS:   x > 0 ? "yes" : "no"
来源：http://sv.muxihuayi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://wj.muxihuayi.cn

Java: x > 0 ? "yes" : "no"
来源：http://aw.yuexingan06.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://eg.9csxet.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://bx.bookmarksfly.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xh.szsharing.cn

[A12] 字符串插值 / 格式化
来源：http://gy.bookmarksfly.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fj.9csxet.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hw.nicolike.cn

JS:   `Hello, ${name}!`
来源：http://mg.jianghongdianzi.cn

TS:   `Hello, ${name}!`
来源：http://ky.9csxet.cn

Java: "Hello, %s!".formatted(name)
来源：http://bq.szsharing.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jj.panjiajie.cn

Ruby: "Hello, #{name}!"
来源：http://cb.wgjwhj.cn

C#:   $"Hello, {name}!"
来源：http://wo.hnjuh.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://wu.shxzskj.cn

Py:   "第一行\n第二行"
来源：http://ps.haigaiapp.cn

PHP:  "第一行\n第二行"
来源：http://tb.panjiajie.cn

JS:   "第一行\n第二行"
来源：http://as.bjjhwx.cn

TS:   "第一行\n第二行"
来源：http://xz.huixinmuqiang.cn

Java: "第一行\n第二行"
来源：http://bz.lnxyls.cn

Go:   "第一行\n第二行"
来源：http://rt.jianghongdianzi.cn

Ruby: "第一行\n第二行"
来源：http://mx.muxihuayi.cn

C#:   "第一行\n第二行"
来源：http://vi.shxzukj.cn

[A14] 注释写法
来源：http://ya.szsharing.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ph.lnxyls.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tu.bjjhwx.cn

JS:   // 单行；/* 多行 */
来源：http://qj.muxihuayi.cn

TS:   // 单行；/* 多行 */
来源：http://st.muxihuayi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://st.chemitech.net.cn

Go:   // 单行；/* 多行 */
来源：http://sf.yuntaijiaju.cn

Ruby: # 单行；=begin 多行 =end
来源：http://em.521024.cn

C#:   // 单行；/* 多行 */
来源：http://hn.nicolike.cn

[A15] 空值判断与默认值
来源：http://dk.huixiangedu.cn

Py:   value = data or "默认值"
来源：http://qs.jctech888.com.cn

PHP:  $value = $data ?? "默认值";
来源：http://dt.jianghongdianzi.cn


<!-- 参考信息 -->