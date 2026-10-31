代发 wailian999

[U63] PHP：文件读写
来源：http://df.yuexingan06.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cx.colortex.cn

[U64] PHP：目录遍历
来源：http://me.muxihuayi.cn

glob("dir/*.php");  scandir("dir");
来源：http://am.jianghongdianzi.cn

[U65] PHP：会话
来源：http://fi.jctech888.com.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://jq.shxzskj.cn

[U66] PHP：设置 Cookie
来源：http://kr.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ym.shtwfgs.cn

[U67] PHP：处理文件上传
来源：http://db.huixiangedu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xl.nszjky.cn

[U68] PHP：PDO 连接
来源：http://kq.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pn.yuexingan06.cn

[U69] PHP：PDO 预处理
来源：http://qf.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://df.yuntaijiaju.cn

[U70] PHP：PDO 事务
来源：http://sv.hahajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qo.yuntaijiaju.cn

[U71] PHP：抛出异常
来源：http://ph.9csxet.cn

throw new RuntimeException("失败", 500);
来源：http://tj.bookmarksfly.cn

[U72] PHP：写错误日志
来源：http://lt.shxzukj.cn

error_log("失败: " . $e->getMessage());
来源：http://ol.chemitech.net.cn

[U73] PHP：读取 ini 配置
来源：http://nn.panjiajie.cn

parse_ini_file("config.ini", true)
来源：http://ch.lnxyls.cn

[U74] PHP：读取环境变量
来源：http://fp.hahajie.cn

getenv("APP_ENV") ?: "production"
来源：http://we.hahajie.cn

[U75] PHP：依赖注入
来源：http://nn.huixiangedu.cn

composer require psr/container
来源：http://ln.szxytkj.cn

[U76] PHP：简单路由
来源：http://sl.yuntaijiaju.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ge.haigaiapp.cn

[U77] PHP：模板渲染
来源：http://ad.huixinmuqiang.cn

composer require twig/twig
来源：http://xn.gzmigu.cn

[U78] PHP：单元测试
来源：http://zj.huanxung.cn

composer require --dev phpunit/phpunit
来源：http://xg.nicolike.cn

[U79] PHP：静态分析
来源：http://lo.yuexingan06.cn

composer require --dev phpstan/phpstan
来源：http://kk.muxihuayi.cn

[U80] PHP：代码规范修复
来源：http://uo.lnxyls.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sg.jctech888.com.cn

[U81] JS：初始化项目
来源：http://ix.haigaiapp.cn

npm init -y;  npm i express
来源：http://of.wgjwhj.cn

[U82] JS：package.json 脚本
来源：http://tu.yuexingan06.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jz.yuntaijiaju.cn

[U83] JS：ES Module 导入导出
来源：http://yz.jianghongdianzi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rx.huanxung.cn

[U84] JS：CommonJS 写法
来源：http://ds.gzmigu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://us.shxzskj.cn

[U85] JS：可选链
来源：http://fm.nszjky.cn

a?.b?.c
来源：http://kc.colortex.cn

[U86] JS：空值合并
来源：http://be.szsharing.cn

a ?? b
来源：http://qs.chemitech.net.cn

[U87] JS：解构默认值
来源：http://cw.yuexingan06.cn

const { a = 1, b = 2 } = obj;
来源：http://au.hahajie.cn

[U88] JS：对象展开合并
来源：http://pr.yuntaijiaju.cn

{ ...a, ...b }
来源：http://vn.nicolike.cn

[U89] JS：数组去重
来源：http://fg.asd995.cn

[...new Set(arr)]
来源：http://wf.bookmarksfly.cn

[U90] JS：数字数组排序
来源：http://gy.chemitech.net.cn

[...arr].sort((a, b) => a - b)
来源：http://da.newstarts.cn

[U91] JS：对象键值遍历
来源：http://yq.jctech888.com.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ui.shxzskj.cn

[U92] JS：深拷贝
来源：http://qk.gzmigu.cn

structuredClone(obj)
来源：http://go.chemitech.net.cn

[U93] JS：模板字符串
来源：http://yh.huanxung.cn

