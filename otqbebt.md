代发 wailian999

[U97] JS：并发请求
来源：http://ou.panjiajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tu.521024.cn

[U98] JS：fetch 带 JSON
来源：http://hk.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ie.gzmigu.cn

[U99] JS：事件监听
来源：http://cw.colortex.cn

el.addEventListener("click", e => {})
来源：http://wn.hnjuh.cn

[U100] JS：DOM 查询
来源：http://sa.hahajie.cn

document.querySelector(".item")
来源：http://ra.nicolike.cn

[U101] JS：classList 操作
来源：http://or.colortex.cn

el.classList.toggle("active")
来源：http://ts.huixiangedu.cn

[U102] JS：本地存储
来源：http://bo.huixiangedu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ej.hnjuh.cn

[U103] JS：定时器
来源：http://ov.huixinmuqiang.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nm.yuntaijiaju.cn

[U104] JS：防抖
来源：http://vu.huixinmuqiang.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pm.shxzskj.cn

[U105] JS：节流
来源：http://kd.haigaiapp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yl.jianghongdianzi.cn

[U106] JS：日期格式化
来源：http://fz.yuntaijiaju.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://eb.muxihuayi.cn

[U107] JS：数字千分位
来源：http://eh.jianghongdianzi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wi.nszjky.cn

[U108] JS：随机整数
来源：http://kg.muxihuayi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dc.nszjky.cn

[U109] JS：数组分组
来源：http://ju.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://gb.nszjky.cn

[U110] JS：数组分块
来源：http://pa.yuntaijiaju.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xj.haigaiapp.cn

[U111] JS：对象转 Map
来源：http://rp.shxzukj.cn

new Map(Object.entries(obj))
来源：http://gj.nicolike.cn

[U112] JS：字符串补位
来源：http://ju.jianghongdianzi.cn

"7".padStart(3, "0")
来源：http://wd.shtwfgs.cn

[U113] JS：正则替换全部
来源：http://wt.szxytkj.cn

s.replaceAll("a", "b")
来源：http://bs.huanxung.cn

[U114] JS：JSON 深比较
来源：http://xj.asd995.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://bw.521024.cn

[U115] JS：生成 UUID
来源：http://yz.haigaiapp.cn

crypto.randomUUID()
来源：http://zw.huixinmuqiang.cn

[U116] JS：类型检查（JSDoc）
来源：http://vw.lnxyls.cn

/** @param {string} name */ function f(name) {}
来源：http://hk.hahajie.cn

[U117] JS：单元测试
来源：http://iu.gzmigu.cn

npm i -D vitest;  npx vitest
来源：http://oi.asd995.cn

[U118] JS：开发服务器
来源：http://eg.muxihuayi.cn

npm i -D vite;  npx vite
来源：http://oi.newstarts.cn

[U119] JS：生产构建
来源：http://ea.yuntaijiaju.cn

npx vite build
来源：http://fq.panjiajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://uk.bookmarksfly.cn

import.meta.env.VITE_API_URL
来源：http://dv.wgjwhj.cn

================================================================================
来源：http://ha.colortex.cn

统计汇总
来源：http://cs.panjiajie.cn

================================================================================
来源：http://pq.szxytkj.cn

按语言统计（条）：
来源：http://he.nicolike.cn

Python ......... 252
来源：http://ag.jctech888.com.cn

PHP ............ 252
来源：http://mf.jctech888.com.cn

JavaScript ..... 252
来源：http://ug.hahajie.cn

TypeScript ..... 212
来源：http://vj.hnjuh.cn

Java ........... 212
来源：http://jj.haigaiapp.cn

Go ............. 212
来源：http://lc.jctech888.com.cn

Ruby ........... 212
来源：http://ek.521024.cn

C# ............. 212
来源：http://xr.muxihuayi.cn

C .............. 30
来源：http://lk.shtwfgs.cn

