代发 wailian999

[U89] JS：数组去重
来源：http://fe.nszjky.cn

[...new Set(arr)]
来源：http://md.jianghongdianzi.cn

[U90] JS：数字数组排序
来源：http://zm.chemitech.net.cn

[...arr].sort((a, b) => a - b)
来源：http://nv.huixiangedu.cn

[U91] JS：对象键值遍历
来源：http://qo.huixiangedu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yu.shxzukj.cn

[U92] JS：深拷贝
来源：http://ga.huixinmuqiang.cn

structuredClone(obj)
来源：http://cp.muxihuayi.cn

[U93] JS：模板字符串
来源：http://bk.521024.cn

`共 ${n} 条`
来源：http://ge.bookmarksfly.cn

[U94] JS：箭头函数
来源：http://oq.hahajie.cn

const double = x => x * 2;
来源：http://bb.szsharing.cn

[U95] JS：Promise 包装
来源：http://gi.bookmarksfly.cn

new Promise((resolve, reject) => {})
来源：http://ft.panjiajie.cn

[U96] JS：async/await 与异常
来源：http://df.wgjwhj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://en.wgjwhj.cn

[U97] JS：并发请求
来源：http://ly.9csxet.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://or.bookmarksfly.cn

[U98] JS：fetch 带 JSON
来源：http://uz.521024.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yf.huixiangedu.cn

[U99] JS：事件监听
来源：http://hq.hahajie.cn

el.addEventListener("click", e => {})
来源：http://zu.bookmarksfly.cn

[U100] JS：DOM 查询
来源：http://sh.shxzukj.cn

document.querySelector(".item")
来源：http://yc.huixinmuqiang.cn

[U101] JS：classList 操作
来源：http://cu.shxzskj.cn

el.classList.toggle("active")
来源：http://vf.yuexingan06.cn

[U102] JS：本地存储
来源：http://gz.shtwfgs.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://uj.chemitech.net.cn

[U103] JS：定时器
来源：http://sf.9csxet.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://oc.shtwfgs.cn

[U104] JS：防抖
来源：http://zr.huixinmuqiang.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sn.huanxung.cn

[U105] JS：节流
来源：http://gg.chemitech.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zl.asd995.cn

[U106] JS：日期格式化
来源：http://ii.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mf.muxihuayi.cn

[U107] JS：数字千分位
来源：http://od.colortex.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jj.panjiajie.cn

[U108] JS：随机整数
来源：http://bz.shxzskj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qu.newstarts.cn

[U109] JS：数组分组
来源：http://jo.nicolike.cn

Object.groupBy(arr, x => x.type)
来源：http://ef.shxzskj.cn

[U110] JS：数组分块
来源：http://wm.asd995.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ez.nicolike.cn

[U111] JS：对象转 Map
来源：http://ep.521024.cn

new Map(Object.entries(obj))
来源：http://ec.nicolike.cn

[U112] JS：字符串补位
来源：http://cm.shxzskj.cn

"7".padStart(3, "0")
来源：http://uh.jctech888.com.cn

[U113] JS：正则替换全部
来源：http://qw.hahajie.cn

s.replaceAll("a", "b")
来源：http://gy.nszjky.cn

[U114] JS：JSON 深比较
来源：http://ez.shtwfgs.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://uq.bjjhwx.cn

[U115] JS：生成 UUID
来源：http://xe.yuexingan06.cn

crypto.randomUUID()
来源：http://im.szsharing.cn

[U116] JS：类型检查（JSDoc）
来源：http://dn.nicolike.cn

/** @param {string} name */ function f(name) {}
来源：http://kj.jctech888.com.cn

[U117] JS：单元测试
来源：http://qu.jianghongdianzi.cn

npm i -D vitest;  npx vitest
来源：http://ro.shxzukj.cn

[U118] JS：开发服务器
来源：http://hg.bjjhwx.cn

npm i -D vite;  npx vite
来源：http://dy.hnjuh.cn

[U119] JS：生产构建
来源：http://wh.hahajie.cn

npx vite build
来源：http://xt.nicolike.cn

[U120] JS：读取环境变量（Vite）
来源：http://ew.haigaiapp.cn