`共 ${n} 条`
来源：http://vt.521024.cn

[U94] JS：箭头函数
来源：http://fq.huixiangedu.cn

const double = x => x * 2;
来源：http://ag.hahajie.cn

[U95] JS：Promise 包装
来源：http://ck.nicolike.cn

new Promise((resolve, reject) => {})
来源：http://xw.jianghongdianzi.cn

[U96] JS：async/await 与异常
来源：http://sp.chemitech.net.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://db.newstarts.cn

[U97] JS：并发请求
来源：http://as.hahajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zk.bookmarksfly.cn

[U98] JS：fetch 带 JSON
来源：http://iu.shxzukj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ec.shxzukj.cn

[U99] JS：事件监听
来源：http://di.haigaiapp.cn

el.addEventListener("click", e => {})
来源：http://xi.szxytkj.cn

[U100] JS：DOM 查询
来源：http://qe.huixiangedu.cn

document.querySelector(".item")
来源：http://rr.shxzskj.cn

[U101] JS：classList 操作
来源：http://is.lnxyls.cn

el.classList.toggle("active")
来源：http://tv.jianghongdianzi.cn

[U102] JS：本地存储
来源：http://zi.muxihuayi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://af.newstarts.cn

[U103] JS：定时器
来源：http://hj.shxzskj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gb.colortex.cn

[U104] JS：防抖
来源：http://pq.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bm.newstarts.cn

[U105] JS：节流
来源：http://wn.huixinmuqiang.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ro.colortex.cn

[U106] JS：日期格式化
来源：http://yu.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://px.huixinmuqiang.cn

[U107] JS：数字千分位
来源：http://ne.colortex.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ys.shxzskj.cn

[U108] JS：随机整数
来源：http://lf.yuexingan06.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fl.jianghongdianzi.cn

[U109] JS：数组分组
来源：http://nm.521024.cn

Object.groupBy(arr, x => x.type)
来源：http://tn.nszjky.cn

[U110] JS：数组分块
来源：http://oh.gzmigu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dk.nszjky.cn

[U111] JS：对象转 Map
来源：http://pr.huixinmuqiang.cn

new Map(Object.entries(obj))
来源：http://dg.asd995.cn

[U112] JS：字符串补位
来源：http://xi.9csxet.cn

"7".padStart(3, "0")
来源：http://ln.chemitech.net.cn

[U113] JS：正则替换全部
来源：http://zs.wgjwhj.cn

s.replaceAll("a", "b")
来源：http://da.wgjwhj.cn

[U114] JS：JSON 深比较
来源：http://ip.wgjwhj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vy.haigaiapp.cn

[U115] JS：生成 UUID
来源：http://kt.yuntaijiaju.cn

crypto.randomUUID()
来源：http://vn.shxzukj.cn

[U116] JS：类型检查（JSDoc）
来源：http://vu.hnjuh.cn

/** @param {string} name */ function f(name) {}
来源：http://rx.panjiajie.cn

[U117] JS：单元测试
来源：http://lo.chemitech.net.cn

npm i -D vitest;  npx vitest
来源：http://yx.szxytkj.cn

[U118] JS：开发服务器
来源：http://bg.shxzukj.cn

npm i -D vite;  npx vite
来源：http://ap.hnjuh.cn

[U119] JS：生产构建
来源：http://hq.yuexingan06.cn

npx vite build
来源：http://zy.bookmarksfly.cn

[U120] JS：读取环境变量（Vite）
来源：http://ar.asd995.cn

import.meta.env.VITE_API_URL
来源：http://bo.huanxung.cn

================================================================================
来源：http://nx.yuntaijiaju.cn

统计汇总
来源：http://ec.asd995.cn

================================================================================
来源：http://lq.hnjuh.cn

按语言统计（条）：
来源：http://mp.colortex.cn

Python ......... 252
来源：http://np.shxzukj.cn

PHP ............ 252
来源：http://jv.hnjuh.cn

JavaScript ..... 252
来源：http://pg.shxzukj.cn

TypeScript ..... 212
来源：http://qq.lnxyls.cn

Java ........... 212
来源：http://ln.szxytkj.cn

