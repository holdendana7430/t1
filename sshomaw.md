代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://pj.szsharing.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yc.muxihuayi.cn

[U42] PHP：PSR-4 自动加载
来源：http://ol.bookmarksfly.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mf.haigaiapp.cn

[U43] PHP：声明命名空间
来源：http://wk.muxihuayi.cn

namespace App\Http;
来源：http://mu.yuexingan06.cn

[U44] PHP：开启严格类型
来源：http://nd.newstarts.cn

declare(strict_types=1);
来源：http://vy.hnjuh.cn

[U45] PHP：类型声明与返回类型
来源：http://as.szsharing.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jc.huixinmuqiang.cn

[U46] PHP：可空类型
来源：http://bl.colortex.cn

?string $name = null
来源：http://mr.asd995.cn

[U47] PHP：联合类型
来源：http://ee.yuexingan06.cn

int|string $id
来源：http://pa.asd995.cn

[U48] PHP：纯枚举
来源：http://du.huixiangedu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ps.521024.cn

[U49] PHP：只读属性
来源：http://kz.jctech888.com.cn

public readonly string $name
来源：http://wc.9csxet.cn

[U50] PHP：构造器属性提升
来源：http://pp.shtwfgs.cn

public function __construct(private int $id) {}
来源：http://eu.jctech888.com.cn

[U51] PHP：数组解构
来源：http://ch.newstarts.cn

[$a, $b] = $arr;
来源：http://gt.jianghongdianzi.cn

[U52] PHP：箭头函数
来源：http://zf.yuexingan06.cn

$double = fn($x) => $x * 2;
来源：http://nx.haigaiapp.cn

[U53] PHP：空合并运算符
来源：http://pk.colortex.cn

$v = $a ?? $b ?? "default";
来源：http://uq.shxzskj.cn

[U54] PHP：空安全调用
来源：http://cc.shtwfgs.cn

$obj?->method()
来源：http://xe.szsharing.cn

[U55] PHP：match 表达式
来源：http://ke.panjiajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bh.hahajie.cn

[U56] PHP：命名参数
来源：http://qa.haigaiapp.cn

f(a: 1, b: 2)
来源：http://qx.huixiangedu.cn

[U57] PHP：字符串插值
来源：http://qa.lnxyls.cn

"值: {$a}"
来源：http://xt.asd995.cn

[U58] PHP：数组三件套
来源：http://me.nszjky.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://uy.nicolike.cn

[U59] PHP：自定义排序
来源：http://ow.haigaiapp.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fv.huixinmuqiang.cn

[U60] PHP：JSON 编解码
来源：http://yw.chemitech.net.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://td.hahajie.cn

[U61] PHP：正则
来源：http://fu.chemitech.net.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vn.lnxyls.cn

[U62] PHP：日期对象
来源：http://jd.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://oy.bjjhwx.cn

[U63] PHP：文件读写
来源：http://jl.wgjwhj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zr.yuntaijiaju.cn

[U64] PHP：目录遍历
来源：http://rr.szxytkj.cn

glob("dir/*.php");  scandir("dir");
来源：http://po.haigaiapp.cn

[U65] PHP：会话
来源：http://uo.lnxyls.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hp.lnxyls.cn

[U66] PHP：设置 Cookie
来源：http://od.shxzskj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://eg.shxzukj.cn

[U67] PHP：处理文件上传
来源：http://fg.hnjuh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zb.gzmigu.cn

[U68] PHP：PDO 连接
来源：http://vd.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yj.bookmarksfly.cn

[U69] PHP：PDO 预处理
来源：http://kv.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ek.huixiangedu.cn

[U70] PHP：PDO 事务
来源：http://ex.colortex.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xp.huanxung.cn

[U71] PHP：抛出异常
来源：http://wv.bookmarksfly.cn

throw new RuntimeException("失败", 500);
来源：http://lt.nszjky.cn

[U72] PHP：写错误日志
来源：http://eg.huixinmuqiang.cn

error_log("失败: " . $e->getMessage());
来源：http://dp.lnxyls.cn

[U73] PHP：读取 ini 配置
来源：http://ex.shtwfgs.cn

parse_ini_file("config.ini", true)
来源：http://pb.asd995.cn

