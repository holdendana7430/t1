代发 wailian999

[U95] JS：Promise 包装
来源：http://fn.hnjuh.cn

new Promise((resolve, reject) => {})
来源：http://yr.asd995.cn

[U96] JS：async/await 与异常
来源：http://kt.huixinmuqiang.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dd.chemitech.net.cn

[U97] JS：并发请求
来源：http://gv.jianghongdianzi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tt.szsharing.cn

[U98] JS：fetch 带 JSON
来源：http://wd.chemitech.net.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wr.huixinmuqiang.cn

[U99] JS：事件监听
来源：http://dt.gzmigu.cn

el.addEventListener("click", e => {})
来源：http://aq.haigaiapp.cn

[U100] JS：DOM 查询
来源：http://bd.bjjhwx.cn

document.querySelector(".item")
来源：http://mw.gzmigu.cn

[U101] JS：classList 操作
来源：http://mr.hahajie.cn

el.classList.toggle("active")
来源：http://mv.bjjhwx.cn

[U102] JS：本地存储
来源：http://hn.gzmigu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wq.szsharing.cn

[U103] JS：定时器
来源：http://yp.yuexingan06.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xj.huixiangedu.cn

[U104] JS：防抖
来源：http://gx.bookmarksfly.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://np.lnxyls.cn

[U105] JS：节流
来源：http://ir.shtwfgs.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jf.hahajie.cn

[U106] JS：日期格式化
来源：http://jf.colortex.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mv.wgjwhj.cn

[U107] JS：数字千分位
来源：http://cj.521024.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ew.yuntaijiaju.cn

[U108] JS：随机整数
来源：http://jh.newstarts.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gq.haigaiapp.cn

[U109] JS：数组分组
来源：http://tz.muxihuayi.cn

Object.groupBy(arr, x => x.type)
来源：http://fh.asd995.cn

[U110] JS：数组分块
来源：http://zu.nszjky.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dc.asd995.cn

[U111] JS：对象转 Map
来源：http://rd.hahajie.cn

new Map(Object.entries(obj))
来源：http://jx.muxihuayi.cn

[U112] JS：字符串补位
来源：http://io.huanxung.cn

"7".padStart(3, "0")
来源：http://oc.muxihuayi.cn

[U113] JS：正则替换全部
来源：http://lc.panjiajie.cn

s.replaceAll("a", "b")
来源：http://cb.shtwfgs.cn

[U114] JS：JSON 深比较
来源：http://nb.szxytkj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://em.haigaiapp.cn

[U115] JS：生成 UUID
来源：http://af.lnxyls.cn

crypto.randomUUID()
来源：http://ye.chemitech.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://zv.szsharing.cn

/** @param {string} name */ function f(name) {}
来源：http://vz.9csxet.cn

[U117] JS：单元测试
来源：http://kv.shxzskj.cn

npm i -D vitest;  npx vitest
来源：http://qf.muxihuayi.cn

[U118] JS：开发服务器
来源：http://cl.huixiangedu.cn

npm i -D vite;  npx vite
来源：http://rq.bjjhwx.cn

[U119] JS：生产构建
来源：http://ls.asd995.cn

npx vite build
来源：http://kf.huixinmuqiang.cn

[U120] JS：读取环境变量（Vite）
来源：http://lw.huixinmuqiang.cn

import.meta.env.VITE_API_URL
来源：http://yl.9csxet.cn

================================================================================
来源：http://fa.haigaiapp.cn

统计汇总
来源：http://we.asd995.cn

================================================================================
来源：http://wj.nszjky.cn

按语言统计（条）：
来源：http://hm.nszjky.cn

Python ......... 252
来源：http://hn.yuntaijiaju.cn

PHP ............ 252
来源：http://fz.newstarts.cn

JavaScript ..... 252
来源：http://ni.jctech888.com.cn

TypeScript ..... 212
来源：http://sk.newstarts.cn

Java ........... 212
来源：http://rv.9csxet.cn

Go ............. 212
来源：http://js.shtwfgs.cn

