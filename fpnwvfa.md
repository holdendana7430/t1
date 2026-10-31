代发 wailian999

[U75] PHP：依赖注入
来源：http://kd.bookmarksfly.cn

composer require psr/container
来源：http://bd.chemitech.net.cn

[U76] PHP：简单路由
来源：http://ox.szsharing.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yx.bookmarksfly.cn

[U77] PHP：模板渲染
来源：http://ho.9csxet.cn

composer require twig/twig
来源：http://cc.muxihuayi.cn

[U78] PHP：单元测试
来源：http://uy.shtwfgs.cn

composer require --dev phpunit/phpunit
来源：http://ej.shxzskj.cn

[U79] PHP：静态分析
来源：http://iz.huixiangedu.cn

composer require --dev phpstan/phpstan
来源：http://zl.colortex.cn

[U80] PHP：代码规范修复
来源：http://xk.panjiajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jb.bjjhwx.cn

[U81] JS：初始化项目
来源：http://cx.szsharing.cn

npm init -y;  npm i express
来源：http://op.521024.cn

[U82] JS：package.json 脚本
来源：http://qi.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fv.9csxet.cn

[U83] JS：ES Module 导入导出
来源：http://le.521024.cn

export const a = 1;  import { a } from "./m.js";
来源：http://if.huanxung.cn

[U84] JS：CommonJS 写法
来源：http://dm.yuntaijiaju.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fk.shxzukj.cn

[U85] JS：可选链
来源：http://hs.521024.cn

a?.b?.c
来源：http://lq.jctech888.com.cn

[U86] JS：空值合并
来源：http://un.colortex.cn

a ?? b
来源：http://kz.shxzukj.cn

[U87] JS：解构默认值
来源：http://gp.lnxyls.cn

const { a = 1, b = 2 } = obj;
来源：http://wb.wgjwhj.cn

[U88] JS：对象展开合并
来源：http://kb.chemitech.net.cn

{ ...a, ...b }
来源：http://vr.yuexingan06.cn

[U89] JS：数组去重
来源：http://nu.gzmigu.cn

[...new Set(arr)]
来源：http://rz.lnxyls.cn

[U90] JS：数字数组排序
来源：http://uu.szxytkj.cn

[...arr].sort((a, b) => a - b)
来源：http://dl.haigaiapp.cn

[U91] JS：对象键值遍历
来源：http://ph.chemitech.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bs.hahajie.cn

[U92] JS：深拷贝
来源：http://ei.lnxyls.cn

structuredClone(obj)
来源：http://ww.shxzskj.cn

[U93] JS：模板字符串
来源：http://yp.hnjuh.cn

`共 ${n} 条`
来源：http://ob.haigaiapp.cn

[U94] JS：箭头函数
来源：http://ux.nicolike.cn

const double = x => x * 2;
来源：http://vf.9csxet.cn

[U95] JS：Promise 包装
来源：http://vt.szxytkj.cn

new Promise((resolve, reject) => {})
来源：http://cx.muxihuayi.cn

[U96] JS：async/await 与异常
来源：http://xr.shxzukj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ck.szsharing.cn

[U97] JS：并发请求
来源：http://iq.nszjky.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zb.yuexingan06.cn

[U98] JS：fetch 带 JSON
来源：http://gv.yuexingan06.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://oz.jianghongdianzi.cn

[U99] JS：事件监听
来源：http://ss.hnjuh.cn

el.addEventListener("click", e => {})
来源：http://pi.hnjuh.cn

[U100] JS：DOM 查询
来源：http://sh.szsharing.cn

document.querySelector(".item")
来源：http://pr.yuexingan06.cn

[U101] JS：classList 操作
来源：http://os.yuexingan06.cn

el.classList.toggle("active")
来源：http://gx.szsharing.cn

[U102] JS：本地存储
来源：http://vx.szsharing.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kp.newstarts.cn

[U103] JS：定时器
来源：http://am.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ed.huanxung.cn

[U104] JS：防抖
来源：http://dt.hahajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aa.panjiajie.cn