[U74] PHP：读取环境变量
来源：http://hd.haigaiapp.cn

getenv("APP_ENV") ?: "production"
来源：http://ky.9csxet.cn

[U75] PHP：依赖注入
来源：http://ss.jctech888.com.cn

composer require psr/container
来源：http://fk.shxzskj.cn

[U76] PHP：简单路由
来源：http://sj.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sl.gzmigu.cn

[U77] PHP：模板渲染
来源：http://ge.panjiajie.cn

composer require twig/twig
来源：http://pa.bjjhwx.cn

[U78] PHP：单元测试
来源：http://ox.jctech888.com.cn

composer require --dev phpunit/phpunit
来源：http://vu.hnjuh.cn

[U79] PHP：静态分析
来源：http://ht.huixinmuqiang.cn

composer require --dev phpstan/phpstan
来源：http://mz.bookmarksfly.cn

[U80] PHP：代码规范修复
来源：http://an.huixiangedu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sv.szxytkj.cn

[U81] JS：初始化项目
来源：http://vd.gzmigu.cn

npm init -y;  npm i express
来源：http://dg.jctech888.com.cn

[U82] JS：package.json 脚本
来源：http://gj.panjiajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ea.521024.cn

[U83] JS：ES Module 导入导出
来源：http://vl.chemitech.net.cn

export const a = 1;  import { a } from "./m.js";
来源：http://pd.jianghongdianzi.cn

[U84] JS：CommonJS 写法
来源：http://zh.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bd.nicolike.cn

[U85] JS：可选链
来源：http://ue.yuexingan06.cn

a?.b?.c
来源：http://jx.huixiangedu.cn

[U86] JS：空值合并
来源：http://oh.colortex.cn

a ?? b
来源：http://qw.panjiajie.cn

[U87] JS：解构默认值
来源：http://ez.shxzukj.cn

const { a = 1, b = 2 } = obj;
来源：http://hx.szxytkj.cn

[U88] JS：对象展开合并
来源：http://so.haigaiapp.cn

{ ...a, ...b }
来源：http://na.shxzukj.cn

[U89] JS：数组去重
来源：http://kh.shxzukj.cn

[...new Set(arr)]
来源：http://jn.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://qc.shxzskj.cn

[...arr].sort((a, b) => a - b)
来源：http://im.shtwfgs.cn

[U91] JS：对象键值遍历
来源：http://wg.wgjwhj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xe.wgjwhj.cn

[U92] JS：深拷贝
来源：http://tp.bookmarksfly.cn

structuredClone(obj)
来源：http://ry.lnxyls.cn

[U93] JS：模板字符串
来源：http://lp.nszjky.cn

`共 ${n} 条`
来源：http://bi.gzmigu.cn

[U94] JS：箭头函数
来源：http://ld.lnxyls.cn

const double = x => x * 2;
来源：http://te.chemitech.net.cn

[U95] JS：Promise 包装
来源：http://ev.shtwfgs.cn

new Promise((resolve, reject) => {})
来源：http://dn.asd995.cn

[U96] JS：async/await 与异常
来源：http://ui.haigaiapp.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ch.lnxyls.cn

[U97] JS：并发请求
来源：http://jm.shtwfgs.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dd.521024.cn

[U98] JS：fetch 带 JSON
来源：http://xu.muxihuayi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ni.huixiangedu.cn

[U99] JS：事件监听
来源：http://mh.asd995.cn

el.addEventListener("click", e => {})
来源：http://ik.colortex.cn

[U100] JS：DOM 查询
来源：http://ep.9csxet.cn

document.querySelector(".item")
来源：http://pc.muxihuayi.cn

[U101] JS：classList 操作
来源：http://rm.lnxyls.cn

el.classList.toggle("active")
来源：http://pr.bjjhwx.cn

[U102] JS：本地存储
来源：http://pw.shxzskj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jo.haigaiapp.cn

[U103] JS：定时器
来源：http://th.bookmarksfly.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://im.szxytkj.cn

[U104] JS：防抖
来源：http://uc.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qf.huixinmuqiang.cn

[U105] JS：节流
来源：http://gj.521024.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ko.hnjuh.cn

[U106] JS：日期格式化
来源：http://bs.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ty.521024.cn

[U107] JS：数字千分位
来源：http://ff.hahajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pw.newstarts.cn