import.meta.env.VITE_API_URL
来源：http://um.muxihuayi.cn

================================================================================
来源：http://fe.hahajie.cn

统计汇总
来源：http://sr.asd995.cn

================================================================================
来源：http://wu.bjjhwx.cn

按语言统计（条）：
来源：http://qu.haigaiapp.cn

Python ......... 252
来源：http://uz.jianghongdianzi.cn

PHP ............ 252
来源：http://ug.shxzukj.cn

JavaScript ..... 252
来源：http://gl.bjjhwx.cn

TypeScript ..... 212
来源：http://gm.bookmarksfly.cn

Java ........... 212
来源：http://ry.hahajie.cn

Go ............. 212
来源：http://ip.jianghongdianzi.cn

Ruby ........... 212
来源：http://ly.yuntaijiaju.cn

C# ............. 212
来源：http://ig.asd995.cn

C .............. 30
来源：http://gx.haigaiapp.cn

C++ ............ 30
来源：http://ge.nicolike.cn

SQL ............ 90
来源：http://um.panjiajie.cn

Bash ........... 80
来源：http://zh.panjiajie.cn

Kotlin ......... 15
来源：http://fl.haigaiapp.cn

Swift .......... 15
来源：http://uu.szsharing.cn

Lua ............ 10
来源：http://kl.jctech888.com.cn

Perl ........... 10
来源：http://uh.szsharing.cn

Scala .......... 10
来源：http://io.nszjky.cn

------------------------------------
来源：http://br.chemitech.net.cn

合计 ........... 2106 条
来源：http://yk.asd995.cn

按章节统计：
来源：http://hk.nicolike.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cm.szxytkj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tf.nicolike.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jc.yuntaijiaju.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kc.hnjuh.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rq.panjiajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lo.asd995.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dt.huixinmuqiang.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cp.huixinmuqiang.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sb.bjjhwx.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jc.shxzskj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yo.yuntaijiaju.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ru.nicolike.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ra.hnjuh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rg.huanxung.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://da.nszjky.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pi.shxzskj.cn

Q SQL 专题                              90
来源：http://tg.chemitech.net.cn

R Bash 专题                             80
来源：http://ox.asd995.cn

S C / C++ 专题                          60
来源：http://gc.shtwfgs.cn

T 其他语言补充                          60
来源：http://lw.nicolike.cn

U 高频实用片段                         120
来源：http://az.wgjwhj.cn

------------------------------------
来源：http://wn.shtwfgs.cn

合计                                  2106 条
来源：http://ca.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://iz.muxihuayi.cn

使用提醒
来源：http://tt.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://ag.huanxung.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bk.huixinmuqiang.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gv.nicolike.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bu.szsharing.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://bu.shxzskj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ca.huixinmuqiang.cn

—— 文件结束 ——
来源：http://jz.asd995.cn

================================================================================
来源：http://ey.jianghongdianzi.cn

程序语言常见例子速查手册（2024 版）
来源：http://wm.huixiangedu.cn

Common Programming Examples Cheat Book
来源：http://by.9csxet.cn

================================================================================
来源：http://be.newstarts.cn

【收录内容】
来源：http://au.521024.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://iy.shtwfgs.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cc.huanxung.cn

SQL · Bash · C · C++
来源：http://qr.9csxet.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ow.shtwfgs.cn

【使用说明】
来源：http://zm.nicolike.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qj.521024.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rr.hahajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tc.wgjwhj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bx.huixiangedu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://zx.wgjwhj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rn.asd995.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gu.szxytkj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ah.szxytkj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uh.huanxung.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ub.newstarts.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://su.chemitech.net.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zr.bjjhwx.cn

【文件统计】
来源：http://ld.wgjwhj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mu.521024.cn

--------------------------------------------------------------------------------
来源：http://ns.bjjhwx.cn

目  录
来源：http://fs.nszjky.cn

