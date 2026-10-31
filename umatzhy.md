代发 wailian999

[U57] PHP：字符串插值
来源：http://ak.huanxung.cn

"值: {$a}"
来源：http://rk.shtwfgs.cn

[U58] PHP：数组三件套
来源：http://pv.haigaiapp.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qo.huixinmuqiang.cn

[U59] PHP：自定义排序
来源：http://sx.newstarts.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bz.9csxet.cn

[U60] PHP：JSON 编解码
来源：http://ea.shxzskj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ur.wgjwhj.cn

[U61] PHP：正则
来源：http://nu.bjjhwx.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pm.nicolike.cn

[U62] PHP：日期对象
来源：http://pu.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lk.hahajie.cn

[U63] PHP：文件读写
来源：http://ph.colortex.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hh.asd995.cn

[U64] PHP：目录遍历
来源：http://zc.huixiangedu.cn

glob("dir/*.php");  scandir("dir");
来源：http://be.bookmarksfly.cn

[U65] PHP：会话
来源：http://wa.huanxung.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tr.shtwfgs.cn

[U66] PHP：设置 Cookie
来源：http://nh.asd995.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dn.huanxung.cn

[U67] PHP：处理文件上传
来源：http://vg.shxzukj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ua.jctech888.com.cn

[U68] PHP：PDO 连接
来源：http://jj.bjjhwx.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cb.bjjhwx.cn

[U69] PHP：PDO 预处理
来源：http://vu.yuexingan06.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ds.shtwfgs.cn

[U70] PHP：PDO 事务
来源：http://im.bookmarksfly.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tt.jianghongdianzi.cn

[U71] PHP：抛出异常
来源：http://cg.shtwfgs.cn

throw new RuntimeException("失败", 500);
来源：http://ky.shxzukj.cn

[U72] PHP：写错误日志
来源：http://dx.shxzukj.cn

error_log("失败: " . $e->getMessage());
来源：http://qw.yuntaijiaju.cn

[U73] PHP：读取 ini 配置
来源：http://se.wgjwhj.cn

parse_ini_file("config.ini", true)
来源：http://bl.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://vy.newstarts.cn

getenv("APP_ENV") ?: "production"
来源：http://gc.panjiajie.cn

[U75] PHP：依赖注入
来源：http://wx.hnjuh.cn

composer require psr/container
来源：http://vp.haigaiapp.cn

[U76] PHP：简单路由
来源：http://ng.hahajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tv.colortex.cn

[U77] PHP：模板渲染
来源：http://fe.colortex.cn

composer require twig/twig
来源：http://sz.lnxyls.cn

[U78] PHP：单元测试
来源：http://sk.nicolike.cn

composer require --dev phpunit/phpunit
来源：http://ns.yuntaijiaju.cn

[U79] PHP：静态分析
来源：http://qc.colortex.cn

composer require --dev phpstan/phpstan
来源：http://hq.yuexingan06.cn

[U80] PHP：代码规范修复
来源：http://wz.hnjuh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zg.yuntaijiaju.cn

[U81] JS：初始化项目
来源：http://sy.szxytkj.cn

npm init -y;  npm i express
来源：http://oh.chemitech.net.cn

[U82] JS：package.json 脚本
来源：http://eg.jianghongdianzi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fo.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://bd.huixiangedu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ys.hahajie.cn

[U84] JS：CommonJS 写法
来源：http://pq.hahajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bn.yuexingan06.cn

[U85] JS：可选链
来源：http://lq.asd995.cn

a?.b?.c
来源：http://us.9csxet.cn

[U86] JS：空值合并
来源：http://mj.szxytkj.cn

a ?? b
来源：http://kn.szsharing.cn

[U87] JS：解构默认值
来源：http://cj.bookmarksfly.cn

const { a = 1, b = 2 } = obj;
来源：http://ra.colortex.cn

[U88] JS：对象展开合并
来源：http://ju.szsharing.cn

{ ...a, ...b }
来源：http://gq.newstarts.cn

[U89] JS：数组去重
来源：http://nx.521024.cn