Go ............. 212
来源：http://vf.yuntaijiaju.cn

Ruby ........... 212
来源：http://zd.yuexingan06.cn

C# ............. 212
来源：http://df.chemitech.net.cn

C .............. 30
来源：http://uo.521024.cn

C++ ............ 30
来源：http://ol.chemitech.net.cn

SQL ............ 90
来源：http://qj.yuexingan06.cn

Bash ........... 80
来源：http://is.nicolike.cn

Kotlin ......... 15
来源：http://jd.huixinmuqiang.cn

Swift .......... 15
来源：http://gl.huanxung.cn

Lua ............ 10
来源：http://ly.chemitech.net.cn

Perl ........... 10
来源：http://lf.szxytkj.cn

Scala .......... 10
来源：http://zv.bjjhwx.cn

------------------------------------
来源：http://dc.yuexingan06.cn

合计 ........... 2106 条
来源：http://su.huixiangedu.cn

按章节统计：
来源：http://ux.muxihuayi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tu.hnjuh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uu.chemitech.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://oo.jctech888.com.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ue.yuntaijiaju.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cl.haigaiapp.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://to.huanxung.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ss.huixiangedu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hf.shtwfgs.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zy.haigaiapp.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gg.9csxet.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ll.wgjwhj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dt.szsharing.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sv.huanxung.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gj.nicolike.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ac.shxzukj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wd.yuexingan06.cn

Q SQL 专题                              90
来源：http://pc.shxzukj.cn

R Bash 专题                             80
来源：http://yn.9csxet.cn

S C / C++ 专题                          60
来源：http://ab.shxzskj.cn

T 其他语言补充                          60
来源：http://nt.muxihuayi.cn

U 高频实用片段                         120
来源：http://ac.haigaiapp.cn

------------------------------------
来源：http://fo.nszjky.cn

合计                                  2106 条
来源：http://bs.nicolike.cn

--------------------------------------------------------------------------------
来源：http://ft.9csxet.cn

使用提醒
来源：http://ib.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://vb.nszjky.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ks.shxzukj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mg.nszjky.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ed.shtwfgs.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://lq.lnxyls.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ph.hahajie.cn

—— 文件结束 ——
来源：http://lx.521024.cn

================================================================================
来源：http://ru.shtwfgs.cn

程序语言常见例子速查手册（2024 版）
来源：http://wr.nicolike.cn

Common Programming Examples Cheat Book
来源：http://mc.bjjhwx.cn

================================================================================
来源：http://ai.haigaiapp.cn

【收录内容】
来源：http://aq.muxihuayi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://yd.nszjky.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pl.yuexingan06.cn

SQL · Bash · C · C++
来源：http://pz.9csxet.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://is.newstarts.cn

【使用说明】
来源：http://ui.huanxung.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://io.chemitech.net.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://sk.nicolike.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lg.newstarts.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jc.muxihuayi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://no.jianghongdianzi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jz.521024.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zh.9csxet.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wt.jctech888.com.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://no.bookmarksfly.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://my.wgjwhj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ia.jctech888.com.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xz.nicolike.cn

【文件统计】
来源：http://xa.gzmigu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yl.newstarts.cn

--------------------------------------------------------------------------------
来源：http://pd.huixiangedu.cn

目  录
来源：http://mc.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://ix.9csxet.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tq.shxzukj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zp.szxytkj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fv.shxzskj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ej.szsharing.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fh.muxihuayi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yv.asd995.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bl.wgjwhj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://na.521024.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xt.bjjhwx.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nc.szxytkj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ht.nicolike.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xa.bookmarksfly.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fy.chemitech.net.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wb.bjjhwx.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://if.lnxyls.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://uu.muxihuayi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bp.szxytkj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wx.hahajie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://aq.nszjky.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rj.bookmarksfly.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vt.9csxet.cn

================================================================================
来源：http://gq.nszjky.cn

A. 基础语法与类型
来源：http://tk.hahajie.cn

================================================================================
来源：http://zu.yuexingan06.cn

[A01] Hello World
来源：http://ku.huixinmuqiang.cn

