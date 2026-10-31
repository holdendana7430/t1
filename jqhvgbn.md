代发 wailian999

[U77] PHP：模板渲染
来源：http://zz.shxzskj.cn

composer require twig/twig
来源：http://zx.jctech888.com.cn

[U78] PHP：单元测试
来源：http://bn.hahajie.cn

composer require --dev phpunit/phpunit
来源：http://en.yuntaijiaju.cn

[U79] PHP：静态分析
来源：http://wi.haigaiapp.cn

composer require --dev phpstan/phpstan
来源：http://ht.shxzskj.cn

[U80] PHP：代码规范修复
来源：http://zy.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qv.szsharing.cn

[U81] JS：初始化项目
来源：http://qt.szxytkj.cn

npm init -y;  npm i express
来源：http://po.jianghongdianzi.cn

[U82] JS：package.json 脚本
来源：http://he.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qi.bjjhwx.cn

[U83] JS：ES Module 导入导出
来源：http://av.wgjwhj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tv.hahajie.cn

[U84] JS：CommonJS 写法
来源：http://ap.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ez.yuexingan06.cn

[U85] JS：可选链
来源：http://gc.newstarts.cn

a?.b?.c
来源：http://jc.9csxet.cn

[U86] JS：空值合并
来源：http://ei.jianghongdianzi.cn

a ?? b
来源：http://ma.bjjhwx.cn

[U87] JS：解构默认值
来源：http://kq.panjiajie.cn

const { a = 1, b = 2 } = obj;
来源：http://qz.gzmigu.cn

[U88] JS：对象展开合并
来源：http://ya.wgjwhj.cn

{ ...a, ...b }
来源：http://ta.shxzskj.cn

[U89] JS：数组去重
来源：http://yb.szsharing.cn

[...new Set(arr)]
来源：http://on.hnjuh.cn

[U90] JS：数字数组排序
来源：http://ev.haigaiapp.cn

[...arr].sort((a, b) => a - b)
来源：http://bf.bookmarksfly.cn

[U91] JS：对象键值遍历
来源：http://mq.jianghongdianzi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vd.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://iz.jctech888.com.cn

structuredClone(obj)
来源：http://vp.asd995.cn

[U93] JS：模板字符串
来源：http://ky.nicolike.cn

`共 ${n} 条`
来源：http://sh.lnxyls.cn

[U94] JS：箭头函数
来源：http://yo.muxihuayi.cn

const double = x => x * 2;
来源：http://dg.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://sh.szxytkj.cn

new Promise((resolve, reject) => {})
来源：http://qc.panjiajie.cn

[U96] JS：async/await 与异常
来源：http://yj.colortex.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jc.huanxung.cn

[U97] JS：并发请求
来源：http://wu.jianghongdianzi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zn.haigaiapp.cn

[U98] JS：fetch 带 JSON
来源：http://ck.hahajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jh.gzmigu.cn

[U99] JS：事件监听
来源：http://zs.wgjwhj.cn

el.addEventListener("click", e => {})
来源：http://kl.gzmigu.cn

[U100] JS：DOM 查询
来源：http://ku.shxzskj.cn

document.querySelector(".item")
来源：http://ty.bookmarksfly.cn

[U101] JS：classList 操作
来源：http://eo.gzmigu.cn

el.classList.toggle("active")
来源：http://es.wgjwhj.cn

[U102] JS：本地存储
来源：http://ro.hnjuh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hs.asd995.cn

[U103] JS：定时器
来源：http://br.521024.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pn.wgjwhj.cn

[U104] JS：防抖
来源：http://zk.huixiangedu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lq.szxytkj.cn

[U105] JS：节流
来源：http://tx.asd995.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://si.muxihuayi.cn

[U106] JS：日期格式化
来源：http://mb.wgjwhj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pf.huixinmuqiang.cn

[U107] JS：数字千分位
来源：http://xc.hahajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ss.hahajie.cn

[U108] JS：随机整数
来源：http://du.bookmarksfly.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://br.chemitech.net.cn

