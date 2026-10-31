代发 wailian999

[U59] PHP：自定义排序
来源：http://hc.hnjuh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://em.yuntaijiaju.cn

[U60] PHP：JSON 编解码
来源：http://eg.shxzukj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vh.nicolike.cn

[U61] PHP：正则
来源：http://pd.hahajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gr.chemitech.net.cn

[U62] PHP：日期对象
来源：http://mg.shtwfgs.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tm.huixinmuqiang.cn

[U63] PHP：文件读写
来源：http://bo.lnxyls.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ul.bjjhwx.cn

[U64] PHP：目录遍历
来源：http://ob.lnxyls.cn

glob("dir/*.php");  scandir("dir");
来源：http://lh.chemitech.net.cn

[U65] PHP：会话
来源：http://qk.wgjwhj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pr.panjiajie.cn

[U66] PHP：设置 Cookie
来源：http://qb.haigaiapp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bb.asd995.cn

[U67] PHP：处理文件上传
来源：http://gw.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fu.huixinmuqiang.cn

[U68] PHP：PDO 连接
来源：http://wv.shxzskj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ex.shxzskj.cn

[U69] PHP：PDO 预处理
来源：http://tb.yuntaijiaju.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hy.newstarts.cn

[U70] PHP：PDO 事务
来源：http://zl.jctech888.com.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bt.521024.cn

[U71] PHP：抛出异常
来源：http://tv.huanxung.cn

throw new RuntimeException("失败", 500);
来源：http://dm.hahajie.cn

[U72] PHP：写错误日志
来源：http://ia.muxihuayi.cn

error_log("失败: " . $e->getMessage());
来源：http://xy.colortex.cn

[U73] PHP：读取 ini 配置
来源：http://hp.yuntaijiaju.cn

parse_ini_file("config.ini", true)
来源：http://wb.nszjky.cn

[U74] PHP：读取环境变量
来源：http://vc.521024.cn

getenv("APP_ENV") ?: "production"
来源：http://uc.chemitech.net.cn

[U75] PHP：依赖注入
来源：http://mc.shxzskj.cn

composer require psr/container
来源：http://xl.yuexingan06.cn

[U76] PHP：简单路由
来源：http://lk.panjiajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zp.521024.cn

[U77] PHP：模板渲染
来源：http://np.szxytkj.cn

composer require twig/twig
来源：http://kf.nszjky.cn

[U78] PHP：单元测试
来源：http://vk.shtwfgs.cn

composer require --dev phpunit/phpunit
来源：http://jm.huixiangedu.cn

[U79] PHP：静态分析
来源：http://dp.asd995.cn

composer require --dev phpstan/phpstan
来源：http://gy.jctech888.com.cn

[U80] PHP：代码规范修复
来源：http://iq.huanxung.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hd.panjiajie.cn

[U81] JS：初始化项目
来源：http://hh.9csxet.cn

npm init -y;  npm i express
来源：http://gu.szxytkj.cn

[U82] JS：package.json 脚本
来源：http://wl.newstarts.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wk.shxzukj.cn

[U83] JS：ES Module 导入导出
来源：http://gg.asd995.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zg.lnxyls.cn

[U84] JS：CommonJS 写法
来源：http://es.bjjhwx.cn

module.exports = { a };  const { a } = require("./m");
来源：http://un.lnxyls.cn

[U85] JS：可选链
来源：http://sr.nicolike.cn

a?.b?.c
来源：http://oo.9csxet.cn

[U86] JS：空值合并
来源：http://zl.shtwfgs.cn

a ?? b
来源：http://mh.szxytkj.cn

[U87] JS：解构默认值
来源：http://ag.shtwfgs.cn

const { a = 1, b = 2 } = obj;
来源：http://id.szsharing.cn

[U88] JS：对象展开合并
来源：http://zp.shxzskj.cn

{ ...a, ...b }
来源：http://ld.szxytkj.cn

[U89] JS：数组去重
来源：http://cd.yuexingan06.cn

[...new Set(arr)]
来源：http://nf.bookmarksfly.cn

[U90] JS：数字数组排序
来源：http://vz.nszjky.cn

