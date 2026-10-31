代发 wailian999

[U67] PHP：处理文件上传
来源：http://ov.nicolike.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jj.colortex.cn

[U68] PHP：PDO 连接
来源：http://bz.9csxet.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uz.shxzukj.cn

[U69] PHP：PDO 预处理
来源：http://yd.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fr.lnxyls.cn

[U70] PHP：PDO 事务
来源：http://ng.szsharing.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lw.huanxung.cn

[U71] PHP：抛出异常
来源：http://av.shxzskj.cn

throw new RuntimeException("失败", 500);
来源：http://mt.hahajie.cn

[U72] PHP：写错误日志
来源：http://va.bookmarksfly.cn

error_log("失败: " . $e->getMessage());
来源：http://hz.jctech888.com.cn

[U73] PHP：读取 ini 配置
来源：http://yh.szxytkj.cn

parse_ini_file("config.ini", true)
来源：http://ic.szxytkj.cn

[U74] PHP：读取环境变量
来源：http://qe.lnxyls.cn

getenv("APP_ENV") ?: "production"
来源：http://sw.jctech888.com.cn

[U75] PHP：依赖注入
来源：http://cc.chemitech.net.cn

composer require psr/container
来源：http://lc.jianghongdianzi.cn

[U76] PHP：简单路由
来源：http://yg.wgjwhj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xi.yuntaijiaju.cn

[U77] PHP：模板渲染
来源：http://vd.muxihuayi.cn

composer require twig/twig
来源：http://xh.hahajie.cn

[U78] PHP：单元测试
来源：http://vu.nszjky.cn

composer require --dev phpunit/phpunit
来源：http://hy.szxytkj.cn

[U79] PHP：静态分析
来源：http://ol.9csxet.cn

composer require --dev phpstan/phpstan
来源：http://uf.yuntaijiaju.cn

[U80] PHP：代码规范修复
来源：http://zr.muxihuayi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vk.nszjky.cn

[U81] JS：初始化项目
来源：http://ie.huixinmuqiang.cn

npm init -y;  npm i express
来源：http://cp.shtwfgs.cn

[U82] JS：package.json 脚本
来源：http://dj.yuntaijiaju.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nh.shtwfgs.cn

[U83] JS：ES Module 导入导出
来源：http://oa.colortex.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zy.newstarts.cn

[U84] JS：CommonJS 写法
来源：http://xb.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://sq.9csxet.cn

[U85] JS：可选链
来源：http://nk.nicolike.cn

a?.b?.c
来源：http://wr.huixinmuqiang.cn

[U86] JS：空值合并
来源：http://be.panjiajie.cn

a ?? b
来源：http://dw.chemitech.net.cn

[U87] JS：解构默认值
来源：http://vq.nszjky.cn

const { a = 1, b = 2 } = obj;
来源：http://jd.huanxung.cn

[U88] JS：对象展开合并
来源：http://ak.yuntaijiaju.cn

{ ...a, ...b }
来源：http://ah.panjiajie.cn

[U89] JS：数组去重
来源：http://kp.muxihuayi.cn

[...new Set(arr)]
来源：http://lj.szsharing.cn

[U90] JS：数字数组排序
来源：http://sk.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://ta.bjjhwx.cn

[U91] JS：对象键值遍历
来源：http://cw.hahajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://au.bookmarksfly.cn

[U92] JS：深拷贝
来源：http://yk.gzmigu.cn

structuredClone(obj)
来源：http://bm.gzmigu.cn

[U93] JS：模板字符串
来源：http://wj.shtwfgs.cn

`共 ${n} 条`
来源：http://gm.9csxet.cn

[U94] JS：箭头函数
来源：http://mj.huixinmuqiang.cn

const double = x => x * 2;
来源：http://xg.muxihuayi.cn

[U95] JS：Promise 包装
来源：http://oe.jianghongdianzi.cn

new Promise((resolve, reject) => {})
来源：http://xm.gzmigu.cn

[U96] JS：async/await 与异常
来源：http://po.shxzskj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jz.9csxet.cn

[U97] JS：并发请求
来源：http://wm.szsharing.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://sx.huixiangedu.cn