[...new Set(arr)]
来源：http://no.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://yv.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://kd.huixiangedu.cn

[U91] JS：对象键值遍历
来源：http://ew.huanxung.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://uf.hnjuh.cn

[U92] JS：深拷贝
来源：http://ay.yuexingan06.cn

structuredClone(obj)
来源：http://al.shxzskj.cn

[U93] JS：模板字符串
来源：http://zr.huanxung.cn

`共 ${n} 条`
来源：http://ov.muxihuayi.cn

[U94] JS：箭头函数
来源：http://li.yuexingan06.cn

const double = x => x * 2;
来源：http://mb.jctech888.com.cn

[U95] JS：Promise 包装
来源：http://zb.shxzskj.cn

new Promise((resolve, reject) => {})
来源：http://fz.wgjwhj.cn

[U96] JS：async/await 与异常
来源：http://ex.lnxyls.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ed.jianghongdianzi.cn

[U97] JS：并发请求
来源：http://dg.chemitech.net.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zd.yuexingan06.cn

[U98] JS：fetch 带 JSON
来源：http://zr.szsharing.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sc.521024.cn

[U99] JS：事件监听
来源：http://iw.9csxet.cn

el.addEventListener("click", e => {})
来源：http://ar.szxytkj.cn

[U100] JS：DOM 查询
来源：http://da.yuntaijiaju.cn

document.querySelector(".item")
来源：http://ui.huixiangedu.cn

[U101] JS：classList 操作
来源：http://ry.nicolike.cn

el.classList.toggle("active")
来源：http://mj.muxihuayi.cn

[U102] JS：本地存储
来源：http://oi.bjjhwx.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://al.shxzukj.cn

[U103] JS：定时器
来源：http://it.bookmarksfly.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://me.chemitech.net.cn

[U104] JS：防抖
来源：http://ns.asd995.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ip.shtwfgs.cn

[U105] JS：节流
来源：http://nn.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ku.huixiangedu.cn

[U106] JS：日期格式化
来源：http://fu.521024.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://aa.bjjhwx.cn

[U107] JS：数字千分位
来源：http://ja.newstarts.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pi.521024.cn

[U108] JS：随机整数
来源：http://ya.hahajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://he.hnjuh.cn

[U109] JS：数组分组
来源：http://gl.9csxet.cn

Object.groupBy(arr, x => x.type)
来源：http://uz.bjjhwx.cn

[U110] JS：数组分块
来源：http://hq.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yk.bookmarksfly.cn

[U111] JS：对象转 Map
来源：http://pf.huixinmuqiang.cn

new Map(Object.entries(obj))
来源：http://uo.colortex.cn

[U112] JS：字符串补位
来源：http://yk.chemitech.net.cn

"7".padStart(3, "0")
来源：http://ym.bjjhwx.cn

[U113] JS：正则替换全部
来源：http://bw.gzmigu.cn

s.replaceAll("a", "b")
来源：http://cc.jctech888.com.cn

[U114] JS：JSON 深比较
来源：http://bb.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ph.chemitech.net.cn

[U115] JS：生成 UUID
来源：http://ot.panjiajie.cn

crypto.randomUUID()
来源：http://fz.hahajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://lo.bjjhwx.cn

/** @param {string} name */ function f(name) {}
来源：http://bt.9csxet.cn

[U117] JS：单元测试
来源：http://tg.shtwfgs.cn

npm i -D vitest;  npx vitest
来源：http://qf.colortex.cn

[U118] JS：开发服务器
来源：http://jd.yuexingan06.cn

npm i -D vite;  npx vite
来源：http://ju.shxzukj.cn

[U119] JS：生产构建
来源：http://wl.521024.cn

npx vite build
来源：http://ri.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://rf.huixinmuqiang.cn

import.meta.env.VITE_API_URL
来源：http://ut.9csxet.cn

================================================================================
来源：http://oc.panjiajie.cn

统计汇总
来源：http://ym.hahajie.cn

================================================================================
来源：http://et.521024.cn

按语言统计（条）：
来源：http://xj.jianghongdianzi.cn

