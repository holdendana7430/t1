代发 wailian999

[U65] PHP：会话
来源：http://bz.muxihuayi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lr.jianghongdianzi.cn

[U66] PHP：设置 Cookie
来源：http://bc.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xq.lnxyls.cn

[U67] PHP：处理文件上传
来源：http://gw.nicolike.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qb.chemitech.net.cn

[U68] PHP：PDO 连接
来源：http://bh.colortex.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cl.hahajie.cn

[U69] PHP：PDO 预处理
来源：http://ci.nicolike.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://so.wgjwhj.cn

[U70] PHP：PDO 事务
来源：http://up.panjiajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cd.hahajie.cn

[U71] PHP：抛出异常
来源：http://me.yuexingan06.cn

throw new RuntimeException("失败", 500);
来源：http://yd.chemitech.net.cn

[U72] PHP：写错误日志
来源：http://rr.nicolike.cn

error_log("失败: " . $e->getMessage());
来源：http://rl.yuntaijiaju.cn

[U73] PHP：读取 ini 配置
来源：http://xg.hnjuh.cn

parse_ini_file("config.ini", true)
来源：http://uv.shxzukj.cn

[U74] PHP：读取环境变量
来源：http://uf.yuntaijiaju.cn

getenv("APP_ENV") ?: "production"
来源：http://ce.haigaiapp.cn

[U75] PHP：依赖注入
来源：http://wh.521024.cn

composer require psr/container
来源：http://od.haigaiapp.cn

[U76] PHP：简单路由
来源：http://el.gzmigu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://io.gzmigu.cn

[U77] PHP：模板渲染
来源：http://qz.shxzskj.cn

composer require twig/twig
来源：http://ol.huixinmuqiang.cn

[U78] PHP：单元测试
来源：http://zz.wgjwhj.cn

composer require --dev phpunit/phpunit
来源：http://em.chemitech.net.cn

[U79] PHP：静态分析
来源：http://yq.muxihuayi.cn

composer require --dev phpstan/phpstan
来源：http://cc.szsharing.cn

[U80] PHP：代码规范修复
来源：http://zj.huanxung.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sb.nicolike.cn

[U81] JS：初始化项目
来源：http://ct.shxzskj.cn

npm init -y;  npm i express
来源：http://gg.yuexingan06.cn

[U82] JS：package.json 脚本
来源：http://he.colortex.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://iy.colortex.cn

[U83] JS：ES Module 导入导出
来源：http://wm.yuntaijiaju.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ah.chemitech.net.cn

[U84] JS：CommonJS 写法
来源：http://vr.huanxung.cn

module.exports = { a };  const { a } = require("./m");
来源：http://uw.jctech888.com.cn

[U85] JS：可选链
来源：http://vp.muxihuayi.cn

a?.b?.c
来源：http://no.nszjky.cn

[U86] JS：空值合并
来源：http://vr.hahajie.cn

a ?? b
来源：http://vt.newstarts.cn

[U87] JS：解构默认值
来源：http://xh.jianghongdianzi.cn

const { a = 1, b = 2 } = obj;
来源：http://pb.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://dh.szxytkj.cn

{ ...a, ...b }
来源：http://qp.shxzukj.cn

[U89] JS：数组去重
来源：http://il.nszjky.cn

[...new Set(arr)]
来源：http://ej.haigaiapp.cn

[U90] JS：数字数组排序
来源：http://ye.lnxyls.cn

[...arr].sort((a, b) => a - b)
来源：http://em.lnxyls.cn

[U91] JS：对象键值遍历
来源：http://rb.nszjky.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://si.yuexingan06.cn

[U92] JS：深拷贝
来源：http://bh.bookmarksfly.cn

structuredClone(obj)
来源：http://qz.lnxyls.cn

[U93] JS：模板字符串
来源：http://hv.haigaiapp.cn

`共 ${n} 条`
来源：http://ur.hahajie.cn

[U94] JS：箭头函数
来源：http://mc.yuexingan06.cn

const double = x => x * 2;
来源：http://cx.colortex.cn

