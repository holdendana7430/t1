代发 wailian999

[U89] JS：数组去重
来源：http://br.asd995.cn

[...new Set(arr)]
来源：http://fo.hnjuh.cn

[U90] JS：数字数组排序
来源：http://ci.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://wb.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://nr.szsharing.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zn.jctech888.com.cn

[U92] JS：深拷贝
来源：http://co.huixiangedu.cn

structuredClone(obj)
来源：http://rq.jctech888.com.cn

[U93] JS：模板字符串
来源：http://yg.shtwfgs.cn

`共 ${n} 条`
来源：http://oa.yuexingan06.cn

[U94] JS：箭头函数
来源：http://cc.bjjhwx.cn

const double = x => x * 2;
来源：http://br.shxzukj.cn

[U95] JS：Promise 包装
来源：http://ik.gzmigu.cn

new Promise((resolve, reject) => {})
来源：http://tc.huanxung.cn

[U96] JS：async/await 与异常
来源：http://sj.huanxung.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uy.nszjky.cn

[U97] JS：并发请求
来源：http://kw.jctech888.com.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://np.haigaiapp.cn

[U98] JS：fetch 带 JSON
来源：http://fz.gzmigu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://to.hahajie.cn

[U99] JS：事件监听
来源：http://rn.haigaiapp.cn

el.addEventListener("click", e => {})
来源：http://qj.haigaiapp.cn

[U100] JS：DOM 查询
来源：http://jo.muxihuayi.cn

document.querySelector(".item")
来源：http://xm.jianghongdianzi.cn

[U101] JS：classList 操作
来源：http://lu.bookmarksfly.cn

el.classList.toggle("active")
来源：http://un.szxytkj.cn

[U102] JS：本地存储
来源：http://ye.szsharing.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xy.hahajie.cn

[U103] JS：定时器
来源：http://el.nszjky.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zi.shxzukj.cn

[U104] JS：防抖
来源：http://gx.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tc.shxzukj.cn

[U105] JS：节流
来源：http://rd.jianghongdianzi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rp.hnjuh.cn

[U106] JS：日期格式化
来源：http://pm.haigaiapp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mc.nszjky.cn

[U107] JS：数字千分位
来源：http://fe.shxzukj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dw.jianghongdianzi.cn

[U108] JS：随机整数
来源：http://gt.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uw.colortex.cn

[U109] JS：数组分组
来源：http://fz.521024.cn

Object.groupBy(arr, x => x.type)
来源：http://qv.yuexingan06.cn

[U110] JS：数组分块
来源：http://ak.gzmigu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://px.nszjky.cn

[U111] JS：对象转 Map
来源：http://rt.lnxyls.cn

new Map(Object.entries(obj))
来源：http://dy.shxzukj.cn

[U112] JS：字符串补位
来源：http://ne.szxytkj.cn

"7".padStart(3, "0")
来源：http://uz.asd995.cn

[U113] JS：正则替换全部
来源：http://ib.szxytkj.cn

s.replaceAll("a", "b")
来源：http://mr.shxzskj.cn

[U114] JS：JSON 深比较
来源：http://du.gzmigu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://aw.colortex.cn

[U115] JS：生成 UUID
来源：http://vv.chemitech.net.cn

crypto.randomUUID()
来源：http://ja.newstarts.cn

[U116] JS：类型检查（JSDoc）
来源：http://pi.bjjhwx.cn

/** @param {string} name */ function f(name) {}
来源：http://qn.nicolike.cn

[U117] JS：单元测试
来源：http://nu.521024.cn

npm i -D vitest;  npx vitest
来源：http://mg.nicolike.cn

[U118] JS：开发服务器
来源：http://tx.9csxet.cn

npm i -D vite;  npx vite
来源：http://hj.bookmarksfly.cn

[U119] JS：生产构建
来源：http://zm.yuexingan06.cn

npx vite build
来源：http://sw.jianghongdianzi.cn

[U120] JS：读取环境变量（Vite）
来源：http://lw.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://il.shxzukj.cn