Python ......... 252
来源：http://es.szxytkj.cn

PHP ............ 252
来源：http://fm.nicolike.cn

JavaScript ..... 252
来源：http://zz.lnxyls.cn

TypeScript ..... 212
来源：http://rt.shxzukj.cn

Java ........... 212
来源：http://jy.9csxet.cn

Go ............. 212
来源：http://sd.shtwfgs.cn

Ruby ........... 212
来源：http://wp.bjjhwx.cn

C# ............. 212
来源：http://op.newstarts.cn

C .............. 30
来源：http://wh.9csxet.cn

C++ ............ 30
来源：http://ml.newstarts.cn

SQL ............ 90
来源：http://ai.szsharing.cn

Bash ........... 80
来源：http://dl.hahajie.cn

Kotlin ......... 15
来源：http://pn.gzmigu.cn

Swift .......... 15
来源：http://rb.bjjhwx.cn

Lua ............ 10
来源：http://dw.huanxung.cn

Perl ........... 10
来源：http://lg.wgjwhj.cn

Scala .......... 10
来源：http://sc.yuexingan06.cn

------------------------------------
来源：http://jc.shxzskj.cn

合计 ........... 2106 条
来源：http://aj.shxzskj.cn

按章节统计：
来源：http://jf.jctech888.com.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ce.muxihuayi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gh.yuntaijiaju.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jb.bjjhwx.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zd.panjiajie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vj.jianghongdianzi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pl.nicolike.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qi.szxytkj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ys.521024.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ce.nszjky.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gn.asd995.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ic.bookmarksfly.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mg.shxzskj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://az.haigaiapp.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kk.bookmarksfly.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://th.nicolike.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cp.panjiajie.cn

Q SQL 专题                              90
来源：http://wg.shxzskj.cn

R Bash 专题                             80
来源：http://ot.nicolike.cn

S C / C++ 专题                          60
来源：http://on.521024.cn

T 其他语言补充                          60
来源：http://wi.shxzskj.cn

U 高频实用片段                         120
来源：http://sj.jianghongdianzi.cn

------------------------------------
来源：http://cg.asd995.cn

合计                                  2106 条
来源：http://lw.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://oo.haigaiapp.cn

使用提醒
来源：http://cj.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://wn.huanxung.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qf.szxytkj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xp.yuexingan06.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xp.9csxet.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vg.bjjhwx.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qp.yuexingan06.cn

—— 文件结束 ——
来源：http://qp.hnjuh.cn

================================================================================
来源：http://lz.huixinmuqiang.cn

程序语言常见例子速查手册（2024 版）
来源：http://nm.szsharing.cn

Common Programming Examples Cheat Book
来源：http://se.shxzskj.cn

================================================================================
来源：http://na.szsharing.cn

【收录内容】
来源：http://tq.bookmarksfly.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vv.shtwfgs.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ua.bookmarksfly.cn

SQL · Bash · C · C++
来源：http://sv.szxytkj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://te.nszjky.cn

【使用说明】
来源：http://lp.lnxyls.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://oq.panjiajie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vt.jctech888.com.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wb.yuexingan06.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zg.shxzskj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qq.jianghongdianzi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://na.nszjky.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xl.shxzskj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fl.huixinmuqiang.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uz.hnjuh.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gv.bjjhwx.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rg.huixinmuqiang.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gg.bookmarksfly.cn

【文件统计】
来源：http://uz.lnxyls.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ca.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://bq.gzmigu.cn

目  录
来源：http://lo.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://fh.chemitech.net.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://su.yuexingan06.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cx.wgjwhj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://me.shtwfgs.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://sq.huixinmuqiang.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://iw.nszjky.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ly.hnjuh.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://va.huixiangedu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jm.shxzskj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ua.hahajie.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vj.chemitech.net.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kl.szxytkj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ro.521024.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://oj.hnjuh.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ie.shxzskj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ct.panjiajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jq.huanxung.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kh.wgjwhj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hy.9csxet.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pc.lnxyls.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fz.jianghongdianzi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yp.nicolike.cn