[U95] JS：Promise 包装
来源：http://kl.szxytkj.cn

new Promise((resolve, reject) => {})
来源：http://bt.nicolike.cn

[U96] JS：async/await 与异常
来源：http://th.hnjuh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bm.panjiajie.cn

[U97] JS：并发请求
来源：http://bx.wgjwhj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://oo.521024.cn

[U98] JS：fetch 带 JSON
来源：http://it.jianghongdianzi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mr.hnjuh.cn

[U99] JS：事件监听
来源：http://hw.bookmarksfly.cn

el.addEventListener("click", e => {})
来源：http://zt.gzmigu.cn

[U100] JS：DOM 查询
来源：http://gk.huixinmuqiang.cn

document.querySelector(".item")
来源：http://zs.yuntaijiaju.cn

[U101] JS：classList 操作
来源：http://la.jctech888.com.cn

el.classList.toggle("active")
来源：http://xm.bookmarksfly.cn

[U102] JS：本地存储
来源：http://mk.wgjwhj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fu.shtwfgs.cn

[U103] JS：定时器
来源：http://po.asd995.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ly.asd995.cn

[U104] JS：防抖
来源：http://aj.jianghongdianzi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://um.bookmarksfly.cn

[U105] JS：节流
来源：http://mo.muxihuayi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ro.9csxet.cn

[U106] JS：日期格式化
来源：http://xm.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ab.yuntaijiaju.cn

[U107] JS：数字千分位
来源：http://qj.9csxet.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lz.9csxet.cn

[U108] JS：随机整数
来源：http://eb.521024.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ro.yuexingan06.cn

[U109] JS：数组分组
来源：http://qs.jianghongdianzi.cn

Object.groupBy(arr, x => x.type)
来源：http://di.newstarts.cn

[U110] JS：数组分块
来源：http://xb.nszjky.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iv.jctech888.com.cn

[U111] JS：对象转 Map
来源：http://vf.haigaiapp.cn

new Map(Object.entries(obj))
来源：http://em.9csxet.cn

[U112] JS：字符串补位
来源：http://pu.hnjuh.cn

"7".padStart(3, "0")
来源：http://iy.asd995.cn

[U113] JS：正则替换全部
来源：http://iy.szxytkj.cn

s.replaceAll("a", "b")
来源：http://ku.yuexingan06.cn

[U114] JS：JSON 深比较
来源：http://du.newstarts.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rd.521024.cn

[U115] JS：生成 UUID
来源：http://xq.hnjuh.cn

crypto.randomUUID()
来源：http://wx.huixiangedu.cn

[U116] JS：类型检查（JSDoc）
来源：http://as.huixiangedu.cn

/** @param {string} name */ function f(name) {}
来源：http://sd.lnxyls.cn

[U117] JS：单元测试
来源：http://sc.huanxung.cn

npm i -D vitest;  npx vitest
来源：http://qw.hnjuh.cn

[U118] JS：开发服务器
来源：http://be.gzmigu.cn

npm i -D vite;  npx vite
来源：http://st.colortex.cn

[U119] JS：生产构建
来源：http://nx.haigaiapp.cn

npx vite build
来源：http://ky.shxzukj.cn

[U120] JS：读取环境变量（Vite）
来源：http://et.nszjky.cn

import.meta.env.VITE_API_URL
来源：http://le.shxzskj.cn

================================================================================
来源：http://lq.asd995.cn

统计汇总
来源：http://ax.yuexingan06.cn

================================================================================
来源：http://pm.jctech888.com.cn

按语言统计（条）：
来源：http://je.lnxyls.cn

Python ......... 252
来源：http://lb.bookmarksfly.cn

PHP ............ 252
来源：http://co.nszjky.cn

JavaScript ..... 252
来源：http://yv.chemitech.net.cn

TypeScript ..... 212
来源：http://wx.shtwfgs.cn

Java ........... 212
来源：http://pw.nicolike.cn

Go ............. 212
来源：http://fg.nicolike.cn

Ruby ........... 212
来源：http://al.jctech888.com.cn

C# ............. 212
来源：http://bg.newstarts.cn