[U105] JS：节流
来源：http://it.haigaiapp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://du.yuexingan06.cn

[U106] JS：日期格式化
来源：http://js.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zf.nicolike.cn

[U107] JS：数字千分位
来源：http://nu.huixinmuqiang.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mg.shxzskj.cn

[U108] JS：随机整数
来源：http://en.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xk.hahajie.cn

[U109] JS：数组分组
来源：http://bb.shxzukj.cn

Object.groupBy(arr, x => x.type)
来源：http://lx.huixiangedu.cn

[U110] JS：数组分块
来源：http://ym.hnjuh.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qf.jianghongdianzi.cn

[U111] JS：对象转 Map
来源：http://qr.hahajie.cn

new Map(Object.entries(obj))
来源：http://on.shxzskj.cn

[U112] JS：字符串补位
来源：http://af.9csxet.cn

"7".padStart(3, "0")
来源：http://wi.huixinmuqiang.cn

[U113] JS：正则替换全部
来源：http://ou.jianghongdianzi.cn

s.replaceAll("a", "b")
来源：http://tw.hnjuh.cn

[U114] JS：JSON 深比较
来源：http://ls.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gp.huixinmuqiang.cn

[U115] JS：生成 UUID
来源：http://jm.hahajie.cn

crypto.randomUUID()
来源：http://pm.521024.cn

[U116] JS：类型检查（JSDoc）
来源：http://ir.9csxet.cn

/** @param {string} name */ function f(name) {}
来源：http://om.asd995.cn

[U117] JS：单元测试
来源：http://wk.haigaiapp.cn

npm i -D vitest;  npx vitest
来源：http://fa.hahajie.cn

[U118] JS：开发服务器
来源：http://ww.szsharing.cn

npm i -D vite;  npx vite
来源：http://ge.colortex.cn

[U119] JS：生产构建
来源：http://zf.huixiangedu.cn

npx vite build
来源：http://di.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://du.yuntaijiaju.cn

import.meta.env.VITE_API_URL
来源：http://ey.gzmigu.cn

================================================================================
来源：http://fq.haigaiapp.cn

统计汇总
来源：http://rj.wgjwhj.cn

================================================================================
来源：http://yl.haigaiapp.cn

按语言统计（条）：
来源：http://al.bjjhwx.cn

Python ......... 252
来源：http://bu.hahajie.cn

PHP ............ 252
来源：http://xa.panjiajie.cn

JavaScript ..... 252
来源：http://nc.chemitech.net.cn

TypeScript ..... 212
来源：http://zr.shxzukj.cn

Java ........... 212
来源：http://rp.lnxyls.cn

Go ............. 212
来源：http://ox.shtwfgs.cn

Ruby ........... 212
来源：http://zr.shxzskj.cn

C# ............. 212
来源：http://zo.chemitech.net.cn

C .............. 30
来源：http://nl.bookmarksfly.cn

C++ ............ 30
来源：http://fh.bjjhwx.cn

SQL ............ 90
来源：http://dr.9csxet.cn

Bash ........... 80
来源：http://lb.gzmigu.cn

Kotlin ......... 15
来源：http://nw.szsharing.cn

Swift .......... 15
来源：http://lg.9csxet.cn

Lua ............ 10
来源：http://bx.lnxyls.cn

Perl ........... 10
来源：http://ca.huanxung.cn

Scala .......... 10
来源：http://is.nicolike.cn

------------------------------------
来源：http://rm.bjjhwx.cn

合计 ........... 2106 条
来源：http://kk.shxzskj.cn

按章节统计：
来源：http://bc.nicolike.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://iz.shxzukj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sl.asd995.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rl.nicolike.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://iq.jctech888.com.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yh.jianghongdianzi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ue.bjjhwx.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rs.9csxet.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nx.colortex.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qg.yuexingan06.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gi.bjjhwx.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wd.hnjuh.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qj.bjjhwx.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yu.huanxung.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rz.yuexingan06.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ex.szxytkj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wu.colortex.cn

