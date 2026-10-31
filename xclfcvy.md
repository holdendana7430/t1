代发 wailian999

[U87] JS：解构默认值
来源：http://na.newstarts.cn

const { a = 1, b = 2 } = obj;
来源：http://qv.gzmigu.cn

[U88] JS：对象展开合并
来源：http://rr.gzmigu.cn

{ ...a, ...b }
来源：http://zg.huixiangedu.cn

[U89] JS：数组去重
来源：http://gm.lnxyls.cn

[...new Set(arr)]
来源：http://de.huanxung.cn

[U90] JS：数字数组排序
来源：http://lb.gzmigu.cn

[...arr].sort((a, b) => a - b)
来源：http://yg.muxihuayi.cn

[U91] JS：对象键值遍历
来源：http://lc.jctech888.com.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ir.hnjuh.cn

[U92] JS：深拷贝
来源：http://ez.wgjwhj.cn

structuredClone(obj)
来源：http://vj.gzmigu.cn

[U93] JS：模板字符串
来源：http://bk.haigaiapp.cn

`共 ${n} 条`
来源：http://tz.bjjhwx.cn

[U94] JS：箭头函数
来源：http://dt.9csxet.cn

const double = x => x * 2;
来源：http://ep.newstarts.cn

[U95] JS：Promise 包装
来源：http://xe.521024.cn

new Promise((resolve, reject) => {})
来源：http://dm.shtwfgs.cn

[U96] JS：async/await 与异常
来源：http://ay.yuexingan06.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vx.lnxyls.cn

[U97] JS：并发请求
来源：http://ma.huanxung.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dc.haigaiapp.cn

[U98] JS：fetch 带 JSON
来源：http://cw.nszjky.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rk.muxihuayi.cn

[U99] JS：事件监听
来源：http://xx.bjjhwx.cn

el.addEventListener("click", e => {})
来源：http://zq.jianghongdianzi.cn

[U100] JS：DOM 查询
来源：http://rh.521024.cn

document.querySelector(".item")
来源：http://kp.haigaiapp.cn

[U101] JS：classList 操作
来源：http://cr.shxzukj.cn

el.classList.toggle("active")
来源：http://ln.nszjky.cn

[U102] JS：本地存储
来源：http://wn.gzmigu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sv.yuexingan06.cn

[U103] JS：定时器
来源：http://fb.hnjuh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gi.bookmarksfly.cn

[U104] JS：防抖
来源：http://rl.chemitech.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ti.bjjhwx.cn

[U105] JS：节流
来源：http://ib.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://af.bjjhwx.cn

[U106] JS：日期格式化
来源：http://oa.gzmigu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ua.yuexingan06.cn

[U107] JS：数字千分位
来源：http://gx.yuntaijiaju.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nj.jianghongdianzi.cn

[U108] JS：随机整数
来源：http://qv.asd995.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cp.521024.cn

[U109] JS：数组分组
来源：http://xt.yuntaijiaju.cn

Object.groupBy(arr, x => x.type)
来源：http://ed.bookmarksfly.cn

[U110] JS：数组分块
来源：http://vz.chemitech.net.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ig.yuexingan06.cn

[U111] JS：对象转 Map
来源：http://qc.hnjuh.cn

new Map(Object.entries(obj))
来源：http://bo.muxihuayi.cn

[U112] JS：字符串补位
来源：http://jv.521024.cn

"7".padStart(3, "0")
来源：http://be.bjjhwx.cn

[U113] JS：正则替换全部
来源：http://jp.haigaiapp.cn

s.replaceAll("a", "b")
来源：http://gv.jianghongdianzi.cn

[U114] JS：JSON 深比较
来源：http://vu.huixinmuqiang.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cs.huanxung.cn

[U115] JS：生成 UUID
来源：http://up.hnjuh.cn

crypto.randomUUID()
来源：http://yy.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://ww.bookmarksfly.cn

/** @param {string} name */ function f(name) {}
来源：http://ye.haigaiapp.cn

[U117] JS：单元测试
来源：http://sv.bookmarksfly.cn