Py:   print("Hello, World!")
来源：http://ic.bjjhwx.cn

PHP:  echo "Hello, World!";
来源：http://jy.lnxyls.cn

JS:   console.log("Hello, World!");
来源：http://th.panjiajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://km.yuntaijiaju.cn

Java: System.out.println("Hello, World!");
来源：http://ro.colortex.cn

Go:   fmt.Println("Hello, World!")
来源：http://wd.yuntaijiaju.cn

Ruby: puts "Hello, World!"
来源：http://fg.9csxet.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zz.colortex.cn

[A02] 变量声明与赋值
来源：http://qu.nszjky.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zk.yuexingan06.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qn.haigaiapp.cn

JS:   let name = "Alex"; const age = 20;
来源：http://wh.lnxyls.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fg.huixiangedu.cn

Java: String name = "Alex"; int age = 20;
来源：http://zm.521024.cn

Go:   name := "Alex"; age := 20
来源：http://ec.haigaiapp.cn

Ruby: name = "Alex"; age = 20
来源：http://sb.gzmigu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://zf.colortex.cn

[A03] 常量定义
来源：http://sd.jianghongdianzi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zb.hahajie.cn

PHP:  const PI = 3.14159;
来源：http://oy.muxihuayi.cn

JS:   const PI = 3.14159;
来源：http://za.asd995.cn

TS:   const PI: number = 3.14159;
来源：http://kw.colortex.cn

Java: static final double PI = 3.14159;
来源：http://fl.chemitech.net.cn

Go:   const PI = 3.14159
来源：http://xp.huixiangedu.cn

Ruby: PI = 3.14159
来源：http://hi.yuexingan06.cn

C#:   const double PI = 3.14159;
来源：http://cr.nicolike.cn

[A04] 判断变量类型
来源：http://qr.hnjuh.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ji.nszjky.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ib.yuexingan06.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ap.haigaiapp.cn

TS:   typeof x; x instanceof Date
来源：http://ip.gzmigu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tw.521024.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hi.colortex.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://jh.huanxung.cn

C#:   x.GetType().Name; x is int
来源：http://wy.bookmarksfly.cn

[A05] 整数除法与取模
来源：http://rb.bookmarksfly.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://md.shtwfgs.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://cr.gzmigu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://io.huixiangedu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gi.szsharing.cn

Java: 7 / 2; 7 % 2
来源：http://cz.muxihuayi.cn

Go:   7 / 2; 7 % 2
来源：http://tg.yuexingan06.cn

Ruby: 7 / 2; 7 % 2
来源：http://yx.gzmigu.cn

C#:   7 / 2; 7 % 2
来源：http://wi.wgjwhj.cn

[A06] 字符串转数字
来源：http://fj.szsharing.cn

Py:   int("42"); float("3.14")
来源：http://jq.asd995.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fc.yuntaijiaju.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fr.lnxyls.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ge.521024.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cy.wgjwhj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xy.bjjhwx.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zm.hahajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mq.bookmarksfly.cn

[A07] 数字转字符串
来源：http://oc.nszjky.cn

Py:   str(42)
来源：http://cr.huixiangedu.cn

PHP:  (string) 42; strval(42)
来源：http://vd.bjjhwx.cn

JS:   String(42); (42).toString()
来源：http://kn.shtwfgs.cn

TS:   String(42)
来源：http://qs.colortex.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xq.bookmarksfly.cn

Go:   strconv.Itoa(42)
来源：http://bl.shtwfgs.cn

Ruby: 42.to_s
来源：http://ef.shxzukj.cn

C#:   42.ToString()
来源：http://my.panjiajie.cn

[A08] 取整与四舍五入
来源：http://yq.shxzskj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mx.nszjky.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yr.shxzskj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zl.colortex.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gq.hahajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lu.9csxet.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vl.chemitech.net.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ix.jianghongdianzi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yr.yuntaijiaju.cn

[A09] 绝对值与最大最小值
来源：http://vl.huixiangedu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rl.newstarts.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qj.panjiajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bg.yuexingan06.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zq.nicolike.cn


<!-- 参考信息 -->