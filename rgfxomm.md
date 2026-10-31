代发 wailian999

[U67] PHP：处理文件上传
来源：http://ib.huixiangedu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gk.yuntaijiaju.cn

[U68] PHP：PDO 连接
来源：http://wb.szsharing.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bt.chemitech.net.cn

[U69] PHP：PDO 预处理
来源：http://iq.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dj.newstarts.cn

[U70] PHP：PDO 事务
来源：http://ye.hnjuh.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tq.wgjwhj.cn

[U71] PHP：抛出异常
来源：http://kn.hnjuh.cn

throw new RuntimeException("失败", 500);
来源：http://qr.yuntaijiaju.cn

[U72] PHP：写错误日志
来源：http://hc.hahajie.cn

error_log("失败: " . $e->getMessage());
来源：http://fx.haigaiapp.cn

[U73] PHP：读取 ini 配置
来源：http://ic.nszjky.cn

parse_ini_file("config.ini", true)
来源：http://ai.521024.cn

[U74] PHP：读取环境变量
来源：http://di.huixinmuqiang.cn

getenv("APP_ENV") ?: "production"
来源：http://hy.hahajie.cn

[U75] PHP：依赖注入
来源：http://nk.newstarts.cn

composer require psr/container
来源：http://we.shxzskj.cn

[U76] PHP：简单路由
来源：http://ey.gzmigu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sa.9csxet.cn

[U77] PHP：模板渲染
来源：http://ip.hahajie.cn

composer require twig/twig
来源：http://ie.nszjky.cn

[U78] PHP：单元测试
来源：http://qx.huixinmuqiang.cn

composer require --dev phpunit/phpunit
来源：http://au.bookmarksfly.cn

[U79] PHP：静态分析
来源：http://kh.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://bo.521024.cn

[U80] PHP：代码规范修复
来源：http://fl.huanxung.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zc.muxihuayi.cn

[U81] JS：初始化项目
来源：http://sv.haigaiapp.cn

npm init -y;  npm i express
来源：http://mj.yuntaijiaju.cn

[U82] JS：package.json 脚本
来源：http://pw.szxytkj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pa.shxzukj.cn

[U83] JS：ES Module 导入导出
来源：http://ku.shxzukj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://pc.haigaiapp.cn

[U84] JS：CommonJS 写法
来源：http://na.wgjwhj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wk.panjiajie.cn

[U85] JS：可选链
来源：http://ve.szsharing.cn

a?.b?.c
来源：http://wb.bjjhwx.cn

[U86] JS：空值合并
来源：http://mt.chemitech.net.cn

a ?? b
来源：http://qc.gzmigu.cn

[U87] JS：解构默认值
来源：http://yz.newstarts.cn

const { a = 1, b = 2 } = obj;
来源：http://hc.nicolike.cn

[U88] JS：对象展开合并
来源：http://zr.colortex.cn

{ ...a, ...b }
来源：http://xg.colortex.cn

[U89] JS：数组去重
来源：http://gl.chemitech.net.cn

[...new Set(arr)]
来源：http://sv.521024.cn

[U90] JS：数字数组排序
来源：http://fc.9csxet.cn

[...arr].sort((a, b) => a - b)
来源：http://sx.haigaiapp.cn

[U91] JS：对象键值遍历
来源：http://uj.bjjhwx.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://od.jianghongdianzi.cn

[U92] JS：深拷贝
来源：http://wk.wgjwhj.cn

structuredClone(obj)
来源：http://ap.shtwfgs.cn

[U93] JS：模板字符串
来源：http://ow.gzmigu.cn

`共 ${n} 条`
来源：http://hy.panjiajie.cn

[U94] JS：箭头函数
来源：http://cu.colortex.cn

const double = x => x * 2;
来源：http://cx.yuntaijiaju.cn

[U95] JS：Promise 包装
来源：http://si.jctech888.com.cn

new Promise((resolve, reject) => {})
来源：http://ox.huixiangedu.cn

[U96] JS：async/await 与异常
来源：http://nf.shxzukj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zu.yuexingan06.cn

