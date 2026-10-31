代发 wailian999

[U85] JS：可选链
来源：http://cn.huanxung.cn

a?.b?.c
来源：http://iu.colortex.cn

[U86] JS：空值合并
来源：http://wn.nicolike.cn

a ?? b
来源：http://qf.yuntaijiaju.cn

[U87] JS：解构默认值
来源：http://gv.yuntaijiaju.cn

const { a = 1, b = 2 } = obj;
来源：http://id.wgjwhj.cn

[U88] JS：对象展开合并
来源：http://sq.521024.cn

{ ...a, ...b }
来源：http://lm.shxzukj.cn

[U89] JS：数组去重
来源：http://ty.bookmarksfly.cn

[...new Set(arr)]
来源：http://nw.nicolike.cn

[U90] JS：数字数组排序
来源：http://qr.huixiangedu.cn

[...arr].sort((a, b) => a - b)
来源：http://xt.newstarts.cn

[U91] JS：对象键值遍历
来源：http://mu.gzmigu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dy.hnjuh.cn

[U92] JS：深拷贝
来源：http://tp.jctech888.com.cn

structuredClone(obj)
来源：http://li.hahajie.cn

[U93] JS：模板字符串
来源：http://hl.haigaiapp.cn

`共 ${n} 条`
来源：http://cv.gzmigu.cn

[U94] JS：箭头函数
来源：http://up.shxzskj.cn

const double = x => x * 2;
来源：http://jc.521024.cn

[U95] JS：Promise 包装
来源：http://me.haigaiapp.cn

new Promise((resolve, reject) => {})
来源：http://sz.wgjwhj.cn

[U96] JS：async/await 与异常
来源：http://zj.jctech888.com.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bh.panjiajie.cn

[U97] JS：并发请求
来源：http://di.asd995.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://uw.newstarts.cn

[U98] JS：fetch 带 JSON
来源：http://gs.wgjwhj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fs.hnjuh.cn

[U99] JS：事件监听
来源：http://tx.jianghongdianzi.cn

el.addEventListener("click", e => {})
来源：http://yv.gzmigu.cn

[U100] JS：DOM 查询
来源：http://cj.bookmarksfly.cn

document.querySelector(".item")
来源：http://pu.shtwfgs.cn

[U101] JS：classList 操作
来源：http://zd.gzmigu.cn

el.classList.toggle("active")
来源：http://wv.chemitech.net.cn

[U102] JS：本地存储
来源：http://do.panjiajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ly.hnjuh.cn

[U103] JS：定时器
来源：http://uf.szxytkj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://io.huanxung.cn

[U104] JS：防抖
来源：http://rm.newstarts.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cv.shxzukj.cn

[U105] JS：节流
来源：http://gx.panjiajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cg.huanxung.cn

[U106] JS：日期格式化
来源：http://hz.szxytkj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rk.shxzukj.cn

[U107] JS：数字千分位
来源：http://lh.huanxung.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ct.yuexingan06.cn

[U108] JS：随机整数
来源：http://zp.muxihuayi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ua.huanxung.cn

[U109] JS：数组分组
来源：http://zi.hnjuh.cn

Object.groupBy(arr, x => x.type)
来源：http://cb.shtwfgs.cn

[U110] JS：数组分块
来源：http://ae.nszjky.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jh.panjiajie.cn

[U111] JS：对象转 Map
来源：http://uu.chemitech.net.cn

new Map(Object.entries(obj))
来源：http://yc.asd995.cn

[U112] JS：字符串补位
来源：http://mj.shxzskj.cn

"7".padStart(3, "0")
来源：http://cf.bjjhwx.cn

[U113] JS：正则替换全部
来源：http://ao.huixinmuqiang.cn

s.replaceAll("a", "b")
来源：http://bb.jctech888.com.cn

[U114] JS：JSON 深比较
来源：http://nv.521024.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pq.colortex.cn

[U115] JS：生成 UUID
来源：http://fy.shxzskj.cn

crypto.randomUUID()
来源：http://mg.shxzukj.cn