[U109] JS：数组分组
来源：http://ea.nszjky.cn

Object.groupBy(arr, x => x.type)
来源：http://jl.yuntaijiaju.cn

[U110] JS：数组分块
来源：http://ok.yuexingan06.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pg.colortex.cn

[U111] JS：对象转 Map
来源：http://gg.bookmarksfly.cn

new Map(Object.entries(obj))
来源：http://nv.lnxyls.cn

[U112] JS：字符串补位
来源：http://dj.yuexingan06.cn

"7".padStart(3, "0")
来源：http://ad.521024.cn

[U113] JS：正则替换全部
来源：http://uj.nicolike.cn

s.replaceAll("a", "b")
来源：http://ft.colortex.cn

[U114] JS：JSON 深比较
来源：http://uv.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tf.szxytkj.cn

[U115] JS：生成 UUID
来源：http://fp.szxytkj.cn

crypto.randomUUID()
来源：http://af.colortex.cn

[U116] JS：类型检查（JSDoc）
来源：http://gd.haigaiapp.cn

/** @param {string} name */ function f(name) {}
来源：http://yr.9csxet.cn

[U117] JS：单元测试
来源：http://dv.shxzskj.cn

npm i -D vitest;  npx vitest
来源：http://gy.yuntaijiaju.cn

[U118] JS：开发服务器
来源：http://sb.gzmigu.cn

npm i -D vite;  npx vite
来源：http://tj.colortex.cn

[U119] JS：生产构建
来源：http://rj.jctech888.com.cn

npx vite build
来源：http://jo.huixiangedu.cn

[U120] JS：读取环境变量（Vite）
来源：http://kv.shxzskj.cn

import.meta.env.VITE_API_URL
来源：http://ln.shxzukj.cn

================================================================================
来源：http://ft.huixinmuqiang.cn

统计汇总
来源：http://py.bjjhwx.cn

================================================================================
来源：http://rw.bookmarksfly.cn

按语言统计（条）：
来源：http://fw.huanxung.cn

Python ......... 252
来源：http://ik.muxihuayi.cn

PHP ............ 252
来源：http://au.shtwfgs.cn

JavaScript ..... 252
来源：http://yx.newstarts.cn

TypeScript ..... 212
来源：http://am.huixinmuqiang.cn

Java ........... 212
来源：http://fe.yuntaijiaju.cn

Go ............. 212
来源：http://yt.nszjky.cn

Ruby ........... 212
来源：http://up.asd995.cn

C# ............. 212
来源：http://ux.lnxyls.cn

C .............. 30
来源：http://uh.asd995.cn

C++ ............ 30
来源：http://vq.hnjuh.cn

SQL ............ 90
来源：http://mk.yuexingan06.cn

Bash ........... 80
来源：http://hm.hahajie.cn

Kotlin ......... 15
来源：http://ba.yuexingan06.cn

Swift .......... 15
来源：http://de.jctech888.com.cn

Lua ............ 10
来源：http://fk.nszjky.cn

Perl ........... 10
来源：http://we.jctech888.com.cn

Scala .......... 10
来源：http://ad.colortex.cn

------------------------------------
来源：http://ak.chemitech.net.cn

合计 ........... 2106 条
来源：http://yx.bookmarksfly.cn

按章节统计：
来源：http://ll.huanxung.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ln.muxihuayi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gl.9csxet.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qf.szsharing.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mn.hnjuh.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://iu.haigaiapp.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sd.jianghongdianzi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nx.9csxet.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gi.yuntaijiaju.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ph.haigaiapp.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jf.szsharing.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nd.panjiajie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bq.gzmigu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://oj.hahajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://aa.9csxet.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://em.lnxyls.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gv.shxzskj.cn

Q SQL 专题                              90
来源：http://zc.bjjhwx.cn

R Bash 专题                             80
来源：http://et.hahajie.cn

S C / C++ 专题                          60
来源：http://mj.chemitech.net.cn

T 其他语言补充                          60
来源：http://ti.bjjhwx.cn

