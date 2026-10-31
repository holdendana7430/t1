代发 wailian999

[U63] PHP：文件读写
来源：http://ok.huixiangedu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nv.bookmarksfly.cn

[U64] PHP：目录遍历
来源：http://xd.jianghongdianzi.cn

glob("dir/*.php");  scandir("dir");
来源：http://uw.huanxung.cn

[U65] PHP：会话
来源：http://wo.haigaiapp.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cy.haigaiapp.cn

[U66] PHP：设置 Cookie
来源：http://wc.haigaiapp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rs.jctech888.com.cn

[U67] PHP：处理文件上传
来源：http://bi.521024.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pa.yuntaijiaju.cn

[U68] PHP：PDO 连接
来源：http://sb.panjiajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vh.chemitech.net.cn

[U69] PHP：PDO 预处理
来源：http://df.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://af.szxytkj.cn

[U70] PHP：PDO 事务
来源：http://lh.colortex.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://im.shtwfgs.cn

[U71] PHP：抛出异常
来源：http://pc.hnjuh.cn

throw new RuntimeException("失败", 500);
来源：http://qe.szsharing.cn

[U72] PHP：写错误日志
来源：http://uk.chemitech.net.cn

error_log("失败: " . $e->getMessage());
来源：http://mo.9csxet.cn

[U73] PHP：读取 ini 配置
来源：http://fs.huixinmuqiang.cn

parse_ini_file("config.ini", true)
来源：http://gt.wgjwhj.cn

[U74] PHP：读取环境变量
来源：http://da.hahajie.cn

getenv("APP_ENV") ?: "production"
来源：http://gd.szsharing.cn

[U75] PHP：依赖注入
来源：http://uk.haigaiapp.cn

composer require psr/container
来源：http://xc.newstarts.cn

[U76] PHP：简单路由
来源：http://nk.shtwfgs.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cu.hnjuh.cn

[U77] PHP：模板渲染
来源：http://zu.huixinmuqiang.cn

composer require twig/twig
来源：http://js.muxihuayi.cn

[U78] PHP：单元测试
来源：http://is.huanxung.cn

composer require --dev phpunit/phpunit
来源：http://yg.chemitech.net.cn

[U79] PHP：静态分析
来源：http://fd.huanxung.cn

composer require --dev phpstan/phpstan
来源：http://nz.jctech888.com.cn

[U80] PHP：代码规范修复
来源：http://tj.521024.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ob.newstarts.cn

[U81] JS：初始化项目
来源：http://io.nszjky.cn

npm init -y;  npm i express
来源：http://gn.yuntaijiaju.cn

[U82] JS：package.json 脚本
来源：http://rn.hahajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wr.jianghongdianzi.cn

[U83] JS：ES Module 导入导出
来源：http://zv.jctech888.com.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bm.shxzskj.cn

[U84] JS：CommonJS 写法
来源：http://li.bjjhwx.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xd.huanxung.cn

[U85] JS：可选链
来源：http://yj.huanxung.cn

a?.b?.c
来源：http://fe.hahajie.cn

[U86] JS：空值合并
来源：http://ol.newstarts.cn

a ?? b
来源：http://lf.huixiangedu.cn

[U87] JS：解构默认值
来源：http://wt.bjjhwx.cn

const { a = 1, b = 2 } = obj;
来源：http://up.nszjky.cn

[U88] JS：对象展开合并
来源：http://et.szsharing.cn

{ ...a, ...b }
来源：http://hz.panjiajie.cn

[U89] JS：数组去重
来源：http://yn.haigaiapp.cn

[...new Set(arr)]
来源：http://oc.chemitech.net.cn

[U90] JS：数字数组排序
来源：http://ot.521024.cn

[...arr].sort((a, b) => a - b)
来源：http://vi.9csxet.cn

[U91] JS：对象键值遍历
来源：http://bn.jctech888.com.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://og.shxzskj.cn

[U92] JS：深拷贝
来源：http://bp.colortex.cn

structuredClone(obj)
来源：http://zr.nicolike.cn

[U93] JS：模板字符串
来源：http://wo.newstarts.cn

`共 ${n} 条`
来源：http://sk.nszjky.cn

