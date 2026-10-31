代发 wailian999

[U93] JS：模板字符串
来源：http://vk.lnxyls.cn

`共 ${n} 条`
来源：http://gt.jctech888.com.cn

[U94] JS：箭头函数
来源：http://xg.wgjwhj.cn

const double = x => x * 2;
来源：http://cg.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://lo.muxihuayi.cn

new Promise((resolve, reject) => {})
来源：http://jc.muxihuayi.cn

[U96] JS：async/await 与异常
来源：http://pc.haigaiapp.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pz.haigaiapp.cn

[U97] JS：并发请求
来源：http://av.nszjky.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zh.haigaiapp.cn

[U98] JS：fetch 带 JSON
来源：http://ec.szsharing.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ih.521024.cn

[U99] JS：事件监听
来源：http://tf.huixiangedu.cn

el.addEventListener("click", e => {})
来源：http://ka.shtwfgs.cn

[U100] JS：DOM 查询
来源：http://li.szxytkj.cn

document.querySelector(".item")
来源：http://aj.lnxyls.cn

[U101] JS：classList 操作
来源：http://jq.haigaiapp.cn

el.classList.toggle("active")
来源：http://yd.wgjwhj.cn

[U102] JS：本地存储
来源：http://wj.newstarts.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://tr.huixinmuqiang.cn

[U103] JS：定时器
来源：http://us.huixiangedu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xa.jctech888.com.cn

[U104] JS：防抖
来源：http://qc.haigaiapp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qz.huanxung.cn

[U105] JS：节流
来源：http://zq.bjjhwx.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://le.panjiajie.cn

[U106] JS：日期格式化
来源：http://yf.shxzukj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ux.szsharing.cn

[U107] JS：数字千分位
来源：http://td.gzmigu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qa.huixiangedu.cn

[U108] JS：随机整数
来源：http://ac.wgjwhj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://od.szxytkj.cn

[U109] JS：数组分组
来源：http://qp.lnxyls.cn

Object.groupBy(arr, x => x.type)
来源：http://ta.521024.cn

[U110] JS：数组分块
来源：http://ok.521024.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xr.jctech888.com.cn

[U111] JS：对象转 Map
来源：http://qx.nszjky.cn

new Map(Object.entries(obj))
来源：http://ky.huixinmuqiang.cn

[U112] JS：字符串补位
来源：http://pj.shtwfgs.cn

"7".padStart(3, "0")
来源：http://sx.muxihuayi.cn

[U113] JS：正则替换全部
来源：http://cs.jianghongdianzi.cn

s.replaceAll("a", "b")
来源：http://vj.huixiangedu.cn

[U114] JS：JSON 深比较
来源：http://ag.shtwfgs.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://no.shxzskj.cn

[U115] JS：生成 UUID
来源：http://ps.muxihuayi.cn

crypto.randomUUID()
来源：http://on.chemitech.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://tw.shxzskj.cn

/** @param {string} name */ function f(name) {}
来源：http://yo.521024.cn

[U117] JS：单元测试
来源：http://ff.huixiangedu.cn

npm i -D vitest;  npx vitest
来源：http://nk.jianghongdianzi.cn

[U118] JS：开发服务器
来源：http://fy.huixinmuqiang.cn

npm i -D vite;  npx vite
来源：http://rr.chemitech.net.cn

[U119] JS：生产构建
来源：http://td.muxihuayi.cn

npx vite build
来源：http://hg.asd995.cn

[U120] JS：读取环境变量（Vite）
来源：http://ni.nszjky.cn

import.meta.env.VITE_API_URL
来源：http://lo.muxihuayi.cn

================================================================================
来源：http://ah.yuntaijiaju.cn

统计汇总
来源：http://rh.gzmigu.cn

================================================================================
来源：http://jj.chemitech.net.cn

按语言统计（条）：
来源：http://yy.lnxyls.cn

Python ......... 252
来源：http://dy.panjiajie.cn

PHP ............ 252
来源：http://mo.jctech888.com.cn