[U97] JS：并发请求
来源：http://tw.szsharing.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://fk.9csxet.cn

[U98] JS：fetch 带 JSON
来源：http://xx.huixinmuqiang.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cf.521024.cn

[U99] JS：事件监听
来源：http://rx.hahajie.cn

el.addEventListener("click", e => {})
来源：http://bq.yuntaijiaju.cn

[U100] JS：DOM 查询
来源：http://iz.huanxung.cn

document.querySelector(".item")
来源：http://sh.muxihuayi.cn

[U101] JS：classList 操作
来源：http://yc.bookmarksfly.cn

el.classList.toggle("active")
来源：http://xg.huanxung.cn

[U102] JS：本地存储
来源：http://jb.szsharing.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ol.huanxung.cn

[U103] JS：定时器
来源：http://cg.yuexingan06.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nq.hnjuh.cn

[U104] JS：防抖
来源：http://tj.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mw.szxytkj.cn

[U105] JS：节流
来源：http://li.nszjky.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sz.bjjhwx.cn

[U106] JS：日期格式化
来源：http://us.newstarts.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ib.huanxung.cn

[U107] JS：数字千分位
来源：http://qc.shtwfgs.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ft.521024.cn

[U108] JS：随机整数
来源：http://xv.nszjky.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://co.newstarts.cn

[U109] JS：数组分组
来源：http://td.521024.cn

Object.groupBy(arr, x => x.type)
来源：http://mj.panjiajie.cn

[U110] JS：数组分块
来源：http://te.asd995.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bn.hnjuh.cn

[U111] JS：对象转 Map
来源：http://ls.panjiajie.cn

new Map(Object.entries(obj))
来源：http://vu.szxytkj.cn

[U112] JS：字符串补位
来源：http://ij.newstarts.cn

"7".padStart(3, "0")
来源：http://wp.panjiajie.cn

[U113] JS：正则替换全部
来源：http://ti.szxytkj.cn

s.replaceAll("a", "b")
来源：http://gq.szsharing.cn

[U114] JS：JSON 深比较
来源：http://ss.nicolike.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ke.lnxyls.cn

[U115] JS：生成 UUID
来源：http://sq.wgjwhj.cn

crypto.randomUUID()
来源：http://vq.gzmigu.cn

[U116] JS：类型检查（JSDoc）
来源：http://ye.bjjhwx.cn

/** @param {string} name */ function f(name) {}
来源：http://kg.huixiangedu.cn

[U117] JS：单元测试
来源：http://vr.chemitech.net.cn

npm i -D vitest;  npx vitest
来源：http://oc.bjjhwx.cn

[U118] JS：开发服务器
来源：http://cd.muxihuayi.cn

npm i -D vite;  npx vite
来源：http://qm.9csxet.cn

[U119] JS：生产构建
来源：http://ux.huixinmuqiang.cn

npx vite build
来源：http://ud.haigaiapp.cn

[U120] JS：读取环境变量（Vite）
来源：http://ir.nszjky.cn

import.meta.env.VITE_API_URL
来源：http://gz.hahajie.cn

================================================================================
来源：http://fs.521024.cn

统计汇总
来源：http://uf.gzmigu.cn

================================================================================
来源：http://us.szsharing.cn

按语言统计（条）：
来源：http://rl.yuexingan06.cn

Python ......... 252
来源：http://ei.chemitech.net.cn

PHP ............ 252
来源：http://on.bookmarksfly.cn

JavaScript ..... 252
来源：http://lt.521024.cn

TypeScript ..... 212
来源：http://xa.asd995.cn

Java ........... 212
来源：http://bq.jctech888.com.cn

Go ............. 212
来源：http://js.yuexingan06.cn

Ruby ........... 212
来源：http://zi.hahajie.cn

C# ............. 212
来源：http://vf.szxytkj.cn

C .............. 30
来源：http://vi.colortex.cn

C++ ............ 30
来源：http://rd.huixiangedu.cn

SQL ............ 90
来源：http://fb.huixiangedu.cn

