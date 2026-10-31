代发 wailian999

[U47] PHP：联合类型
来源：http://gw.hnjuh.cn

int|string $id
来源：http://pl.asd995.cn

[U48] PHP：纯枚举
来源：http://qk.szsharing.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pp.9csxet.cn

[U49] PHP：只读属性
来源：http://lg.newstarts.cn

public readonly string $name
来源：http://iu.szsharing.cn

[U50] PHP：构造器属性提升
来源：http://xm.szsharing.cn

public function __construct(private int $id) {}
来源：http://nc.asd995.cn

[U51] PHP：数组解构
来源：http://be.haigaiapp.cn

[$a, $b] = $arr;
来源：http://it.shxzskj.cn

[U52] PHP：箭头函数
来源：http://ql.bjjhwx.cn

$double = fn($x) => $x * 2;
来源：http://po.huanxung.cn

[U53] PHP：空合并运算符
来源：http://it.haigaiapp.cn

$v = $a ?? $b ?? "default";
来源：http://wi.9csxet.cn

[U54] PHP：空安全调用
来源：http://ta.haigaiapp.cn

$obj?->method()
来源：http://pi.jianghongdianzi.cn

[U55] PHP：match 表达式
来源：http://bt.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://aw.hnjuh.cn

[U56] PHP：命名参数
来源：http://sv.szsharing.cn

f(a: 1, b: 2)
来源：http://hd.yuexingan06.cn

[U57] PHP：字符串插值
来源：http://qh.nicolike.cn

"值: {$a}"
来源：http://hp.lnxyls.cn

[U58] PHP：数组三件套
来源：http://dr.colortex.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jm.muxihuayi.cn

[U59] PHP：自定义排序
来源：http://vd.panjiajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yb.jctech888.com.cn

[U60] PHP：JSON 编解码
来源：http://we.9csxet.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ub.panjiajie.cn

[U61] PHP：正则
来源：http://bx.wgjwhj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wk.haigaiapp.cn

[U62] PHP：日期对象
来源：http://us.chemitech.net.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gp.jianghongdianzi.cn

[U63] PHP：文件读写
来源：http://zb.szxytkj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vx.shxzskj.cn

[U64] PHP：目录遍历
来源：http://cf.bjjhwx.cn

glob("dir/*.php");  scandir("dir");
来源：http://yk.panjiajie.cn

[U65] PHP：会话
来源：http://wv.bookmarksfly.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sy.hahajie.cn

[U66] PHP：设置 Cookie
来源：http://rr.hahajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nz.huixinmuqiang.cn

[U67] PHP：处理文件上传
来源：http://ax.haigaiapp.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yl.shtwfgs.cn

[U68] PHP：PDO 连接
来源：http://om.huixiangedu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wd.wgjwhj.cn

[U69] PHP：PDO 预处理
来源：http://fc.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zg.huanxung.cn

[U70] PHP：PDO 事务
来源：http://il.hnjuh.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jv.gzmigu.cn

[U71] PHP：抛出异常
来源：http://va.huixinmuqiang.cn

throw new RuntimeException("失败", 500);
来源：http://xc.gzmigu.cn

[U72] PHP：写错误日志
来源：http://ap.gzmigu.cn

error_log("失败: " . $e->getMessage());
来源：http://ql.yuntaijiaju.cn

[U73] PHP：读取 ini 配置
来源：http://nr.jctech888.com.cn

parse_ini_file("config.ini", true)
来源：http://hz.wgjwhj.cn

[U74] PHP：读取环境变量
来源：http://qt.chemitech.net.cn

getenv("APP_ENV") ?: "production"
来源：http://mx.bookmarksfly.cn

[U75] PHP：依赖注入
来源：http://op.gzmigu.cn

composer require psr/container
来源：http://ec.colortex.cn

[U76] PHP：简单路由
来源：http://lc.shxzukj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bd.wgjwhj.cn

[U77] PHP：模板渲染
来源：http://ts.szxytkj.cn

composer require twig/twig
来源：http://ff.gzmigu.cn

[U78] PHP：单元测试
来源：http://fh.panjiajie.cn

composer require --dev phpunit/phpunit
来源：http://gw.bjjhwx.cn

[U79] PHP：静态分析
来源：http://vb.jctech888.com.cn

