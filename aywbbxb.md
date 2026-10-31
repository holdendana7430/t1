代发 wailian999

[U65] PHP：会话
来源：http://lo.panjiajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ts.gzmigu.cn

[U66] PHP：设置 Cookie
来源：http://ok.colortex.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gx.bjjhwx.cn

[U67] PHP：处理文件上传
来源：http://sx.shtwfgs.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ru.huanxung.cn

[U68] PHP：PDO 连接
来源：http://hc.panjiajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mg.yuexingan06.cn

[U69] PHP：PDO 预处理
来源：http://zv.haigaiapp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cu.yuexingan06.cn

[U70] PHP：PDO 事务
来源：http://pv.szxytkj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fm.wgjwhj.cn

[U71] PHP：抛出异常
来源：http://xc.shtwfgs.cn

throw new RuntimeException("失败", 500);
来源：http://qr.szsharing.cn

[U72] PHP：写错误日志
来源：http://gs.jianghongdianzi.cn

error_log("失败: " . $e->getMessage());
来源：http://pz.chemitech.net.cn

[U73] PHP：读取 ini 配置
来源：http://jc.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://nv.szxytkj.cn

[U74] PHP：读取环境变量
来源：http://nf.newstarts.cn

getenv("APP_ENV") ?: "production"
来源：http://np.szsharing.cn

[U75] PHP：依赖注入
来源：http://qn.huixiangedu.cn

composer require psr/container
来源：http://db.huixiangedu.cn

[U76] PHP：简单路由
来源：http://gm.gzmigu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pt.yuntaijiaju.cn

[U77] PHP：模板渲染
来源：http://nb.nszjky.cn

composer require twig/twig
来源：http://hq.szxytkj.cn

[U78] PHP：单元测试
来源：http://zs.newstarts.cn

composer require --dev phpunit/phpunit
来源：http://yb.szsharing.cn

[U79] PHP：静态分析
来源：http://qc.huanxung.cn

composer require --dev phpstan/phpstan
来源：http://es.wgjwhj.cn

[U80] PHP：代码规范修复
来源：http://vg.yuntaijiaju.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ic.asd995.cn

[U81] JS：初始化项目
来源：http://pw.nszjky.cn

npm init -y;  npm i express
来源：http://wy.shxzukj.cn

[U82] JS：package.json 脚本
来源：http://dn.shtwfgs.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://au.shxzukj.cn

[U83] JS：ES Module 导入导出
来源：http://ov.hahajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zw.hnjuh.cn

[U84] JS：CommonJS 写法
来源：http://xr.muxihuayi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://it.hahajie.cn

[U85] JS：可选链
来源：http://xf.nicolike.cn

a?.b?.c
来源：http://qf.haigaiapp.cn

[U86] JS：空值合并
来源：http://el.shtwfgs.cn

a ?? b
来源：http://la.yuntaijiaju.cn

[U87] JS：解构默认值
来源：http://at.yuexingan06.cn

const { a = 1, b = 2 } = obj;
来源：http://wd.jianghongdianzi.cn

[U88] JS：对象展开合并
来源：http://kt.9csxet.cn

{ ...a, ...b }
来源：http://gn.chemitech.net.cn

[U89] JS：数组去重
来源：http://wg.huixinmuqiang.cn

[...new Set(arr)]
来源：http://qm.nicolike.cn

[U90] JS：数字数组排序
来源：http://oq.chemitech.net.cn

[...arr].sort((a, b) => a - b)
来源：http://yt.hahajie.cn

[U91] JS：对象键值遍历
来源：http://nm.shxzukj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wg.nicolike.cn

[U92] JS：深拷贝
来源：http://lv.jctech888.com.cn

structuredClone(obj)
来源：http://ji.hahajie.cn

[U93] JS：模板字符串
来源：http://vy.muxihuayi.cn

`共 ${n} 条`
来源：http://kz.wgjwhj.cn

[U94] JS：箭头函数
来源：http://zr.asd995.cn

const double = x => x * 2;
来源：http://ht.szsharing.cn