================================================================================
来源：http://ok.bookmarksfly.cn

统计汇总
来源：http://vk.huixiangedu.cn

================================================================================
来源：http://fn.nicolike.cn

按语言统计（条）：
来源：http://ih.huixiangedu.cn

Python ......... 252
来源：http://gu.jianghongdianzi.cn

PHP ............ 252
来源：http://xx.hahajie.cn

JavaScript ..... 252
来源：http://lb.wgjwhj.cn

TypeScript ..... 212
来源：http://ay.huanxung.cn

Java ........... 212
来源：http://ub.newstarts.cn

Go ............. 212
来源：http://sg.colortex.cn

Ruby ........... 212
来源：http://pl.yuntaijiaju.cn

C# ............. 212
来源：http://xn.huixiangedu.cn

C .............. 30
来源：http://sl.521024.cn

C++ ............ 30
来源：http://yj.hahajie.cn

SQL ............ 90
来源：http://bg.shxzskj.cn

Bash ........... 80
来源：http://da.colortex.cn

Kotlin ......... 15
来源：http://kd.hahajie.cn

Swift .......... 15
来源：http://yk.szsharing.cn

Lua ............ 10
来源：http://ok.huixinmuqiang.cn

Perl ........... 10
来源：http://ps.haigaiapp.cn

Scala .......... 10
来源：http://kg.jctech888.com.cn

------------------------------------
来源：http://el.szxytkj.cn

合计 ........... 2106 条
来源：http://uu.jctech888.com.cn

按章节统计：
来源：http://as.panjiajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wm.shxzskj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bw.nszjky.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bt.jctech888.com.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yz.bjjhwx.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gh.hahajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://di.bookmarksfly.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dr.shxzukj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pi.muxihuayi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mp.hahajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://aa.shxzukj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zo.wgjwhj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dy.shtwfgs.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yl.yuexingan06.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ge.hnjuh.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://od.szsharing.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://as.chemitech.net.cn

Q SQL 专题                              90
来源：http://xp.9csxet.cn

R Bash 专题                             80
来源：http://gq.shxzukj.cn

S C / C++ 专题                          60
来源：http://tf.haigaiapp.cn

T 其他语言补充                          60
来源：http://no.muxihuayi.cn

U 高频实用片段                         120
来源：http://ax.shxzukj.cn

------------------------------------
来源：http://rn.asd995.cn

合计                                  2106 条
来源：http://jn.huanxung.cn

--------------------------------------------------------------------------------
来源：http://gk.yuexingan06.cn

使用提醒
来源：http://kd.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://cn.wgjwhj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://eb.shtwfgs.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xz.hahajie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lx.nszjky.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ks.9csxet.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wa.nicolike.cn

—— 文件结束 ——
来源：http://is.shxzskj.cn

================================================================================
来源：http://fy.colortex.cn

程序语言常见例子速查手册（2024 版）
来源：http://rv.nicolike.cn

Common Programming Examples Cheat Book
来源：http://fv.newstarts.cn

================================================================================
来源：http://yl.panjiajie.cn

【收录内容】
来源：http://uj.jctech888.com.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://xv.hnjuh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vr.521024.cn

SQL · Bash · C · C++
来源：http://me.wgjwhj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ua.521024.cn

【使用说明】
来源：http://ja.yuntaijiaju.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cw.asd995.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vh.lnxyls.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://un.szxytkj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ml.nicolike.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qi.shtwfgs.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mw.nszjky.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xt.colortex.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vl.szsharing.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kv.yuexingan06.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ie.hnjuh.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ta.shtwfgs.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yb.bookmarksfly.cn

【文件统计】
来源：http://ja.nszjky.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nx.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://ol.szsharing.cn

