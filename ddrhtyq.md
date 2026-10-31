代发 wailian999

[U91] JS：对象键值遍历
来源：http://tx.jctech888.com.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cw.hahajie.cn

[U92] JS：深拷贝
来源：http://mq.hnjuh.cn

structuredClone(obj)
来源：http://qt.shtwfgs.cn

[U93] JS：模板字符串
来源：http://up.colortex.cn

`共 ${n} 条`
来源：http://jz.shxzskj.cn

[U94] JS：箭头函数
来源：http://qm.shxzskj.cn

const double = x => x * 2;
来源：http://rj.asd995.cn

[U95] JS：Promise 包装
来源：http://ud.jctech888.com.cn

new Promise((resolve, reject) => {})
来源：http://ot.yuntaijiaju.cn

[U96] JS：async/await 与异常
来源：http://mf.lnxyls.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ct.muxihuayi.cn

[U97] JS：并发请求
来源：http://oa.muxihuayi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lz.asd995.cn

[U98] JS：fetch 带 JSON
来源：http://pc.wgjwhj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://du.huixiangedu.cn

[U99] JS：事件监听
来源：http://dj.huixiangedu.cn

el.addEventListener("click", e => {})
来源：http://qt.nszjky.cn

[U100] JS：DOM 查询
来源：http://kx.shxzukj.cn

document.querySelector(".item")
来源：http://vo.newstarts.cn

[U101] JS：classList 操作
来源：http://hj.newstarts.cn

el.classList.toggle("active")
来源：http://uh.muxihuayi.cn

[U102] JS：本地存储
来源：http://zj.shxzskj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://px.haigaiapp.cn

[U103] JS：定时器
来源：http://nv.huixiangedu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yz.shxzskj.cn

[U104] JS：防抖
来源：http://od.huixiangedu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qh.shxzukj.cn

[U105] JS：节流
来源：http://fx.9csxet.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zu.shxzskj.cn

[U106] JS：日期格式化
来源：http://wr.szxytkj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sp.shxzukj.cn

[U107] JS：数字千分位
来源：http://fj.panjiajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xr.bookmarksfly.cn

[U108] JS：随机整数
来源：http://ez.jianghongdianzi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qj.bookmarksfly.cn

[U109] JS：数组分组
来源：http://bf.huixinmuqiang.cn

Object.groupBy(arr, x => x.type)
来源：http://dr.muxihuayi.cn

[U110] JS：数组分块
来源：http://vb.lnxyls.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jc.muxihuayi.cn

[U111] JS：对象转 Map
来源：http://rh.chemitech.net.cn

new Map(Object.entries(obj))
来源：http://ew.haigaiapp.cn

[U112] JS：字符串补位
来源：http://wi.jianghongdianzi.cn

"7".padStart(3, "0")
来源：http://ln.wgjwhj.cn

[U113] JS：正则替换全部
来源：http://oo.huixinmuqiang.cn

s.replaceAll("a", "b")
来源：http://ls.newstarts.cn

[U114] JS：JSON 深比较
来源：http://np.huixiangedu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ta.chemitech.net.cn

[U115] JS：生成 UUID
来源：http://zr.hahajie.cn

crypto.randomUUID()
来源：http://on.nicolike.cn

[U116] JS：类型检查（JSDoc）
来源：http://oa.gzmigu.cn

/** @param {string} name */ function f(name) {}
来源：http://rf.muxihuayi.cn

[U117] JS：单元测试
来源：http://vn.yuntaijiaju.cn

npm i -D vitest;  npx vitest
来源：http://uc.nszjky.cn

[U118] JS：开发服务器
来源：http://lz.bjjhwx.cn

npm i -D vite;  npx vite
来源：http://to.muxihuayi.cn

[U119] JS：生产构建
来源：http://sf.szsharing.cn

npx vite build
来源：http://id.muxihuayi.cn

[U120] JS：读取环境变量（Vite）
来源：http://wz.yuntaijiaju.cn

import.meta.env.VITE_API_URL
来源：http://wr.asd995.cn