Q SQL 专题                              90
来源：http://im.muxihuayi.cn

R Bash 专题                             80
来源：http://eb.huixiangedu.cn

S C / C++ 专题                          60
来源：http://za.jianghongdianzi.cn

T 其他语言补充                          60
来源：http://sm.yuexingan06.cn

U 高频实用片段                         120
来源：http://jg.hahajie.cn

------------------------------------
来源：http://ka.nicolike.cn

合计                                  2106 条
来源：http://un.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://ul.huixiangedu.cn

使用提醒
来源：http://pe.newstarts.cn

--------------------------------------------------------------------------------
来源：http://ux.nszjky.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ao.newstarts.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fw.huanxung.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://za.gzmigu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://hv.colortex.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bq.bookmarksfly.cn

—— 文件结束 ——
来源：http://hs.gzmigu.cn

================================================================================
来源：http://oi.521024.cn

程序语言常见例子速查手册（2024 版）
来源：http://cp.muxihuayi.cn

Common Programming Examples Cheat Book
来源：http://hy.colortex.cn

================================================================================
来源：http://wv.521024.cn

【收录内容】
来源：http://gh.asd995.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://tk.yuexingan06.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sz.szsharing.cn

SQL · Bash · C · C++
来源：http://to.asd995.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jt.bjjhwx.cn

【使用说明】
来源：http://nt.nszjky.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://is.shxzukj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ro.521024.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yr.hnjuh.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ot.bookmarksfly.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://sv.muxihuayi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ig.panjiajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ek.bookmarksfly.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://uu.9csxet.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nw.yuexingan06.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://px.yuexingan06.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fa.szsharing.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zj.panjiajie.cn

【文件统计】
来源：http://bq.newstarts.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pl.521024.cn

--------------------------------------------------------------------------------
来源：http://gp.lnxyls.cn

目  录
来源：http://ty.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://re.9csxet.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ly.colortex.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dp.shxzukj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kb.nicolike.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fd.gzmigu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ho.bjjhwx.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zo.9csxet.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rg.yuntaijiaju.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wr.jianghongdianzi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ir.yuexingan06.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://un.jctech888.com.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rp.lnxyls.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://il.muxihuayi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://at.szxytkj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wo.colortex.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://np.9csxet.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wo.lnxyls.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pc.yuexingan06.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hl.chemitech.net.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tg.lnxyls.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kz.hnjuh.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zh.hahajie.cn

================================================================================
来源：http://tr.jctech888.com.cn

A. 基础语法与类型
来源：http://tt.panjiajie.cn

================================================================================
来源：http://fc.haigaiapp.cn

[A01] Hello World
来源：http://ko.colortex.cn

Py:   print("Hello, World!")
来源：http://zy.jctech888.com.cn

PHP:  echo "Hello, World!";
来源：http://fp.nicolike.cn

JS:   console.log("Hello, World!");
来源：http://uf.lnxyls.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ec.colortex.cn

Java: System.out.println("Hello, World!");
来源：http://bo.newstarts.cn

Go:   fmt.Println("Hello, World!")
来源：http://yi.chemitech.net.cn

Ruby: puts "Hello, World!"
来源：http://pb.shtwfgs.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ki.asd995.cn

[A02] 变量声明与赋值
来源：http://fn.yuexingan06.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qy.hahajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qs.bookmarksfly.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hp.huixiangedu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xl.gzmigu.cn

Java: String name = "Alex"; int age = 20;
来源：http://mr.panjiajie.cn

Go:   name := "Alex"; age := 20
来源：http://hd.asd995.cn

Ruby: name = "Alex"; age = 20
来源：http://oq.newstarts.cn

C#:   string name = "Alex"; int age = 20;
来源：http://zk.asd995.cn

[A03] 常量定义
来源：http://az.9csxet.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hu.hnjuh.cn

PHP:  const PI = 3.14159;
来源：http://wh.shxzukj.cn

JS:   const PI = 3.14159;
来源：http://bt.shxzukj.cn

TS:   const PI: number = 3.14159;
来源：http://dd.haigaiapp.cn

