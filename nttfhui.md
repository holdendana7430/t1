代发 wailian999

[U91] JS：对象键值遍历
来源：http://jg.bjjhwx.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xk.panjiajie.cn

[U92] JS：深拷贝
来源：http://mx.panjiajie.cn

structuredClone(obj)
来源：http://cb.nszjky.cn

[U93] JS：模板字符串
来源：http://vj.wgjwhj.cn

`共 ${n} 条`
来源：http://sr.9csxet.cn

[U94] JS：箭头函数
来源：http://bq.jianghongdianzi.cn

const double = x => x * 2;
来源：http://mj.521024.cn

[U95] JS：Promise 包装
来源：http://fe.nszjky.cn

new Promise((resolve, reject) => {})
来源：http://pf.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://ot.szsharing.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hu.nicolike.cn

[U97] JS：并发请求
来源：http://vn.9csxet.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pq.yuntaijiaju.cn

[U98] JS：fetch 带 JSON
来源：http://qw.chemitech.net.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://re.asd995.cn

[U99] JS：事件监听
来源：http://ql.chemitech.net.cn

el.addEventListener("click", e => {})
来源：http://er.bjjhwx.cn

[U100] JS：DOM 查询
来源：http://ol.haigaiapp.cn

document.querySelector(".item")
来源：http://aq.hnjuh.cn

[U101] JS：classList 操作
来源：http://rm.huixiangedu.cn

el.classList.toggle("active")
来源：http://nr.colortex.cn

[U102] JS：本地存储
来源：http://ab.nicolike.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jr.szxytkj.cn

[U103] JS：定时器
来源：http://py.huixinmuqiang.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uo.bookmarksfly.cn

[U104] JS：防抖
来源：http://wu.chemitech.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://os.nszjky.cn

[U105] JS：节流
来源：http://bb.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hf.panjiajie.cn

[U106] JS：日期格式化
来源：http://dv.521024.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gb.shxzukj.cn

[U107] JS：数字千分位
来源：http://zb.huanxung.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cz.shxzukj.cn

[U108] JS：随机整数
来源：http://yr.jctech888.com.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://iu.shxzskj.cn

[U109] JS：数组分组
来源：http://ak.shtwfgs.cn

Object.groupBy(arr, x => x.type)
来源：http://fg.colortex.cn

[U110] JS：数组分块
来源：http://qw.gzmigu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gd.hahajie.cn

[U111] JS：对象转 Map
来源：http://je.wgjwhj.cn

new Map(Object.entries(obj))
来源：http://fm.yuexingan06.cn

[U112] JS：字符串补位
来源：http://vk.newstarts.cn

"7".padStart(3, "0")
来源：http://tf.szxytkj.cn

[U113] JS：正则替换全部
来源：http://xj.newstarts.cn

s.replaceAll("a", "b")
来源：http://hr.bookmarksfly.cn

[U114] JS：JSON 深比较
来源：http://hx.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://il.lnxyls.cn

[U115] JS：生成 UUID
来源：http://wx.muxihuayi.cn

crypto.randomUUID()
来源：http://sv.muxihuayi.cn

[U116] JS：类型检查（JSDoc）
来源：http://hb.muxihuayi.cn

/** @param {string} name */ function f(name) {}
来源：http://po.huixinmuqiang.cn

[U117] JS：单元测试
来源：http://eu.nicolike.cn

npm i -D vitest;  npx vitest
来源：http://qx.panjiajie.cn

[U118] JS：开发服务器
来源：http://ty.colortex.cn

npm i -D vite;  npx vite
来源：http://py.panjiajie.cn

[U119] JS：生产构建
来源：http://km.yuexingan06.cn

npx vite build
来源：http://bt.gzmigu.cn

[U120] JS：读取环境变量（Vite）
来源：http://em.9csxet.cn

import.meta.env.VITE_API_URL
来源：http://co.szsharing.cn

================================================================================
来源：http://wz.bjjhwx.cn

统计汇总
来源：http://sf.521024.cn

================================================================================
来源：http://pk.hnjuh.cn

