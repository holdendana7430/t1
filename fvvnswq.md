代发 wailian999

[U63] PHP：文件读写
来源：http://tz.huanxung.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fl.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://xo.9csxet.cn

glob("dir/*.php");  scandir("dir");
来源：http://hk.shxzskj.cn

[U65] PHP：会话
来源：http://ir.colortex.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kn.wgjwhj.cn

[U66] PHP：设置 Cookie
来源：http://bg.yuexingan06.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kx.jctech888.com.cn

[U67] PHP：处理文件上传
来源：http://cy.nszjky.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ca.huixiangedu.cn

[U68] PHP：PDO 连接
来源：http://aj.huanxung.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ak.szsharing.cn

[U69] PHP：PDO 预处理
来源：http://nc.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fy.newstarts.cn

[U70] PHP：PDO 事务
来源：http://ge.yuntaijiaju.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dd.shxzukj.cn

[U71] PHP：抛出异常
来源：http://ei.shtwfgs.cn

throw new RuntimeException("失败", 500);
来源：http://ew.bookmarksfly.cn

[U72] PHP：写错误日志
来源：http://fp.lnxyls.cn

error_log("失败: " . $e->getMessage());
来源：http://gg.hnjuh.cn

[U73] PHP：读取 ini 配置
来源：http://ei.521024.cn

parse_ini_file("config.ini", true)
来源：http://qt.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://lo.9csxet.cn

getenv("APP_ENV") ?: "production"
来源：http://xv.panjiajie.cn

[U75] PHP：依赖注入
来源：http://hn.bookmarksfly.cn

composer require psr/container
来源：http://vh.panjiajie.cn

[U76] PHP：简单路由
来源：http://vn.nszjky.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yi.yuexingan06.cn

[U77] PHP：模板渲染
来源：http://bt.jctech888.com.cn

composer require twig/twig
来源：http://rm.hahajie.cn

[U78] PHP：单元测试
来源：http://ff.shxzskj.cn

composer require --dev phpunit/phpunit
来源：http://rp.asd995.cn

[U79] PHP：静态分析
来源：http://tu.shtwfgs.cn

composer require --dev phpstan/phpstan
来源：http://ra.lnxyls.cn

[U80] PHP：代码规范修复
来源：http://kx.chemitech.net.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rq.bjjhwx.cn

[U81] JS：初始化项目
来源：http://of.gzmigu.cn

npm init -y;  npm i express
来源：http://kv.huixinmuqiang.cn

[U82] JS：package.json 脚本
来源：http://cv.huixiangedu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ug.shxzskj.cn

[U83] JS：ES Module 导入导出
来源：http://sc.jianghongdianzi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kn.shxzukj.cn

[U84] JS：CommonJS 写法
来源：http://zc.shtwfgs.cn

module.exports = { a };  const { a } = require("./m");
来源：http://db.shxzukj.cn

[U85] JS：可选链
来源：http://ym.huixiangedu.cn

a?.b?.c
来源：http://uv.jctech888.com.cn

[U86] JS：空值合并
来源：http://sf.newstarts.cn

a ?? b
来源：http://qh.huixiangedu.cn

[U87] JS：解构默认值
来源：http://fa.nszjky.cn

const { a = 1, b = 2 } = obj;
来源：http://cm.szsharing.cn

[U88] JS：对象展开合并
来源：http://nb.huixinmuqiang.cn

{ ...a, ...b }
来源：http://vc.lnxyls.cn

[U89] JS：数组去重
来源：http://ai.muxihuayi.cn

[...new Set(arr)]
来源：http://ua.newstarts.cn

[U90] JS：数字数组排序
来源：http://jq.yuntaijiaju.cn

[...arr].sort((a, b) => a - b)
来源：http://zz.huanxung.cn

[U91] JS：对象键值遍历
来源：http://ze.9csxet.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jx.newstarts.cn

[U92] JS：深拷贝
来源：http://tn.lnxyls.cn

structuredClone(obj)
来源：http://xj.huixiangedu.cn

[U93] JS：模板字符串
来源：http://si.shxzskj.cn