[U94] JS：箭头函数
来源：http://tv.asd995.cn

const double = x => x * 2;
来源：http://ku.yuexingan06.cn

[U95] JS：Promise 包装
来源：http://xt.hnjuh.cn

new Promise((resolve, reject) => {})
来源：http://vo.chemitech.net.cn

[U96] JS：async/await 与异常
来源：http://zh.newstarts.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tv.yuntaijiaju.cn

[U97] JS：并发请求
来源：http://qf.gzmigu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://as.huixinmuqiang.cn

[U98] JS：fetch 带 JSON
来源：http://cp.hahajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://no.hahajie.cn

[U99] JS：事件监听
来源：http://xj.jctech888.com.cn

el.addEventListener("click", e => {})
来源：http://xm.haigaiapp.cn

[U100] JS：DOM 查询
来源：http://jo.shxzukj.cn

document.querySelector(".item")
来源：http://oc.huixinmuqiang.cn

[U101] JS：classList 操作
来源：http://pe.chemitech.net.cn

el.classList.toggle("active")
来源：http://ar.yuntaijiaju.cn

[U102] JS：本地存储
来源：http://rq.yuexingan06.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bz.hnjuh.cn

[U103] JS：定时器
来源：http://ln.wgjwhj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qn.bookmarksfly.cn

[U104] JS：防抖
来源：http://sn.shtwfgs.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://so.shxzukj.cn

[U105] JS：节流
来源：http://ei.bookmarksfly.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wx.jianghongdianzi.cn

[U106] JS：日期格式化
来源：http://ze.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hc.bookmarksfly.cn

[U107] JS：数字千分位
来源：http://xm.bookmarksfly.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ez.yuexingan06.cn

[U108] JS：随机整数
来源：http://oq.huanxung.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rj.yuexingan06.cn

[U109] JS：数组分组
来源：http://li.lnxyls.cn

Object.groupBy(arr, x => x.type)
来源：http://xi.hahajie.cn

[U110] JS：数组分块
来源：http://fq.lnxyls.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hy.hnjuh.cn

[U111] JS：对象转 Map
来源：http://ew.huixiangedu.cn

new Map(Object.entries(obj))
来源：http://to.haigaiapp.cn

[U112] JS：字符串补位
来源：http://do.shxzukj.cn

"7".padStart(3, "0")
来源：http://ue.hahajie.cn

[U113] JS：正则替换全部
来源：http://am.wgjwhj.cn

s.replaceAll("a", "b")
来源：http://yv.hnjuh.cn

[U114] JS：JSON 深比较
来源：http://km.haigaiapp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://uv.jianghongdianzi.cn

[U115] JS：生成 UUID
来源：http://ch.bookmarksfly.cn

crypto.randomUUID()
来源：http://ge.szsharing.cn

[U116] JS：类型检查（JSDoc）
来源：http://rd.nicolike.cn

/** @param {string} name */ function f(name) {}
来源：http://mv.huanxung.cn

[U117] JS：单元测试
来源：http://zn.szxytkj.cn

npm i -D vitest;  npx vitest
来源：http://ax.yuntaijiaju.cn

[U118] JS：开发服务器
来源：http://ok.huanxung.cn

npm i -D vite;  npx vite
来源：http://no.521024.cn

[U119] JS：生产构建
来源：http://eo.lnxyls.cn

npx vite build
来源：http://cn.jctech888.com.cn

[U120] JS：读取环境变量（Vite）
来源：http://ge.9csxet.cn

import.meta.env.VITE_API_URL
来源：http://kw.hnjuh.cn

================================================================================
来源：http://zs.lnxyls.cn

统计汇总
来源：http://ec.jianghongdianzi.cn

================================================================================
来源：http://hq.wgjwhj.cn

按语言统计（条）：
来源：http://wa.jctech888.com.cn

Python ......... 252
来源：http://zv.wgjwhj.cn

PHP ............ 252
来源：http://fv.nicolike.cn

JavaScript ..... 252
来源：http://rn.nicolike.cn

TypeScript ..... 212
来源：http://wm.9csxet.cn

Java ........... 212
来源：http://al.shtwfgs.cn

Go ............. 212
来源：http://tz.huixinmuqiang.cn