C++ ............ 30
来源：http://uy.huixinmuqiang.cn

SQL ............ 90
来源：http://gm.bookmarksfly.cn

Bash ........... 80
来源：http://jx.jctech888.com.cn

Kotlin ......... 15
来源：http://jn.shxzskj.cn

Swift .......... 15
来源：http://gg.nicolike.cn

Lua ............ 10
来源：http://mv.jctech888.com.cn

Perl ........... 10
来源：http://mu.521024.cn

Scala .......... 10
来源：http://cn.nszjky.cn

------------------------------------
来源：http://bi.haigaiapp.cn

合计 ........... 2106 条
来源：http://jo.jctech888.com.cn

按章节统计：
来源：http://nq.asd995.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yr.shtwfgs.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uj.521024.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xi.chemitech.net.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fd.lnxyls.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fy.newstarts.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bb.nicolike.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zi.gzmigu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ff.huixinmuqiang.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rg.szxytkj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zg.muxihuayi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fv.shtwfgs.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vw.huixiangedu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yq.huanxung.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rs.shxzskj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fz.newstarts.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://go.shxzukj.cn

Q SQL 专题                              90
来源：http://hj.szxytkj.cn

R Bash 专题                             80
来源：http://zz.yuexingan06.cn

S C / C++ 专题                          60
来源：http://ef.chemitech.net.cn

T 其他语言补充                          60
来源：http://ob.chemitech.net.cn

U 高频实用片段                         120
来源：http://ym.wgjwhj.cn

------------------------------------
来源：http://az.nicolike.cn

合计                                  2106 条
来源：http://gn.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://xu.gzmigu.cn

使用提醒
来源：http://yn.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://wy.yuexingan06.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wm.chemitech.net.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pm.nicolike.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ma.hahajie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gq.chemitech.net.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dp.jianghongdianzi.cn

—— 文件结束 ——
来源：http://xe.szsharing.cn

================================================================================
来源：http://hj.yuntaijiaju.cn

程序语言常见例子速查手册（2024 版）
来源：http://bv.muxihuayi.cn

Common Programming Examples Cheat Book
来源：http://tx.gzmigu.cn

================================================================================
来源：http://bu.jianghongdianzi.cn

【收录内容】
来源：http://mn.bjjhwx.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jo.gzmigu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ec.hahajie.cn

SQL · Bash · C · C++
来源：http://pe.colortex.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cq.yuexingan06.cn

【使用说明】
来源：http://qm.szsharing.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://za.lnxyls.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gk.newstarts.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ck.lnxyls.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://em.wgjwhj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://so.hnjuh.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://aw.colortex.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dr.chemitech.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bv.yuexingan06.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rq.huanxung.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cn.nicolike.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pg.9csxet.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ac.yuexingan06.cn

【文件统计】
来源：http://mk.shxzskj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://za.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://lk.gzmigu.cn

目  录
来源：http://gu.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://vt.lnxyls.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fc.asd995.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://op.lnxyls.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sf.asd995.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://oy.nszjky.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://na.panjiajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pa.hahajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zh.9csxet.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bg.muxihuayi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mm.nicolike.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yi.szsharing.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bv.shxzukj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sf.newstarts.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yy.colortex.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ge.huixiangedu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://iu.jianghongdianzi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://uh.panjiajie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rh.bookmarksfly.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ea.shtwfgs.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dj.gzmigu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://we.asd995.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ts.9csxet.cn

================================================================================
来源：http://qr.huixiangedu.cn

A. 基础语法与类型
来源：http://oq.muxihuayi.cn

================================================================================
来源：http://xz.hnjuh.cn

[A01] Hello World
来源：http://mf.chemitech.net.cn

Py:   print("Hello, World!")
来源：http://ix.muxihuayi.cn

PHP:  echo "Hello, World!";
来源：http://bb.shtwfgs.cn

JS:   console.log("Hello, World!");
来源：http://ks.9csxet.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://df.huanxung.cn