`共 ${n} 条`
来源：http://yd.hnjuh.cn

[U94] JS：箭头函数
来源：http://vs.shxzukj.cn

const double = x => x * 2;
来源：http://ij.szsharing.cn

[U95] JS：Promise 包装
来源：http://jt.shtwfgs.cn

new Promise((resolve, reject) => {})
来源：http://lt.panjiajie.cn

[U96] JS：async/await 与异常
来源：http://nd.shxzskj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://re.jianghongdianzi.cn

[U97] JS：并发请求
来源：http://kt.lnxyls.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tw.huixinmuqiang.cn

[U98] JS：fetch 带 JSON
来源：http://ar.wgjwhj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yk.bookmarksfly.cn

[U99] JS：事件监听
来源：http://wd.haigaiapp.cn

el.addEventListener("click", e => {})
来源：http://yh.bookmarksfly.cn

[U100] JS：DOM 查询
来源：http://rw.yuexingan06.cn

document.querySelector(".item")
来源：http://do.shxzskj.cn

[U101] JS：classList 操作
来源：http://sq.huanxung.cn

el.classList.toggle("active")
来源：http://gm.chemitech.net.cn

[U102] JS：本地存储
来源：http://vf.jianghongdianzi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sa.huixinmuqiang.cn

[U103] JS：定时器
来源：http://fj.521024.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cc.wgjwhj.cn

[U104] JS：防抖
来源：http://sc.hnjuh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yd.panjiajie.cn

[U105] JS：节流
来源：http://hl.huixinmuqiang.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nv.521024.cn

[U106] JS：日期格式化
来源：http://co.bjjhwx.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mg.521024.cn

[U107] JS：数字千分位
来源：http://au.haigaiapp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sr.szsharing.cn

[U108] JS：随机整数
来源：http://zv.panjiajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tf.yuexingan06.cn

[U109] JS：数组分组
来源：http://ba.shxzskj.cn

Object.groupBy(arr, x => x.type)
来源：http://xm.9csxet.cn

[U110] JS：数组分块
来源：http://zd.huanxung.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lj.shxzukj.cn

[U111] JS：对象转 Map
来源：http://ls.asd995.cn

new Map(Object.entries(obj))
来源：http://ns.shtwfgs.cn

[U112] JS：字符串补位
来源：http://vh.9csxet.cn

"7".padStart(3, "0")
来源：http://wo.bjjhwx.cn

[U113] JS：正则替换全部
来源：http://ho.jctech888.com.cn

s.replaceAll("a", "b")
来源：http://iz.szxytkj.cn

[U114] JS：JSON 深比较
来源：http://za.lnxyls.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dc.huixinmuqiang.cn

[U115] JS：生成 UUID
来源：http://xq.9csxet.cn

crypto.randomUUID()
来源：http://ys.9csxet.cn

[U116] JS：类型检查（JSDoc）
来源：http://sp.jctech888.com.cn

/** @param {string} name */ function f(name) {}
来源：http://fz.nicolike.cn

[U117] JS：单元测试
来源：http://fn.huanxung.cn

npm i -D vitest;  npx vitest
来源：http://od.haigaiapp.cn

[U118] JS：开发服务器
来源：http://tr.9csxet.cn

npm i -D vite;  npx vite
来源：http://my.gzmigu.cn

[U119] JS：生产构建
来源：http://xo.panjiajie.cn

npx vite build
来源：http://hr.bjjhwx.cn

[U120] JS：读取环境变量（Vite）
来源：http://qh.asd995.cn

import.meta.env.VITE_API_URL
来源：http://rd.haigaiapp.cn

================================================================================
来源：http://jv.chemitech.net.cn

统计汇总
来源：http://jq.nicolike.cn

================================================================================
来源：http://ms.panjiajie.cn

按语言统计（条）：
来源：http://jg.szsharing.cn

Python ......... 252
来源：http://le.bjjhwx.cn

PHP ............ 252
来源：http://nd.nicolike.cn

JavaScript ..... 252
来源：http://in.nicolike.cn

TypeScript ..... 212
来源：http://dd.huixiangedu.cn