composer require --dev phpstan/phpstan
来源：http://jk.huixiangedu.cn

[U80] PHP：代码规范修复
来源：http://ip.nszjky.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://eu.huanxung.cn

[U81] JS：初始化项目
来源：http://ux.9csxet.cn

npm init -y;  npm i express
来源：http://iz.hahajie.cn

[U82] JS：package.json 脚本
来源：http://ri.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bm.521024.cn

[U83] JS：ES Module 导入导出
来源：http://nv.9csxet.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tj.bjjhwx.cn

[U84] JS：CommonJS 写法
来源：http://ro.muxihuayi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://po.bookmarksfly.cn

[U85] JS：可选链
来源：http://bt.newstarts.cn

a?.b?.c
来源：http://wg.gzmigu.cn

[U86] JS：空值合并
来源：http://pb.gzmigu.cn

a ?? b
来源：http://dz.lnxyls.cn

[U87] JS：解构默认值
来源：http://to.yuexingan06.cn

const { a = 1, b = 2 } = obj;
来源：http://cd.yuntaijiaju.cn

[U88] JS：对象展开合并
来源：http://yx.hahajie.cn

{ ...a, ...b }
来源：http://dg.jctech888.com.cn

[U89] JS：数组去重
来源：http://ck.huanxung.cn

[...new Set(arr)]
来源：http://xz.hahajie.cn

[U90] JS：数字数组排序
来源：http://ia.shxzskj.cn

[...arr].sort((a, b) => a - b)
来源：http://sm.huanxung.cn

[U91] JS：对象键值遍历
来源：http://hh.lnxyls.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://it.haigaiapp.cn

[U92] JS：深拷贝
来源：http://db.shxzukj.cn

structuredClone(obj)
来源：http://fc.shtwfgs.cn

[U93] JS：模板字符串
来源：http://xc.nicolike.cn

`共 ${n} 条`
来源：http://jg.asd995.cn

[U94] JS：箭头函数
来源：http://tl.szxytkj.cn

const double = x => x * 2;
来源：http://uc.yuntaijiaju.cn

[U95] JS：Promise 包装
来源：http://vb.huixinmuqiang.cn

new Promise((resolve, reject) => {})
来源：http://xs.newstarts.cn

[U96] JS：async/await 与异常
来源：http://zd.shxzukj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rr.shtwfgs.cn

[U97] JS：并发请求
来源：http://bm.jianghongdianzi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://er.yuntaijiaju.cn

[U98] JS：fetch 带 JSON
来源：http://aq.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bp.gzmigu.cn

[U99] JS：事件监听
来源：http://lh.gzmigu.cn

el.addEventListener("click", e => {})
来源：http://vl.huanxung.cn

[U100] JS：DOM 查询
来源：http://tm.gzmigu.cn

document.querySelector(".item")
来源：http://dg.yuntaijiaju.cn

[U101] JS：classList 操作
来源：http://eb.nszjky.cn

el.classList.toggle("active")
来源：http://rk.9csxet.cn

[U102] JS：本地存储
来源：http://lo.szxytkj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ab.bookmarksfly.cn

[U103] JS：定时器
来源：http://hr.chemitech.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://il.newstarts.cn

[U104] JS：防抖
来源：http://vm.szsharing.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ef.yuntaijiaju.cn

[U105] JS：节流
来源：http://ye.asd995.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ws.jianghongdianzi.cn

[U106] JS：日期格式化
来源：http://oy.bjjhwx.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qk.9csxet.cn

[U107] JS：数字千分位
来源：http://ni.gzmigu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pe.hahajie.cn

[U108] JS：随机整数
来源：http://rt.shxzukj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bi.colortex.cn

[U109] JS：数组分组
来源：http://bg.lnxyls.cn

Object.groupBy(arr, x => x.type)
来源：http://zt.haigaiapp.cn

[U110] JS：数组分块
来源：http://nb.nicolike.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ec.bookmarksfly.cn

[U111] JS：对象转 Map
来源：http://mw.huixiangedu.cn

new Map(Object.entries(obj))
来源：http://ix.colortex.cn

[U112] JS：字符串补位
来源：http://qw.nszjky.cn

"7".padStart(3, "0")
来源：http://sb.yuntaijiaju.cn