按语言统计（条）：
来源：http://hv.jianghongdianzi.cn

Python ......... 252
来源：http://mo.asd995.cn

PHP ............ 252
来源：http://as.521024.cn

JavaScript ..... 252
来源：http://fz.bookmarksfly.cn

TypeScript ..... 212
来源：http://wf.huixiangedu.cn

Java ........... 212
来源：http://vm.newstarts.cn

Go ............. 212
来源：http://sj.nicolike.cn

Ruby ........... 212
来源：http://qq.gzmigu.cn

C# ............. 212
来源：http://ne.szsharing.cn

C .............. 30
来源：http://sd.newstarts.cn

C++ ............ 30
来源：http://rm.panjiajie.cn

SQL ............ 90
来源：http://zc.nicolike.cn

Bash ........... 80
来源：http://cy.asd995.cn

Kotlin ......... 15
来源：http://ae.huixiangedu.cn

Swift .......... 15
来源：http://sp.muxihuayi.cn

Lua ............ 10
来源：http://kr.muxihuayi.cn

Perl ........... 10
来源：http://ly.muxihuayi.cn

Scala .......... 10
来源：http://ad.colortex.cn

------------------------------------
来源：http://eq.szsharing.cn

合计 ........... 2106 条
来源：http://eh.hnjuh.cn

按章节统计：
来源：http://xu.panjiajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cn.hahajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tm.haigaiapp.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://me.hahajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jz.yuntaijiaju.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xf.newstarts.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ff.jctech888.com.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uj.yuntaijiaju.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cc.huixiangedu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rl.asd995.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jt.gzmigu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ph.haigaiapp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gn.shtwfgs.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ha.hahajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tr.jctech888.com.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rh.521024.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fx.yuexingan06.cn

Q SQL 专题                              90
来源：http://xo.nicolike.cn

R Bash 专题                             80
来源：http://ao.muxihuayi.cn

S C / C++ 专题                          60
来源：http://vi.shxzskj.cn

T 其他语言补充                          60
来源：http://ep.yuexingan06.cn

U 高频实用片段                         120
来源：http://ma.szsharing.cn

------------------------------------
来源：http://xd.muxihuayi.cn

合计                                  2106 条
来源：http://gf.nicolike.cn

--------------------------------------------------------------------------------
来源：http://tn.yuexingan06.cn

使用提醒
来源：http://cp.asd995.cn

--------------------------------------------------------------------------------
来源：http://dt.lnxyls.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cc.wgjwhj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bl.shxzskj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ge.chemitech.net.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ww.panjiajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://op.szxytkj.cn

—— 文件结束 ——
来源：http://fx.lnxyls.cn

================================================================================
来源：http://xs.bookmarksfly.cn

程序语言常见例子速查手册（2024 版）
来源：http://kj.muxihuayi.cn

Common Programming Examples Cheat Book
来源：http://pe.newstarts.cn

================================================================================
来源：http://ii.huixiangedu.cn

【收录内容】
来源：http://tl.haigaiapp.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ys.szsharing.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vl.colortex.cn

SQL · Bash · C · C++
来源：http://og.lnxyls.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lk.shtwfgs.cn

【使用说明】
来源：http://zx.asd995.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tf.hahajie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xo.shtwfgs.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lz.bookmarksfly.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hj.jctech888.com.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ew.gzmigu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ey.shxzukj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jf.hnjuh.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dr.jianghongdianzi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mx.colortex.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ff.huixinmuqiang.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mz.nszjky.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ai.yuexingan06.cn

【文件统计】
来源：http://jc.huixiangedu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sd.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://sh.bookmarksfly.cn

目  录
来源：http://lj.huanxung.cn

--------------------------------------------------------------------------------
来源：http://ab.shxzukj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mc.521024.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kt.shxzskj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ii.panjiajie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ea.521024.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yo.hnjuh.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qo.wgjwhj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kg.wgjwhj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pv.hnjuh.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sx.haigaiapp.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://sj.haigaiapp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wm.shxzskj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.panjiajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hh.nszjky.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zz.panjiajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xx.colortex.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://oh.bjjhwx.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hb.jianghongdianzi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://de.hnjuh.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hw.newstarts.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qd.huixiangedu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kh.hnjuh.cn