[...arr].sort((a, b) => a - b)
来源：http://fo.shxzukj.cn

[U91] JS：对象键值遍历
来源：http://tj.chemitech.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qe.panjiajie.cn

[U92] JS：深拷贝
来源：http://zv.lnxyls.cn

structuredClone(obj)
来源：http://un.wgjwhj.cn

[U93] JS：模板字符串
来源：http://xn.szxytkj.cn

`共 ${n} 条`
来源：http://nu.gzmigu.cn

[U94] JS：箭头函数
来源：http://mp.gzmigu.cn

const double = x => x * 2;
来源：http://ht.9csxet.cn

[U95] JS：Promise 包装
来源：http://km.huixiangedu.cn

new Promise((resolve, reject) => {})
来源：http://gf.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://ki.yuexingan06.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tp.yuntaijiaju.cn

[U97] JS：并发请求
来源：http://tt.lnxyls.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rq.shxzskj.cn

[U98] JS：fetch 带 JSON
来源：http://mi.huanxung.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vr.newstarts.cn

[U99] JS：事件监听
来源：http://eq.colortex.cn

el.addEventListener("click", e => {})
来源：http://sw.lnxyls.cn

[U100] JS：DOM 查询
来源：http://bs.huixiangedu.cn

document.querySelector(".item")
来源：http://vu.jctech888.com.cn

[U101] JS：classList 操作
来源：http://hh.bookmarksfly.cn

el.classList.toggle("active")
来源：http://dd.huixinmuqiang.cn

[U102] JS：本地存储
来源：http://zx.9csxet.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ok.panjiajie.cn

[U103] JS：定时器
来源：http://ju.shxzskj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zd.huixinmuqiang.cn

[U104] JS：防抖
来源：http://he.chemitech.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://um.521024.cn

[U105] JS：节流
来源：http://pc.huixinmuqiang.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ux.haigaiapp.cn

[U106] JS：日期格式化
来源：http://ny.shtwfgs.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gt.asd995.cn

[U107] JS：数字千分位
来源：http://sv.huanxung.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fs.muxihuayi.cn

[U108] JS：随机整数
来源：http://nr.panjiajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bq.shxzskj.cn

[U109] JS：数组分组
来源：http://xb.haigaiapp.cn

Object.groupBy(arr, x => x.type)
来源：http://en.gzmigu.cn

[U110] JS：数组分块
来源：http://ml.gzmigu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ut.huixiangedu.cn

[U111] JS：对象转 Map
来源：http://er.szsharing.cn

new Map(Object.entries(obj))
来源：http://bl.szsharing.cn

[U112] JS：字符串补位
来源：http://nf.jctech888.com.cn

"7".padStart(3, "0")
来源：http://om.521024.cn

[U113] JS：正则替换全部
来源：http://wn.9csxet.cn

s.replaceAll("a", "b")
来源：http://wl.shxzskj.cn

[U114] JS：JSON 深比较
来源：http://on.szxytkj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fa.shxzukj.cn

[U115] JS：生成 UUID
来源：http://fa.haigaiapp.cn

crypto.randomUUID()
来源：http://tu.yuexingan06.cn

[U116] JS：类型检查（JSDoc）
来源：http://zn.wgjwhj.cn

/** @param {string} name */ function f(name) {}
来源：http://fk.panjiajie.cn

[U117] JS：单元测试
来源：http://ig.yuntaijiaju.cn

npm i -D vitest;  npx vitest
来源：http://tz.shxzukj.cn

[U118] JS：开发服务器
来源：http://ad.wgjwhj.cn

npm i -D vite;  npx vite
来源：http://tj.gzmigu.cn

[U119] JS：生产构建
来源：http://fr.asd995.cn

npx vite build
来源：http://kb.nicolike.cn

[U120] JS：读取环境变量（Vite）
来源：http://ml.huixiangedu.cn

import.meta.env.VITE_API_URL
来源：http://po.newstarts.cn

================================================================================
来源：http://zm.nszjky.cn

统计汇总
来源：http://wr.szsharing.cn

================================================================================
来源：http://fg.chemitech.net.cn

按语言统计（条）：
来源：http://wk.muxihuayi.cn