C .............. 30
来源：http://ah.yuntaijiaju.cn

C++ ............ 30
来源：http://lw.9csxet.cn

SQL ............ 90
来源：http://xn.9csxet.cn

Bash ........... 80
来源：http://zg.yuntaijiaju.cn

Kotlin ......... 15
来源：http://xn.gzmigu.cn

Swift .......... 15
来源：http://zr.szxytkj.cn

Lua ............ 10
来源：http://fd.lnxyls.cn

Perl ........... 10
来源：http://xc.jianghongdianzi.cn

Scala .......... 10
来源：http://yk.shxzukj.cn

------------------------------------
来源：http://xh.lnxyls.cn

合计 ........... 2106 条
来源：http://fs.wgjwhj.cn

按章节统计：
来源：http://uy.muxihuayi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hp.shxzskj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pj.newstarts.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zi.hahajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pw.shxzukj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lc.haigaiapp.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ot.huixinmuqiang.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://te.panjiajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gp.shxzskj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ze.muxihuayi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tj.shtwfgs.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ws.asd995.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://oq.panjiajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gy.newstarts.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://eh.shxzskj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lo.jianghongdianzi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pu.shtwfgs.cn

Q SQL 专题                              90
来源：http://hz.521024.cn

R Bash 专题                             80
来源：http://vb.huanxung.cn

S C / C++ 专题                          60
来源：http://jn.newstarts.cn

T 其他语言补充                          60
来源：http://yw.huanxung.cn

U 高频实用片段                         120
来源：http://dx.haigaiapp.cn

------------------------------------
来源：http://uf.bjjhwx.cn

合计                                  2106 条
来源：http://nh.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://or.lnxyls.cn

使用提醒
来源：http://bf.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://qb.bjjhwx.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kn.9csxet.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cp.panjiajie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wh.9csxet.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vh.shtwfgs.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jt.shxzukj.cn

—— 文件结束 ——
来源：http://ct.panjiajie.cn

================================================================================
来源：http://km.chemitech.net.cn

程序语言常见例子速查手册（2024 版）
来源：http://fk.yuntaijiaju.cn

Common Programming Examples Cheat Book
来源：http://ca.gzmigu.cn

================================================================================
来源：http://os.jctech888.com.cn

【收录内容】
来源：http://xd.jianghongdianzi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ur.jctech888.com.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ya.huixinmuqiang.cn

SQL · Bash · C · C++
来源：http://gt.shxzskj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qz.521024.cn

【使用说明】
来源：http://tu.hahajie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ux.bjjhwx.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nw.muxihuayi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mz.asd995.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://po.shtwfgs.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ah.huanxung.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yr.panjiajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ib.jctech888.com.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lr.szsharing.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ts.shxzskj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://md.9csxet.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://sf.newstarts.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tx.jianghongdianzi.cn

【文件统计】
来源：http://gl.szsharing.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ko.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://qc.lnxyls.cn

目  录
来源：http://zl.nicolike.cn

--------------------------------------------------------------------------------
来源：http://zp.shxzukj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://af.muxihuayi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://in.521024.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cm.wgjwhj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tp.hahajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jj.szsharing.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kt.lnxyls.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://iu.nicolike.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pk.panjiajie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cy.asd995.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qs.hnjuh.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://me.521024.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pe.9csxet.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zo.521024.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ct.shtwfgs.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xx.nszjky.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wk.9csxet.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sv.haigaiapp.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://mb.hnjuh.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jo.521024.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mr.nicolike.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hy.chemitech.net.cn

================================================================================
来源：http://gx.shtwfgs.cn

A. 基础语法与类型
来源：http://if.shxzukj.cn

================================================================================
来源：http://te.muxihuayi.cn

[A01] Hello World
来源：http://mt.jctech888.com.cn

Py:   print("Hello, World!")
来源：http://um.yuexingan06.cn

PHP:  echo "Hello, World!";
来源：http://xm.521024.cn

JS:   console.log("Hello, World!");
来源：http://pa.yuntaijiaju.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mb.jianghongdianzi.cn