[U116] JS：类型检查（JSDoc）
来源：http://ra.521024.cn

/** @param {string} name */ function f(name) {}
来源：http://qa.yuntaijiaju.cn

[U117] JS：单元测试
来源：http://bi.colortex.cn

npm i -D vitest;  npx vitest
来源：http://xh.gzmigu.cn

[U118] JS：开发服务器
来源：http://aw.newstarts.cn

npm i -D vite;  npx vite
来源：http://pb.szsharing.cn

[U119] JS：生产构建
来源：http://bk.jianghongdianzi.cn

npx vite build
来源：http://sj.bjjhwx.cn

[U120] JS：读取环境变量（Vite）
来源：http://ib.nicolike.cn

import.meta.env.VITE_API_URL
来源：http://nj.colortex.cn

================================================================================
来源：http://vc.yuntaijiaju.cn

统计汇总
来源：http://wn.nicolike.cn

================================================================================
来源：http://nl.gzmigu.cn

按语言统计（条）：
来源：http://ce.haigaiapp.cn

Python ......... 252
来源：http://yu.haigaiapp.cn

PHP ............ 252
来源：http://kf.jctech888.com.cn

JavaScript ..... 252
来源：http://cu.521024.cn

TypeScript ..... 212
来源：http://ql.hnjuh.cn

Java ........... 212
来源：http://tl.jianghongdianzi.cn

Go ............. 212
来源：http://hf.shxzukj.cn

Ruby ........... 212
来源：http://vf.hahajie.cn

C# ............. 212
来源：http://hq.hnjuh.cn

C .............. 30
来源：http://rv.nszjky.cn

C++ ............ 30
来源：http://oy.haigaiapp.cn

SQL ............ 90
来源：http://cl.bookmarksfly.cn

Bash ........... 80
来源：http://dp.asd995.cn

Kotlin ......... 15
来源：http://ho.shxzskj.cn

Swift .......... 15
来源：http://qg.hahajie.cn

Lua ............ 10
来源：http://nn.panjiajie.cn

Perl ........... 10
来源：http://hg.gzmigu.cn

Scala .......... 10
来源：http://te.jianghongdianzi.cn

------------------------------------
来源：http://sk.szsharing.cn

合计 ........... 2106 条
来源：http://cp.huixiangedu.cn

按章节统计：
来源：http://eg.newstarts.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ac.yuntaijiaju.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dy.jianghongdianzi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fm.shtwfgs.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hm.yuntaijiaju.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xr.haigaiapp.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pc.wgjwhj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hn.yuntaijiaju.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kn.wgjwhj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hk.colortex.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://an.9csxet.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qy.chemitech.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://of.shxzskj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://co.huixinmuqiang.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ef.szsharing.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ua.hahajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://op.nicolike.cn

Q SQL 专题                              90
来源：http://zv.shtwfgs.cn

R Bash 专题                             80
来源：http://ol.bookmarksfly.cn

S C / C++ 专题                          60
来源：http://ka.panjiajie.cn

T 其他语言补充                          60
来源：http://wm.asd995.cn

U 高频实用片段                         120
来源：http://cp.huixiangedu.cn

------------------------------------
来源：http://ro.chemitech.net.cn

合计                                  2106 条
来源：http://rc.hahajie.cn

--------------------------------------------------------------------------------
来源：http://wj.lnxyls.cn

使用提醒
来源：http://uc.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://mm.panjiajie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dz.huanxung.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://su.521024.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nx.lnxyls.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ip.hnjuh.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://oh.shxzukj.cn

—— 文件结束 ——
来源：http://zm.chemitech.net.cn

================================================================================
来源：http://da.colortex.cn

程序语言常见例子速查手册（2024 版）
来源：http://zt.shtwfgs.cn

Common Programming Examples Cheat Book
来源：http://ot.nicolike.cn

================================================================================
来源：http://vz.newstarts.cn

【收录内容】
来源：http://rp.hnjuh.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://xx.szsharing.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ea.haigaiapp.cn

SQL · Bash · C · C++
来源：http://sy.yuexingan06.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://by.szsharing.cn