[U95] JS：Promise 包装
来源：http://ij.bjjhwx.cn

new Promise((resolve, reject) => {})
来源：http://qj.yuexingan06.cn

[U96] JS：async/await 与异常
来源：http://mx.shxzskj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bb.szxytkj.cn

[U97] JS：并发请求
来源：http://or.bjjhwx.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tk.szxytkj.cn

[U98] JS：fetch 带 JSON
来源：http://ug.yuexingan06.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vr.shtwfgs.cn

[U99] JS：事件监听
来源：http://su.wgjwhj.cn

el.addEventListener("click", e => {})
来源：http://dc.jctech888.com.cn

[U100] JS：DOM 查询
来源：http://di.huanxung.cn

document.querySelector(".item")
来源：http://zl.newstarts.cn

[U101] JS：classList 操作
来源：http://tp.hnjuh.cn

el.classList.toggle("active")
来源：http://eb.hnjuh.cn

[U102] JS：本地存储
来源：http://li.newstarts.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wu.asd995.cn

[U103] JS：定时器
来源：http://xp.szsharing.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ct.panjiajie.cn

[U104] JS：防抖
来源：http://ca.yuexingan06.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rj.9csxet.cn

[U105] JS：节流
来源：http://ua.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yx.szxytkj.cn

[U106] JS：日期格式化
来源：http://th.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rx.wgjwhj.cn

[U107] JS：数字千分位
来源：http://fs.wgjwhj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rt.wgjwhj.cn

[U108] JS：随机整数
来源：http://rl.hahajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mk.nszjky.cn

[U109] JS：数组分组
来源：http://vj.bjjhwx.cn

Object.groupBy(arr, x => x.type)
来源：http://lu.newstarts.cn

[U110] JS：数组分块
来源：http://ui.jctech888.com.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xx.asd995.cn

[U111] JS：对象转 Map
来源：http://co.huixiangedu.cn

new Map(Object.entries(obj))
来源：http://jd.huixinmuqiang.cn

[U112] JS：字符串补位
来源：http://hr.wgjwhj.cn

"7".padStart(3, "0")
来源：http://an.nszjky.cn

[U113] JS：正则替换全部
来源：http://zf.hnjuh.cn

s.replaceAll("a", "b")
来源：http://ev.yuexingan06.cn

[U114] JS：JSON 深比较
来源：http://ci.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fl.yuntaijiaju.cn

[U115] JS：生成 UUID
来源：http://xl.jctech888.com.cn

crypto.randomUUID()
来源：http://rz.panjiajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://mb.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://cb.jianghongdianzi.cn

[U117] JS：单元测试
来源：http://fu.yuexingan06.cn

npm i -D vitest;  npx vitest
来源：http://xx.lnxyls.cn

[U118] JS：开发服务器
来源：http://xq.jianghongdianzi.cn

npm i -D vite;  npx vite
来源：http://lf.chemitech.net.cn

[U119] JS：生产构建
来源：http://kp.szsharing.cn

npx vite build
来源：http://mp.newstarts.cn

[U120] JS：读取环境变量（Vite）
来源：http://xr.shtwfgs.cn

import.meta.env.VITE_API_URL
来源：http://vd.gzmigu.cn

================================================================================
来源：http://vb.hnjuh.cn

统计汇总
来源：http://ys.bjjhwx.cn

================================================================================
来源：http://gp.jianghongdianzi.cn

按语言统计（条）：
来源：http://ek.huanxung.cn

Python ......... 252
来源：http://zt.gzmigu.cn

PHP ............ 252
来源：http://xx.szsharing.cn

JavaScript ..... 252
来源：http://pb.521024.cn

TypeScript ..... 212
来源：http://ii.yuexingan06.cn

Java ........... 212
来源：http://an.521024.cn

Go ............. 212
来源：http://hm.szsharing.cn

Ruby ........... 212
来源：http://ra.newstarts.cn

C# ............. 212
来源：http://ff.shxzskj.cn

C .............. 30
来源：http://dx.hahajie.cn

C++ ............ 30
来源：http://zl.nszjky.cn

SQL ............ 90
来源：http://iz.nszjky.cn