Ruby ........... 212
来源：http://gt.newstarts.cn

C# ............. 212
来源：http://xd.huixiangedu.cn

C .............. 30
来源：http://tx.huixiangedu.cn

C++ ............ 30
来源：http://nx.hnjuh.cn

SQL ............ 90
来源：http://cp.asd995.cn

Bash ........... 80
来源：http://cq.chemitech.net.cn

Kotlin ......... 15
来源：http://ia.yuntaijiaju.cn

Swift .......... 15
来源：http://gp.szsharing.cn

Lua ............ 10
来源：http://nd.wgjwhj.cn

Perl ........... 10
来源：http://fw.haigaiapp.cn

Scala .......... 10
来源：http://cz.jianghongdianzi.cn

------------------------------------
来源：http://lk.szsharing.cn

合计 ........... 2106 条
来源：http://ed.lnxyls.cn

按章节统计：
来源：http://lx.huixiangedu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ih.szxytkj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qm.yuntaijiaju.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qs.panjiajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://oa.jctech888.com.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bi.huanxung.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nm.lnxyls.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ya.bjjhwx.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tn.huixiangedu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vr.521024.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://he.hahajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wt.lnxyls.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nz.muxihuayi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gw.szxytkj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jo.hnjuh.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://en.newstarts.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ve.shxzukj.cn

Q SQL 专题                              90
来源：http://fk.huixiangedu.cn

R Bash 专题                             80
来源：http://ik.panjiajie.cn

S C / C++ 专题                          60
来源：http://gh.szsharing.cn

T 其他语言补充                          60
来源：http://cq.521024.cn

U 高频实用片段                         120
来源：http://dp.shxzskj.cn

------------------------------------
来源：http://lm.szxytkj.cn

合计                                  2106 条
来源：http://qa.hahajie.cn

--------------------------------------------------------------------------------
来源：http://sw.shxzukj.cn

使用提醒
来源：http://jc.asd995.cn

--------------------------------------------------------------------------------
来源：http://qk.bjjhwx.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zj.szxytkj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mu.hnjuh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ac.bjjhwx.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vc.jianghongdianzi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hl.szsharing.cn

—— 文件结束 ——
来源：http://hr.bjjhwx.cn

================================================================================
来源：http://rb.shxzukj.cn

程序语言常见例子速查手册（2024 版）
来源：http://ll.chemitech.net.cn

Common Programming Examples Cheat Book
来源：http://md.nicolike.cn

================================================================================
来源：http://dx.szsharing.cn

【收录内容】
来源：http://ns.bookmarksfly.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vl.huixiangedu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rn.521024.cn

SQL · Bash · C · C++
来源：http://vq.jianghongdianzi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lk.panjiajie.cn

【使用说明】
来源：http://sf.panjiajie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bz.jianghongdianzi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://eo.521024.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://cn.nicolike.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bx.muxihuayi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://nv.bookmarksfly.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bv.chemitech.net.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vx.jianghongdianzi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ni.huanxung.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wc.hnjuh.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tn.haigaiapp.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rj.yuntaijiaju.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://aq.521024.cn

【文件统计】
来源：http://gu.nicolike.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qg.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://yb.huanxung.cn

目  录
来源：http://iv.9csxet.cn

--------------------------------------------------------------------------------
来源：http://yi.yuexingan06.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cw.szsharing.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ow.hahajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pb.szxytkj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qd.jctech888.com.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://he.szsharing.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://or.bjjhwx.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ec.colortex.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ob.huanxung.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xs.chemitech.net.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bt.hahajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xn.shtwfgs.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://eo.nszjky.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fr.hahajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fm.yuntaijiaju.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tj.panjiajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ks.lnxyls.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ks.panjiajie.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ek.nszjky.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://my.haigaiapp.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ak.panjiajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hb.colortex.cn

================================================================================
来源：http://zz.nicolike.cn

A. 基础语法与类型
来源：http://qw.bookmarksfly.cn

================================================================================
来源：http://dg.shxzskj.cn

[A01] Hello World
来源：http://yu.szxytkj.cn

Py:   print("Hello, World!")
来源：http://zf.panjiajie.cn