JavaScript ..... 252
来源：http://mx.newstarts.cn

TypeScript ..... 212
来源：http://rg.jctech888.com.cn

Java ........... 212
来源：http://zt.muxihuayi.cn

Go ............. 212
来源：http://xx.wgjwhj.cn

Ruby ........... 212
来源：http://eo.yuntaijiaju.cn

C# ............. 212
来源：http://jt.shxzukj.cn

C .............. 30
来源：http://wj.gzmigu.cn

C++ ............ 30
来源：http://uf.huixinmuqiang.cn

SQL ............ 90
来源：http://qx.yuntaijiaju.cn

Bash ........... 80
来源：http://le.asd995.cn

Kotlin ......... 15
来源：http://lo.huixinmuqiang.cn

Swift .......... 15
来源：http://ha.huanxung.cn

Lua ............ 10
来源：http://km.jctech888.com.cn

Perl ........... 10
来源：http://yf.szsharing.cn

Scala .......... 10
来源：http://hd.huanxung.cn

------------------------------------
来源：http://pd.shxzskj.cn

合计 ........... 2106 条
来源：http://bw.szsharing.cn

按章节统计：
来源：http://yv.hahajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gz.muxihuayi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ul.muxihuayi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ce.wgjwhj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ll.huanxung.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fb.huixiangedu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vy.jianghongdianzi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ix.huanxung.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nh.chemitech.net.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ui.yuexingan06.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dz.lnxyls.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sd.bjjhwx.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xr.gzmigu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ot.colortex.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://of.szxytkj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dp.nszjky.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zb.yuexingan06.cn

Q SQL 专题                              90
来源：http://pa.colortex.cn

R Bash 专题                             80
来源：http://su.shxzskj.cn

S C / C++ 专题                          60
来源：http://wa.shxzukj.cn

T 其他语言补充                          60
来源：http://ie.wgjwhj.cn

U 高频实用片段                         120
来源：http://ks.bjjhwx.cn

------------------------------------
来源：http://pv.yuexingan06.cn

合计                                  2106 条
来源：http://wj.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://ug.haigaiapp.cn

使用提醒
来源：http://jk.colortex.cn

--------------------------------------------------------------------------------
来源：http://el.jianghongdianzi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pr.gzmigu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ap.521024.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ck.lnxyls.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://nc.bookmarksfly.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lw.szxytkj.cn

—— 文件结束 ——
来源：http://oh.panjiajie.cn

================================================================================
来源：http://sd.asd995.cn

程序语言常见例子速查手册（2024 版）
来源：http://ys.yuexingan06.cn

Common Programming Examples Cheat Book
来源：http://ia.huanxung.cn

================================================================================
来源：http://uf.jctech888.com.cn

【收录内容】
来源：http://lo.gzmigu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ju.gzmigu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ed.jianghongdianzi.cn

SQL · Bash · C · C++
来源：http://gg.newstarts.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bb.jctech888.com.cn

【使用说明】
来源：http://xv.szsharing.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ye.hnjuh.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fr.bjjhwx.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gi.muxihuayi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://da.shxzukj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://gx.nicolike.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bc.szsharing.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://uz.muxihuayi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://om.newstarts.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gt.wgjwhj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gi.521024.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wz.bjjhwx.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tt.bookmarksfly.cn

【文件统计】
来源：http://av.yuntaijiaju.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ob.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://tq.asd995.cn

目  录
来源：http://gl.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://jp.shxzskj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://je.nicolike.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ei.nicolike.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dz.asd995.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pc.panjiajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ah.521024.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://sd.hahajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lv.521024.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://km.shxzukj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://it.shxzukj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wc.panjiajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gb.haigaiapp.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gl.521024.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://va.jctech888.com.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://za.hnjuh.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://es.9csxet.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ne.bjjhwx.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xu.521024.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vw.muxihuayi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://iw.huixiangedu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xt.szsharing.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dm.shtwfgs.cn

================================================================================
来源：http://di.huanxung.cn

A. 基础语法与类型
来源：http://ea.bookmarksfly.cn