Bash ........... 80
来源：http://hm.wgjwhj.cn

Kotlin ......... 15
来源：http://iw.hahajie.cn

Swift .......... 15
来源：http://ot.shtwfgs.cn

Lua ............ 10
来源：http://jr.huanxung.cn

Perl ........... 10
来源：http://wi.szxytkj.cn

Scala .......... 10
来源：http://wc.newstarts.cn

------------------------------------
来源：http://hc.shxzukj.cn

合计 ........... 2106 条
来源：http://vh.jianghongdianzi.cn

按章节统计：
来源：http://ly.nszjky.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bf.asd995.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lq.jianghongdianzi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rx.nszjky.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://io.newstarts.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zh.shxzskj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yn.hahajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ww.bjjhwx.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://uv.bookmarksfly.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://km.huixiangedu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bc.nicolike.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hb.szsharing.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fa.huixinmuqiang.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mx.panjiajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ax.nszjky.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zh.szsharing.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ti.shxzskj.cn

Q SQL 专题                              90
来源：http://zm.shxzukj.cn

R Bash 专题                             80
来源：http://bh.chemitech.net.cn

S C / C++ 专题                          60
来源：http://bh.chemitech.net.cn

T 其他语言补充                          60
来源：http://hb.haigaiapp.cn

U 高频实用片段                         120
来源：http://bz.wgjwhj.cn

------------------------------------
来源：http://om.newstarts.cn

合计                                  2106 条
来源：http://dy.521024.cn

--------------------------------------------------------------------------------
来源：http://zm.9csxet.cn

使用提醒
来源：http://cc.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://nq.szxytkj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://oi.nicolike.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jt.521024.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mw.shtwfgs.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://og.hahajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://df.lnxyls.cn

—— 文件结束 ——
来源：http://li.hnjuh.cn

================================================================================
来源：http://ld.muxihuayi.cn

程序语言常见例子速查手册（2024 版）
来源：http://be.9csxet.cn

Common Programming Examples Cheat Book
来源：http://jv.colortex.cn

================================================================================
来源：http://mp.hahajie.cn

【收录内容】
来源：http://cs.shtwfgs.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://sm.colortex.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vd.hahajie.cn

SQL · Bash · C · C++
来源：http://qf.newstarts.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xx.huixiangedu.cn

【使用说明】
来源：http://gn.huixinmuqiang.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vg.jianghongdianzi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zj.nszjky.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ti.lnxyls.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dp.muxihuayi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://cm.muxihuayi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bs.wgjwhj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qk.9csxet.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wo.9csxet.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ws.hahajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gs.lnxyls.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zx.asd995.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vg.nszjky.cn

【文件统计】
来源：http://gs.colortex.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zq.nszjky.cn

--------------------------------------------------------------------------------
来源：http://ah.shxzukj.cn

目  录
来源：http://dy.521024.cn

--------------------------------------------------------------------------------
来源：http://kx.bjjhwx.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ik.521024.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sy.bjjhwx.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ov.newstarts.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.newstarts.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://un.gzmigu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ox.huixiangedu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bz.jianghongdianzi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qc.shxzskj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://oo.shxzukj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vp.9csxet.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zd.yuexingan06.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lp.haigaiapp.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wk.bookmarksfly.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zi.huanxung.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fh.bjjhwx.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://da.panjiajie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mc.shtwfgs.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wc.shtwfgs.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ox.chemitech.net.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fl.jctech888.com.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nf.huixinmuqiang.cn

================================================================================
来源：http://lv.gzmigu.cn

A. 基础语法与类型
来源：http://ut.jianghongdianzi.cn

================================================================================
来源：http://xa.9csxet.cn

[A01] Hello World
来源：http://lr.nicolike.cn

Py:   print("Hello, World!")
来源：http://nb.nszjky.cn

PHP:  echo "Hello, World!";
来源：http://fb.wgjwhj.cn

JS:   console.log("Hello, World!");
来源：http://es.yuexingan06.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ln.shxzukj.cn

Java: System.out.println("Hello, World!");
来源：http://cr.huixinmuqiang.cn