[U98] JS：fetch 带 JSON
来源：http://pp.muxihuayi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yu.huanxung.cn

[U99] JS：事件监听
来源：http://fm.chemitech.net.cn

el.addEventListener("click", e => {})
来源：http://zq.9csxet.cn

[U100] JS：DOM 查询
来源：http://th.bookmarksfly.cn

document.querySelector(".item")
来源：http://ew.9csxet.cn

[U101] JS：classList 操作
来源：http://rs.muxihuayi.cn

el.classList.toggle("active")
来源：http://rp.hnjuh.cn

[U102] JS：本地存储
来源：http://je.jianghongdianzi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://uh.szsharing.cn

[U103] JS：定时器
来源：http://me.yuntaijiaju.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qw.9csxet.cn

[U104] JS：防抖
来源：http://lt.panjiajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bc.colortex.cn

[U105] JS：节流
来源：http://gh.szsharing.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ic.haigaiapp.cn

[U106] JS：日期格式化
来源：http://px.huixiangedu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vp.jianghongdianzi.cn

[U107] JS：数字千分位
来源：http://na.chemitech.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ep.muxihuayi.cn

[U108] JS：随机整数
来源：http://fc.shxzukj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dr.shtwfgs.cn

[U109] JS：数组分组
来源：http://uy.521024.cn

Object.groupBy(arr, x => x.type)
来源：http://uq.bookmarksfly.cn

[U110] JS：数组分块
来源：http://sd.bookmarksfly.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pv.szxytkj.cn

[U111] JS：对象转 Map
来源：http://hr.shxzskj.cn

new Map(Object.entries(obj))
来源：http://dp.gzmigu.cn

[U112] JS：字符串补位
来源：http://hy.yuntaijiaju.cn

"7".padStart(3, "0")
来源：http://nn.shtwfgs.cn

[U113] JS：正则替换全部
来源：http://vs.521024.cn

s.replaceAll("a", "b")
来源：http://mm.jctech888.com.cn

[U114] JS：JSON 深比较
来源：http://xj.panjiajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pw.muxihuayi.cn

[U115] JS：生成 UUID
来源：http://hl.gzmigu.cn

crypto.randomUUID()
来源：http://vt.gzmigu.cn

[U116] JS：类型检查（JSDoc）
来源：http://dq.muxihuayi.cn

/** @param {string} name */ function f(name) {}
来源：http://pd.yuexingan06.cn

[U117] JS：单元测试
来源：http://pr.gzmigu.cn

npm i -D vitest;  npx vitest
来源：http://ez.colortex.cn

[U118] JS：开发服务器
来源：http://jm.shxzskj.cn

npm i -D vite;  npx vite
来源：http://cb.hnjuh.cn

[U119] JS：生产构建
来源：http://me.wgjwhj.cn

npx vite build
来源：http://ab.lnxyls.cn

[U120] JS：读取环境变量（Vite）
来源：http://fn.hahajie.cn

import.meta.env.VITE_API_URL
来源：http://ff.asd995.cn

================================================================================
来源：http://ys.jctech888.com.cn

统计汇总
来源：http://ll.jctech888.com.cn

================================================================================
来源：http://vx.wgjwhj.cn

按语言统计（条）：
来源：http://ro.bookmarksfly.cn

Python ......... 252
来源：http://nr.9csxet.cn

PHP ............ 252
来源：http://xw.521024.cn

JavaScript ..... 252
来源：http://zr.nszjky.cn

TypeScript ..... 212
来源：http://bv.nszjky.cn

Java ........... 212
来源：http://js.szsharing.cn

Go ............. 212
来源：http://zu.shxzskj.cn

Ruby ........... 212
来源：http://ll.9csxet.cn

C# ............. 212
来源：http://cq.shxzukj.cn

C .............. 30
来源：http://xg.colortex.cn

C++ ............ 30
来源：http://gu.shxzskj.cn

SQL ............ 90
来源：http://or.nszjky.cn

Bash ........... 80
来源：http://hr.panjiajie.cn