================================================================================
来源：http://hf.9csxet.cn

A. 基础语法与类型
来源：http://tl.521024.cn

================================================================================
来源：http://qk.muxihuayi.cn

[A01] Hello World
来源：http://gv.newstarts.cn

Py:   print("Hello, World!")
来源：http://cg.muxihuayi.cn

PHP:  echo "Hello, World!";
来源：http://jk.colortex.cn

JS:   console.log("Hello, World!");
来源：http://nv.shxzukj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dz.colortex.cn

Java: System.out.println("Hello, World!");
来源：http://uh.shxzskj.cn

Go:   fmt.Println("Hello, World!")
来源：http://mz.hahajie.cn

Ruby: puts "Hello, World!"
来源：http://lr.chemitech.net.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://co.panjiajie.cn

[A02] 变量声明与赋值
来源：http://tt.haigaiapp.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vx.hahajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ij.hnjuh.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ac.jctech888.com.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yt.huixinmuqiang.cn

Java: String name = "Alex"; int age = 20;
来源：http://re.hnjuh.cn

Go:   name := "Alex"; age := 20
来源：http://zx.muxihuayi.cn

Ruby: name = "Alex"; age = 20
来源：http://om.nicolike.cn

C#:   string name = "Alex"; int age = 20;
来源：http://kc.colortex.cn

[A03] 常量定义
来源：http://gh.chemitech.net.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vi.chemitech.net.cn

PHP:  const PI = 3.14159;
来源：http://fp.jctech888.com.cn

JS:   const PI = 3.14159;
来源：http://eo.9csxet.cn

TS:   const PI: number = 3.14159;
来源：http://ee.wgjwhj.cn

Java: static final double PI = 3.14159;
来源：http://ul.bjjhwx.cn

Go:   const PI = 3.14159
来源：http://ha.bookmarksfly.cn

Ruby: PI = 3.14159
来源：http://je.panjiajie.cn

C#:   const double PI = 3.14159;
来源：http://pm.jianghongdianzi.cn

[A04] 判断变量类型
来源：http://fg.bjjhwx.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://go.panjiajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ac.bookmarksfly.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dv.huixiangedu.cn

TS:   typeof x; x instanceof Date
来源：http://nz.huanxung.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jm.yuexingan06.cn

Go:   reflect.TypeOf(x).Name()
来源：http://jb.wgjwhj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tx.colortex.cn

C#:   x.GetType().Name; x is int
来源：http://ee.huanxung.cn

[A05] 整数除法与取模
来源：http://oi.chemitech.net.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bw.huixiangedu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zv.lnxyls.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xk.lnxyls.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ed.bookmarksfly.cn

Java: 7 / 2; 7 % 2
来源：http://li.yuntaijiaju.cn

Go:   7 / 2; 7 % 2
来源：http://zr.colortex.cn

Ruby: 7 / 2; 7 % 2
来源：http://pr.chemitech.net.cn

C#:   7 / 2; 7 % 2
来源：http://wc.lnxyls.cn

[A06] 字符串转数字
来源：http://mn.lnxyls.cn

Py:   int("42"); float("3.14")
来源：http://hf.asd995.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ln.huanxung.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fc.colortex.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cd.bookmarksfly.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://is.521024.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vj.gzmigu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ed.asd995.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ai.szxytkj.cn

[A07] 数字转字符串
来源：http://zr.shtwfgs.cn

Py:   str(42)
来源：http://dn.yuexingan06.cn

PHP:  (string) 42; strval(42)
来源：http://ue.jianghongdianzi.cn

JS:   String(42); (42).toString()
来源：http://nz.jctech888.com.cn

TS:   String(42)
来源：http://fb.bookmarksfly.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xa.gzmigu.cn

Go:   strconv.Itoa(42)
来源：http://cr.521024.cn

Ruby: 42.to_s
来源：http://lw.asd995.cn

C#:   42.ToString()
来源：http://cd.huanxung.cn