Java: static final double PI = 3.14159;
来源：http://xv.hnjuh.cn

Go:   const PI = 3.14159
来源：http://bf.yuntaijiaju.cn

Ruby: PI = 3.14159
来源：http://dk.newstarts.cn

C#:   const double PI = 3.14159;
来源：http://el.shxzskj.cn

[A04] 判断变量类型
来源：http://cf.shtwfgs.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://av.panjiajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://sf.shxzskj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tf.yuexingan06.cn

TS:   typeof x; x instanceof Date
来源：http://fy.hahajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vr.jctech888.com.cn

Go:   reflect.TypeOf(x).Name()
来源：http://qz.shxzukj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://mq.chemitech.net.cn

C#:   x.GetType().Name; x is int
来源：http://xv.yuntaijiaju.cn

[A05] 整数除法与取模
来源：http://he.shxzukj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zb.haigaiapp.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ts.haigaiapp.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ar.jctech888.com.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ii.wgjwhj.cn

Java: 7 / 2; 7 % 2
来源：http://kf.hnjuh.cn

Go:   7 / 2; 7 % 2
来源：http://gp.jianghongdianzi.cn

Ruby: 7 / 2; 7 % 2
来源：http://vb.colortex.cn

C#:   7 / 2; 7 % 2
来源：http://tb.shxzukj.cn

[A06] 字符串转数字
来源：http://be.shtwfgs.cn

Py:   int("42"); float("3.14")
来源：http://fz.nszjky.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://et.hahajie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yi.shxzukj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://lx.muxihuayi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wc.huixiangedu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vx.chemitech.net.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://yn.bjjhwx.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ep.wgjwhj.cn

[A07] 数字转字符串
来源：http://fk.yuexingan06.cn

Py:   str(42)
来源：http://wr.9csxet.cn

PHP:  (string) 42; strval(42)
来源：http://zi.muxihuayi.cn

JS:   String(42); (42).toString()
来源：http://fp.521024.cn

TS:   String(42)
来源：http://sl.shxzukj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ql.yuexingan06.cn

Go:   strconv.Itoa(42)
来源：http://gf.lnxyls.cn

Ruby: 42.to_s
来源：http://em.bjjhwx.cn

C#:   42.ToString()
来源：http://id.hahajie.cn

[A08] 取整与四舍五入
来源：http://jm.shxzukj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cl.9csxet.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://pa.colortex.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sv.huanxung.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sg.jctech888.com.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pe.haigaiapp.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zo.shtwfgs.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://nb.huixiangedu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tk.bjjhwx.cn

[A09] 绝对值与最大最小值
来源：http://us.huixinmuqiang.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://eq.panjiajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jt.muxihuayi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hq.nicolike.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://os.huanxung.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://up.521024.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bn.gzmigu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://sy.huixiangedu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://nk.colortex.cn

[A10] 生成随机数
来源：http://bb.9csxet.cn

Py:   import random; random.randint(1, 100)
来源：http://ex.panjiajie.cn

PHP:  random_int(1, 100);
来源：http://oz.chemitech.net.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pm.hahajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ir.newstarts.cn

Java: new Random().nextInt(100) + 1
来源：http://je.haigaiapp.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dy.jianghongdianzi.cn

Ruby: rand(1..100)
来源：http://sb.nicolike.cn

C#:   new Random().Next(1, 101)
来源：http://on.yuntaijiaju.cn

[A11] 条件表达式（三元）
来源：http://om.yuntaijiaju.cn

Py:   "yes" if x > 0 else "no"
来源：http://nk.huanxung.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://hb.9csxet.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ne.gzmigu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ro.hnjuh.cn

Java: x > 0 ? "yes" : "no"
来源：http://fk.bjjhwx.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://bh.bookmarksfly.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://kb.521024.cn

C#:   x > 0 ? "yes" : "no"
来源：http://gr.huanxung.cn

[A12] 字符串插值 / 格式化
来源：http://rc.shxzskj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nt.haigaiapp.cn


<!-- 参考信息 -->