Ruby ........... 212
来源：http://rm.521024.cn

C# ............. 212
来源：http://zz.bookmarksfly.cn

C .............. 30
来源：http://vo.wgjwhj.cn

C++ ............ 30
来源：http://ak.huixinmuqiang.cn

SQL ............ 90
来源：http://jc.szxytkj.cn

Bash ........... 80
来源：http://tw.yuexingan06.cn

Kotlin ......... 15
来源：http://lm.nszjky.cn

Swift .......... 15
来源：http://lx.szsharing.cn

Lua ............ 10
来源：http://zq.panjiajie.cn

Perl ........... 10
来源：http://bk.nszjky.cn

Scala .......... 10
来源：http://tq.hahajie.cn

------------------------------------
来源：http://ls.yuexingan06.cn

合计 ........... 2106 条
来源：http://rc.colortex.cn

按章节统计：
来源：http://iy.chemitech.net.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ho.colortex.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kc.asd995.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tp.9csxet.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bl.shxzskj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qn.szsharing.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ws.huixiangedu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vu.chemitech.net.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ey.szxytkj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bz.shtwfgs.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://af.bjjhwx.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ll.huixinmuqiang.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ti.szxytkj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ll.jctech888.com.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vf.newstarts.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vx.szsharing.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wm.521024.cn

Q SQL 专题                              90
来源：http://ca.wgjwhj.cn

R Bash 专题                             80
来源：http://un.9csxet.cn

S C / C++ 专题                          60
来源：http://gl.nicolike.cn

T 其他语言补充                          60
来源：http://ha.chemitech.net.cn

U 高频实用片段                         120
来源：http://ba.wgjwhj.cn

------------------------------------
来源：http://wt.shtwfgs.cn

合计                                  2106 条
来源：http://ut.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://hl.chemitech.net.cn

使用提醒
来源：http://yw.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://lj.nszjky.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zx.chemitech.net.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mh.9csxet.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://od.nszjky.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://bi.lnxyls.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jy.huixiangedu.cn

—— 文件结束 ——
来源：http://fa.bjjhwx.cn

================================================================================
来源：http://lm.panjiajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://tp.newstarts.cn

Common Programming Examples Cheat Book
来源：http://al.colortex.cn

================================================================================
来源：http://nb.chemitech.net.cn

【收录内容】
来源：http://ep.huanxung.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ya.lnxyls.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fg.newstarts.cn

SQL · Bash · C · C++
来源：http://oq.9csxet.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://iy.9csxet.cn

【使用说明】
来源：http://al.yuntaijiaju.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dp.521024.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mq.panjiajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qb.huixiangedu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cm.bjjhwx.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://dy.colortex.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fn.shtwfgs.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lr.521024.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dm.shxzukj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wz.haigaiapp.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vv.muxihuayi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nr.bjjhwx.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://rp.hahajie.cn

【文件统计】
来源：http://ov.szsharing.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vg.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://lo.yuexingan06.cn

目  录
来源：http://pg.colortex.cn

--------------------------------------------------------------------------------
来源：http://zt.lnxyls.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vx.panjiajie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://as.yuntaijiaju.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bb.panjiajie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vx.huanxung.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vp.huixinmuqiang.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://as.shxzskj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wq.hnjuh.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jy.shxzskj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://yg.hahajie.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yk.shxzukj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mf.yuntaijiaju.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ii.asd995.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://sz.hahajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hf.jianghongdianzi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vz.jctech888.com.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jq.hahajie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://es.yuexingan06.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://fj.wgjwhj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pu.yuexingan06.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cx.muxihuayi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://oi.huanxung.cn

================================================================================
来源：http://sa.szxytkj.cn

A. 基础语法与类型
来源：http://pv.chemitech.net.cn

================================================================================
来源：http://jj.colortex.cn

[A01] Hello World
来源：http://yc.yuexingan06.cn

Py:   print("Hello, World!")
来源：http://ib.shtwfgs.cn

