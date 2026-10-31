代发 wailian999

[U67] PHP：处理文件上传
来源：http://yx.jctech888.com.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pi.asd995.cn

[U68] PHP：PDO 连接
来源：http://im.bjjhwx.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lf.muxihuayi.cn

[U69] PHP：PDO 预处理
来源：http://vq.yuexingan06.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zm.shxzskj.cn

[U70] PHP：PDO 事务
来源：http://jc.hnjuh.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zd.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://ku.nszjky.cn

throw new RuntimeException("失败", 500);
来源：http://ql.panjiajie.cn

[U72] PHP：写错误日志
来源：http://ub.muxihuayi.cn

error_log("失败: " . $e->getMessage());
来源：http://fu.huixiangedu.cn

[U73] PHP：读取 ini 配置
来源：http://wu.lnxyls.cn

parse_ini_file("config.ini", true)
来源：http://bh.huixiangedu.cn

[U74] PHP：读取环境变量
来源：http://qs.jianghongdianzi.cn

getenv("APP_ENV") ?: "production"
来源：http://nm.bjjhwx.cn

[U75] PHP：依赖注入
来源：http://kc.hnjuh.cn

composer require psr/container
来源：http://qv.szxytkj.cn

[U76] PHP：简单路由
来源：http://ze.nicolike.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tv.yuntaijiaju.cn

[U77] PHP：模板渲染
来源：http://qa.shxzukj.cn

composer require twig/twig
来源：http://yp.521024.cn

[U78] PHP：单元测试
来源：http://tn.shtwfgs.cn

composer require --dev phpunit/phpunit
来源：http://xc.nicolike.cn

[U79] PHP：静态分析
来源：http://js.gzmigu.cn

composer require --dev phpstan/phpstan
来源：http://yy.gzmigu.cn

[U80] PHP：代码规范修复
来源：http://id.gzmigu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ay.szsharing.cn

[U81] JS：初始化项目
来源：http://wl.9csxet.cn

npm init -y;  npm i express
来源：http://qq.haigaiapp.cn

[U82] JS：package.json 脚本
来源：http://tj.shxzukj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tr.chemitech.net.cn

[U83] JS：ES Module 导入导出
来源：http://qp.jctech888.com.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wu.chemitech.net.cn

[U84] JS：CommonJS 写法
来源：http://od.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gd.yuexingan06.cn

[U85] JS：可选链
来源：http://ke.hahajie.cn

a?.b?.c
来源：http://kc.521024.cn

[U86] JS：空值合并
来源：http://sd.yuexingan06.cn

a ?? b
来源：http://ph.shxzskj.cn

[U87] JS：解构默认值
来源：http://lq.bookmarksfly.cn

const { a = 1, b = 2 } = obj;
来源：http://ed.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://pe.shtwfgs.cn

{ ...a, ...b }
来源：http://he.gzmigu.cn

[U89] JS：数组去重
来源：http://ik.szxytkj.cn

[...new Set(arr)]
来源：http://tj.nszjky.cn

[U90] JS：数字数组排序
来源：http://ed.wgjwhj.cn

[...arr].sort((a, b) => a - b)
来源：http://cz.gzmigu.cn

[U91] JS：对象键值遍历
来源：http://ic.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jx.shxzukj.cn

[U92] JS：深拷贝
来源：http://ty.nszjky.cn

structuredClone(obj)
来源：http://mr.huixinmuqiang.cn

[U93] JS：模板字符串
来源：http://ur.lnxyls.cn

`共 ${n} 条`
来源：http://xq.shxzskj.cn

[U94] JS：箭头函数
来源：http://xh.lnxyls.cn

const double = x => x * 2;
来源：http://tz.gzmigu.cn

[U95] JS：Promise 包装
来源：http://qq.shxzukj.cn

new Promise((resolve, reject) => {})
来源：http://lq.huixinmuqiang.cn

[U96] JS：async/await 与异常
来源：http://of.hnjuh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ib.shtwfgs.cn

[U97] JS：并发请求
来源：http://ln.huixiangedu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://iz.muxihuayi.cn