npm i -D vitest;  npx vitest
来源：http://vy.chemitech.net.cn

[U118] JS：开发服务器
来源：http://ni.wgjwhj.cn

npm i -D vite;  npx vite
来源：http://jy.bookmarksfly.cn

[U119] JS：生产构建
来源：http://oz.shxzskj.cn

npx vite build
来源：http://bn.shtwfgs.cn

[U120] JS：读取环境变量（Vite）
来源：http://ac.bookmarksfly.cn

import.meta.env.VITE_API_URL
来源：http://xg.szxytkj.cn

================================================================================
来源：http://nu.gzmigu.cn

统计汇总
来源：http://yh.huanxung.cn

================================================================================
来源：http://ba.521024.cn

按语言统计（条）：
来源：http://iq.chemitech.net.cn

Python ......... 252
来源：http://jg.521024.cn

PHP ............ 252
来源：http://bm.panjiajie.cn

JavaScript ..... 252
来源：http://yo.szxytkj.cn

TypeScript ..... 212
来源：http://ds.bjjhwx.cn

Java ........... 212
来源：http://xu.hnjuh.cn

Go ............. 212
来源：http://eq.newstarts.cn

Ruby ........... 212
来源：http://mv.huanxung.cn

C# ............. 212
来源：http://gb.yuntaijiaju.cn

C .............. 30
来源：http://zg.wgjwhj.cn

C++ ............ 30
来源：http://fp.nszjky.cn

SQL ............ 90
来源：http://of.yuntaijiaju.cn

Bash ........... 80
来源：http://va.hahajie.cn

Kotlin ......... 15
来源：http://ro.bjjhwx.cn

Swift .......... 15
来源：http://ly.newstarts.cn

Lua ............ 10
来源：http://ko.chemitech.net.cn

Perl ........... 10
来源：http://qv.hnjuh.cn

Scala .......... 10
来源：http://cu.chemitech.net.cn

------------------------------------
来源：http://um.shxzukj.cn

合计 ........... 2106 条
来源：http://lc.yuntaijiaju.cn

按章节统计：
来源：http://ko.panjiajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zs.hnjuh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lb.chemitech.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ta.hahajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jw.gzmigu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gl.yuntaijiaju.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wx.chemitech.net.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gq.panjiajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://im.gzmigu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pp.huanxung.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qw.yuexingan06.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pk.jianghongdianzi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ak.nszjky.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dj.gzmigu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lt.huixinmuqiang.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hm.wgjwhj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yz.wgjwhj.cn

Q SQL 专题                              90
来源：http://oa.521024.cn

R Bash 专题                             80
来源：http://el.gzmigu.cn

S C / C++ 专题                          60
来源：http://om.bjjhwx.cn

T 其他语言补充                          60
来源：http://qy.9csxet.cn

U 高频实用片段                         120
来源：http://ub.asd995.cn

------------------------------------
来源：http://kr.hahajie.cn

合计                                  2106 条
来源：http://ui.asd995.cn

--------------------------------------------------------------------------------
来源：http://co.szsharing.cn

使用提醒
来源：http://kf.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://es.bookmarksfly.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ci.asd995.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://af.gzmigu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gp.9csxet.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ur.nszjky.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jw.szxytkj.cn

—— 文件结束 ——
来源：http://ur.nicolike.cn

================================================================================
来源：http://pp.huixiangedu.cn

程序语言常见例子速查手册（2024 版）
来源：http://qc.jctech888.com.cn

Common Programming Examples Cheat Book
来源：http://ac.shtwfgs.cn

================================================================================
来源：http://cc.shtwfgs.cn

【收录内容】
来源：http://bt.colortex.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://no.nszjky.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wc.szxytkj.cn

SQL · Bash · C · C++
来源：http://jt.huixinmuqiang.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bx.shxzukj.cn

【使用说明】
来源：http://hk.jianghongdianzi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bq.hnjuh.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bm.jianghongdianzi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lq.muxihuayi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vd.nszjky.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://bs.shxzukj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://am.szxytkj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://te.jianghongdianzi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://eq.panjiajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://it.nicolike.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://be.asd995.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ch.shtwfgs.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kc.hahajie.cn