[U108] JS：随机整数
来源：http://ax.bjjhwx.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yd.huixiangedu.cn

[U109] JS：数组分组
来源：http://ie.gzmigu.cn

Object.groupBy(arr, x => x.type)
来源：http://va.wgjwhj.cn

[U110] JS：数组分块
来源：http://oc.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rb.huanxung.cn

[U111] JS：对象转 Map
来源：http://ft.shxzukj.cn

new Map(Object.entries(obj))
来源：http://dg.gzmigu.cn

[U112] JS：字符串补位
来源：http://zj.muxihuayi.cn

"7".padStart(3, "0")
来源：http://jk.jianghongdianzi.cn

[U113] JS：正则替换全部
来源：http://eu.gzmigu.cn

s.replaceAll("a", "b")
来源：http://tf.shtwfgs.cn

[U114] JS：JSON 深比较
来源：http://en.huanxung.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pu.panjiajie.cn

[U115] JS：生成 UUID
来源：http://rr.gzmigu.cn

crypto.randomUUID()
来源：http://fr.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://nb.szsharing.cn

/** @param {string} name */ function f(name) {}
来源：http://ge.yuntaijiaju.cn

[U117] JS：单元测试
来源：http://ra.huanxung.cn

npm i -D vitest;  npx vitest
来源：http://pt.huixinmuqiang.cn

[U118] JS：开发服务器
来源：http://sg.huanxung.cn

npm i -D vite;  npx vite
来源：http://fm.nicolike.cn

[U119] JS：生产构建
来源：http://za.huixinmuqiang.cn

npx vite build
来源：http://si.shtwfgs.cn

[U120] JS：读取环境变量（Vite）
来源：http://ya.szxytkj.cn

import.meta.env.VITE_API_URL
来源：http://ab.haigaiapp.cn

================================================================================
来源：http://pg.shxzukj.cn

统计汇总
来源：http://tr.huanxung.cn

================================================================================
来源：http://de.yuexingan06.cn

按语言统计（条）：
来源：http://ox.jctech888.com.cn

Python ......... 252
来源：http://sl.nszjky.cn

PHP ............ 252
来源：http://kq.wgjwhj.cn

JavaScript ..... 252
来源：http://bl.szxytkj.cn

TypeScript ..... 212
来源：http://qi.jctech888.com.cn

Java ........... 212
来源：http://lc.gzmigu.cn

Go ............. 212
来源：http://ua.asd995.cn

Ruby ........... 212
来源：http://cg.lnxyls.cn

C# ............. 212
来源：http://ah.szsharing.cn

C .............. 30
来源：http://al.nicolike.cn

C++ ............ 30
来源：http://zc.nszjky.cn

SQL ............ 90
来源：http://bk.szxytkj.cn

Bash ........... 80
来源：http://nk.wgjwhj.cn

Kotlin ......... 15
来源：http://bx.huixinmuqiang.cn

Swift .......... 15
来源：http://lj.chemitech.net.cn

Lua ............ 10
来源：http://iw.huixinmuqiang.cn

Perl ........... 10
来源：http://yb.huanxung.cn

Scala .......... 10
来源：http://su.yuexingan06.cn

------------------------------------
来源：http://ej.colortex.cn

合计 ........... 2106 条
来源：http://re.wgjwhj.cn

按章节统计：
来源：http://qi.lnxyls.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pv.shxzskj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vr.huixiangedu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zn.wgjwhj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xl.shxzskj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://aw.szsharing.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vv.chemitech.net.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gt.shxzukj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ob.bookmarksfly.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ei.szsharing.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qf.nicolike.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cc.lnxyls.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://eu.jianghongdianzi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cv.newstarts.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yx.hnjuh.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xr.szxytkj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hg.colortex.cn

Q SQL 专题                              90
来源：http://xf.wgjwhj.cn

R Bash 专题                             80
来源：http://nj.szsharing.cn

S C / C++ 专题                          60
来源：http://yt.bookmarksfly.cn

T 其他语言补充                          60
来源：http://am.521024.cn

U 高频实用片段                         120
来源：http://hj.muxihuayi.cn

------------------------------------
来源：http://ak.521024.cn

合计                                  2106 条
来源：http://yl.nszjky.cn