--------------------------------------------------------------------------------
来源：http://jt.panjiajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rc.szxytkj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jm.haigaiapp.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dm.hnjuh.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bk.chemitech.net.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pw.szsharing.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://of.yuntaijiaju.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://iu.asd995.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qc.huixinmuqiang.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ys.huixinmuqiang.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xo.wgjwhj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://uc.shtwfgs.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pf.chemitech.net.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rh.asd995.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lh.9csxet.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ys.nszjky.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://oq.lnxyls.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gn.muxihuayi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://fc.haigaiapp.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ov.jctech888.com.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rd.521024.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dn.wgjwhj.cn

================================================================================
来源：http://xn.shtwfgs.cn

A. 基础语法与类型
来源：http://dt.jianghongdianzi.cn

================================================================================
来源：http://et.colortex.cn

[A01] Hello World
来源：http://mq.521024.cn

Py:   print("Hello, World!")
来源：http://dp.gzmigu.cn

PHP:  echo "Hello, World!";
来源：http://fz.huixiangedu.cn

JS:   console.log("Hello, World!");
来源：http://ik.haigaiapp.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nz.hnjuh.cn

Java: System.out.println("Hello, World!");
来源：http://qq.huanxung.cn

Go:   fmt.Println("Hello, World!")
来源：http://ot.nszjky.cn

Ruby: puts "Hello, World!"
来源：http://xx.nszjky.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://hj.9csxet.cn

[A02] 变量声明与赋值
来源：http://av.yuexingan06.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bb.shxzukj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ok.chemitech.net.cn

JS:   let name = "Alex"; const age = 20;
来源：http://bg.yuexingan06.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ux.bjjhwx.cn

Java: String name = "Alex"; int age = 20;
来源：http://se.bookmarksfly.cn

Go:   name := "Alex"; age := 20
来源：http://lw.wgjwhj.cn

Ruby: name = "Alex"; age = 20
来源：http://sf.huixinmuqiang.cn

C#:   string name = "Alex"; int age = 20;
来源：http://yb.shxzskj.cn

[A03] 常量定义
来源：http://ap.jctech888.com.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tp.yuntaijiaju.cn

PHP:  const PI = 3.14159;
来源：http://zc.9csxet.cn

JS:   const PI = 3.14159;
来源：http://cx.521024.cn

TS:   const PI: number = 3.14159;
来源：http://uu.gzmigu.cn

Java: static final double PI = 3.14159;
来源：http://tf.shxzukj.cn

Go:   const PI = 3.14159
来源：http://kg.yuexingan06.cn

Ruby: PI = 3.14159
来源：http://ke.newstarts.cn

C#:   const double PI = 3.14159;
来源：http://op.bookmarksfly.cn

[A04] 判断变量类型
来源：http://kt.nicolike.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ej.wgjwhj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qa.haigaiapp.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ev.wgjwhj.cn

TS:   typeof x; x instanceof Date
来源：http://rs.yuexingan06.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ph.szsharing.cn

Go:   reflect.TypeOf(x).Name()
来源：http://wb.yuexingan06.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ja.yuexingan06.cn

C#:   x.GetType().Name; x is int
来源：http://ox.shxzukj.cn

[A05] 整数除法与取模
来源：http://zo.yuntaijiaju.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wr.9csxet.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ib.colortex.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bt.shxzskj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tv.nicolike.cn

Java: 7 / 2; 7 % 2
来源：http://mm.huixiangedu.cn

Go:   7 / 2; 7 % 2
来源：http://xd.szxytkj.cn

Ruby: 7 / 2; 7 % 2
来源：http://mo.bookmarksfly.cn

C#:   7 / 2; 7 % 2
来源：http://fe.huixinmuqiang.cn

[A06] 字符串转数字
来源：http://ly.huixinmuqiang.cn

Py:   int("42"); float("3.14")
来源：http://bd.chemitech.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ye.shxzskj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dy.gzmigu.cn

TS:   parseInt("42", 10); Number("42")
来源：http://un.bookmarksfly.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pc.bookmarksfly.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fl.jianghongdianzi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fg.wgjwhj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wk.bjjhwx.cn

[A07] 数字转字符串
来源：http://zs.asd995.cn

Py:   str(42)
来源：http://jr.chemitech.net.cn

PHP:  (string) 42; strval(42)
来源：http://oo.newstarts.cn