[U113] JS：正则替换全部
来源：http://hr.muxihuayi.cn

s.replaceAll("a", "b")
来源：http://dy.yuntaijiaju.cn

[U114] JS：JSON 深比较
来源：http://qn.panjiajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ex.hahajie.cn

[U115] JS：生成 UUID
来源：http://tz.chemitech.net.cn

crypto.randomUUID()
来源：http://zn.chemitech.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://rd.newstarts.cn

/** @param {string} name */ function f(name) {}
来源：http://uv.shtwfgs.cn

[U117] JS：单元测试
来源：http://ud.hnjuh.cn

npm i -D vitest;  npx vitest
来源：http://zj.chemitech.net.cn

[U118] JS：开发服务器
来源：http://ht.hahajie.cn

npm i -D vite;  npx vite
来源：http://vm.newstarts.cn

[U119] JS：生产构建
来源：http://hr.nicolike.cn

npx vite build
来源：http://jb.jianghongdianzi.cn

[U120] JS：读取环境变量（Vite）
来源：http://xj.colortex.cn

import.meta.env.VITE_API_URL
来源：http://gj.jctech888.com.cn

================================================================================
来源：http://om.huixiangedu.cn

统计汇总
来源：http://vo.yuexingan06.cn

================================================================================
来源：http://gg.521024.cn

按语言统计（条）：
来源：http://hj.9csxet.cn

Python ......... 252
来源：http://zb.nicolike.cn

PHP ............ 252
来源：http://lz.hahajie.cn

JavaScript ..... 252
来源：http://bo.521024.cn

TypeScript ..... 212
来源：http://dl.haigaiapp.cn

Java ........... 212
来源：http://qk.jianghongdianzi.cn

Go ............. 212
来源：http://if.colortex.cn

Ruby ........... 212
来源：http://nl.9csxet.cn

C# ............. 212
来源：http://oh.wgjwhj.cn

C .............. 30
来源：http://ve.jctech888.com.cn

C++ ............ 30
来源：http://yu.szsharing.cn

SQL ............ 90
来源：http://vd.521024.cn

Bash ........... 80
来源：http://ds.lnxyls.cn

Kotlin ......... 15
来源：http://ak.lnxyls.cn

Swift .......... 15
来源：http://kh.bjjhwx.cn

Lua ............ 10
来源：http://gi.wgjwhj.cn

Perl ........... 10
来源：http://yo.colortex.cn

Scala .......... 10
来源：http://rg.muxihuayi.cn

------------------------------------
来源：http://nf.haigaiapp.cn

合计 ........... 2106 条
来源：http://ir.9csxet.cn

按章节统计：
来源：http://uv.wgjwhj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ah.nicolike.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wk.newstarts.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jn.newstarts.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bd.huixiangedu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ac.hahajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bz.asd995.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sb.jctech888.com.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gh.haigaiapp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ev.hahajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kf.huixinmuqiang.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://be.haigaiapp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ex.asd995.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ub.nszjky.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hr.hnjuh.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yc.shtwfgs.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://sx.lnxyls.cn

Q SQL 专题                              90
来源：http://qi.haigaiapp.cn

R Bash 专题                             80
来源：http://yk.9csxet.cn

S C / C++ 专题                          60
来源：http://je.haigaiapp.cn

T 其他语言补充                          60
来源：http://lg.huixiangedu.cn

U 高频实用片段                         120
来源：http://sb.nicolike.cn

------------------------------------
来源：http://ba.9csxet.cn

合计                                  2106 条
来源：http://xz.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://xv.jianghongdianzi.cn

使用提醒
来源：http://rm.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://xj.yuexingan06.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ag.shxzukj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cd.bookmarksfly.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jl.shxzskj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ol.gzmigu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bh.muxihuayi.cn

—— 文件结束 ——
来源：http://em.chemitech.net.cn

================================================================================
来源：http://zu.asd995.cn

程序语言常见例子速查手册（2024 版）
来源：http://pk.jctech888.com.cn

Common Programming Examples Cheat Book
来源：http://zm.szsharing.cn

================================================================================
来源：http://be.nicolike.cn

【收录内容】
来源：http://il.shxzukj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://bc.jctech888.com.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cy.huanxung.cn