Python ......... 252
来源：http://mj.hnjuh.cn

PHP ............ 252
来源：http://ak.jianghongdianzi.cn

JavaScript ..... 252
来源：http://rr.asd995.cn

TypeScript ..... 212
来源：http://yt.asd995.cn

Java ........... 212
来源：http://qr.jctech888.com.cn

Go ............. 212
来源：http://lb.521024.cn

Ruby ........... 212
来源：http://dz.jianghongdianzi.cn

C# ............. 212
来源：http://cv.nicolike.cn

C .............. 30
来源：http://oz.shxzskj.cn

C++ ............ 30
来源：http://oj.newstarts.cn

SQL ............ 90
来源：http://nx.bookmarksfly.cn

Bash ........... 80
来源：http://zy.shxzskj.cn

Kotlin ......... 15
来源：http://oa.colortex.cn

Swift .......... 15
来源：http://rm.asd995.cn

Lua ............ 10
来源：http://xr.hahajie.cn

Perl ........... 10
来源：http://uy.shxzskj.cn

Scala .......... 10
来源：http://td.haigaiapp.cn

------------------------------------
来源：http://fy.hnjuh.cn

合计 ........... 2106 条
来源：http://hu.jctech888.com.cn

按章节统计：
来源：http://un.hnjuh.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ur.szsharing.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zr.huixiangedu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mo.chemitech.net.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xt.szxytkj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kn.bjjhwx.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uk.huixiangedu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tu.huixinmuqiang.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://uq.hnjuh.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ku.haigaiapp.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mn.colortex.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://td.huixinmuqiang.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nd.colortex.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ig.wgjwhj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://in.panjiajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qu.nszjky.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wx.lnxyls.cn

Q SQL 专题                              90
来源：http://wy.yuexingan06.cn

R Bash 专题                             80
来源：http://xs.gzmigu.cn

S C / C++ 专题                          60
来源：http://bs.shxzskj.cn

T 其他语言补充                          60
来源：http://kj.newstarts.cn

U 高频实用片段                         120
来源：http://cd.521024.cn

------------------------------------
来源：http://gd.chemitech.net.cn

合计                                  2106 条
来源：http://qu.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://po.nicolike.cn

使用提醒
来源：http://yh.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://oy.yuexingan06.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qk.lnxyls.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ef.gzmigu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pq.bookmarksfly.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://sz.hahajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vk.521024.cn

—— 文件结束 ——
来源：http://lz.muxihuayi.cn

================================================================================
来源：http://pf.shxzskj.cn

程序语言常见例子速查手册（2024 版）
来源：http://xd.huixiangedu.cn

Common Programming Examples Cheat Book
来源：http://gp.nszjky.cn

================================================================================
来源：http://bw.szsharing.cn

【收录内容】
来源：http://iu.nszjky.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://sl.huixinmuqiang.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kw.yuexingan06.cn

SQL · Bash · C · C++
来源：http://hu.chemitech.net.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sy.yuexingan06.cn

【使用说明】
来源：http://fp.lnxyls.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://im.chemitech.net.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jl.yuexingan06.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jz.jctech888.com.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cf.shxzskj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://zj.jctech888.com.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hl.szxytkj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://li.szxytkj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vl.shtwfgs.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wb.bjjhwx.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ne.gzmigu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fi.wgjwhj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ek.hnjuh.cn

【文件统计】
来源：http://up.wgjwhj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ws.nszjky.cn

--------------------------------------------------------------------------------
来源：http://uj.jianghongdianzi.cn

目  录
来源：http://mj.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://jy.huixinmuqiang.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ll.chemitech.net.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zh.bookmarksfly.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ye.yuexingan06.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://za.jianghongdianzi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xd.9csxet.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jh.521024.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nf.szxytkj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ln.shxzskj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lr.nszjky.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cp.huixiangedu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kq.huanxung.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xv.nszjky.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rl.huanxung.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://uq.nicolike.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yc.nszjky.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wr.shtwfgs.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://it.jctech888.com.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://nb.szxytkj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xo.shxzukj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fd.wgjwhj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qc.shxzukj.cn

================================================================================
来源：http://oq.shxzukj.cn