Java: System.out.println("Hello, World!");
来源：http://xr.gzmigu.cn

Go:   fmt.Println("Hello, World!")
来源：http://xl.huanxung.cn

Ruby: puts "Hello, World!"
来源：http://up.newstarts.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zz.bookmarksfly.cn

[A02] 变量声明与赋值
来源：http://od.szxytkj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nc.newstarts.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://jf.bookmarksfly.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vk.9csxet.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qp.bjjhwx.cn

Java: String name = "Alex"; int age = 20;
来源：http://bi.huanxung.cn

Go:   name := "Alex"; age := 20
来源：http://iv.shtwfgs.cn

Ruby: name = "Alex"; age = 20
来源：http://np.huixiangedu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://vf.hahajie.cn

[A03] 常量定义
来源：http://sp.hnjuh.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qm.9csxet.cn

PHP:  const PI = 3.14159;
来源：http://tj.lnxyls.cn

JS:   const PI = 3.14159;
来源：http://kf.huanxung.cn

TS:   const PI: number = 3.14159;
来源：http://de.9csxet.cn

Java: static final double PI = 3.14159;
来源：http://en.jctech888.com.cn

Go:   const PI = 3.14159
来源：http://gw.gzmigu.cn

Ruby: PI = 3.14159
来源：http://px.bjjhwx.cn

C#:   const double PI = 3.14159;
来源：http://ca.521024.cn

[A04] 判断变量类型
来源：http://ax.panjiajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://mh.muxihuayi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cz.hahajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://eb.nszjky.cn

TS:   typeof x; x instanceof Date
来源：http://sk.9csxet.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bc.haigaiapp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://cy.chemitech.net.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ar.nszjky.cn

C#:   x.GetType().Name; x is int
来源：http://wd.huixinmuqiang.cn

[A05] 整数除法与取模
来源：http://xh.9csxet.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://in.521024.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vy.haigaiapp.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jd.hnjuh.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sb.yuntaijiaju.cn

Java: 7 / 2; 7 % 2
来源：http://fu.panjiajie.cn

Go:   7 / 2; 7 % 2
来源：http://sj.nicolike.cn

Ruby: 7 / 2; 7 % 2
来源：http://uv.wgjwhj.cn

C#:   7 / 2; 7 % 2
来源：http://yg.haigaiapp.cn

[A06] 字符串转数字
来源：http://vo.hnjuh.cn

Py:   int("42"); float("3.14")
来源：http://wq.521024.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ug.huixinmuqiang.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://us.huixinmuqiang.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xg.panjiajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ui.huixiangedu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bp.huixinmuqiang.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hm.panjiajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dc.muxihuayi.cn

[A07] 数字转字符串
来源：http://wa.huanxung.cn

Py:   str(42)
来源：http://ki.jianghongdianzi.cn

PHP:  (string) 42; strval(42)
来源：http://gg.shtwfgs.cn

JS:   String(42); (42).toString()
来源：http://zg.nszjky.cn

TS:   String(42)
来源：http://wm.haigaiapp.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xg.gzmigu.cn

Go:   strconv.Itoa(42)
来源：http://kh.colortex.cn

Ruby: 42.to_s
来源：http://kw.gzmigu.cn

C#:   42.ToString()
来源：http://ll.shxzskj.cn

[A08] 取整与四舍五入
来源：http://ci.huixinmuqiang.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pa.szsharing.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ql.yuexingan06.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://od.shxzukj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fb.bookmarksfly.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cz.lnxyls.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xf.yuntaijiaju.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mr.shxzukj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fs.nszjky.cn

[A09] 绝对值与最大最小值
来源：http://to.huanxung.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ox.hahajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ve.yuntaijiaju.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ew.huanxung.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vk.jctech888.com.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vl.gzmigu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ei.bjjhwx.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wc.jianghongdianzi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ct.521024.cn