SQL · Bash · C · C++
来源：http://uy.hnjuh.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gp.szxytkj.cn

【使用说明】
来源：http://xs.colortex.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yt.asd995.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rr.bookmarksfly.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hk.muxihuayi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://er.hnjuh.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://bq.shxzskj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dj.wgjwhj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xr.huixiangedu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ce.wgjwhj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://iq.nicolike.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jy.lnxyls.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pj.gzmigu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mn.jctech888.com.cn

【文件统计】
来源：http://tv.shxzskj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qw.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://rt.panjiajie.cn

目  录
来源：http://us.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://bq.haigaiapp.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rp.lnxyls.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://uo.nicolike.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ui.gzmigu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ee.lnxyls.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fo.521024.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xn.jctech888.com.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uq.muxihuayi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hd.hnjuh.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lj.huixinmuqiang.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lz.521024.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wm.colortex.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xu.hahajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vc.chemitech.net.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://da.szsharing.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qm.9csxet.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ev.newstarts.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ph.shxzskj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hv.lnxyls.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mi.szsharing.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ll.yuntaijiaju.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pj.lnxyls.cn

================================================================================
来源：http://ez.wgjwhj.cn

A. 基础语法与类型
来源：http://mz.szsharing.cn

================================================================================
来源：http://ck.hahajie.cn

[A01] Hello World
来源：http://tw.panjiajie.cn

Py:   print("Hello, World!")
来源：http://kw.bjjhwx.cn

PHP:  echo "Hello, World!";
来源：http://kr.yuntaijiaju.cn

JS:   console.log("Hello, World!");
来源：http://lj.szxytkj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ct.shtwfgs.cn

Java: System.out.println("Hello, World!");
来源：http://dz.yuntaijiaju.cn

Go:   fmt.Println("Hello, World!")
来源：http://ae.shtwfgs.cn

Ruby: puts "Hello, World!"
来源：http://cm.asd995.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vy.521024.cn

[A02] 变量声明与赋值
来源：http://zn.lnxyls.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://eb.yuexingan06.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://zj.bookmarksfly.cn

JS:   let name = "Alex"; const age = 20;
来源：http://sb.wgjwhj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://iq.szxytkj.cn

Java: String name = "Alex"; int age = 20;
来源：http://ta.szsharing.cn

Go:   name := "Alex"; age := 20
来源：http://ct.bjjhwx.cn

Ruby: name = "Alex"; age = 20
来源：http://sk.muxihuayi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://rv.bookmarksfly.cn

[A03] 常量定义
来源：http://zh.huanxung.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xy.yuntaijiaju.cn

PHP:  const PI = 3.14159;
来源：http://ri.jctech888.com.cn

JS:   const PI = 3.14159;
来源：http://tr.nicolike.cn

TS:   const PI: number = 3.14159;
来源：http://ny.521024.cn

Java: static final double PI = 3.14159;
来源：http://vh.huanxung.cn

Go:   const PI = 3.14159
来源：http://xg.haigaiapp.cn

Ruby: PI = 3.14159
来源：http://uu.muxihuayi.cn

C#:   const double PI = 3.14159;
来源：http://fg.lnxyls.cn

[A04] 判断变量类型
来源：http://ht.yuntaijiaju.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://gb.hnjuh.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fp.bookmarksfly.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cn.shxzukj.cn

TS:   typeof x; x instanceof Date
来源：http://sg.bjjhwx.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ow.huanxung.cn

Go:   reflect.TypeOf(x).Name()
来源：http://xd.huixinmuqiang.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ub.hnjuh.cn

C#:   x.GetType().Name; x is int
来源：http://gr.huixiangedu.cn

[A05] 整数除法与取模
来源：http://nr.jianghongdianzi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://sz.haigaiapp.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://eg.huixinmuqiang.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ir.haigaiapp.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fe.szsharing.cn

Java: 7 / 2; 7 % 2
来源：http://bu.nicolike.cn

Go:   7 / 2; 7 % 2
来源：http://yl.nszjky.cn

Ruby: 7 / 2; 7 % 2
来源：http://fb.nszjky.cn

C#:   7 / 2; 7 % 2
来源：http://co.nicolike.cn


<!-- 参考信息 -->