目  录
来源：http://tt.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://yg.yuexingan06.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vz.huixinmuqiang.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cb.huanxung.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qk.szxytkj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kx.bjjhwx.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ly.muxihuayi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jx.huixiangedu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fm.hnjuh.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ur.chemitech.net.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qi.huanxung.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ae.lnxyls.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://he.yuexingan06.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jb.gzmigu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://uc.jctech888.com.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gx.jianghongdianzi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wv.yuexingan06.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fl.jctech888.com.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bp.wgjwhj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ek.bjjhwx.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://er.lnxyls.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pl.asd995.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ey.szsharing.cn

================================================================================
来源：http://wb.muxihuayi.cn

A. 基础语法与类型
来源：http://wo.huanxung.cn

================================================================================
来源：http://tk.yuexingan06.cn

[A01] Hello World
来源：http://tw.muxihuayi.cn

Py:   print("Hello, World!")
来源：http://bj.huixiangedu.cn

PHP:  echo "Hello, World!";
来源：http://iq.shtwfgs.cn

JS:   console.log("Hello, World!");
来源：http://vj.nszjky.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fz.asd995.cn

Java: System.out.println("Hello, World!");
来源：http://sa.jianghongdianzi.cn

Go:   fmt.Println("Hello, World!")
来源：http://fw.asd995.cn

Ruby: puts "Hello, World!"
来源：http://ac.gzmigu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jb.bookmarksfly.cn

[A02] 变量声明与赋值
来源：http://se.bookmarksfly.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mc.muxihuayi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://gt.bjjhwx.cn

JS:   let name = "Alex"; const age = 20;
来源：http://bp.newstarts.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bu.yuntaijiaju.cn

Java: String name = "Alex"; int age = 20;
来源：http://ni.muxihuayi.cn

Go:   name := "Alex"; age := 20
来源：http://we.lnxyls.cn

Ruby: name = "Alex"; age = 20
来源：http://tz.muxihuayi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ld.nszjky.cn

[A03] 常量定义
来源：http://vu.asd995.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kr.hnjuh.cn

PHP:  const PI = 3.14159;
来源：http://hx.chemitech.net.cn

JS:   const PI = 3.14159;
来源：http://zy.lnxyls.cn

TS:   const PI: number = 3.14159;
来源：http://ob.wgjwhj.cn

Java: static final double PI = 3.14159;
来源：http://ne.lnxyls.cn

Go:   const PI = 3.14159
来源：http://lc.521024.cn

Ruby: PI = 3.14159
来源：http://rb.521024.cn

C#:   const double PI = 3.14159;
来源：http://ei.9csxet.cn

[A04] 判断变量类型
来源：http://up.muxihuayi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vh.nicolike.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ku.lnxyls.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ui.bjjhwx.cn

TS:   typeof x; x instanceof Date
来源：http://zn.lnxyls.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://la.asd995.cn

Go:   reflect.TypeOf(x).Name()
来源：http://op.bookmarksfly.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://hm.bjjhwx.cn

C#:   x.GetType().Name; x is int
来源：http://sp.szsharing.cn

[A05] 整数除法与取模
来源：http://mb.colortex.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cd.hahajie.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://do.hahajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yt.asd995.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hw.haigaiapp.cn

Java: 7 / 2; 7 % 2
来源：http://lt.huanxung.cn

Go:   7 / 2; 7 % 2
来源：http://nx.shxzukj.cn

Ruby: 7 / 2; 7 % 2
来源：http://aa.colortex.cn

C#:   7 / 2; 7 % 2
来源：http://by.yuntaijiaju.cn

[A06] 字符串转数字
来源：http://cu.huixiangedu.cn

Py:   int("42"); float("3.14")
来源：http://jc.hahajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pq.shxzskj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dl.huixinmuqiang.cn

TS:   parseInt("42", 10); Number("42")
来源：http://bb.nszjky.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://eh.huixinmuqiang.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pm.lnxyls.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zx.nicolike.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://we.szxytkj.cn

[A07] 数字转字符串
来源：http://ii.szxytkj.cn

Py:   str(42)
来源：http://ha.colortex.cn

PHP:  (string) 42; strval(42)
来源：http://bl.jctech888.com.cn