Kotlin ......... 15
来源：http://yz.chemitech.net.cn

Swift .......... 15
来源：http://mg.jianghongdianzi.cn

Lua ............ 10
来源：http://kr.asd995.cn

Perl ........... 10
来源：http://pb.huixinmuqiang.cn

Scala .......... 10
来源：http://jo.jctech888.com.cn

------------------------------------
来源：http://yu.asd995.cn

合计 ........... 2106 条
来源：http://du.huixiangedu.cn

按章节统计：
来源：http://ua.shxzskj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bq.bookmarksfly.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://eq.hnjuh.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://op.jianghongdianzi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ib.nicolike.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rm.huanxung.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tv.521024.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yp.yuexingan06.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gz.yuntaijiaju.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yu.jctech888.com.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://an.hnjuh.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jw.asd995.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://oc.wgjwhj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wl.shtwfgs.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nc.chemitech.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ca.asd995.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hs.huixiangedu.cn

Q SQL 专题                              90
来源：http://fc.huixinmuqiang.cn

R Bash 专题                             80
来源：http://vb.bjjhwx.cn

S C / C++ 专题                          60
来源：http://vt.shxzskj.cn

T 其他语言补充                          60
来源：http://to.szxytkj.cn

U 高频实用片段                         120
来源：http://ri.lnxyls.cn

------------------------------------
来源：http://zl.szxytkj.cn

合计                                  2106 条
来源：http://lh.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://gg.9csxet.cn

使用提醒
来源：http://yl.nszjky.cn

--------------------------------------------------------------------------------
来源：http://om.yuexingan06.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pj.bjjhwx.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://oq.lnxyls.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wi.hahajie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://yt.9csxet.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://es.muxihuayi.cn

—— 文件结束 ——
来源：http://vr.jctech888.com.cn

================================================================================
来源：http://jl.chemitech.net.cn

程序语言常见例子速查手册（2024 版）
来源：http://mz.szxytkj.cn

Common Programming Examples Cheat Book
来源：http://tk.colortex.cn

================================================================================
来源：http://mr.gzmigu.cn

【收录内容】
来源：http://pd.nszjky.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://hd.yuexingan06.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pp.szxytkj.cn

SQL · Bash · C · C++
来源：http://qo.huixinmuqiang.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qb.chemitech.net.cn

【使用说明】
来源：http://tw.bookmarksfly.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ze.521024.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://an.jctech888.com.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pk.shxzukj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ke.huanxung.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://hn.nszjky.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ur.colortex.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://du.hnjuh.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://an.szsharing.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gz.521024.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://po.nicolike.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ip.colortex.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qv.colortex.cn

【文件统计】
来源：http://bz.jctech888.com.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yg.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://se.hahajie.cn

目  录
来源：http://uh.521024.cn

--------------------------------------------------------------------------------
来源：http://uk.521024.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xa.haigaiapp.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lq.szsharing.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ea.shxzukj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yl.huixinmuqiang.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tx.huixinmuqiang.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://sa.hahajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wp.colortex.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kx.jianghongdianzi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sc.hnjuh.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ls.nicolike.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jn.huanxung.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bl.521024.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qg.wgjwhj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://za.bjjhwx.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jc.yuntaijiaju.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bo.gzmigu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ew.newstarts.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xz.szsharing.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dw.szsharing.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://eh.bjjhwx.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vp.bjjhwx.cn

================================================================================
来源：http://ke.9csxet.cn

A. 基础语法与类型
来源：http://oq.haigaiapp.cn

================================================================================
来源：http://uq.hahajie.cn

[A01] Hello World
来源：http://mc.nicolike.cn

Py:   print("Hello, World!")
来源：http://zq.jctech888.com.cn

PHP:  echo "Hello, World!";
来源：http://wr.shxzskj.cn

JS:   console.log("Hello, World!");
来源：http://xk.hnjuh.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qx.nicolike.cn

Java: System.out.println("Hello, World!");
来源：http://ta.huixinmuqiang.cn

Go:   fmt.Println("Hello, World!")
来源：http://gt.lnxyls.cn

Ruby: puts "Hello, World!"
来源：http://ux.hnjuh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://pn.asd995.cn