U 高频实用片段                         120
来源：http://vu.nicolike.cn

------------------------------------
来源：http://ey.lnxyls.cn

合计                                  2106 条
来源：http://dt.hahajie.cn

--------------------------------------------------------------------------------
来源：http://cz.bookmarksfly.cn

使用提醒
来源：http://xo.colortex.cn

--------------------------------------------------------------------------------
来源：http://vx.colortex.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rf.shxzskj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yt.lnxyls.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sw.colortex.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://am.nszjky.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fm.yuntaijiaju.cn

—— 文件结束 ——
来源：http://pr.yuexingan06.cn

================================================================================
来源：http://tz.nicolike.cn

程序语言常见例子速查手册（2024 版）
来源：http://kz.huixiangedu.cn

Common Programming Examples Cheat Book
来源：http://ep.nszjky.cn

================================================================================
来源：http://ch.shxzukj.cn

【收录内容】
来源：http://dz.nszjky.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rh.szxytkj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gm.szxytkj.cn

SQL · Bash · C · C++
来源：http://if.jianghongdianzi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ko.muxihuayi.cn

【使用说明】
来源：http://jk.huixiangedu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nd.szsharing.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vo.bjjhwx.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ch.jianghongdianzi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hm.bookmarksfly.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://pv.jctech888.com.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ma.newstarts.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zc.shtwfgs.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yu.haigaiapp.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://za.asd995.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vu.haigaiapp.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wj.szsharing.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lg.colortex.cn

【文件统计】
来源：http://wn.wgjwhj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ma.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://nb.521024.cn

目  录
来源：http://oz.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://ph.colortex.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lf.9csxet.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ge.yuexingan06.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kn.muxihuayi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://of.panjiajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fe.lnxyls.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ha.jianghongdianzi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bs.jianghongdianzi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mx.colortex.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qq.shtwfgs.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://sb.521024.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yi.yuntaijiaju.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ie.newstarts.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://up.hnjuh.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pd.szxytkj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gy.bookmarksfly.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gs.colortex.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fq.bookmarksfly.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://si.yuntaijiaju.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qw.colortex.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://sg.newstarts.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yj.chemitech.net.cn

================================================================================
来源：http://uz.shxzskj.cn

A. 基础语法与类型
来源：http://iz.yuntaijiaju.cn

================================================================================
来源：http://ks.jctech888.com.cn

[A01] Hello World
来源：http://qj.chemitech.net.cn

Py:   print("Hello, World!")
来源：http://yj.yuexingan06.cn

PHP:  echo "Hello, World!";
来源：http://rr.hahajie.cn

JS:   console.log("Hello, World!");
来源：http://zg.nszjky.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wn.newstarts.cn

Java: System.out.println("Hello, World!");
来源：http://ue.hnjuh.cn

Go:   fmt.Println("Hello, World!")
来源：http://du.shtwfgs.cn

Ruby: puts "Hello, World!"
来源：http://gh.wgjwhj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://cv.newstarts.cn

[A02] 变量声明与赋值
来源：http://ui.yuexingan06.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bc.wgjwhj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ku.hnjuh.cn

JS:   let name = "Alex"; const age = 20;
来源：http://yc.gzmigu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pq.hnjuh.cn

Java: String name = "Alex"; int age = 20;
来源：http://zq.9csxet.cn

Go:   name := "Alex"; age := 20
来源：http://jo.bookmarksfly.cn

Ruby: name = "Alex"; age = 20
来源：http://kw.szsharing.cn

C#:   string name = "Alex"; int age = 20;
来源：http://pu.gzmigu.cn

[A03] 常量定义
来源：http://vq.wgjwhj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sf.jianghongdianzi.cn

PHP:  const PI = 3.14159;
来源：http://fa.wgjwhj.cn

JS:   const PI = 3.14159;
来源：http://sa.521024.cn

TS:   const PI: number = 3.14159;
来源：http://hq.yuexingan06.cn

Java: static final double PI = 3.14159;
来源：http://vt.shtwfgs.cn