Java ........... 212
来源：http://gb.huixinmuqiang.cn

Go ............. 212
来源：http://eb.szxytkj.cn

Ruby ........... 212
来源：http://wy.shxzukj.cn

C# ............. 212
来源：http://nj.szsharing.cn

C .............. 30
来源：http://nw.shxzskj.cn

C++ ............ 30
来源：http://pm.hahajie.cn

SQL ............ 90
来源：http://xi.haigaiapp.cn

Bash ........... 80
来源：http://ug.bookmarksfly.cn

Kotlin ......... 15
来源：http://sa.haigaiapp.cn

Swift .......... 15
来源：http://ah.wgjwhj.cn

Lua ............ 10
来源：http://gr.huanxung.cn

Perl ........... 10
来源：http://ul.521024.cn

Scala .......... 10
来源：http://vw.newstarts.cn

------------------------------------
来源：http://cl.9csxet.cn

合计 ........... 2106 条
来源：http://uq.bookmarksfly.cn

按章节统计：
来源：http://hu.newstarts.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bf.521024.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lq.huanxung.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mm.colortex.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://iw.521024.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sh.huixiangedu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ss.wgjwhj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kz.chemitech.net.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lj.huanxung.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pn.szsharing.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rp.haigaiapp.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://eh.shxzukj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://aa.chemitech.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ix.panjiajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dr.gzmigu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zj.wgjwhj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ur.hahajie.cn

Q SQL 专题                              90
来源：http://vl.yuexingan06.cn

R Bash 专题                             80
来源：http://bj.asd995.cn

S C / C++ 专题                          60
来源：http://kq.szsharing.cn

T 其他语言补充                          60
来源：http://ph.huixinmuqiang.cn

U 高频实用片段                         120
来源：http://rb.bookmarksfly.cn

------------------------------------
来源：http://tr.newstarts.cn

合计                                  2106 条
来源：http://cf.asd995.cn

--------------------------------------------------------------------------------
来源：http://rk.chemitech.net.cn

使用提醒
来源：http://vs.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://mg.wgjwhj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xs.521024.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mm.szxytkj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ku.colortex.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gg.yuexingan06.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mg.9csxet.cn

—— 文件结束 ——
来源：http://sc.yuntaijiaju.cn

================================================================================
来源：http://jq.521024.cn

程序语言常见例子速查手册（2024 版）
来源：http://rq.muxihuayi.cn

Common Programming Examples Cheat Book
来源：http://hs.lnxyls.cn

================================================================================
来源：http://uy.huanxung.cn

【收录内容】
来源：http://mb.newstarts.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vm.bookmarksfly.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wr.bjjhwx.cn

SQL · Bash · C · C++
来源：http://sk.shxzskj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sj.jianghongdianzi.cn

【使用说明】
来源：http://tb.jianghongdianzi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tv.nicolike.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gr.huixiangedu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nn.huanxung.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wx.yuntaijiaju.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://yx.hahajie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lo.huixiangedu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://my.huixiangedu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hl.9csxet.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://da.shxzukj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hi.huixinmuqiang.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://el.lnxyls.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tu.panjiajie.cn

【文件统计】
来源：http://ic.521024.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lo.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://kx.huixinmuqiang.cn

目  录
来源：http://xn.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://ix.muxihuayi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qj.bjjhwx.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lp.panjiajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ac.9csxet.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mm.huanxung.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ou.521024.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mk.huixinmuqiang.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bl.nszjky.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fz.muxihuayi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fz.yuntaijiaju.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bj.jctech888.com.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://aj.nicolike.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bb.hahajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bj.panjiajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tf.jctech888.com.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ao.bjjhwx.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qw.chemitech.net.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ez.yuexingan06.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://cp.huixiangedu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jh.yuntaijiaju.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yb.yuntaijiaju.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qr.huanxung.cn

================================================================================
来源：http://ro.szsharing.cn

A. 基础语法与类型
来源：http://nx.chemitech.net.cn

================================================================================
来源：http://qm.huanxung.cn

[A01] Hello World
来源：http://oh.521024.cn