================================================================================
来源：http://df.yuntaijiaju.cn

统计汇总
来源：http://ej.9csxet.cn

================================================================================
来源：http://sf.nszjky.cn

按语言统计（条）：
来源：http://fi.shtwfgs.cn

Python ......... 252
来源：http://tz.jianghongdianzi.cn

PHP ............ 252
来源：http://hd.hahajie.cn

JavaScript ..... 252
来源：http://so.hahajie.cn

TypeScript ..... 212
来源：http://ep.colortex.cn

Java ........... 212
来源：http://wy.nicolike.cn

Go ............. 212
来源：http://jo.9csxet.cn

Ruby ........... 212
来源：http://yq.huanxung.cn

C# ............. 212
来源：http://pn.jianghongdianzi.cn

C .............. 30
来源：http://oc.shxzukj.cn

C++ ............ 30
来源：http://sm.bjjhwx.cn

SQL ............ 90
来源：http://si.szsharing.cn

Bash ........... 80
来源：http://pw.gzmigu.cn

Kotlin ......... 15
来源：http://hf.szxytkj.cn

Swift .......... 15
来源：http://lp.hahajie.cn

Lua ............ 10
来源：http://mt.gzmigu.cn

Perl ........... 10
来源：http://gk.haigaiapp.cn

Scala .......... 10
来源：http://uu.jianghongdianzi.cn

------------------------------------
来源：http://dv.bookmarksfly.cn

合计 ........... 2106 条
来源：http://ji.newstarts.cn

按章节统计：
来源：http://wm.lnxyls.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yf.shtwfgs.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qi.haigaiapp.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xd.szsharing.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lf.yuntaijiaju.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mf.yuexingan06.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nd.szxytkj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xy.bjjhwx.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jx.chemitech.net.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://il.bookmarksfly.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ww.jctech888.com.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gi.521024.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cl.colortex.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zw.huixinmuqiang.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qo.muxihuayi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yl.yuexingan06.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rr.colortex.cn

Q SQL 专题                              90
来源：http://oh.colortex.cn

R Bash 专题                             80
来源：http://nq.asd995.cn

S C / C++ 专题                          60
来源：http://gg.nicolike.cn

T 其他语言补充                          60
来源：http://xn.lnxyls.cn

U 高频实用片段                         120
来源：http://vd.nicolike.cn

------------------------------------
来源：http://ro.nszjky.cn

合计                                  2106 条
来源：http://hj.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://gz.huixiangedu.cn

使用提醒
来源：http://lg.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://kl.chemitech.net.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pa.newstarts.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://iu.521024.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pj.hnjuh.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ic.huixiangedu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://re.szxytkj.cn

—— 文件结束 ——
来源：http://ps.shtwfgs.cn

================================================================================
来源：http://dd.jianghongdianzi.cn

程序语言常见例子速查手册（2024 版）
来源：http://bl.haigaiapp.cn

Common Programming Examples Cheat Book
来源：http://xd.hnjuh.cn

================================================================================
来源：http://qt.asd995.cn

【收录内容】
来源：http://dt.nicolike.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://my.newstarts.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qi.gzmigu.cn

SQL · Bash · C · C++
来源：http://mz.nszjky.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://va.lnxyls.cn

【使用说明】
来源：http://fr.nszjky.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://an.asd995.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ix.huixiangedu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pc.shxzskj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kl.yuntaijiaju.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://il.bjjhwx.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.yuntaijiaju.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jq.jianghongdianzi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dw.lnxyls.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qe.panjiajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mg.asd995.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yk.nicolike.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vr.asd995.cn

【文件统计】
来源：http://hr.chemitech.net.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dh.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://fg.bookmarksfly.cn

目  录
来源：http://bg.newstarts.cn