PHP:  echo "Hello, World!";
来源：http://tv.jianghongdianzi.cn

JS:   console.log("Hello, World!");
来源：http://kd.szxytkj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yy.chemitech.net.cn

Java: System.out.println("Hello, World!");
来源：http://ja.huixiangedu.cn

Go:   fmt.Println("Hello, World!")
来源：http://mn.lnxyls.cn

Ruby: puts "Hello, World!"
来源：http://ba.panjiajie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ye.9csxet.cn

[A02] 变量声明与赋值
来源：http://ly.bjjhwx.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wr.chemitech.net.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xh.shtwfgs.cn

JS:   let name = "Alex"; const age = 20;
来源：http://kd.newstarts.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rd.shxzukj.cn

Java: String name = "Alex"; int age = 20;
来源：http://xh.huixinmuqiang.cn

Go:   name := "Alex"; age := 20
来源：http://bk.asd995.cn

Ruby: name = "Alex"; age = 20
来源：http://mm.bjjhwx.cn

C#:   string name = "Alex"; int age = 20;
来源：http://nc.nszjky.cn

[A03] 常量定义
来源：http://gl.szsharing.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ur.huanxung.cn

PHP:  const PI = 3.14159;
来源：http://dh.nicolike.cn

JS:   const PI = 3.14159;
来源：http://hm.huixinmuqiang.cn

TS:   const PI: number = 3.14159;
来源：http://ru.hahajie.cn

Java: static final double PI = 3.14159;
来源：http://jp.newstarts.cn

Go:   const PI = 3.14159
来源：http://lp.nicolike.cn

Ruby: PI = 3.14159
来源：http://se.lnxyls.cn

C#:   const double PI = 3.14159;
来源：http://di.shxzukj.cn

[A04] 判断变量类型
来源：http://ri.asd995.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://jh.huanxung.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lx.nszjky.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lh.lnxyls.cn

TS:   typeof x; x instanceof Date
来源：http://pm.huixiangedu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zw.haigaiapp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hs.jctech888.com.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yd.haigaiapp.cn

C#:   x.GetType().Name; x is int
来源：http://eg.lnxyls.cn

[A05] 整数除法与取模
来源：http://bu.chemitech.net.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://sy.asd995.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://rh.hahajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ki.muxihuayi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tm.9csxet.cn

Java: 7 / 2; 7 % 2
来源：http://fc.shtwfgs.cn

Go:   7 / 2; 7 % 2
来源：http://nf.huixinmuqiang.cn

Ruby: 7 / 2; 7 % 2
来源：http://vd.szxytkj.cn

C#:   7 / 2; 7 % 2
来源：http://hj.panjiajie.cn

[A06] 字符串转数字
来源：http://up.huixiangedu.cn

Py:   int("42"); float("3.14")
来源：http://yg.jctech888.com.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://go.haigaiapp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pt.bjjhwx.cn

TS:   parseInt("42", 10); Number("42")
来源：http://jb.521024.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ca.chemitech.net.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vh.wgjwhj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ab.huixiangedu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tl.9csxet.cn

[A07] 数字转字符串
来源：http://th.9csxet.cn

Py:   str(42)
来源：http://yf.wgjwhj.cn

PHP:  (string) 42; strval(42)
来源：http://gh.panjiajie.cn

JS:   String(42); (42).toString()
来源：http://lz.muxihuayi.cn

TS:   String(42)
来源：http://rv.newstarts.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ce.521024.cn

Go:   strconv.Itoa(42)
来源：http://gp.521024.cn

Ruby: 42.to_s
来源：http://mh.shxzukj.cn

C#:   42.ToString()
来源：http://db.szxytkj.cn

[A08] 取整与四舍五入
来源：http://ls.panjiajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gx.521024.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jj.hahajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tf.gzmigu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tp.muxihuayi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sw.lnxyls.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rd.wgjwhj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://dz.jianghongdianzi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fm.lnxyls.cn

