代发 wailian999

[U61] PHP：正则
来源：http://ja.asd995.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://da.panjiajie.cn

[U62] PHP：日期对象
来源：http://yt.panjiajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kt.asd995.cn

[U63] PHP：文件读写
来源：http://cn.yuntaijiaju.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vd.huixiangedu.cn

[U64] PHP：目录遍历
来源：http://pc.newstarts.cn

glob("dir/*.php");  scandir("dir");
来源：http://ga.9csxet.cn

[U65] PHP：会话
来源：http://ax.nszjky.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://be.huixiangedu.cn

[U66] PHP：设置 Cookie
来源：http://nw.muxihuayi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mb.nszjky.cn

[U67] PHP：处理文件上传
来源：http://hz.asd995.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xi.wgjwhj.cn

[U68] PHP：PDO 连接
来源：http://vy.nicolike.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sy.haigaiapp.cn

[U69] PHP：PDO 预处理
来源：http://fm.gzmigu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rt.521024.cn

[U70] PHP：PDO 事务
来源：http://rz.jianghongdianzi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yb.bookmarksfly.cn

[U71] PHP：抛出异常
来源：http://it.hnjuh.cn

throw new RuntimeException("失败", 500);
来源：http://ss.asd995.cn

[U72] PHP：写错误日志
来源：http://ae.haigaiapp.cn

error_log("失败: " . $e->getMessage());
来源：http://yd.jianghongdianzi.cn

[U73] PHP：读取 ini 配置
来源：http://ux.521024.cn

parse_ini_file("config.ini", true)
来源：http://ih.nicolike.cn

[U74] PHP：读取环境变量
来源：http://nq.muxihuayi.cn

getenv("APP_ENV") ?: "production"
来源：http://bv.chemitech.net.cn

[U75] PHP：依赖注入
来源：http://ms.nszjky.cn

composer require psr/container
来源：http://ry.shxzukj.cn

[U76] PHP：简单路由
来源：http://aw.szsharing.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gx.nicolike.cn

[U77] PHP：模板渲染
来源：http://uy.panjiajie.cn

composer require twig/twig
来源：http://vl.bookmarksfly.cn

[U78] PHP：单元测试
来源：http://iv.bookmarksfly.cn

composer require --dev phpunit/phpunit
来源：http://of.huanxung.cn

[U79] PHP：静态分析
来源：http://yh.haigaiapp.cn

composer require --dev phpstan/phpstan
来源：http://bb.shxzukj.cn

[U80] PHP：代码规范修复
来源：http://fa.wgjwhj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wr.huanxung.cn

[U81] JS：初始化项目
来源：http://pp.jctech888.com.cn

npm init -y;  npm i express
来源：http://vb.shxzukj.cn

[U82] JS：package.json 脚本
来源：http://cr.gzmigu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ri.newstarts.cn

[U83] JS：ES Module 导入导出
来源：http://zu.bjjhwx.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ps.szsharing.cn

[U84] JS：CommonJS 写法
来源：http://wa.nszjky.cn

module.exports = { a };  const { a } = require("./m");
来源：http://us.shtwfgs.cn

[U85] JS：可选链
来源：http://bu.nicolike.cn

a?.b?.c
来源：http://qt.colortex.cn

[U86] JS：空值合并
来源：http://km.yuexingan06.cn

a ?? b
来源：http://rg.nszjky.cn

[U87] JS：解构默认值
来源：http://do.huixiangedu.cn

const { a = 1, b = 2 } = obj;
来源：http://id.nszjky.cn

[U88] JS：对象展开合并
来源：http://hd.huanxung.cn

{ ...a, ...b }
来源：http://zg.jctech888.com.cn

[U89] JS：数组去重
来源：http://ht.nszjky.cn

[...new Set(arr)]
来源：http://tu.newstarts.cn

[U90] JS：数字数组排序
来源：http://ll.nicolike.cn

[...arr].sort((a, b) => a - b)
来源：http://hd.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://jb.szsharing.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mz.shxzukj.cn

[U92] JS：深拷贝
来源：http://zd.panjiajie.cn

structuredClone(obj)
来源：http://oo.521024.cn