【文件统计】
来源：http://xu.jianghongdianzi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lo.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://ms.yuntaijiaju.cn

目  录
来源：http://mc.colortex.cn

--------------------------------------------------------------------------------
来源：http://dy.shxzskj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ez.chemitech.net.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dh.huixinmuqiang.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://on.nicolike.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qx.muxihuayi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dh.hahajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pj.muxihuayi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://oo.chemitech.net.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gd.wgjwhj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ft.haigaiapp.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rf.szxytkj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xw.muxihuayi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qq.muxihuayi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ud.gzmigu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xv.huixiangedu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ni.newstarts.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yp.jianghongdianzi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gg.chemitech.net.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wp.chemitech.net.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yq.shxzukj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yp.9csxet.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lf.asd995.cn

================================================================================
来源：http://if.shxzukj.cn

A. 基础语法与类型
来源：http://yw.colortex.cn

================================================================================
来源：http://nu.jianghongdianzi.cn

[A01] Hello World
来源：http://cw.szxytkj.cn

Py:   print("Hello, World!")
来源：http://fm.bookmarksfly.cn

PHP:  echo "Hello, World!";
来源：http://fc.nszjky.cn

JS:   console.log("Hello, World!");
来源：http://ap.huanxung.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ei.chemitech.net.cn

Java: System.out.println("Hello, World!");
来源：http://hm.shtwfgs.cn

Go:   fmt.Println("Hello, World!")
来源：http://yo.newstarts.cn

Ruby: puts "Hello, World!"
来源：http://ir.huixiangedu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://rh.gzmigu.cn

[A02] 变量声明与赋值
来源：http://jq.nicolike.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yw.huixiangedu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://yp.nicolike.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ek.huanxung.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vf.nszjky.cn

Java: String name = "Alex"; int age = 20;
来源：http://hx.nszjky.cn

Go:   name := "Alex"; age := 20
来源：http://cs.nszjky.cn

Ruby: name = "Alex"; age = 20
来源：http://sc.shtwfgs.cn

C#:   string name = "Alex"; int age = 20;
来源：http://oi.nszjky.cn

[A03] 常量定义
来源：http://ko.haigaiapp.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hh.haigaiapp.cn

PHP:  const PI = 3.14159;
来源：http://pf.shxzukj.cn

JS:   const PI = 3.14159;
来源：http://ka.jianghongdianzi.cn

TS:   const PI: number = 3.14159;
来源：http://yo.shtwfgs.cn

Java: static final double PI = 3.14159;
来源：http://ou.muxihuayi.cn

Go:   const PI = 3.14159
来源：http://wu.hahajie.cn

Ruby: PI = 3.14159
来源：http://in.asd995.cn

C#:   const double PI = 3.14159;
来源：http://ur.nszjky.cn

[A04] 判断变量类型
来源：http://bn.haigaiapp.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vk.szxytkj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ah.gzmigu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qm.yuntaijiaju.cn

TS:   typeof x; x instanceof Date
来源：http://yd.nszjky.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kf.asd995.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fg.hahajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xe.shtwfgs.cn

C#:   x.GetType().Name; x is int
来源：http://yn.hnjuh.cn

[A05] 整数除法与取模
来源：http://et.hahajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rn.chemitech.net.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ib.panjiajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vp.yuexingan06.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ei.szxytkj.cn

Java: 7 / 2; 7 % 2
来源：http://mk.shxzskj.cn

Go:   7 / 2; 7 % 2
来源：http://nu.asd995.cn

Ruby: 7 / 2; 7 % 2
来源：http://nb.huixinmuqiang.cn

C#:   7 / 2; 7 % 2
来源：http://ib.asd995.cn

[A06] 字符串转数字
来源：http://tn.hnjuh.cn

Py:   int("42"); float("3.14")
来源：http://oy.hahajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://sq.huixiangedu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ln.wgjwhj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://gi.wgjwhj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wy.haigaiapp.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uf.gzmigu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://sa.bookmarksfly.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://up.chemitech.net.cn