--------------------------------------------------------------------------------
来源：http://vc.chemitech.net.cn

使用提醒
来源：http://qa.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://ug.szxytkj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rd.yuexingan06.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://so.gzmigu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ny.shxzskj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wn.jianghongdianzi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ng.shtwfgs.cn

—— 文件结束 ——
来源：http://oc.haigaiapp.cn

================================================================================
来源：http://ha.shxzukj.cn

程序语言常见例子速查手册（2024 版）
来源：http://ta.bookmarksfly.cn

Common Programming Examples Cheat Book
来源：http://fh.jianghongdianzi.cn

================================================================================
来源：http://vi.jctech888.com.cn

【收录内容】
来源：http://cr.chemitech.net.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://wy.gzmigu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rh.szsharing.cn

SQL · Bash · C · C++
来源：http://kl.hnjuh.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ac.bjjhwx.cn

【使用说明】
来源：http://lm.yuexingan06.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nr.yuntaijiaju.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://im.panjiajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://br.9csxet.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://oq.521024.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ru.haigaiapp.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gi.yuntaijiaju.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://uu.huixiangedu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ei.chemitech.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yw.nicolike.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pn.gzmigu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://eb.hnjuh.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xn.chemitech.net.cn

【文件统计】
来源：http://zr.nicolike.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hf.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://qf.yuexingan06.cn

目  录
来源：http://mp.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://gg.bjjhwx.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tc.huixiangedu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zc.nicolike.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nk.bjjhwx.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ia.bjjhwx.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://oe.colortex.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://iy.hnjuh.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zu.newstarts.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ia.shxzukj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ho.muxihuayi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://aq.haigaiapp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ca.huixinmuqiang.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qe.nicolike.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lr.shxzukj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yc.nicolike.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kl.huanxung.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dp.hahajie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rq.521024.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://uy.bookmarksfly.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sm.9csxet.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ng.shxzskj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nq.szsharing.cn

================================================================================
来源：http://ip.haigaiapp.cn

A. 基础语法与类型
来源：http://gm.yuexingan06.cn

================================================================================
来源：http://hv.wgjwhj.cn

[A01] Hello World
来源：http://bc.muxihuayi.cn

Py:   print("Hello, World!")
来源：http://cb.9csxet.cn

PHP:  echo "Hello, World!";
来源：http://gj.yuntaijiaju.cn

JS:   console.log("Hello, World!");
来源：http://rr.521024.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ep.yuntaijiaju.cn

Java: System.out.println("Hello, World!");
来源：http://oo.colortex.cn

Go:   fmt.Println("Hello, World!")
来源：http://ku.bookmarksfly.cn

Ruby: puts "Hello, World!"
来源：http://vn.haigaiapp.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://sd.nicolike.cn

[A02] 变量声明与赋值
来源：http://pw.haigaiapp.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jy.jctech888.com.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://up.shtwfgs.cn

JS:   let name = "Alex"; const age = 20;
来源：http://pw.muxihuayi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vk.huixiangedu.cn

Java: String name = "Alex"; int age = 20;
来源：http://zw.szsharing.cn

Go:   name := "Alex"; age := 20
来源：http://kl.haigaiapp.cn

Ruby: name = "Alex"; age = 20
来源：http://qw.9csxet.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ep.huanxung.cn

[A03] 常量定义
来源：http://ad.muxihuayi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ye.lnxyls.cn

PHP:  const PI = 3.14159;
来源：http://yu.haigaiapp.cn

JS:   const PI = 3.14159;
来源：http://pd.asd995.cn

TS:   const PI: number = 3.14159;
来源：http://lq.9csxet.cn

Java: static final double PI = 3.14159;
来源：http://nw.shxzukj.cn

Go:   const PI = 3.14159
来源：http://yj.9csxet.cn

Ruby: PI = 3.14159
来源：http://io.huixinmuqiang.cn

C#:   const double PI = 3.14159;
来源：http://ew.hnjuh.cn

[A04] 判断变量类型
来源：http://ld.gzmigu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hh.huixinmuqiang.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vp.colortex.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yq.szsharing.cn

TS:   typeof x; x instanceof Date
来源：http://qe.shxzskj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xa.asd995.cn


<!-- 参考信息 -->