[A02] 变量声明与赋值
来源：http://gl.colortex.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qv.lnxyls.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://sl.chemitech.net.cn

JS:   let name = "Alex"; const age = 20;
来源：http://nj.hahajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://oa.huixiangedu.cn

Java: String name = "Alex"; int age = 20;
来源：http://ff.hnjuh.cn

Go:   name := "Alex"; age := 20
来源：http://qh.huanxung.cn

Ruby: name = "Alex"; age = 20
来源：http://ko.asd995.cn

C#:   string name = "Alex"; int age = 20;
来源：http://xt.gzmigu.cn

[A03] 常量定义
来源：http://ha.9csxet.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://la.panjiajie.cn

PHP:  const PI = 3.14159;
来源：http://ir.lnxyls.cn

JS:   const PI = 3.14159;
来源：http://ro.521024.cn

TS:   const PI: number = 3.14159;
来源：http://vv.szxytkj.cn

Java: static final double PI = 3.14159;
来源：http://qt.asd995.cn

Go:   const PI = 3.14159
来源：http://vz.jianghongdianzi.cn

Ruby: PI = 3.14159
来源：http://ee.shtwfgs.cn

C#:   const double PI = 3.14159;
来源：http://wb.panjiajie.cn

[A04] 判断变量类型
来源：http://yq.bjjhwx.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://lz.szsharing.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ab.szsharing.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cg.newstarts.cn

TS:   typeof x; x instanceof Date
来源：http://xj.jianghongdianzi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jn.jianghongdianzi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://dg.yuexingan06.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ud.hahajie.cn

C#:   x.GetType().Name; x is int
来源：http://tb.jianghongdianzi.cn

[A05] 整数除法与取模
来源：http://vu.huixinmuqiang.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qh.shxzukj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://rt.panjiajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dh.521024.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://au.yuntaijiaju.cn

Java: 7 / 2; 7 % 2
来源：http://mp.shtwfgs.cn

Go:   7 / 2; 7 % 2
来源：http://rp.shtwfgs.cn

Ruby: 7 / 2; 7 % 2
来源：http://lm.9csxet.cn

C#:   7 / 2; 7 % 2
来源：http://dg.9csxet.cn

[A06] 字符串转数字
来源：http://bq.huixiangedu.cn

Py:   int("42"); float("3.14")
来源：http://tv.muxihuayi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bi.9csxet.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mi.shxzskj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://fq.521024.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gu.szxytkj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://li.jianghongdianzi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://op.newstarts.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qm.jctech888.com.cn

[A07] 数字转字符串
来源：http://hm.yuexingan06.cn

Py:   str(42)
来源：http://xw.huixiangedu.cn

PHP:  (string) 42; strval(42)
来源：http://yu.yuntaijiaju.cn

JS:   String(42); (42).toString()
来源：http://sy.bjjhwx.cn

TS:   String(42)
来源：http://nj.gzmigu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ki.shxzukj.cn

Go:   strconv.Itoa(42)
来源：http://ke.haigaiapp.cn

Ruby: 42.to_s
来源：http://ee.yuntaijiaju.cn

C#:   42.ToString()
来源：http://nz.szxytkj.cn

[A08] 取整与四舍五入
来源：http://pr.szsharing.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vw.lnxyls.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://go.huixinmuqiang.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ax.chemitech.net.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://es.bjjhwx.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sy.bjjhwx.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gc.szxytkj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://bm.chemitech.net.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dm.yuntaijiaju.cn

[A09] 绝对值与最大最小值
来源：http://ud.szsharing.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://et.hnjuh.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wd.shxzskj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lm.shxzskj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mt.gzmigu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://va.lnxyls.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://um.chemitech.net.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://eq.huanxung.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gq.yuexingan06.cn

[A10] 生成随机数
来源：http://sb.yuntaijiaju.cn

Py:   import random; random.randint(1, 100)
来源：http://ck.jctech888.com.cn

PHP:  random_int(1, 100);
来源：http://ft.muxihuayi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xg.gzmigu.cn


<!-- 参考信息 -->