[A07] 数字转字符串
来源：http://lp.shxzskj.cn

Py:   str(42)
来源：http://as.colortex.cn

PHP:  (string) 42; strval(42)
来源：http://ep.colortex.cn

JS:   String(42); (42).toString()
来源：http://ur.9csxet.cn

TS:   String(42)
来源：http://et.wgjwhj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xf.yuexingan06.cn

Go:   strconv.Itoa(42)
来源：http://nn.yuexingan06.cn

Ruby: 42.to_s
来源：http://rt.hahajie.cn

C#:   42.ToString()
来源：http://wg.hahajie.cn

[A08] 取整与四舍五入
来源：http://wo.nicolike.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qp.huixinmuqiang.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ek.panjiajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://il.muxihuayi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bn.nszjky.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ip.bookmarksfly.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tx.9csxet.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://sa.shtwfgs.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yp.jctech888.com.cn

[A09] 绝对值与最大最小值
来源：http://qa.shtwfgs.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://it.huixiangedu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jv.panjiajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rg.szsharing.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://am.shxzskj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ok.wgjwhj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mg.huixiangedu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://sx.chemitech.net.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://eg.jianghongdianzi.cn

[A10] 生成随机数
来源：http://dn.huixinmuqiang.cn

Py:   import random; random.randint(1, 100)
来源：http://jw.521024.cn

PHP:  random_int(1, 100);
来源：http://ws.nicolike.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fd.shtwfgs.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ps.asd995.cn

Java: new Random().nextInt(100) + 1
来源：http://yz.chemitech.net.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://sq.nszjky.cn

Ruby: rand(1..100)
来源：http://sa.yuntaijiaju.cn

C#:   new Random().Next(1, 101)
来源：http://iv.huixinmuqiang.cn

[A11] 条件表达式（三元）
来源：http://yw.shxzukj.cn

Py:   "yes" if x > 0 else "no"
来源：http://ww.newstarts.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rb.haigaiapp.cn

JS:   x > 0 ? "yes" : "no"
来源：http://lo.muxihuayi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dm.hnjuh.cn

Java: x > 0 ? "yes" : "no"
来源：http://qq.bookmarksfly.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://vp.hnjuh.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://py.gzmigu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ma.hnjuh.cn

[A12] 字符串插值 / 格式化
来源：http://eq.shtwfgs.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rw.panjiajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://su.jianghongdianzi.cn

JS:   `Hello, ${name}!`
来源：http://wb.bookmarksfly.cn

TS:   `Hello, ${name}!`
来源：http://vg.jctech888.com.cn

Java: "Hello, %s!".formatted(name)
来源：http://zq.szxytkj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://km.hahajie.cn

Ruby: "Hello, #{name}!"
来源：http://rp.shxzskj.cn

C#:   $"Hello, {name}!"
来源：http://hk.chemitech.net.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://lo.lnxyls.cn

Py:   "第一行\n第二行"
来源：http://sq.hahajie.cn

PHP:  "第一行\n第二行"
来源：http://bc.shxzskj.cn

JS:   "第一行\n第二行"
来源：http://pr.521024.cn

TS:   "第一行\n第二行"
来源：http://sm.bjjhwx.cn

Java: "第一行\n第二行"
来源：http://ly.szxytkj.cn

Go:   "第一行\n第二行"
来源：http://ev.hahajie.cn

Ruby: "第一行\n第二行"
来源：http://if.shxzukj.cn

C#:   "第一行\n第二行"
来源：http://eh.gzmigu.cn

[A14] 注释写法
来源：http://bf.asd995.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://uu.nicolike.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://oh.hahajie.cn

JS:   // 单行；/* 多行 */
来源：http://fp.bookmarksfly.cn

TS:   // 单行；/* 多行 */
来源：http://le.bookmarksfly.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bf.shxzskj.cn

Go:   // 单行；/* 多行 */
来源：http://fk.jianghongdianzi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://lj.gzmigu.cn


<!-- 参考信息 -->