Bash ........... 80
来源：http://yw.muxihuayi.cn

Kotlin ......... 15
来源：http://od.haigaiapp.cn

Swift .......... 15
来源：http://pw.9csxet.cn

Lua ............ 10
来源：http://tr.bookmarksfly.cn

Perl ........... 10
来源：http://oh.newstarts.cn

Scala .......... 10
来源：http://qk.shtwfgs.cn

------------------------------------
来源：http://jt.shtwfgs.cn

合计 ........... 2106 条
来源：http://dv.shtwfgs.cn

按章节统计：
来源：http://rj.huixinmuqiang.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xk.lnxyls.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://su.gzmigu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gq.hnjuh.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wa.yuntaijiaju.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sk.colortex.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gw.huixiangedu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jg.haigaiapp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ht.bookmarksfly.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://go.hnjuh.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vn.hahajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rz.yuexingan06.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dj.shxzskj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://az.lnxyls.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ao.bjjhwx.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lf.muxihuayi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ui.muxihuayi.cn

Q SQL 专题                              90
来源：http://qp.wgjwhj.cn

R Bash 专题                             80
来源：http://tf.huixinmuqiang.cn

S C / C++ 专题                          60
来源：http://jd.shtwfgs.cn

T 其他语言补充                          60
来源：http://pf.asd995.cn

U 高频实用片段                         120
来源：http://aj.hnjuh.cn

------------------------------------
来源：http://bo.chemitech.net.cn

合计                                  2106 条
来源：http://ue.colortex.cn

--------------------------------------------------------------------------------
来源：http://jt.szsharing.cn

使用提醒
来源：http://jj.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://kg.gzmigu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dn.szsharing.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://me.colortex.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cj.hahajie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://af.huanxung.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wn.wgjwhj.cn

—— 文件结束 ——
来源：http://tk.shxzskj.cn

================================================================================
来源：http://tx.chemitech.net.cn

程序语言常见例子速查手册（2024 版）
来源：http://pl.huixinmuqiang.cn

Common Programming Examples Cheat Book
来源：http://jm.nicolike.cn

================================================================================
来源：http://hi.bjjhwx.cn

【收录内容】
来源：http://px.yuexingan06.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://um.hnjuh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ty.lnxyls.cn

SQL · Bash · C · C++
来源：http://ma.shxzskj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://so.asd995.cn

【使用说明】
来源：http://yg.muxihuayi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vr.wgjwhj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dy.nicolike.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://cw.szsharing.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yz.hahajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fo.newstarts.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://um.newstarts.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bn.newstarts.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ya.szsharing.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vy.huixiangedu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zd.shxzskj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kv.asd995.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pw.yuexingan06.cn

【文件统计】
来源：http://bq.huanxung.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ql.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://uh.nszjky.cn

目  录
来源：http://sw.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://cp.szxytkj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hr.nicolike.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jo.bookmarksfly.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yv.gzmigu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qg.chemitech.net.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ih.huixiangedu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gw.shtwfgs.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nz.asd995.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yd.521024.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dk.521024.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jj.huixiangedu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bg.szsharing.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qh.nicolike.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vz.hahajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rj.yuexingan06.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xb.muxihuayi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ni.asd995.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zu.szxytkj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ho.wgjwhj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hf.jianghongdianzi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nq.muxihuayi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hh.wgjwhj.cn

================================================================================
来源：http://vu.muxihuayi.cn

A. 基础语法与类型
来源：http://jz.chemitech.net.cn

================================================================================
来源：http://bc.jianghongdianzi.cn

[A01] Hello World
来源：http://ax.haigaiapp.cn

Py:   print("Hello, World!")
来源：http://ek.hnjuh.cn

PHP:  echo "Hello, World!";
来源：http://wp.chemitech.net.cn

JS:   console.log("Hello, World!");
来源：http://fj.chemitech.net.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fk.nszjky.cn

Java: System.out.println("Hello, World!");
来源：http://vt.hnjuh.cn

Go:   fmt.Println("Hello, World!")
来源：http://zj.asd995.cn