[U98] JS：fetch 带 JSON
来源：http://rx.huanxung.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mz.nszjky.cn

[U99] JS：事件监听
来源：http://hn.newstarts.cn

el.addEventListener("click", e => {})
来源：http://km.yuntaijiaju.cn

[U100] JS：DOM 查询
来源：http://ct.9csxet.cn

document.querySelector(".item")
来源：http://cq.huixiangedu.cn

[U101] JS：classList 操作
来源：http://gn.shxzukj.cn

el.classList.toggle("active")
来源：http://lb.shtwfgs.cn

[U102] JS：本地存储
来源：http://vr.asd995.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gq.nicolike.cn

[U103] JS：定时器
来源：http://im.9csxet.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ht.szxytkj.cn

[U104] JS：防抖
来源：http://le.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pm.hnjuh.cn

[U105] JS：节流
来源：http://dp.9csxet.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sz.shxzskj.cn

[U106] JS：日期格式化
来源：http://iz.muxihuayi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rh.bjjhwx.cn

[U107] JS：数字千分位
来源：http://jm.shxzukj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gs.szsharing.cn

[U108] JS：随机整数
来源：http://hi.yuexingan06.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vl.huixiangedu.cn

[U109] JS：数组分组
来源：http://eo.lnxyls.cn

Object.groupBy(arr, x => x.type)
来源：http://dr.shxzskj.cn

[U110] JS：数组分块
来源：http://mk.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kh.huixinmuqiang.cn

[U111] JS：对象转 Map
来源：http://zn.nszjky.cn

new Map(Object.entries(obj))
来源：http://kv.szxytkj.cn

[U112] JS：字符串补位
来源：http://zo.szxytkj.cn

"7".padStart(3, "0")
来源：http://ci.muxihuayi.cn

[U113] JS：正则替换全部
来源：http://wv.huixiangedu.cn

s.replaceAll("a", "b")
来源：http://rf.9csxet.cn

[U114] JS：JSON 深比较
来源：http://xp.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pv.wgjwhj.cn

[U115] JS：生成 UUID
来源：http://mi.jianghongdianzi.cn

crypto.randomUUID()
来源：http://nr.shxzskj.cn

[U116] JS：类型检查（JSDoc）
来源：http://ax.szxytkj.cn

/** @param {string} name */ function f(name) {}
来源：http://zu.521024.cn

[U117] JS：单元测试
来源：http://cc.shtwfgs.cn

npm i -D vitest;  npx vitest
来源：http://lm.chemitech.net.cn

[U118] JS：开发服务器
来源：http://lz.gzmigu.cn

npm i -D vite;  npx vite
来源：http://tf.hahajie.cn

[U119] JS：生产构建
来源：http://qn.jianghongdianzi.cn

npx vite build
来源：http://nf.asd995.cn

[U120] JS：读取环境变量（Vite）
来源：http://xv.szxytkj.cn

import.meta.env.VITE_API_URL
来源：http://up.hnjuh.cn

================================================================================
来源：http://hf.521024.cn

统计汇总
来源：http://yd.lnxyls.cn

================================================================================
来源：http://ke.yuexingan06.cn

按语言统计（条）：
来源：http://na.nicolike.cn

Python ......... 252
来源：http://li.shxzskj.cn

PHP ............ 252
来源：http://xz.yuexingan06.cn

JavaScript ..... 252
来源：http://gh.bookmarksfly.cn

TypeScript ..... 212
来源：http://zt.chemitech.net.cn

Java ........... 212
来源：http://gg.bookmarksfly.cn

Go ............. 212
来源：http://xg.newstarts.cn

Ruby ........... 212
来源：http://gy.gzmigu.cn

C# ............. 212
来源：http://nc.lnxyls.cn

C .............. 30
来源：http://ft.jianghongdianzi.cn

C++ ............ 30
来源：http://js.colortex.cn

SQL ............ 90
来源：http://lm.shxzskj.cn

Bash ........... 80
来源：http://dr.muxihuayi.cn

Kotlin ......... 15
来源：http://ce.haigaiapp.cn