[U93] JS：模板字符串
来源：http://bq.huixinmuqiang.cn

`共 ${n} 条`
来源：http://lf.521024.cn

[U94] JS：箭头函数
来源：http://mp.lnxyls.cn

const double = x => x * 2;
来源：http://ra.nszjky.cn

[U95] JS：Promise 包装
来源：http://vb.bookmarksfly.cn

new Promise((resolve, reject) => {})
来源：http://zz.muxihuayi.cn

[U96] JS：async/await 与异常
来源：http://li.521024.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jg.jianghongdianzi.cn

[U97] JS：并发请求
来源：http://wx.nszjky.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://wi.shxzukj.cn

[U98] JS：fetch 带 JSON
来源：http://ih.huixinmuqiang.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xy.bookmarksfly.cn

[U99] JS：事件监听
来源：http://ok.szsharing.cn

el.addEventListener("click", e => {})
来源：http://qi.hnjuh.cn

[U100] JS：DOM 查询
来源：http://ca.bookmarksfly.cn

document.querySelector(".item")
来源：http://qn.panjiajie.cn

[U101] JS：classList 操作
来源：http://cc.lnxyls.cn

el.classList.toggle("active")
来源：http://hj.szxytkj.cn

[U102] JS：本地存储
来源：http://ui.gzmigu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fl.jctech888.com.cn

[U103] JS：定时器
来源：http://vb.muxihuayi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://za.newstarts.cn

[U104] JS：防抖
来源：http://zb.huanxung.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dq.muxihuayi.cn

[U105] JS：节流
来源：http://rl.nicolike.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gf.lnxyls.cn

[U106] JS：日期格式化
来源：http://op.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://so.521024.cn

[U107] JS：数字千分位
来源：http://ls.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yh.bjjhwx.cn

[U108] JS：随机整数
来源：http://yr.chemitech.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sr.nicolike.cn

[U109] JS：数组分组
来源：http://ue.panjiajie.cn

Object.groupBy(arr, x => x.type)
来源：http://ed.newstarts.cn

[U110] JS：数组分块
来源：http://wu.asd995.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sd.newstarts.cn

[U111] JS：对象转 Map
来源：http://pq.gzmigu.cn

new Map(Object.entries(obj))
来源：http://rc.chemitech.net.cn

[U112] JS：字符串补位
来源：http://wc.shtwfgs.cn

"7".padStart(3, "0")
来源：http://xu.chemitech.net.cn

[U113] JS：正则替换全部
来源：http://ef.jctech888.com.cn

s.replaceAll("a", "b")
来源：http://bg.9csxet.cn

[U114] JS：JSON 深比较
来源：http://rr.huixinmuqiang.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://sf.lnxyls.cn

[U115] JS：生成 UUID
来源：http://hn.gzmigu.cn

crypto.randomUUID()
来源：http://jf.nicolike.cn

[U116] JS：类型检查（JSDoc）
来源：http://eg.bjjhwx.cn

/** @param {string} name */ function f(name) {}
来源：http://zk.szxytkj.cn

[U117] JS：单元测试
来源：http://vb.shxzskj.cn

npm i -D vitest;  npx vitest
来源：http://jj.shxzskj.cn

[U118] JS：开发服务器
来源：http://ud.huixiangedu.cn

npm i -D vite;  npx vite
来源：http://ds.hnjuh.cn

[U119] JS：生产构建
来源：http://vx.shtwfgs.cn

npx vite build
来源：http://dq.jianghongdianzi.cn

[U120] JS：读取环境变量（Vite）
来源：http://ca.bookmarksfly.cn

import.meta.env.VITE_API_URL
来源：http://yc.nicolike.cn

================================================================================
来源：http://us.nicolike.cn

统计汇总
来源：http://ce.521024.cn

================================================================================
来源：http://hb.nicolike.cn

按语言统计（条）：
来源：http://gh.haigaiapp.cn

Python ......... 252
来源：http://ot.bookmarksfly.cn

PHP ............ 252
来源：http://cw.bookmarksfly.cn

JavaScript ..... 252
来源：http://mo.wgjwhj.cn

TypeScript ..... 212
来源：http://vw.wgjwhj.cn