Ruby: puts "Hello, World!"
来源：http://lj.521024.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://co.szsharing.cn

[A02] 变量声明与赋值
来源：http://ry.muxihuayi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ef.bookmarksfly.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://dt.shxzukj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xa.bjjhwx.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kj.jianghongdianzi.cn

Java: String name = "Alex"; int age = 20;
来源：http://qf.szsharing.cn

Go:   name := "Alex"; age := 20
来源：http://si.gzmigu.cn

Ruby: name = "Alex"; age = 20
来源：http://qq.jctech888.com.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ch.bookmarksfly.cn

[A03] 常量定义
来源：http://zl.asd995.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fd.colortex.cn

PHP:  const PI = 3.14159;
来源：http://eo.lnxyls.cn

JS:   const PI = 3.14159;
来源：http://rk.521024.cn

TS:   const PI: number = 3.14159;
来源：http://xy.panjiajie.cn

Java: static final double PI = 3.14159;
来源：http://li.jctech888.com.cn

Go:   const PI = 3.14159
来源：http://ee.newstarts.cn

Ruby: PI = 3.14159
来源：http://nd.shtwfgs.cn

C#:   const double PI = 3.14159;
来源：http://fo.nicolike.cn

[A04] 判断变量类型
来源：http://pz.huixiangedu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qc.shxzskj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fx.bjjhwx.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ht.shtwfgs.cn

TS:   typeof x; x instanceof Date
来源：http://do.shxzukj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://af.newstarts.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ng.yuexingan06.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://hl.newstarts.cn

C#:   x.GetType().Name; x is int
来源：http://od.shtwfgs.cn

[A05] 整数除法与取模
来源：http://oe.shxzskj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://sw.bjjhwx.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://eb.yuntaijiaju.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kn.newstarts.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fs.hahajie.cn

Java: 7 / 2; 7 % 2
来源：http://tq.huanxung.cn

Go:   7 / 2; 7 % 2
来源：http://bb.shtwfgs.cn

Ruby: 7 / 2; 7 % 2
来源：http://ce.muxihuayi.cn

C#:   7 / 2; 7 % 2
来源：http://su.huixiangedu.cn

[A06] 字符串转数字
来源：http://ow.chemitech.net.cn

Py:   int("42"); float("3.14")
来源：http://gg.huixinmuqiang.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qf.wgjwhj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ui.bjjhwx.cn

TS:   parseInt("42", 10); Number("42")
来源：http://lg.bjjhwx.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gh.9csxet.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gs.huixiangedu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ru.jianghongdianzi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qc.shtwfgs.cn

[A07] 数字转字符串
来源：http://zp.521024.cn

Py:   str(42)
来源：http://rz.521024.cn

PHP:  (string) 42; strval(42)
来源：http://qe.shxzskj.cn

JS:   String(42); (42).toString()
来源：http://yp.bjjhwx.cn

TS:   String(42)
来源：http://af.asd995.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://cs.szxytkj.cn

Go:   strconv.Itoa(42)
来源：http://ai.jianghongdianzi.cn

Ruby: 42.to_s
来源：http://sl.bookmarksfly.cn

C#:   42.ToString()
来源：http://iy.panjiajie.cn

[A08] 取整与四舍五入
来源：http://ei.panjiajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://st.jctech888.com.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tq.newstarts.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pc.shxzskj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rv.colortex.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lf.newstarts.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lh.jianghongdianzi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pp.shxzskj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fn.nszjky.cn

[A09] 绝对值与最大最小值
来源：http://tv.bjjhwx.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ea.muxihuayi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gv.huixinmuqiang.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://if.chemitech.net.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kk.yuntaijiaju.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://de.shxzskj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://up.haigaiapp.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wp.shxzskj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jf.huixiangedu.cn

[A10] 生成随机数
来源：http://il.huanxung.cn

Py:   import random; random.randint(1, 100)
来源：http://yy.newstarts.cn

PHP:  random_int(1, 100);
来源：http://uw.shtwfgs.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qe.newstarts.cn


<!-- 参考信息 -->