PHP:  echo "Hello, World!";
来源：http://ro.huixinmuqiang.cn

JS:   console.log("Hello, World!");
来源：http://lv.szxytkj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qn.lnxyls.cn

Java: System.out.println("Hello, World!");
来源：http://cp.shtwfgs.cn

Go:   fmt.Println("Hello, World!")
来源：http://gd.bjjhwx.cn

Ruby: puts "Hello, World!"
来源：http://ty.huanxung.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://yt.colortex.cn

[A02] 变量声明与赋值
来源：http://aq.shxzukj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ox.lnxyls.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://mh.lnxyls.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dl.szxytkj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ow.haigaiapp.cn

Java: String name = "Alex"; int age = 20;
来源：http://sg.wgjwhj.cn

Go:   name := "Alex"; age := 20
来源：http://ov.chemitech.net.cn

Ruby: name = "Alex"; age = 20
来源：http://tb.yuexingan06.cn

C#:   string name = "Alex"; int age = 20;
来源：http://xh.yuntaijiaju.cn

[A03] 常量定义
来源：http://zd.muxihuayi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ot.haigaiapp.cn

PHP:  const PI = 3.14159;
来源：http://zn.bjjhwx.cn

JS:   const PI = 3.14159;
来源：http://zx.shxzukj.cn

TS:   const PI: number = 3.14159;
来源：http://ff.bookmarksfly.cn

Java: static final double PI = 3.14159;
来源：http://av.yuntaijiaju.cn

Go:   const PI = 3.14159
来源：http://pl.bookmarksfly.cn

Ruby: PI = 3.14159
来源：http://lu.newstarts.cn

C#:   const double PI = 3.14159;
来源：http://pf.asd995.cn

[A04] 判断变量类型
来源：http://yo.yuntaijiaju.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://sl.szsharing.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://oz.yuexingan06.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ya.yuexingan06.cn

TS:   typeof x; x instanceof Date
来源：http://ai.szsharing.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kl.bookmarksfly.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ts.lnxyls.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://nc.gzmigu.cn

C#:   x.GetType().Name; x is int
来源：http://oi.shxzukj.cn

[A05] 整数除法与取模
来源：http://nf.shxzskj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qw.huixiangedu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ri.szsharing.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hf.nszjky.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://um.shxzskj.cn

Java: 7 / 2; 7 % 2
来源：http://ai.yuexingan06.cn

Go:   7 / 2; 7 % 2
来源：http://fx.nszjky.cn

Ruby: 7 / 2; 7 % 2
来源：http://tz.lnxyls.cn

C#:   7 / 2; 7 % 2
来源：http://ot.jianghongdianzi.cn

[A06] 字符串转数字
来源：http://gk.yuntaijiaju.cn

Py:   int("42"); float("3.14")
来源：http://rj.lnxyls.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://il.gzmigu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wm.colortex.cn

TS:   parseInt("42", 10); Number("42")
来源：http://tw.bjjhwx.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fx.wgjwhj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fc.521024.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://bd.szsharing.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://id.huanxung.cn

[A07] 数字转字符串
来源：http://uw.jctech888.com.cn

Py:   str(42)
来源：http://ef.chemitech.net.cn

PHP:  (string) 42; strval(42)
来源：http://xz.szxytkj.cn

JS:   String(42); (42).toString()
来源：http://rq.jianghongdianzi.cn

TS:   String(42)
来源：http://mk.asd995.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://fq.bjjhwx.cn

Go:   strconv.Itoa(42)
来源：http://dj.shxzukj.cn

Ruby: 42.to_s
来源：http://rq.nicolike.cn

C#:   42.ToString()
来源：http://gx.wgjwhj.cn

[A08] 取整与四舍五入
来源：http://bo.huixiangedu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gb.huixinmuqiang.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lv.9csxet.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pd.nszjky.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zs.jctech888.com.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cj.jctech888.com.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mw.shxzukj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://vh.shtwfgs.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://uq.yuexingan06.cn

[A09] 绝对值与最大最小值
来源：http://lz.nszjky.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gf.nicolike.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ux.huixinmuqiang.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://te.huixiangedu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kq.asd995.cn


<!-- 参考信息 -->