--------------------------------------------------------------------------------
来源：http://oh.newstarts.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ev.hnjuh.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://yi.chemitech.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://so.colortex.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://np.szsharing.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://eh.huanxung.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yg.chemitech.net.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dh.nicolike.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tb.huixinmuqiang.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bb.jianghongdianzi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://sd.huanxung.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ei.haigaiapp.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cr.jctech888.com.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ha.bjjhwx.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wi.521024.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xv.szxytkj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bg.hnjuh.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xw.nicolike.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://dn.huanxung.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rv.haigaiapp.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ir.gzmigu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lh.nicolike.cn

================================================================================
来源：http://zv.muxihuayi.cn

A. 基础语法与类型
来源：http://rn.szsharing.cn

================================================================================
来源：http://nv.gzmigu.cn

[A01] Hello World
来源：http://dh.lnxyls.cn

Py:   print("Hello, World!")
来源：http://ud.yuntaijiaju.cn

PHP:  echo "Hello, World!";
来源：http://lt.huanxung.cn

JS:   console.log("Hello, World!");
来源：http://jq.shtwfgs.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ls.521024.cn

Java: System.out.println("Hello, World!");
来源：http://hu.bookmarksfly.cn

Go:   fmt.Println("Hello, World!")
来源：http://au.colortex.cn

Ruby: puts "Hello, World!"
来源：http://eg.9csxet.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://cc.szsharing.cn

[A02] 变量声明与赋值
来源：http://ju.jctech888.com.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nj.gzmigu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://mm.bookmarksfly.cn

JS:   let name = "Alex"; const age = 20;
来源：http://if.9csxet.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://za.hahajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://kr.hahajie.cn

Go:   name := "Alex"; age := 20
来源：http://ez.huixiangedu.cn

Ruby: name = "Alex"; age = 20
来源：http://jg.wgjwhj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://sa.9csxet.cn

[A03] 常量定义
来源：http://uz.huixinmuqiang.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nj.lnxyls.cn

PHP:  const PI = 3.14159;
来源：http://ea.szxytkj.cn

JS:   const PI = 3.14159;
来源：http://iq.panjiajie.cn

TS:   const PI: number = 3.14159;
来源：http://df.521024.cn

Java: static final double PI = 3.14159;
来源：http://cy.newstarts.cn

Go:   const PI = 3.14159
来源：http://kb.hnjuh.cn

Ruby: PI = 3.14159
来源：http://wm.shxzukj.cn

C#:   const double PI = 3.14159;
来源：http://kn.huanxung.cn

[A04] 判断变量类型
来源：http://wp.jianghongdianzi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://rq.yuexingan06.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qe.asd995.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nk.shtwfgs.cn

TS:   typeof x; x instanceof Date
来源：http://vn.muxihuayi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ll.jctech888.com.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ps.yuntaijiaju.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://zk.nicolike.cn

C#:   x.GetType().Name; x is int
来源：http://fi.nszjky.cn

[A05] 整数除法与取模
来源：http://er.wgjwhj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ow.haigaiapp.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zo.wgjwhj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bn.huixiangedu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qq.szsharing.cn

Java: 7 / 2; 7 % 2
来源：http://is.shxzskj.cn

Go:   7 / 2; 7 % 2
来源：http://cd.shxzskj.cn

Ruby: 7 / 2; 7 % 2
来源：http://dw.szsharing.cn

C#:   7 / 2; 7 % 2
来源：http://cq.gzmigu.cn

[A06] 字符串转数字
来源：http://zw.bjjhwx.cn

Py:   int("42"); float("3.14")
来源：http://lj.shxzukj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vi.newstarts.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ug.lnxyls.cn

TS:   parseInt("42", 10); Number("42")
来源：http://pb.hnjuh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://du.nszjky.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://oe.yuexingan06.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fy.bjjhwx.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qg.shxzukj.cn

[A07] 数字转字符串
来源：http://ha.yuexingan06.cn

Py:   str(42)
来源：http://iz.yuntaijiaju.cn

PHP:  (string) 42; strval(42)
来源：http://dm.panjiajie.cn

JS:   String(42); (42).toString()
来源：http://cg.hnjuh.cn

TS:   String(42)
来源：http://tq.asd995.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://sy.newstarts.cn