[A09] 绝对值与最大最小值
来源：http://sa.bjjhwx.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://si.szsharing.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bd.gzmigu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mj.newstarts.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nz.colortex.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qf.szxytkj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ev.chemitech.net.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xs.521024.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mn.jianghongdianzi.cn

[A10] 生成随机数
来源：http://ql.huanxung.cn

Py:   import random; random.randint(1, 100)
来源：http://wa.newstarts.cn

PHP:  random_int(1, 100);
来源：http://ir.bjjhwx.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://re.hnjuh.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gr.huixiangedu.cn

Java: new Random().nextInt(100) + 1
来源：http://an.gzmigu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wy.bookmarksfly.cn

Ruby: rand(1..100)
来源：http://iq.lnxyls.cn

C#:   new Random().Next(1, 101)
来源：http://yf.chemitech.net.cn

[A11] 条件表达式（三元）
来源：http://rw.huixinmuqiang.cn

Py:   "yes" if x > 0 else "no"
来源：http://yf.shxzukj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://te.newstarts.cn

JS:   x > 0 ? "yes" : "no"
来源：http://dt.huixinmuqiang.cn

TS:   x > 0 ? "yes" : "no"
来源：http://oa.shtwfgs.cn

Java: x > 0 ? "yes" : "no"
来源：http://mr.lnxyls.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zw.szsharing.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vo.nicolike.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ua.shtwfgs.cn

[A12] 字符串插值 / 格式化
来源：http://cb.bjjhwx.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qg.nicolike.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bv.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://sg.shxzukj.cn

TS:   `Hello, ${name}!`
来源：http://jc.9csxet.cn

Java: "Hello, %s!".formatted(name)
来源：http://mt.yuexingan06.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://oe.wgjwhj.cn

Ruby: "Hello, #{name}!"
来源：http://ac.muxihuayi.cn

C#:   $"Hello, {name}!"
来源：http://al.huixiangedu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://al.huixinmuqiang.cn

Py:   "第一行\n第二行"
来源：http://xq.jianghongdianzi.cn

PHP:  "第一行\n第二行"
来源：http://vu.yuntaijiaju.cn

JS:   "第一行\n第二行"
来源：http://or.huixiangedu.cn

TS:   "第一行\n第二行"
来源：http://dh.hahajie.cn

Java: "第一行\n第二行"
来源：http://na.asd995.cn

Go:   "第一行\n第二行"
来源：http://me.yuntaijiaju.cn

Ruby: "第一行\n第二行"
来源：http://id.huanxung.cn

C#:   "第一行\n第二行"
来源：http://jw.panjiajie.cn

[A14] 注释写法
来源：http://rq.huanxung.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://es.szsharing.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://zn.shxzskj.cn

JS:   // 单行；/* 多行 */
来源：http://rc.gzmigu.cn

TS:   // 单行；/* 多行 */
来源：http://qs.shtwfgs.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fk.9csxet.cn

Go:   // 单行；/* 多行 */
来源：http://wa.muxihuayi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://jt.hahajie.cn

C#:   // 单行；/* 多行 */
来源：http://sd.wgjwhj.cn

[A15] 空值判断与默认值
来源：http://ox.hnjuh.cn

Py:   value = data or "默认值"
来源：http://ui.muxihuayi.cn

PHP:  $value = $data ?? "默认值";
来源：http://np.huanxung.cn

JS:   const value = data ?? "默认值";
来源：http://zn.nicolike.cn

TS:   const value = data ?? "默认值";
来源：http://ki.9csxet.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pw.hnjuh.cn

Go:   if data == "" { data = "默认值" }
来源：http://gw.panjiajie.cn

Ruby: value = data || "默认值"
来源：http://gl.bookmarksfly.cn

C#:   var value = data ?? "默认值";
来源：http://pp.lnxyls.cn

[A16] 真假值判断规则
来源：http://zo.gzmigu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gs.bookmarksfly.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cu.9csxet.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wj.bookmarksfly.cn

TS:   if (!x) {}
来源：http://lq.wgjwhj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xy.jianghongdianzi.cn


<!-- 参考信息 -->