================================================================================
来源：http://np.nszjky.cn

[A01] Hello World
来源：http://kn.jctech888.com.cn

Py:   print("Hello, World!")
来源：http://gk.huixiangedu.cn

PHP:  echo "Hello, World!";
来源：http://af.bjjhwx.cn

JS:   console.log("Hello, World!");
来源：http://ji.huanxung.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://oh.huixinmuqiang.cn

Java: System.out.println("Hello, World!");
来源：http://wt.panjiajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://vm.nszjky.cn

Ruby: puts "Hello, World!"
来源：http://jc.hnjuh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://yx.huixinmuqiang.cn

[A02] 变量声明与赋值
来源：http://ec.nicolike.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kn.jianghongdianzi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ur.szxytkj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xv.haigaiapp.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vv.yuntaijiaju.cn

Java: String name = "Alex"; int age = 20;
来源：http://nl.newstarts.cn

Go:   name := "Alex"; age := 20
来源：http://jd.jctech888.com.cn

Ruby: name = "Alex"; age = 20
来源：http://yi.colortex.cn

C#:   string name = "Alex"; int age = 20;
来源：http://cv.newstarts.cn

[A03] 常量定义
来源：http://rp.shtwfgs.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mw.szxytkj.cn

PHP:  const PI = 3.14159;
来源：http://un.huixinmuqiang.cn

JS:   const PI = 3.14159;
来源：http://ax.wgjwhj.cn

TS:   const PI: number = 3.14159;
来源：http://bl.huanxung.cn

Java: static final double PI = 3.14159;
来源：http://ns.bjjhwx.cn

Go:   const PI = 3.14159
来源：http://wp.huanxung.cn

Ruby: PI = 3.14159
来源：http://sq.hahajie.cn

C#:   const double PI = 3.14159;
来源：http://iy.jianghongdianzi.cn

[A04] 判断变量类型
来源：http://vr.bjjhwx.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://tl.bjjhwx.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kq.wgjwhj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ns.shtwfgs.cn

TS:   typeof x; x instanceof Date
来源：http://eg.yuexingan06.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pf.huanxung.cn

Go:   reflect.TypeOf(x).Name()
来源：http://dg.shxzukj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://al.szxytkj.cn

C#:   x.GetType().Name; x is int
来源：http://wy.colortex.cn

[A05] 整数除法与取模
来源：http://zp.muxihuayi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wx.asd995.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://jd.hahajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nf.haigaiapp.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zc.hahajie.cn

Java: 7 / 2; 7 % 2
来源：http://lc.colortex.cn

Go:   7 / 2; 7 % 2
来源：http://sp.521024.cn

Ruby: 7 / 2; 7 % 2
来源：http://wa.521024.cn

C#:   7 / 2; 7 % 2
来源：http://ye.panjiajie.cn

[A06] 字符串转数字
来源：http://gp.shtwfgs.cn

Py:   int("42"); float("3.14")
来源：http://xf.haigaiapp.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://iv.huanxung.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cq.newstarts.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ql.shxzskj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gq.bookmarksfly.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vo.yuntaijiaju.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://sb.shtwfgs.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bv.wgjwhj.cn

[A07] 数字转字符串
来源：http://qu.panjiajie.cn

Py:   str(42)
来源：http://wl.chemitech.net.cn

PHP:  (string) 42; strval(42)
来源：http://ty.muxihuayi.cn

JS:   String(42); (42).toString()
来源：http://ii.gzmigu.cn

TS:   String(42)
来源：http://wr.bjjhwx.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://aa.gzmigu.cn

Go:   strconv.Itoa(42)
来源：http://lk.haigaiapp.cn

Ruby: 42.to_s
来源：http://yu.shxzukj.cn

C#:   42.ToString()
来源：http://qf.nicolike.cn

[A08] 取整与四舍五入
来源：http://ub.jctech888.com.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bp.521024.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lj.colortex.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ia.muxihuayi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nh.hahajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ij.wgjwhj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ik.yuexingan06.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://be.jianghongdianzi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xg.shtwfgs.cn