Swift .......... 15
来源：http://kt.yuexingan06.cn

Lua ............ 10
来源：http://zn.jctech888.com.cn

Perl ........... 10
来源：http://db.hnjuh.cn

Scala .......... 10
来源：http://vh.szsharing.cn

------------------------------------
来源：http://ri.bjjhwx.cn

合计 ........... 2106 条
来源：http://zi.colortex.cn

按章节统计：
来源：http://dg.szsharing.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ty.hnjuh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cx.newstarts.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ws.hnjuh.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pa.shxzskj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ug.szsharing.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://eq.newstarts.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://eq.szxytkj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wu.9csxet.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lw.huixiangedu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sl.lnxyls.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pr.szsharing.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cb.bookmarksfly.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tn.szsharing.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kc.nicolike.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yv.haigaiapp.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://iq.szxytkj.cn

Q SQL 专题                              90
来源：http://hp.shxzukj.cn

R Bash 专题                             80
来源：http://cd.jctech888.com.cn

S C / C++ 专题                          60
来源：http://vn.lnxyls.cn

T 其他语言补充                          60
来源：http://wq.szxytkj.cn

U 高频实用片段                         120
来源：http://qq.bookmarksfly.cn

------------------------------------
来源：http://uz.panjiajie.cn

合计                                  2106 条
来源：http://hc.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://rx.shxzskj.cn

使用提醒
来源：http://kd.colortex.cn

--------------------------------------------------------------------------------
来源：http://km.muxihuayi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wu.521024.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hx.chemitech.net.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://oe.gzmigu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qk.hnjuh.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mt.wgjwhj.cn

—— 文件结束 ——
来源：http://zz.9csxet.cn

================================================================================
来源：http://gl.haigaiapp.cn

程序语言常见例子速查手册（2024 版）
来源：http://od.huixinmuqiang.cn

Common Programming Examples Cheat Book
来源：http://wx.colortex.cn

================================================================================
来源：http://he.hnjuh.cn

【收录内容】
来源：http://ax.jianghongdianzi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qk.gzmigu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ja.shxzskj.cn

SQL · Bash · C · C++
来源：http://al.yuexingan06.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hk.nszjky.cn

【使用说明】
来源：http://xr.yuntaijiaju.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ob.nszjky.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://on.newstarts.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nc.lnxyls.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ek.huanxung.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ri.panjiajie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bg.9csxet.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fv.huixiangedu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://po.huixinmuqiang.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wg.nicolike.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://oc.nicolike.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kk.szsharing.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.huixinmuqiang.cn

【文件统计】
来源：http://bl.521024.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://oq.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://ss.shxzukj.cn

目  录
来源：http://gj.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://ll.asd995.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fs.jctech888.com.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://al.newstarts.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sr.yuexingan06.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pk.huanxung.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cc.colortex.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kx.bjjhwx.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vh.gzmigu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://og.szxytkj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ps.shxzskj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ph.asd995.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ap.muxihuayi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://uc.muxihuayi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ao.nicolike.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ur.szxytkj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mo.panjiajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://su.colortex.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qp.szxytkj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://nm.bjjhwx.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pk.shtwfgs.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ae.newstarts.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://sq.szsharing.cn

================================================================================
来源：http://ld.hnjuh.cn

A. 基础语法与类型
来源：http://ri.hnjuh.cn

================================================================================
来源：http://rk.shtwfgs.cn

[A01] Hello World
来源：http://mp.huixinmuqiang.cn

Py:   print("Hello, World!")
来源：http://bh.haigaiapp.cn

PHP:  echo "Hello, World!";
来源：http://fv.huixinmuqiang.cn

JS:   console.log("Hello, World!");
来源：http://um.bookmarksfly.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ve.szxytkj.cn

Java: System.out.println("Hello, World!");
来源：http://du.asd995.cn

Go:   fmt.Println("Hello, World!")
来源：http://ps.9csxet.cn

Ruby: puts "Hello, World!"
来源：http://mx.bjjhwx.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jw.shxzskj.cn