A. 基础语法与类型
来源：http://sg.nszjky.cn

================================================================================
来源：http://ze.haigaiapp.cn

[A01] Hello World
来源：http://wz.nszjky.cn

Py:   print("Hello, World!")
来源：http://yy.shxzskj.cn

PHP:  echo "Hello, World!";
来源：http://qa.colortex.cn

JS:   console.log("Hello, World!");
来源：http://ba.nicolike.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dv.szsharing.cn

Java: System.out.println("Hello, World!");
来源：http://vj.yuntaijiaju.cn

Go:   fmt.Println("Hello, World!")
来源：http://uk.yuexingan06.cn

Ruby: puts "Hello, World!"
来源：http://xk.shxzukj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vz.haigaiapp.cn

[A02] 变量声明与赋值
来源：http://ew.huixiangedu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vd.haigaiapp.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://dx.hnjuh.cn

JS:   let name = "Alex"; const age = 20;
来源：http://mk.bjjhwx.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vv.nszjky.cn

Java: String name = "Alex"; int age = 20;
来源：http://et.panjiajie.cn

Go:   name := "Alex"; age := 20
来源：http://gk.chemitech.net.cn

Ruby: name = "Alex"; age = 20
来源：http://nv.yuntaijiaju.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jz.newstarts.cn

[A03] 常量定义
来源：http://gm.huixiangedu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://se.9csxet.cn

PHP:  const PI = 3.14159;
来源：http://rb.huixinmuqiang.cn

JS:   const PI = 3.14159;
来源：http://uy.gzmigu.cn

TS:   const PI: number = 3.14159;
来源：http://cx.nszjky.cn

Java: static final double PI = 3.14159;
来源：http://tq.bjjhwx.cn

Go:   const PI = 3.14159
来源：http://km.bjjhwx.cn

Ruby: PI = 3.14159
来源：http://zl.wgjwhj.cn

C#:   const double PI = 3.14159;
来源：http://pp.521024.cn

[A04] 判断变量类型
来源：http://gj.huixinmuqiang.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://nv.shxzukj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qe.shxzskj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wv.haigaiapp.cn

TS:   typeof x; x instanceof Date
来源：http://yi.asd995.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lh.newstarts.cn

Go:   reflect.TypeOf(x).Name()
来源：http://zk.bjjhwx.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://dc.bjjhwx.cn

C#:   x.GetType().Name; x is int
来源：http://rh.521024.cn

[A05] 整数除法与取模
来源：http://eg.shxzukj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cv.chemitech.net.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://or.hnjuh.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nr.huixinmuqiang.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://uj.szxytkj.cn

Java: 7 / 2; 7 % 2
来源：http://ep.huixiangedu.cn

Go:   7 / 2; 7 % 2
来源：http://gg.shtwfgs.cn

Ruby: 7 / 2; 7 % 2
来源：http://jf.haigaiapp.cn

C#:   7 / 2; 7 % 2
来源：http://gq.nicolike.cn

[A06] 字符串转数字
来源：http://xd.hahajie.cn

Py:   int("42"); float("3.14")
来源：http://jn.huixinmuqiang.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ez.nszjky.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fa.szxytkj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://aa.haigaiapp.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xv.chemitech.net.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mh.nicolike.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://pb.jctech888.com.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xe.9csxet.cn

[A07] 数字转字符串
来源：http://fk.huanxung.cn

Py:   str(42)
来源：http://nz.newstarts.cn

PHP:  (string) 42; strval(42)
来源：http://lo.chemitech.net.cn

JS:   String(42); (42).toString()
来源：http://lg.panjiajie.cn

TS:   String(42)
来源：http://vg.shxzukj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ut.shxzukj.cn

Go:   strconv.Itoa(42)
来源：http://wo.gzmigu.cn

Ruby: 42.to_s
来源：http://gw.huanxung.cn

C#:   42.ToString()
来源：http://yu.lnxyls.cn

[A08] 取整与四舍五入
来源：http://eb.shtwfgs.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://io.shxzskj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rt.bjjhwx.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dj.hahajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jt.newstarts.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wp.asd995.cn


<!-- 参考信息 -->