Java ........... 212
来源：http://xt.asd995.cn

Go ............. 212
来源：http://re.newstarts.cn

Ruby ........... 212
来源：http://dz.jianghongdianzi.cn

C# ............. 212
来源：http://qv.nszjky.cn

C .............. 30
来源：http://zk.shxzukj.cn

C++ ............ 30
来源：http://jv.521024.cn

SQL ............ 90
来源：http://wx.shtwfgs.cn

Bash ........... 80
来源：http://fi.szsharing.cn

Kotlin ......... 15
来源：http://xp.chemitech.net.cn

Swift .......... 15
来源：http://hz.9csxet.cn

Lua ............ 10
来源：http://ue.nicolike.cn

Perl ........... 10
来源：http://eo.bookmarksfly.cn

Scala .......... 10
来源：http://ha.9csxet.cn

------------------------------------
来源：http://lk.jctech888.com.cn

合计 ........... 2106 条
来源：http://ge.szsharing.cn

按章节统计：
来源：http://ur.hahajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rr.newstarts.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nr.shxzukj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wh.lnxyls.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://om.hnjuh.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ad.nicolike.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rq.asd995.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lq.szsharing.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://my.huixiangedu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wz.huixiangedu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ur.asd995.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qr.wgjwhj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ns.yuexingan06.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://oi.huanxung.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://eo.huanxung.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mo.shtwfgs.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://na.haigaiapp.cn

Q SQL 专题                              90
来源：http://dl.panjiajie.cn

R Bash 专题                             80
来源：http://ud.hahajie.cn

S C / C++ 专题                          60
来源：http://qb.hahajie.cn

T 其他语言补充                          60
来源：http://di.shtwfgs.cn

U 高频实用片段                         120
来源：http://or.panjiajie.cn

------------------------------------
来源：http://vt.shxzskj.cn

合计                                  2106 条
来源：http://kq.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://mv.bjjhwx.cn

使用提醒
来源：http://rp.huanxung.cn

--------------------------------------------------------------------------------
来源：http://za.lnxyls.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nj.9csxet.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pu.hnjuh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nw.newstarts.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://xg.shtwfgs.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ju.nicolike.cn

—— 文件结束 ——
来源：http://ui.bjjhwx.cn

================================================================================
来源：http://kg.jianghongdianzi.cn

程序语言常见例子速查手册（2024 版）
来源：http://xb.9csxet.cn

Common Programming Examples Cheat Book
来源：http://ld.szsharing.cn

================================================================================
来源：http://pu.yuntaijiaju.cn

【收录内容】
来源：http://gx.bjjhwx.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://hv.shtwfgs.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fb.asd995.cn

SQL · Bash · C · C++
来源：http://vy.newstarts.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ic.nicolike.cn

【使用说明】
来源：http://pc.panjiajie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jj.bjjhwx.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pj.muxihuayi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pw.lnxyls.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dd.panjiajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ph.asd995.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ec.huixinmuqiang.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ik.shxzukj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ew.shxzskj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nm.nicolike.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gy.nicolike.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lg.9csxet.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.gzmigu.cn

【文件统计】
来源：http://gy.szsharing.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nh.huanxung.cn

--------------------------------------------------------------------------------
来源：http://fi.chemitech.net.cn

目  录
来源：http://lj.521024.cn

--------------------------------------------------------------------------------
来源：http://ju.wgjwhj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kj.newstarts.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://af.huixinmuqiang.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://je.haigaiapp.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ne.shxzskj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kl.bjjhwx.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dj.bjjhwx.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bx.panjiajie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ba.shtwfgs.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://je.gzmigu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gc.panjiajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tl.lnxyls.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ly.521024.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gc.521024.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jk.haigaiapp.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gr.hahajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vi.szxytkj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fr.newstarts.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://oh.shxzskj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ja.yuntaijiaju.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lz.asd995.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pm.jianghongdianzi.cn

================================================================================
来源：http://oq.yuntaijiaju.cn

A. 基础语法与类型
来源：http://iy.nicolike.cn

================================================================================
来源：http://hj.jctech888.com.cn

[A01] Hello World
来源：http://kx.yuntaijiaju.cn