【使用说明】
来源：http://hp.colortex.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pc.gzmigu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dm.newstarts.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bk.bjjhwx.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://so.huixiangedu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://jk.jctech888.com.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cx.bookmarksfly.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ae.newstarts.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ou.hahajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ch.colortex.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gl.haigaiapp.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gl.haigaiapp.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yc.bjjhwx.cn

【文件统计】
来源：http://gh.yuexingan06.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vi.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://hw.9csxet.cn

目  录
来源：http://uz.szsharing.cn

--------------------------------------------------------------------------------
来源：http://fx.chemitech.net.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://sr.521024.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jh.chemitech.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dl.colortex.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zk.muxihuayi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jz.wgjwhj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mo.szsharing.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wv.gzmigu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vd.bookmarksfly.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ap.shxzskj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yl.szxytkj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://eu.huixinmuqiang.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cn.shxzukj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://eu.colortex.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cg.yuexingan06.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xp.yuntaijiaju.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://du.newstarts.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ck.hnjuh.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ld.9csxet.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vm.wgjwhj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fn.panjiajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ik.wgjwhj.cn

================================================================================
来源：http://la.panjiajie.cn

A. 基础语法与类型
来源：http://yr.521024.cn

================================================================================
来源：http://rj.colortex.cn

[A01] Hello World
来源：http://qq.bookmarksfly.cn

Py:   print("Hello, World!")
来源：http://mt.nicolike.cn

PHP:  echo "Hello, World!";
来源：http://rf.9csxet.cn

JS:   console.log("Hello, World!");
来源：http://hk.szxytkj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mj.9csxet.cn

Java: System.out.println("Hello, World!");
来源：http://ld.bjjhwx.cn

Go:   fmt.Println("Hello, World!")
来源：http://rh.colortex.cn

Ruby: puts "Hello, World!"
来源：http://ij.chemitech.net.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://sp.yuexingan06.cn

[A02] 变量声明与赋值
来源：http://ya.shtwfgs.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wj.nicolike.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://nt.bookmarksfly.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ds.huixinmuqiang.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mn.hnjuh.cn

Java: String name = "Alex"; int age = 20;
来源：http://ga.colortex.cn

Go:   name := "Alex"; age := 20
来源：http://ym.nszjky.cn

Ruby: name = "Alex"; age = 20
来源：http://pu.huixiangedu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://tg.9csxet.cn

[A03] 常量定义
来源：http://fy.9csxet.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xi.chemitech.net.cn

PHP:  const PI = 3.14159;
来源：http://vw.bookmarksfly.cn

JS:   const PI = 3.14159;
来源：http://fs.panjiajie.cn

TS:   const PI: number = 3.14159;
来源：http://nf.bookmarksfly.cn

Java: static final double PI = 3.14159;
来源：http://xe.hnjuh.cn

Go:   const PI = 3.14159
来源：http://hr.haigaiapp.cn

Ruby: PI = 3.14159
来源：http://ux.lnxyls.cn

C#:   const double PI = 3.14159;
来源：http://ng.hahajie.cn

[A04] 判断变量类型
来源：http://lk.panjiajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://lk.nicolike.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://io.nszjky.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ck.9csxet.cn

TS:   typeof x; x instanceof Date
来源：http://wa.panjiajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rl.asd995.cn

Go:   reflect.TypeOf(x).Name()
来源：http://kz.colortex.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://sc.szxytkj.cn

C#:   x.GetType().Name; x is int
来源：http://wt.huixinmuqiang.cn

[A05] 整数除法与取模
来源：http://yc.yuexingan06.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wu.lnxyls.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qe.haigaiapp.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pv.newstarts.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://oo.szxytkj.cn

Java: 7 / 2; 7 % 2
来源：http://fa.szxytkj.cn

Go:   7 / 2; 7 % 2
来源：http://nr.nicolike.cn

Ruby: 7 / 2; 7 % 2
来源：http://ax.jctech888.com.cn

C#:   7 / 2; 7 % 2
来源：http://dt.shtwfgs.cn

[A06] 字符串转数字
来源：http://yv.huixiangedu.cn