[A10] 生成随机数
来源：http://df.lnxyls.cn

Py:   import random; random.randint(1, 100)
来源：http://sk.haigaiapp.cn

PHP:  random_int(1, 100);
来源：http://hu.nszjky.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rf.huixiangedu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ew.nicolike.cn

Java: new Random().nextInt(100) + 1
来源：http://ue.colortex.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ty.shxzukj.cn

Ruby: rand(1..100)
来源：http://pp.wgjwhj.cn

C#:   new Random().Next(1, 101)
来源：http://la.gzmigu.cn

[A11] 条件表达式（三元）
来源：http://ok.shxzskj.cn

Py:   "yes" if x > 0 else "no"
来源：http://tx.nicolike.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ks.wgjwhj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://bu.521024.cn

TS:   x > 0 ? "yes" : "no"
来源：http://bu.huixinmuqiang.cn

Java: x > 0 ? "yes" : "no"
来源：http://nv.haigaiapp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://sn.521024.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://mi.521024.cn

C#:   x > 0 ? "yes" : "no"
来源：http://tk.yuexingan06.cn

[A12] 字符串插值 / 格式化
来源：http://uv.bookmarksfly.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mm.9csxet.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://dw.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://gw.huixiangedu.cn

TS:   `Hello, ${name}!`
来源：http://ab.yuexingan06.cn

Java: "Hello, %s!".formatted(name)
来源：http://vp.gzmigu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ln.colortex.cn

Ruby: "Hello, #{name}!"
来源：http://jb.9csxet.cn

C#:   $"Hello, {name}!"
来源：http://cf.nicolike.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ti.hnjuh.cn

Py:   "第一行\n第二行"
来源：http://jr.szxytkj.cn

PHP:  "第一行\n第二行"
来源：http://ey.jianghongdianzi.cn

JS:   "第一行\n第二行"
来源：http://qj.shxzskj.cn

TS:   "第一行\n第二行"
来源：http://gk.jianghongdianzi.cn

Java: "第一行\n第二行"
来源：http://st.bjjhwx.cn

Go:   "第一行\n第二行"
来源：http://nj.hnjuh.cn

Ruby: "第一行\n第二行"
来源：http://qt.szsharing.cn

C#:   "第一行\n第二行"
来源：http://nb.chemitech.net.cn

[A14] 注释写法
来源：http://ce.521024.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wh.hnjuh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://kh.haigaiapp.cn

JS:   // 单行；/* 多行 */
来源：http://cb.9csxet.cn

TS:   // 单行；/* 多行 */
来源：http://bz.lnxyls.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hi.bookmarksfly.cn

Go:   // 单行；/* 多行 */
来源：http://al.gzmigu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://to.wgjwhj.cn

C#:   // 单行；/* 多行 */
来源：http://jo.szsharing.cn

[A15] 空值判断与默认值
来源：http://ia.yuntaijiaju.cn

Py:   value = data or "默认值"
来源：http://sf.hnjuh.cn

PHP:  $value = $data ?? "默认值";
来源：http://ev.szxytkj.cn

JS:   const value = data ?? "默认值";
来源：http://uk.nicolike.cn

TS:   const value = data ?? "默认值";
来源：http://fr.521024.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yv.chemitech.net.cn

Go:   if data == "" { data = "默认值" }
来源：http://ha.asd995.cn

Ruby: value = data || "默认值"
来源：http://cx.muxihuayi.cn

C#:   var value = data ?? "默认值";
来源：http://ce.haigaiapp.cn

[A16] 真假值判断规则
来源：http://pv.huanxung.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://at.jctech888.com.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tk.hnjuh.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xs.wgjwhj.cn

TS:   if (!x) {}
来源：http://ho.haigaiapp.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ym.haigaiapp.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ko.shxzskj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://up.nszjky.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ox.9csxet.cn

[A17] 位运算
来源：http://gp.521024.cn


<!-- 参考信息 -->