[A02] 变量声明与赋值
来源：http://en.bjjhwx.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ge.huixiangedu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://zi.szsharing.cn

JS:   let name = "Alex"; const age = 20;
来源：http://sl.521024.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nu.huixinmuqiang.cn

Java: String name = "Alex"; int age = 20;
来源：http://ct.colortex.cn

Go:   name := "Alex"; age := 20
来源：http://hg.shxzukj.cn

Ruby: name = "Alex"; age = 20
来源：http://ta.lnxyls.cn

C#:   string name = "Alex"; int age = 20;
来源：http://cn.chemitech.net.cn

[A03] 常量定义
来源：http://bo.colortex.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mm.huixinmuqiang.cn

PHP:  const PI = 3.14159;
来源：http://yt.huanxung.cn

JS:   const PI = 3.14159;
来源：http://dx.yuexingan06.cn

TS:   const PI: number = 3.14159;
来源：http://qr.nicolike.cn

Java: static final double PI = 3.14159;
来源：http://yt.yuntaijiaju.cn

Go:   const PI = 3.14159
来源：http://no.bookmarksfly.cn

Ruby: PI = 3.14159
来源：http://so.yuntaijiaju.cn

C#:   const double PI = 3.14159;
来源：http://iw.gzmigu.cn

[A04] 判断变量类型
来源：http://jb.chemitech.net.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dj.lnxyls.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qz.shtwfgs.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bo.szsharing.cn

TS:   typeof x; x instanceof Date
来源：http://eo.panjiajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ey.nszjky.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fv.chemitech.net.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://dk.jctech888.com.cn

C#:   x.GetType().Name; x is int
来源：http://xi.jianghongdianzi.cn

[A05] 整数除法与取模
来源：http://mc.yuexingan06.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zc.yuntaijiaju.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://wi.yuexingan06.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nw.shxzskj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ml.huanxung.cn

Java: 7 / 2; 7 % 2
来源：http://rs.hahajie.cn

Go:   7 / 2; 7 % 2
来源：http://ce.shtwfgs.cn

Ruby: 7 / 2; 7 % 2
来源：http://hh.huixiangedu.cn

C#:   7 / 2; 7 % 2
来源：http://jz.colortex.cn

[A06] 字符串转数字
来源：http://af.nicolike.cn

Py:   int("42"); float("3.14")
来源：http://wh.gzmigu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://sb.panjiajie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xh.bookmarksfly.cn

TS:   parseInt("42", 10); Number("42")
来源：http://em.hahajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qz.jctech888.com.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ni.huixinmuqiang.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://yy.lnxyls.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://av.szxytkj.cn

[A07] 数字转字符串
来源：http://xg.nszjky.cn

Py:   str(42)
来源：http://gh.huanxung.cn

PHP:  (string) 42; strval(42)
来源：http://ue.colortex.cn

JS:   String(42); (42).toString()
来源：http://bc.huixinmuqiang.cn

TS:   String(42)
来源：http://ox.hahajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://tv.shtwfgs.cn

Go:   strconv.Itoa(42)
来源：http://qi.muxihuayi.cn

Ruby: 42.to_s
来源：http://vh.nicolike.cn

C#:   42.ToString()
来源：http://uh.szsharing.cn

[A08] 取整与四舍五入
来源：http://ne.huanxung.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pj.wgjwhj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rg.9csxet.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mc.shtwfgs.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sj.asd995.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rn.shxzskj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ti.9csxet.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://er.colortex.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://oa.huixinmuqiang.cn

[A09] 绝对值与最大最小值
来源：http://gx.yuexingan06.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lm.9csxet.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cq.muxihuayi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vs.huanxung.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lp.gzmigu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cx.nicolike.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ot.gzmigu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://op.yuntaijiaju.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lg.nicolike.cn

[A10] 生成随机数
来源：http://fe.gzmigu.cn

Py:   import random; random.randint(1, 100)
来源：http://bz.yuexingan06.cn

PHP:  random_int(1, 100);
来源：http://zj.shxzukj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jn.huanxung.cn


<!-- 参考信息 -->