Go:   strconv.Itoa(42)
来源：http://um.yuntaijiaju.cn

Ruby: 42.to_s
来源：http://ck.newstarts.cn

C#:   42.ToString()
来源：http://ws.9csxet.cn

[A08] 取整与四舍五入
来源：http://hr.yuexingan06.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hu.hahajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ha.gzmigu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://up.colortex.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://oq.nicolike.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pv.hahajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://do.hahajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fi.nicolike.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gu.nszjky.cn

[A09] 绝对值与最大最小值
来源：http://vm.huixinmuqiang.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zy.huanxung.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://my.shtwfgs.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pc.chemitech.net.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ko.shxzskj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://za.521024.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gl.huixinmuqiang.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jx.shxzukj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lk.colortex.cn

[A10] 生成随机数
来源：http://ky.shxzukj.cn

Py:   import random; random.randint(1, 100)
来源：http://ax.asd995.cn

PHP:  random_int(1, 100);
来源：http://ec.wgjwhj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://an.haigaiapp.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lw.huanxung.cn

Java: new Random().nextInt(100) + 1
来源：http://ef.asd995.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kl.jctech888.com.cn

Ruby: rand(1..100)
来源：http://tu.lnxyls.cn

C#:   new Random().Next(1, 101)
来源：http://kf.szxytkj.cn

[A11] 条件表达式（三元）
来源：http://yc.chemitech.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://df.shxzskj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://am.shtwfgs.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ei.szxytkj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://hd.nicolike.cn

Java: x > 0 ? "yes" : "no"
来源：http://ar.szsharing.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hg.huixinmuqiang.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://kf.yuntaijiaju.cn

C#:   x > 0 ? "yes" : "no"
来源：http://qu.szsharing.cn

[A12] 字符串插值 / 格式化
来源：http://jx.shxzskj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://te.bjjhwx.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mh.asd995.cn

JS:   `Hello, ${name}!`
来源：http://ez.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://bp.lnxyls.cn

Java: "Hello, %s!".formatted(name)
来源：http://ku.chemitech.net.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zr.huixiangedu.cn

Ruby: "Hello, #{name}!"
来源：http://lt.hahajie.cn

C#:   $"Hello, {name}!"
来源：http://pz.bookmarksfly.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://od.yuexingan06.cn

Py:   "第一行\n第二行"
来源：http://vj.muxihuayi.cn

PHP:  "第一行\n第二行"
来源：http://fw.9csxet.cn

JS:   "第一行\n第二行"
来源：http://cn.szsharing.cn

TS:   "第一行\n第二行"
来源：http://lz.haigaiapp.cn

Java: "第一行\n第二行"
来源：http://wt.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://nu.jctech888.com.cn

Ruby: "第一行\n第二行"
来源：http://wk.lnxyls.cn

C#:   "第一行\n第二行"
来源：http://fn.chemitech.net.cn

[A14] 注释写法
来源：http://fs.hahajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gi.huanxung.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xa.jctech888.com.cn

JS:   // 单行；/* 多行 */
来源：http://oc.newstarts.cn

TS:   // 单行；/* 多行 */
来源：http://nd.521024.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pm.shxzukj.cn

Go:   // 单行；/* 多行 */
来源：http://ot.nszjky.cn

Ruby: # 单行；=begin 多行 =end
来源：http://io.huixinmuqiang.cn

C#:   // 单行；/* 多行 */
来源：http://av.haigaiapp.cn

[A15] 空值判断与默认值
来源：http://es.yuntaijiaju.cn

Py:   value = data or "默认值"
来源：http://rm.colortex.cn

PHP:  $value = $data ?? "默认值";
来源：http://st.chemitech.net.cn

JS:   const value = data ?? "默认值";
来源：http://vk.asd995.cn

TS:   const value = data ?? "默认值";
来源：http://cx.haigaiapp.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vr.huixiangedu.cn

Go:   if data == "" { data = "默认值" }
来源：http://qo.wgjwhj.cn


<!-- 参考信息 -->