JS:   String(42); (42).toString()
来源：http://xg.colortex.cn

TS:   String(42)
来源：http://bu.hahajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zi.yuexingan06.cn

Go:   strconv.Itoa(42)
来源：http://jp.521024.cn

Ruby: 42.to_s
来源：http://xp.szsharing.cn

C#:   42.ToString()
来源：http://fm.lnxyls.cn

[A08] 取整与四舍五入
来源：http://my.szsharing.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://me.nicolike.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nb.wgjwhj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ut.hnjuh.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qk.haigaiapp.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jr.nszjky.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kn.521024.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://lq.muxihuayi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fe.wgjwhj.cn

[A09] 绝对值与最大最小值
来源：http://ni.szsharing.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xm.hahajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://al.szxytkj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ct.huixinmuqiang.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fq.shxzskj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mh.szxytkj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wa.shxzskj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ix.panjiajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ht.yuexingan06.cn

[A10] 生成随机数
来源：http://nc.lnxyls.cn

Py:   import random; random.randint(1, 100)
来源：http://kw.muxihuayi.cn

PHP:  random_int(1, 100);
来源：http://uh.bookmarksfly.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xa.shxzukj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fa.huanxung.cn

Java: new Random().nextInt(100) + 1
来源：http://cz.bjjhwx.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://di.gzmigu.cn

Ruby: rand(1..100)
来源：http://xg.asd995.cn

C#:   new Random().Next(1, 101)
来源：http://iz.9csxet.cn

[A11] 条件表达式（三元）
来源：http://lq.bookmarksfly.cn

Py:   "yes" if x > 0 else "no"
来源：http://hm.9csxet.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ei.szsharing.cn

JS:   x > 0 ? "yes" : "no"
来源：http://wq.chemitech.net.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ud.chemitech.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://bv.hnjuh.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://gk.haigaiapp.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://tx.yuexingan06.cn

C#:   x > 0 ? "yes" : "no"
来源：http://tz.asd995.cn

[A12] 字符串插值 / 格式化
来源：http://mm.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ur.shtwfgs.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ks.asd995.cn

JS:   `Hello, ${name}!`
来源：http://kg.9csxet.cn

TS:   `Hello, ${name}!`
来源：http://vj.nicolike.cn

Java: "Hello, %s!".formatted(name)
来源：http://bs.521024.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ot.chemitech.net.cn

Ruby: "Hello, #{name}!"
来源：http://jy.huanxung.cn

C#:   $"Hello, {name}!"
来源：http://ei.chemitech.net.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://tc.huixinmuqiang.cn

Py:   "第一行\n第二行"
来源：http://gf.colortex.cn

PHP:  "第一行\n第二行"
来源：http://zw.szxytkj.cn

JS:   "第一行\n第二行"
来源：http://io.jianghongdianzi.cn

TS:   "第一行\n第二行"
来源：http://gq.szsharing.cn

Java: "第一行\n第二行"
来源：http://lr.shxzskj.cn

Go:   "第一行\n第二行"
来源：http://iw.hahajie.cn

Ruby: "第一行\n第二行"
来源：http://uj.yuexingan06.cn

C#:   "第一行\n第二行"
来源：http://la.nszjky.cn

[A14] 注释写法
来源：http://yg.newstarts.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://jc.jianghongdianzi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ve.9csxet.cn

JS:   // 单行；/* 多行 */
来源：http://be.shtwfgs.cn

TS:   // 单行；/* 多行 */
来源：http://jr.bookmarksfly.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cu.newstarts.cn

Go:   // 单行；/* 多行 */
来源：http://hk.szxytkj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://va.colortex.cn

C#:   // 单行；/* 多行 */
来源：http://gl.haigaiapp.cn

[A15] 空值判断与默认值
来源：http://vo.hahajie.cn

Py:   value = data or "默认值"
来源：http://ky.bookmarksfly.cn

PHP:  $value = $data ?? "默认值";
来源：http://vs.szxytkj.cn


<!-- 参考信息 -->