Py:   print("Hello, World!")
来源：http://py.521024.cn

PHP:  echo "Hello, World!";
来源：http://eq.szxytkj.cn

JS:   console.log("Hello, World!");
来源：http://hk.nszjky.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://on.bjjhwx.cn

Java: System.out.println("Hello, World!");
来源：http://zk.nszjky.cn

Go:   fmt.Println("Hello, World!")
来源：http://kl.chemitech.net.cn

Ruby: puts "Hello, World!"
来源：http://mz.huixinmuqiang.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vk.hnjuh.cn

[A02] 变量声明与赋值
来源：http://xi.chemitech.net.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ts.szsharing.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://wo.shtwfgs.cn

JS:   let name = "Alex"; const age = 20;
来源：http://yi.shtwfgs.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zm.yuntaijiaju.cn

Java: String name = "Alex"; int age = 20;
来源：http://ly.521024.cn

Go:   name := "Alex"; age := 20
来源：http://gm.chemitech.net.cn

Ruby: name = "Alex"; age = 20
来源：http://sc.shxzukj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://an.muxihuayi.cn

[A03] 常量定义
来源：http://wd.colortex.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xk.haigaiapp.cn

PHP:  const PI = 3.14159;
来源：http://yd.szxytkj.cn

JS:   const PI = 3.14159;
来源：http://ky.jctech888.com.cn

TS:   const PI: number = 3.14159;
来源：http://bu.huanxung.cn

Java: static final double PI = 3.14159;
来源：http://xi.colortex.cn

Go:   const PI = 3.14159
来源：http://sm.yuexingan06.cn

Ruby: PI = 3.14159
来源：http://qn.muxihuayi.cn

C#:   const double PI = 3.14159;
来源：http://jw.asd995.cn

[A04] 判断变量类型
来源：http://pi.shxzskj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://xa.colortex.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kz.lnxyls.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://go.bookmarksfly.cn

TS:   typeof x; x instanceof Date
来源：http://un.asd995.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ca.jctech888.com.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ut.szxytkj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kx.panjiajie.cn

C#:   x.GetType().Name; x is int
来源：http://ay.szsharing.cn

[A05] 整数除法与取模
来源：http://ur.wgjwhj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ws.shxzukj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://bi.lnxyls.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bx.yuexingan06.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qy.huixiangedu.cn

Java: 7 / 2; 7 % 2
来源：http://wu.newstarts.cn

Go:   7 / 2; 7 % 2
来源：http://xp.muxihuayi.cn

Ruby: 7 / 2; 7 % 2
来源：http://by.nszjky.cn

C#:   7 / 2; 7 % 2
来源：http://qo.shtwfgs.cn

[A06] 字符串转数字
来源：http://lw.szxytkj.cn

Py:   int("42"); float("3.14")
来源：http://od.huixinmuqiang.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://uv.bjjhwx.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dc.hahajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://gv.wgjwhj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ds.521024.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dn.gzmigu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://mb.hahajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rk.huanxung.cn

[A07] 数字转字符串
来源：http://hy.yuntaijiaju.cn

Py:   str(42)
来源：http://qt.yuntaijiaju.cn

PHP:  (string) 42; strval(42)
来源：http://pf.yuexingan06.cn

JS:   String(42); (42).toString()
来源：http://gi.shxzukj.cn

TS:   String(42)
来源：http://bw.shxzukj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://wf.huixinmuqiang.cn

Go:   strconv.Itoa(42)
来源：http://gf.9csxet.cn

Ruby: 42.to_s
来源：http://sk.lnxyls.cn

C#:   42.ToString()
来源：http://ut.nszjky.cn

[A08] 取整与四舍五入
来源：http://ss.521024.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gx.shxzskj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://eo.jctech888.com.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xg.wgjwhj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jh.bookmarksfly.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://py.hnjuh.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ur.yuntaijiaju.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://nc.colortex.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wh.gzmigu.cn

[A09] 绝对值与最大最小值
来源：http://wo.wgjwhj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hy.521024.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nz.huixiangedu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ct.hnjuh.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zc.yuntaijiaju.cn


<!-- 参考信息 -->