Py:   int("42"); float("3.14")
来源：http://jp.lnxyls.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mv.jianghongdianzi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pk.muxihuayi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://lo.shtwfgs.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lo.colortex.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pv.huanxung.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://iz.panjiajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rr.lnxyls.cn

[A07] 数字转字符串
来源：http://ex.gzmigu.cn

Py:   str(42)
来源：http://zy.szsharing.cn

PHP:  (string) 42; strval(42)
来源：http://je.9csxet.cn

JS:   String(42); (42).toString()
来源：http://po.9csxet.cn

TS:   String(42)
来源：http://sn.huanxung.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://an.jctech888.com.cn

Go:   strconv.Itoa(42)
来源：http://fn.521024.cn

Ruby: 42.to_s
来源：http://oq.wgjwhj.cn

C#:   42.ToString()
来源：http://tq.jianghongdianzi.cn

[A08] 取整与四舍五入
来源：http://tk.yuexingan06.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tl.newstarts.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ty.9csxet.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zx.huixiangedu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fa.panjiajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dd.bookmarksfly.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://it.lnxyls.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://yq.shtwfgs.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hw.asd995.cn

[A09] 绝对值与最大最小值
来源：http://dl.wgjwhj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vm.shxzukj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://sk.szxytkj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ul.newstarts.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wm.chemitech.net.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bc.colortex.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gp.szsharing.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kl.huixiangedu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://cc.hahajie.cn

[A10] 生成随机数
来源：http://sb.hnjuh.cn

Py:   import random; random.randint(1, 100)
来源：http://pd.haigaiapp.cn

PHP:  random_int(1, 100);
来源：http://ao.nicolike.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wy.521024.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://oe.szsharing.cn

Java: new Random().nextInt(100) + 1
来源：http://bt.asd995.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://nl.hnjuh.cn

Ruby: rand(1..100)
来源：http://qq.jianghongdianzi.cn

C#:   new Random().Next(1, 101)
来源：http://ha.bookmarksfly.cn

[A11] 条件表达式（三元）
来源：http://yw.chemitech.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://iz.muxihuayi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://td.huanxung.cn

JS:   x > 0 ? "yes" : "no"
来源：http://fh.yuntaijiaju.cn

TS:   x > 0 ? "yes" : "no"
来源：http://bw.jianghongdianzi.cn

Java: x > 0 ? "yes" : "no"
来源：http://qt.szsharing.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://gq.gzmigu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ws.newstarts.cn

C#:   x > 0 ? "yes" : "no"
来源：http://qv.newstarts.cn

[A12] 字符串插值 / 格式化
来源：http://ad.chemitech.net.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ki.521024.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ne.521024.cn

JS:   `Hello, ${name}!`
来源：http://li.szsharing.cn

TS:   `Hello, ${name}!`
来源：http://db.szxytkj.cn

Java: "Hello, %s!".formatted(name)
来源：http://hu.chemitech.net.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xa.muxihuayi.cn

Ruby: "Hello, #{name}!"
来源：http://uw.jianghongdianzi.cn

C#:   $"Hello, {name}!"
来源：http://oy.chemitech.net.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://fx.shxzskj.cn

Py:   "第一行\n第二行"
来源：http://na.asd995.cn

PHP:  "第一行\n第二行"
来源：http://zg.huanxung.cn

JS:   "第一行\n第二行"
来源：http://hz.bookmarksfly.cn

TS:   "第一行\n第二行"
来源：http://mm.yuexingan06.cn

Java: "第一行\n第二行"
来源：http://iv.bjjhwx.cn

Go:   "第一行\n第二行"
来源：http://ie.bjjhwx.cn

Ruby: "第一行\n第二行"
来源：http://vl.jianghongdianzi.cn

C#:   "第一行\n第二行"
来源：http://pa.bjjhwx.cn

[A14] 注释写法
来源：http://fi.shtwfgs.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ei.yuexingan06.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://mz.9csxet.cn

JS:   // 单行；/* 多行 */
来源：http://rz.nszjky.cn


<!-- 参考信息 -->