[A08] 取整与四舍五入
来源：http://ni.lnxyls.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ia.huixiangedu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ro.lnxyls.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zo.panjiajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kr.hnjuh.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bw.hahajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gz.jctech888.com.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://tn.huixinmuqiang.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fe.bjjhwx.cn

[A09] 绝对值与最大最小值
来源：http://aa.colortex.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ne.shxzskj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hx.bjjhwx.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mm.asd995.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ki.panjiajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rk.huixiangedu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kw.haigaiapp.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://as.gzmigu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bw.chemitech.net.cn

[A10] 生成随机数
来源：http://uv.gzmigu.cn

Py:   import random; random.randint(1, 100)
来源：http://se.shxzukj.cn

PHP:  random_int(1, 100);
来源：http://ze.9csxet.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://uj.colortex.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pb.huanxung.cn

Java: new Random().nextInt(100) + 1
来源：http://lj.szxytkj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cf.huixiangedu.cn

Ruby: rand(1..100)
来源：http://ke.haigaiapp.cn

C#:   new Random().Next(1, 101)
来源：http://ku.newstarts.cn

[A11] 条件表达式（三元）
来源：http://vz.hnjuh.cn

Py:   "yes" if x > 0 else "no"
来源：http://fh.colortex.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cf.nszjky.cn

JS:   x > 0 ? "yes" : "no"
来源：http://oc.yuntaijiaju.cn

TS:   x > 0 ? "yes" : "no"
来源：http://gq.huanxung.cn

Java: x > 0 ? "yes" : "no"
来源：http://rb.9csxet.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://tx.nicolike.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://hh.shxzskj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://nf.jianghongdianzi.cn

[A12] 字符串插值 / 格式化
来源：http://nt.shxzskj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xb.muxihuayi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://iy.9csxet.cn

JS:   `Hello, ${name}!`
来源：http://cu.hahajie.cn

TS:   `Hello, ${name}!`
来源：http://yt.colortex.cn

Java: "Hello, %s!".formatted(name)
来源：http://gm.szxytkj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cj.yuntaijiaju.cn

Ruby: "Hello, #{name}!"
来源：http://mb.chemitech.net.cn

C#:   $"Hello, {name}!"
来源：http://qe.shxzukj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ku.muxihuayi.cn

Py:   "第一行\n第二行"
来源：http://dz.newstarts.cn

PHP:  "第一行\n第二行"
来源：http://pt.gzmigu.cn

JS:   "第一行\n第二行"
来源：http://zs.bookmarksfly.cn

TS:   "第一行\n第二行"
来源：http://kw.colortex.cn

Java: "第一行\n第二行"
来源：http://az.szsharing.cn

Go:   "第一行\n第二行"
来源：http://ok.chemitech.net.cn

Ruby: "第一行\n第二行"
来源：http://no.shxzskj.cn

C#:   "第一行\n第二行"
来源：http://cn.huixinmuqiang.cn

[A14] 注释写法
来源：http://lk.nicolike.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://me.colortex.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://uc.wgjwhj.cn

JS:   // 单行；/* 多行 */
来源：http://yz.nicolike.cn

TS:   // 单行；/* 多行 */
来源：http://px.hahajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://us.521024.cn

Go:   // 单行；/* 多行 */
来源：http://fl.bookmarksfly.cn

Ruby: # 单行；=begin 多行 =end
来源：http://mi.bjjhwx.cn

C#:   // 单行；/* 多行 */
来源：http://be.colortex.cn

[A15] 空值判断与默认值
来源：http://pa.shxzukj.cn

Py:   value = data or "默认值"
来源：http://tv.yuexingan06.cn

PHP:  $value = $data ?? "默认值";
来源：http://kk.asd995.cn

JS:   const value = data ?? "默认值";
来源：http://ud.hnjuh.cn

TS:   const value = data ?? "默认值";
来源：http://qx.jianghongdianzi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://sl.jianghongdianzi.cn

Go:   if data == "" { data = "默认值" }
来源：http://ay.hahajie.cn


<!-- 参考信息 -->