================================================================================
来源：http://mb.nicolike.cn

A. 基础语法与类型
来源：http://pp.bookmarksfly.cn

================================================================================
来源：http://ni.hahajie.cn

[A01] Hello World
来源：http://pb.lnxyls.cn

Py:   print("Hello, World!")
来源：http://ky.shtwfgs.cn

PHP:  echo "Hello, World!";
来源：http://yn.colortex.cn

JS:   console.log("Hello, World!");
来源：http://nm.lnxyls.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ns.szsharing.cn

Java: System.out.println("Hello, World!");
来源：http://wz.lnxyls.cn

Go:   fmt.Println("Hello, World!")
来源：http://rd.panjiajie.cn

Ruby: puts "Hello, World!"
来源：http://uf.hnjuh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jt.asd995.cn

[A02] 变量声明与赋值
来源：http://le.colortex.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jd.huixiangedu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://dg.bookmarksfly.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ag.9csxet.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kt.bookmarksfly.cn

Java: String name = "Alex"; int age = 20;
来源：http://ek.nicolike.cn

Go:   name := "Alex"; age := 20
来源：http://sh.521024.cn

Ruby: name = "Alex"; age = 20
来源：http://ns.jctech888.com.cn

C#:   string name = "Alex"; int age = 20;
来源：http://cd.jctech888.com.cn

[A03] 常量定义
来源：http://kd.huanxung.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cz.bookmarksfly.cn

PHP:  const PI = 3.14159;
来源：http://ig.bookmarksfly.cn

JS:   const PI = 3.14159;
来源：http://qd.colortex.cn

TS:   const PI: number = 3.14159;
来源：http://re.shtwfgs.cn

Java: static final double PI = 3.14159;
来源：http://ro.shtwfgs.cn

Go:   const PI = 3.14159
来源：http://uo.colortex.cn

Ruby: PI = 3.14159
来源：http://ex.huixiangedu.cn

C#:   const double PI = 3.14159;
来源：http://km.jianghongdianzi.cn

[A04] 判断变量类型
来源：http://rd.shxzukj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ma.huanxung.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gm.bookmarksfly.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ys.szsharing.cn

TS:   typeof x; x instanceof Date
来源：http://ne.yuexingan06.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fc.shtwfgs.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ok.shxzskj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://bb.bookmarksfly.cn

C#:   x.GetType().Name; x is int
来源：http://zi.jctech888.com.cn

[A05] 整数除法与取模
来源：http://at.szsharing.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hd.szxytkj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://hi.muxihuayi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yd.shxzskj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rf.shxzskj.cn

Java: 7 / 2; 7 % 2
来源：http://fh.shtwfgs.cn

Go:   7 / 2; 7 % 2
来源：http://lj.shxzukj.cn

Ruby: 7 / 2; 7 % 2
来源：http://pd.hahajie.cn

C#:   7 / 2; 7 % 2
来源：http://ea.shxzukj.cn

[A06] 字符串转数字
来源：http://gh.jctech888.com.cn

Py:   int("42"); float("3.14")
来源：http://zo.newstarts.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ks.muxihuayi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://en.yuexingan06.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ke.yuexingan06.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ie.hahajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xw.nszjky.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ns.yuntaijiaju.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://be.9csxet.cn

[A07] 数字转字符串
来源：http://yt.hnjuh.cn

Py:   str(42)
来源：http://bm.haigaiapp.cn

PHP:  (string) 42; strval(42)
来源：http://lp.szxytkj.cn

JS:   String(42); (42).toString()
来源：http://ww.jianghongdianzi.cn

TS:   String(42)
来源：http://fa.jianghongdianzi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xc.szxytkj.cn

Go:   strconv.Itoa(42)
来源：http://ix.shtwfgs.cn

Ruby: 42.to_s
来源：http://ui.gzmigu.cn

C#:   42.ToString()
来源：http://oh.jianghongdianzi.cn

[A08] 取整与四舍五入
来源：http://nc.szsharing.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://um.asd995.cn


<!-- 参考信息 -->