Go:   fmt.Println("Hello, World!")
来源：http://hd.lnxyls.cn

Ruby: puts "Hello, World!"
来源：http://wv.shxzskj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ol.colortex.cn

[A02] 变量声明与赋值
来源：http://fy.hnjuh.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ib.colortex.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://nc.yuntaijiaju.cn

JS:   let name = "Alex"; const age = 20;
来源：http://mv.haigaiapp.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mv.shtwfgs.cn

Java: String name = "Alex"; int age = 20;
来源：http://yu.szxytkj.cn

Go:   name := "Alex"; age := 20
来源：http://wi.chemitech.net.cn

Ruby: name = "Alex"; age = 20
来源：http://oy.huixinmuqiang.cn

C#:   string name = "Alex"; int age = 20;
来源：http://bx.wgjwhj.cn

[A03] 常量定义
来源：http://ka.szsharing.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rc.huixinmuqiang.cn

PHP:  const PI = 3.14159;
来源：http://ya.shxzskj.cn

JS:   const PI = 3.14159;
来源：http://yd.wgjwhj.cn

TS:   const PI: number = 3.14159;
来源：http://ot.nszjky.cn

Java: static final double PI = 3.14159;
来源：http://hx.nicolike.cn

Go:   const PI = 3.14159
来源：http://ps.yuexingan06.cn

Ruby: PI = 3.14159
来源：http://xy.huanxung.cn

C#:   const double PI = 3.14159;
来源：http://mo.nszjky.cn

[A04] 判断变量类型
来源：http://mi.haigaiapp.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://rd.newstarts.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qh.hahajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wv.yuntaijiaju.cn

TS:   typeof x; x instanceof Date
来源：http://qd.szsharing.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://px.huixiangedu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://nf.jianghongdianzi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://lk.jianghongdianzi.cn

C#:   x.GetType().Name; x is int
来源：http://cm.nicolike.cn

[A05] 整数除法与取模
来源：http://oc.shxzskj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gv.muxihuayi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://db.yuexingan06.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lj.huixinmuqiang.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ij.521024.cn

Java: 7 / 2; 7 % 2
来源：http://xs.haigaiapp.cn

Go:   7 / 2; 7 % 2
来源：http://vt.521024.cn

Ruby: 7 / 2; 7 % 2
来源：http://vx.jianghongdianzi.cn

C#:   7 / 2; 7 % 2
来源：http://sb.lnxyls.cn

[A06] 字符串转数字
来源：http://ek.hnjuh.cn

Py:   int("42"); float("3.14")
来源：http://cl.szxytkj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qo.muxihuayi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fk.haigaiapp.cn

TS:   parseInt("42", 10); Number("42")
来源：http://mk.yuexingan06.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gs.nicolike.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xk.gzmigu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://lj.521024.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zp.521024.cn

[A07] 数字转字符串
来源：http://kh.szxytkj.cn

Py:   str(42)
来源：http://ny.hahajie.cn

PHP:  (string) 42; strval(42)
来源：http://kt.shtwfgs.cn

JS:   String(42); (42).toString()
来源：http://aq.asd995.cn

TS:   String(42)
来源：http://jl.9csxet.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ed.bjjhwx.cn

Go:   strconv.Itoa(42)
来源：http://ri.panjiajie.cn

Ruby: 42.to_s
来源：http://uf.szsharing.cn

C#:   42.ToString()
来源：http://ov.jctech888.com.cn

[A08] 取整与四舍五入
来源：http://kj.shtwfgs.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uv.haigaiapp.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://is.colortex.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fv.shtwfgs.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ft.hnjuh.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ni.huixinmuqiang.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bv.panjiajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://yz.yuntaijiaju.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xd.bjjhwx.cn

[A09] 绝对值与最大最小值
来源：http://me.hahajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yb.shxzskj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ak.szxytkj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://it.yuexingan06.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yy.huixiangedu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zo.jianghongdianzi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://of.jctech888.com.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://at.yuexingan06.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://op.wgjwhj.cn


<!-- 参考信息 -->