Go:   const PI = 3.14159
来源：http://sd.hnjuh.cn

Ruby: PI = 3.14159
来源：http://jd.9csxet.cn

C#:   const double PI = 3.14159;
来源：http://tb.asd995.cn

[A04] 判断变量类型
来源：http://om.chemitech.net.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://wi.hahajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mb.asd995.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jk.521024.cn

TS:   typeof x; x instanceof Date
来源：http://wn.hnjuh.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mv.szxytkj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hs.panjiajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://jj.shxzskj.cn

C#:   x.GetType().Name; x is int
来源：http://rc.huanxung.cn

[A05] 整数除法与取模
来源：http://je.shtwfgs.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gz.panjiajie.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ea.muxihuayi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bv.521024.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ym.yuntaijiaju.cn

Java: 7 / 2; 7 % 2
来源：http://zl.wgjwhj.cn

Go:   7 / 2; 7 % 2
来源：http://af.nicolike.cn

Ruby: 7 / 2; 7 % 2
来源：http://ru.huanxung.cn

C#:   7 / 2; 7 % 2
来源：http://uf.muxihuayi.cn

[A06] 字符串转数字
来源：http://eq.shtwfgs.cn

Py:   int("42"); float("3.14")
来源：http://ye.yuntaijiaju.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nn.huanxung.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yq.wgjwhj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://oh.huanxung.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ux.huixinmuqiang.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ya.panjiajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hi.huanxung.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lw.521024.cn

[A07] 数字转字符串
来源：http://vd.szxytkj.cn

Py:   str(42)
来源：http://os.lnxyls.cn

PHP:  (string) 42; strval(42)
来源：http://lx.jctech888.com.cn

JS:   String(42); (42).toString()
来源：http://ih.bookmarksfly.cn

TS:   String(42)
来源：http://dk.nicolike.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://sd.9csxet.cn

Go:   strconv.Itoa(42)
来源：http://ew.szxytkj.cn

Ruby: 42.to_s
来源：http://lv.hahajie.cn

C#:   42.ToString()
来源：http://vo.bookmarksfly.cn

[A08] 取整与四舍五入
来源：http://wj.521024.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://np.muxihuayi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ut.9csxet.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://js.asd995.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sm.jctech888.com.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cx.nicolike.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://om.haigaiapp.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ij.lnxyls.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tk.szsharing.cn

[A09] 绝对值与最大最小值
来源：http://ms.haigaiapp.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yb.chemitech.net.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rv.bjjhwx.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dc.yuexingan06.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cl.shxzukj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://da.hnjuh.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://et.shxzskj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lr.lnxyls.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zs.9csxet.cn

[A10] 生成随机数
来源：http://ly.shxzskj.cn

Py:   import random; random.randint(1, 100)
来源：http://ft.huixiangedu.cn

PHP:  random_int(1, 100);
来源：http://yp.chemitech.net.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zg.haigaiapp.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hj.newstarts.cn

Java: new Random().nextInt(100) + 1
来源：http://rl.newstarts.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wo.gzmigu.cn

Ruby: rand(1..100)
来源：http://tu.gzmigu.cn

C#:   new Random().Next(1, 101)
来源：http://rn.jctech888.com.cn

[A11] 条件表达式（三元）
来源：http://fx.chemitech.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://vr.521024.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://sv.huixiangedu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://vj.huixiangedu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://om.huixiangedu.cn

Java: x > 0 ? "yes" : "no"
来源：http://dn.jctech888.com.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zh.shxzukj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ke.newstarts.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fa.szxytkj.cn

[A12] 字符串插值 / 格式化
来源：http://ps.newstarts.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ub.panjiajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gs.hnjuh.cn

JS:   `Hello, ${name}!`
来源：http://mu.bjjhwx.cn

TS:   `Hello, ${name}!`
来源：http://yj.muxihuayi.cn

Java: "Hello, %s!".formatted(name)
来源：http://th.huanxung.cn


<!-- 参考信息 -->