Py:   print("Hello, World!")
来源：http://tp.huixinmuqiang.cn

PHP:  echo "Hello, World!";
来源：http://jk.lnxyls.cn

JS:   console.log("Hello, World!");
来源：http://zg.huixinmuqiang.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bd.gzmigu.cn

Java: System.out.println("Hello, World!");
来源：http://nf.9csxet.cn

Go:   fmt.Println("Hello, World!")
来源：http://kr.bookmarksfly.cn

Ruby: puts "Hello, World!"
来源：http://qw.jctech888.com.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wd.jianghongdianzi.cn

[A02] 变量声明与赋值
来源：http://ca.lnxyls.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gm.521024.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://jg.521024.cn

JS:   let name = "Alex"; const age = 20;
来源：http://zu.huixinmuqiang.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://um.asd995.cn

Java: String name = "Alex"; int age = 20;
来源：http://mk.shtwfgs.cn

Go:   name := "Alex"; age := 20
来源：http://eu.szsharing.cn

Ruby: name = "Alex"; age = 20
来源：http://vq.chemitech.net.cn

C#:   string name = "Alex"; int age = 20;
来源：http://kq.gzmigu.cn

[A03] 常量定义
来源：http://qb.jctech888.com.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hn.nszjky.cn

PHP:  const PI = 3.14159;
来源：http://sp.huixiangedu.cn

JS:   const PI = 3.14159;
来源：http://ze.jctech888.com.cn

TS:   const PI: number = 3.14159;
来源：http://pe.shxzukj.cn

Java: static final double PI = 3.14159;
来源：http://tv.gzmigu.cn

Go:   const PI = 3.14159
来源：http://za.jianghongdianzi.cn

Ruby: PI = 3.14159
来源：http://bs.muxihuayi.cn

C#:   const double PI = 3.14159;
来源：http://na.asd995.cn

[A04] 判断变量类型
来源：http://oo.shxzskj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vo.shtwfgs.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://an.szsharing.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fq.nicolike.cn

TS:   typeof x; x instanceof Date
来源：http://ns.shtwfgs.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xb.bookmarksfly.cn

Go:   reflect.TypeOf(x).Name()
来源：http://sr.panjiajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://fj.yuntaijiaju.cn

C#:   x.GetType().Name; x is int
来源：http://uq.asd995.cn

[A05] 整数除法与取模
来源：http://ga.521024.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bt.panjiajie.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xi.9csxet.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://iv.newstarts.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jq.colortex.cn

Java: 7 / 2; 7 % 2
来源：http://lf.shxzukj.cn

Go:   7 / 2; 7 % 2
来源：http://ce.bookmarksfly.cn

Ruby: 7 / 2; 7 % 2
来源：http://tt.shtwfgs.cn

C#:   7 / 2; 7 % 2
来源：http://ns.jctech888.com.cn

[A06] 字符串转数字
来源：http://cd.shxzskj.cn

Py:   int("42"); float("3.14")
来源：http://ij.wgjwhj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ob.9csxet.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ov.jianghongdianzi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ib.asd995.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vp.shxzukj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cb.haigaiapp.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ox.jianghongdianzi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xs.jianghongdianzi.cn

[A07] 数字转字符串
来源：http://uw.lnxyls.cn

Py:   str(42)
来源：http://ut.hnjuh.cn

PHP:  (string) 42; strval(42)
来源：http://qr.gzmigu.cn

JS:   String(42); (42).toString()
来源：http://dj.shxzskj.cn

TS:   String(42)
来源：http://da.szsharing.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://mb.nicolike.cn

Go:   strconv.Itoa(42)
来源：http://bw.muxihuayi.cn

Ruby: 42.to_s
来源：http://kf.colortex.cn

C#:   42.ToString()
来源：http://hv.newstarts.cn

[A08] 取整与四舍五入
来源：http://tz.hnjuh.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ms.shxzukj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fn.huixinmuqiang.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://eh.nicolike.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wg.wgjwhj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yg.shxzskj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://in.huixinmuqiang.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://dk.521024.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jb.huanxung.cn

[A09] 绝对值与最大最小值
来源：http://sq.yuexingan06.cn


<!-- 参考信息 -->