Java: System.out.println("Hello, World!");
来源：http://yc.hnjuh.cn

Go:   fmt.Println("Hello, World!")
来源：http://sx.szsharing.cn

Ruby: puts "Hello, World!"
来源：http://zd.wgjwhj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xl.nszjky.cn

[A02] 变量声明与赋值
来源：http://xc.nicolike.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gi.gzmigu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://uh.bjjhwx.cn

JS:   let name = "Alex"; const age = 20;
来源：http://mq.haigaiapp.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ls.newstarts.cn

Java: String name = "Alex"; int age = 20;
来源：http://il.nszjky.cn

Go:   name := "Alex"; age := 20
来源：http://yd.yuexingan06.cn

Ruby: name = "Alex"; age = 20
来源：http://pe.huanxung.cn

C#:   string name = "Alex"; int age = 20;
来源：http://gv.shxzskj.cn

[A03] 常量定义
来源：http://lz.huanxung.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zf.yuexingan06.cn

PHP:  const PI = 3.14159;
来源：http://nb.yuntaijiaju.cn

JS:   const PI = 3.14159;
来源：http://ig.huixinmuqiang.cn

TS:   const PI: number = 3.14159;
来源：http://dn.521024.cn

Java: static final double PI = 3.14159;
来源：http://yc.jianghongdianzi.cn

Go:   const PI = 3.14159
来源：http://pw.panjiajie.cn

Ruby: PI = 3.14159
来源：http://dp.hnjuh.cn

C#:   const double PI = 3.14159;
来源：http://co.bjjhwx.cn

[A04] 判断变量类型
来源：http://ib.hahajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://lr.panjiajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bc.asd995.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mc.nszjky.cn

TS:   typeof x; x instanceof Date
来源：http://jo.newstarts.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vq.asd995.cn

Go:   reflect.TypeOf(x).Name()
来源：http://zx.521024.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://lj.muxihuayi.cn

C#:   x.GetType().Name; x is int
来源：http://xi.newstarts.cn

[A05] 整数除法与取模
来源：http://dk.colortex.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fe.asd995.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ze.yuntaijiaju.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://so.newstarts.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ia.hnjuh.cn

Java: 7 / 2; 7 % 2
来源：http://ij.szxytkj.cn

Go:   7 / 2; 7 % 2
来源：http://bl.hnjuh.cn

Ruby: 7 / 2; 7 % 2
来源：http://zp.bookmarksfly.cn

C#:   7 / 2; 7 % 2
来源：http://bs.huanxung.cn

[A06] 字符串转数字
来源：http://xp.newstarts.cn

Py:   int("42"); float("3.14")
来源：http://jj.muxihuayi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mf.nicolike.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nr.521024.cn

TS:   parseInt("42", 10); Number("42")
来源：http://bh.panjiajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://se.lnxyls.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gn.jianghongdianzi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fe.shxzskj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kk.lnxyls.cn

[A07] 数字转字符串
来源：http://ee.muxihuayi.cn

Py:   str(42)
来源：http://dd.shxzskj.cn

PHP:  (string) 42; strval(42)
来源：http://lg.bjjhwx.cn

JS:   String(42); (42).toString()
来源：http://tm.nicolike.cn

TS:   String(42)
来源：http://id.9csxet.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://em.szsharing.cn

Go:   strconv.Itoa(42)
来源：http://cb.muxihuayi.cn

Ruby: 42.to_s
来源：http://mu.newstarts.cn

C#:   42.ToString()
来源：http://nn.nszjky.cn

[A08] 取整与四舍五入
来源：http://ft.bjjhwx.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ug.wgjwhj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cy.asd995.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lp.hnjuh.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xe.szxytkj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qm.colortex.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qh.gzmigu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qs.newstarts.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://iu.hnjuh.cn

[A09] 绝对值与最大最小值
来源：http://tq.jianghongdianzi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gd.huixiangedu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lr.wgjwhj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zx.hahajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://dq.newstarts.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://av.newstarts.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://if.newstarts.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://iu.haigaiapp.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ip.bjjhwx.cn


<!-- 参考信息 -->