JS:   String(42); (42).toString()
来源：http://vy.nszjky.cn

TS:   String(42)
来源：http://rd.colortex.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vd.gzmigu.cn

Go:   strconv.Itoa(42)
来源：http://qp.521024.cn

Ruby: 42.to_s
来源：http://ye.nicolike.cn

C#:   42.ToString()
来源：http://gn.bookmarksfly.cn

[A08] 取整与四舍五入
来源：http://ie.haigaiapp.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cm.wgjwhj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lo.huixinmuqiang.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zh.huixinmuqiang.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://li.huanxung.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xn.bjjhwx.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://js.hahajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mz.wgjwhj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gn.shxzukj.cn

[A09] 绝对值与最大最小值
来源：http://ae.bjjhwx.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ai.shxzskj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hc.colortex.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vy.hnjuh.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ef.shtwfgs.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gt.9csxet.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yy.newstarts.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://aw.shxzskj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zb.shxzukj.cn

[A10] 生成随机数
来源：http://kb.muxihuayi.cn

Py:   import random; random.randint(1, 100)
来源：http://tw.bjjhwx.cn

PHP:  random_int(1, 100);
来源：http://uo.nszjky.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://st.9csxet.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nk.nszjky.cn

Java: new Random().nextInt(100) + 1
来源：http://wr.jianghongdianzi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lr.nicolike.cn

Ruby: rand(1..100)
来源：http://rr.bookmarksfly.cn

C#:   new Random().Next(1, 101)
来源：http://hs.szsharing.cn

[A11] 条件表达式（三元）
来源：http://fw.nicolike.cn

Py:   "yes" if x > 0 else "no"
来源：http://qd.szsharing.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://kf.asd995.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ta.lnxyls.cn

TS:   x > 0 ? "yes" : "no"
来源：http://yw.yuexingan06.cn

Java: x > 0 ? "yes" : "no"
来源：http://fo.jctech888.com.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ip.yuexingan06.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pl.shtwfgs.cn

C#:   x > 0 ? "yes" : "no"
来源：http://wg.hnjuh.cn

[A12] 字符串插值 / 格式化
来源：http://ca.newstarts.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://il.asd995.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vx.asd995.cn

JS:   `Hello, ${name}!`
来源：http://qo.jctech888.com.cn

TS:   `Hello, ${name}!`
来源：http://oj.asd995.cn

Java: "Hello, %s!".formatted(name)
来源：http://cq.chemitech.net.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yx.gzmigu.cn

Ruby: "Hello, #{name}!"
来源：http://rm.bjjhwx.cn

C#:   $"Hello, {name}!"
来源：http://xv.jianghongdianzi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://cp.shtwfgs.cn

Py:   "第一行\n第二行"
来源：http://yu.bookmarksfly.cn

PHP:  "第一行\n第二行"
来源：http://eq.muxihuayi.cn

JS:   "第一行\n第二行"
来源：http://jm.szxytkj.cn

TS:   "第一行\n第二行"
来源：http://if.shxzskj.cn

Java: "第一行\n第二行"
来源：http://ic.shxzukj.cn

Go:   "第一行\n第二行"
来源：http://ug.yuntaijiaju.cn

Ruby: "第一行\n第二行"
来源：http://vt.jianghongdianzi.cn

C#:   "第一行\n第二行"
来源：http://hz.haigaiapp.cn

[A14] 注释写法
来源：http://tn.hnjuh.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://il.wgjwhj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hf.newstarts.cn

JS:   // 单行；/* 多行 */
来源：http://xh.huanxung.cn

TS:   // 单行；/* 多行 */
来源：http://te.yuexingan06.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mm.bjjhwx.cn

Go:   // 单行；/* 多行 */
来源：http://og.shxzskj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://as.shxzukj.cn

C#:   // 单行；/* 多行 */
来源：http://px.huixinmuqiang.cn

[A15] 空值判断与默认值
来源：http://vr.9csxet.cn

Py:   value = data or "默认值"
来源：http://fp.lnxyls.cn

PHP:  $value = $data ?? "默认值";
来源：http://qc.huixiangedu.cn


<!-- 参考信息 -->