[A09] 绝对值与最大最小值
来源：http://cq.chemitech.net.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lb.szsharing.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://za.newstarts.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rt.lnxyls.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bc.gzmigu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vs.huixinmuqiang.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xj.haigaiapp.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nx.szxytkj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://nh.hahajie.cn

[A10] 生成随机数
来源：http://ok.huixiangedu.cn

Py:   import random; random.randint(1, 100)
来源：http://vt.wgjwhj.cn

PHP:  random_int(1, 100);
来源：http://mk.lnxyls.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://oq.muxihuayi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.nszjky.cn

Java: new Random().nextInt(100) + 1
来源：http://ra.nicolike.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://th.shxzukj.cn

Ruby: rand(1..100)
来源：http://fz.asd995.cn

C#:   new Random().Next(1, 101)
来源：http://sh.jctech888.com.cn

[A11] 条件表达式（三元）
来源：http://mb.jianghongdianzi.cn

Py:   "yes" if x > 0 else "no"
来源：http://cp.asd995.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://at.szxytkj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://cj.bookmarksfly.cn

TS:   x > 0 ? "yes" : "no"
来源：http://wa.521024.cn

Java: x > 0 ? "yes" : "no"
来源：http://qx.bjjhwx.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xb.gzmigu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vv.jianghongdianzi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://vg.jctech888.com.cn

[A12] 字符串插值 / 格式化
来源：http://vl.colortex.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cq.nicolike.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://is.yuexingan06.cn

JS:   `Hello, ${name}!`
来源：http://kx.haigaiapp.cn

TS:   `Hello, ${name}!`
来源：http://wv.jctech888.com.cn

Java: "Hello, %s!".formatted(name)
来源：http://kx.lnxyls.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pp.colortex.cn

Ruby: "Hello, #{name}!"
来源：http://wi.huixinmuqiang.cn

C#:   $"Hello, {name}!"
来源：http://eh.huixiangedu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://pt.521024.cn

Py:   "第一行\n第二行"
来源：http://sh.colortex.cn

PHP:  "第一行\n第二行"
来源：http://dx.521024.cn

JS:   "第一行\n第二行"
来源：http://vm.bookmarksfly.cn

TS:   "第一行\n第二行"
来源：http://sq.shxzukj.cn

Java: "第一行\n第二行"
来源：http://gy.shtwfgs.cn

Go:   "第一行\n第二行"
来源：http://nv.yuexingan06.cn

Ruby: "第一行\n第二行"
来源：http://ch.nicolike.cn

C#:   "第一行\n第二行"
来源：http://ds.bookmarksfly.cn

[A14] 注释写法
来源：http://cn.muxihuayi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://uk.jianghongdianzi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://nm.shxzukj.cn

JS:   // 单行；/* 多行 */
来源：http://ad.bookmarksfly.cn

TS:   // 单行；/* 多行 */
来源：http://um.yuntaijiaju.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://si.haigaiapp.cn

Go:   // 单行；/* 多行 */
来源：http://fd.yuntaijiaju.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ze.yuexingan06.cn

C#:   // 单行；/* 多行 */
来源：http://pw.nszjky.cn

[A15] 空值判断与默认值
来源：http://dq.lnxyls.cn

Py:   value = data or "默认值"
来源：http://bf.haigaiapp.cn

PHP:  $value = $data ?? "默认值";
来源：http://wq.szsharing.cn

JS:   const value = data ?? "默认值";
来源：http://hf.hnjuh.cn

TS:   const value = data ?? "默认值";
来源：http://vy.haigaiapp.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fi.szxytkj.cn

Go:   if data == "" { data = "默认值" }
来源：http://uw.hnjuh.cn

Ruby: value = data || "默认值"
来源：http://nm.panjiajie.cn

C#:   var value = data ?? "默认值";
来源：http://zw.panjiajie.cn

[A16] 真假值判断规则
来源：http://ez.colortex.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yo.hnjuh.cn


<!-- 参考信息 -->