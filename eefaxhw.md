代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://xl.muxihuayi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ib.muxihuayi.cn

[U42] PHP：PSR-4 自动加载
来源：http://nk.huixinmuqiang.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gx.newstarts.cn

[U43] PHP：声明命名空间
来源：http://cv.colortex.cn

namespace App\Http;
来源：http://bq.bjjhwx.cn

[U44] PHP：开启严格类型
来源：http://ns.muxihuayi.cn

declare(strict_types=1);
来源：http://fm.nicolike.cn

[U45] PHP：类型声明与返回类型
来源：http://du.shxzskj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://es.521024.cn

[U46] PHP：可空类型
来源：http://xy.asd995.cn

?string $name = null
来源：http://zl.jianghongdianzi.cn

[U47] PHP：联合类型
来源：http://lb.wgjwhj.cn

int|string $id
来源：http://zf.asd995.cn

[U48] PHP：纯枚举
来源：http://qn.nicolike.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ec.gzmigu.cn

[U49] PHP：只读属性
来源：http://zi.yuexingan06.cn

public readonly string $name
来源：http://su.nszjky.cn

[U50] PHP：构造器属性提升
来源：http://ku.hahajie.cn

public function __construct(private int $id) {}
来源：http://ae.hnjuh.cn

[U51] PHP：数组解构
来源：http://al.panjiajie.cn

[$a, $b] = $arr;
来源：http://ow.shxzukj.cn

[U52] PHP：箭头函数
来源：http://sx.nszjky.cn

$double = fn($x) => $x * 2;
来源：http://pg.colortex.cn

[U53] PHP：空合并运算符
来源：http://sy.bjjhwx.cn

$v = $a ?? $b ?? "default";
来源：http://vm.newstarts.cn

[U54] PHP：空安全调用
来源：http://sq.9csxet.cn

$obj?->method()
来源：http://uc.colortex.cn

[U55] PHP：match 表达式
来源：http://tl.colortex.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://oa.newstarts.cn

[U56] PHP：命名参数
来源：http://zz.szsharing.cn

f(a: 1, b: 2)
来源：http://dm.521024.cn

[U57] PHP：字符串插值
来源：http://za.nszjky.cn

"值: {$a}"
来源：http://ew.haigaiapp.cn

[U58] PHP：数组三件套
来源：http://uy.yuntaijiaju.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hm.chemitech.net.cn

[U59] PHP：自定义排序
来源：http://rp.colortex.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wd.hnjuh.cn

[U60] PHP：JSON 编解码
来源：http://zw.jianghongdianzi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://at.bookmarksfly.cn

[U61] PHP：正则
来源：http://ow.521024.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cc.gzmigu.cn

[U62] PHP：日期对象
来源：http://xx.bjjhwx.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ff.newstarts.cn

[U63] PHP：文件读写
来源：http://ox.bookmarksfly.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vr.asd995.cn

[U64] PHP：目录遍历
来源：http://ed.newstarts.cn

glob("dir/*.php");  scandir("dir");
来源：http://xw.panjiajie.cn

[U65] PHP：会话
来源：http://cv.huanxung.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rx.chemitech.net.cn

[U66] PHP：设置 Cookie
来源：http://zy.szxytkj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ol.gzmigu.cn

[U67] PHP：处理文件上传
来源：http://ym.yuexingan06.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yv.jctech888.com.cn

[U68] PHP：PDO 连接
来源：http://si.lnxyls.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uv.nszjky.cn

[U69] PHP：PDO 预处理
来源：http://sc.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vb.nszjky.cn

[U70] PHP：PDO 事务
来源：http://rj.colortex.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pl.shtwfgs.cn

[U71] PHP：抛出异常
来源：http://yq.jctech888.com.cn

throw new RuntimeException("失败", 500);
来源：http://nl.gzmigu.cn

[U72] PHP：写错误日志
来源：http://yn.hahajie.cn

error_log("失败: " . $e->getMessage());
来源：http://dc.wgjwhj.cn

[U73] PHP：读取 ini 配置
来源：http://ny.huixiangedu.cn

parse_ini_file("config.ini", true)
来源：http://rx.huixiangedu.cn

[U74] PHP：读取环境变量
来源：http://ov.gzmigu.cn

getenv("APP_ENV") ?: "production"
来源：http://ig.yuexingan06.cn

[U75] PHP：依赖注入
来源：http://ft.szsharing.cn

composer require psr/container
来源：http://qp.yuntaijiaju.cn

[U76] PHP：简单路由
来源：http://yx.huixiangedu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://et.colortex.cn

[U77] PHP：模板渲染
来源：http://fa.jctech888.com.cn

composer require twig/twig
来源：http://ds.hnjuh.cn

[U78] PHP：单元测试
来源：http://ei.yuexingan06.cn

composer require --dev phpunit/phpunit
来源：http://rz.szsharing.cn

[U79] PHP：静态分析
来源：http://nj.nszjky.cn

composer require --dev phpstan/phpstan
来源：http://pz.bookmarksfly.cn

[U80] PHP：代码规范修复
来源：http://jw.shtwfgs.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ns.shtwfgs.cn

[U81] JS：初始化项目
来源：http://gt.huanxung.cn

npm init -y;  npm i express
来源：http://jg.nszjky.cn

[U82] JS：package.json 脚本
来源：http://ip.bookmarksfly.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://by.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://fg.huanxung.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mh.shxzskj.cn

[U84] JS：CommonJS 写法
来源：http://xj.bjjhwx.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qh.yuntaijiaju.cn

[U85] JS：可选链
来源：http://gt.shxzukj.cn

a?.b?.c
来源：http://lw.jctech888.com.cn

[U86] JS：空值合并
来源：http://nr.colortex.cn

a ?? b
来源：http://zw.521024.cn

[U87] JS：解构默认值
来源：http://vg.chemitech.net.cn

const { a = 1, b = 2 } = obj;
来源：http://dr.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://iv.asd995.cn

{ ...a, ...b }
来源：http://xp.chemitech.net.cn

[U89] JS：数组去重
来源：http://da.asd995.cn

[...new Set(arr)]
来源：http://pn.shtwfgs.cn

[U90] JS：数字数组排序
来源：http://yx.szsharing.cn

[...arr].sort((a, b) => a - b)
来源：http://be.huanxung.cn

[U91] JS：对象键值遍历
来源：http://re.shxzskj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://eo.chemitech.net.cn

[U92] JS：深拷贝
来源：http://wg.huixiangedu.cn

structuredClone(obj)
来源：http://ys.chemitech.net.cn

[U93] JS：模板字符串
来源：http://zv.huixinmuqiang.cn

`共 ${n} 条`
来源：http://kx.newstarts.cn

[U94] JS：箭头函数
来源：http://no.szsharing.cn

const double = x => x * 2;
来源：http://ex.muxihuayi.cn

[U95] JS：Promise 包装
来源：http://sj.muxihuayi.cn

new Promise((resolve, reject) => {})
来源：http://se.bookmarksfly.cn

[U96] JS：async/await 与异常
来源：http://aj.haigaiapp.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kp.huixinmuqiang.cn

[U97] JS：并发请求
来源：http://yj.nszjky.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://cr.nicolike.cn

[U98] JS：fetch 带 JSON
来源：http://jy.gzmigu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://to.bookmarksfly.cn

[U99] JS：事件监听
来源：http://mu.9csxet.cn

el.addEventListener("click", e => {})
来源：http://mh.yuntaijiaju.cn

[U100] JS：DOM 查询
来源：http://yk.hnjuh.cn

document.querySelector(".item")
来源：http://iq.wgjwhj.cn

[U101] JS：classList 操作
来源：http://pa.nszjky.cn

el.classList.toggle("active")
来源：http://jp.huixinmuqiang.cn

[U102] JS：本地存储
来源：http://jd.bjjhwx.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fo.lnxyls.cn

[U103] JS：定时器
来源：http://jv.muxihuayi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pg.gzmigu.cn

[U104] JS：防抖
来源：http://ht.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ei.szsharing.cn

[U105] JS：节流
来源：http://eo.jctech888.com.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dp.haigaiapp.cn

[U106] JS：日期格式化
来源：http://zv.lnxyls.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ye.bookmarksfly.cn

[U107] JS：数字千分位
来源：http://jg.yuexingan06.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lw.shxzskj.cn

[U108] JS：随机整数
来源：http://qk.hnjuh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mq.521024.cn

[U109] JS：数组分组
来源：http://ft.yuntaijiaju.cn

Object.groupBy(arr, x => x.type)
来源：http://yi.9csxet.cn

[U110] JS：数组分块
来源：http://bv.jianghongdianzi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fl.jianghongdianzi.cn

[U111] JS：对象转 Map
来源：http://ju.huanxung.cn

new Map(Object.entries(obj))
来源：http://ex.haigaiapp.cn

[U112] JS：字符串补位
来源：http://ry.muxihuayi.cn

"7".padStart(3, "0")
来源：http://mn.shtwfgs.cn

[U113] JS：正则替换全部
来源：http://ro.chemitech.net.cn

s.replaceAll("a", "b")
来源：http://wz.chemitech.net.cn

[U114] JS：JSON 深比较
来源：http://tp.szsharing.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xr.hahajie.cn

[U115] JS：生成 UUID
来源：http://rc.szsharing.cn

crypto.randomUUID()
来源：http://lm.huanxung.cn

[U116] JS：类型检查（JSDoc）
来源：http://fn.gzmigu.cn

/** @param {string} name */ function f(name) {}
来源：http://pj.huixiangedu.cn

[U117] JS：单元测试
来源：http://lm.huixiangedu.cn

npm i -D vitest;  npx vitest
来源：http://yw.nicolike.cn

[U118] JS：开发服务器
来源：http://mo.muxihuayi.cn

npm i -D vite;  npx vite
来源：http://od.jianghongdianzi.cn

[U119] JS：生产构建
来源：http://xh.521024.cn

npx vite build
来源：http://tx.szsharing.cn

[U120] JS：读取环境变量（Vite）
来源：http://xg.9csxet.cn

import.meta.env.VITE_API_URL
来源：http://fn.szxytkj.cn

================================================================================
来源：http://ds.szsharing.cn

统计汇总
来源：http://fh.shxzukj.cn

================================================================================
来源：http://aq.shtwfgs.cn

按语言统计（条）：
来源：http://xl.9csxet.cn

Python ......... 252
来源：http://eb.colortex.cn

PHP ............ 252
来源：http://kq.muxihuayi.cn

JavaScript ..... 252
来源：http://ds.bjjhwx.cn

TypeScript ..... 212
来源：http://in.yuexingan06.cn

Java ........... 212
来源：http://mf.lnxyls.cn

Go ............. 212
来源：http://pk.shxzukj.cn

Ruby ........... 212
来源：http://yd.wgjwhj.cn

C# ............. 212
来源：http://tw.yuexingan06.cn

C .............. 30
来源：http://dg.bjjhwx.cn

C++ ............ 30
来源：http://ak.bjjhwx.cn

SQL ............ 90
来源：http://ws.lnxyls.cn

Bash ........... 80
来源：http://bc.lnxyls.cn

Kotlin ......... 15
来源：http://nl.yuntaijiaju.cn

Swift .......... 15
来源：http://zn.bookmarksfly.cn

Lua ............ 10
来源：http://hx.newstarts.cn

Perl ........... 10
来源：http://gg.wgjwhj.cn

Scala .......... 10
来源：http://rn.hnjuh.cn

------------------------------------
来源：http://le.shtwfgs.cn

合计 ........... 2106 条
来源：http://bu.huanxung.cn

按章节统计：
来源：http://cn.muxihuayi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://eh.panjiajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tg.yuexingan06.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vx.shtwfgs.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zo.huanxung.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qe.bjjhwx.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dg.9csxet.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qe.shxzskj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tx.huixinmuqiang.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://iv.shtwfgs.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lp.asd995.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wn.haigaiapp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jj.panjiajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://od.colortex.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lt.bjjhwx.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cx.chemitech.net.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://sf.521024.cn

Q SQL 专题                              90
来源：http://bw.wgjwhj.cn

R Bash 专题                             80
来源：http://cl.gzmigu.cn

S C / C++ 专题                          60
来源：http://oh.huixinmuqiang.cn

T 其他语言补充                          60
来源：http://km.panjiajie.cn

U 高频实用片段                         120
来源：http://lz.szsharing.cn

------------------------------------
来源：http://wr.huanxung.cn

合计                                  2106 条
来源：http://yq.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://px.jctech888.com.cn

使用提醒
来源：http://sc.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://iy.bookmarksfly.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://oj.newstarts.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jf.asd995.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://am.hnjuh.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fy.shxzukj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hu.521024.cn

—— 文件结束 ——
来源：http://bm.jianghongdianzi.cn

================================================================================
来源：http://jy.huixinmuqiang.cn

程序语言常见例子速查手册（2024 版）
来源：http://aw.jianghongdianzi.cn

Common Programming Examples Cheat Book
来源：http://hj.lnxyls.cn

================================================================================
来源：http://ea.nicolike.cn

【收录内容】
来源：http://cr.hnjuh.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://kp.colortex.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fx.yuexingan06.cn

SQL · Bash · C · C++
来源：http://pg.shtwfgs.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mn.colortex.cn

【使用说明】
来源：http://ny.bjjhwx.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lo.szxytkj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jf.bjjhwx.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://si.bjjhwx.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xv.szxytkj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ve.szsharing.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://me.jctech888.com.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vq.gzmigu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dg.yuntaijiaju.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://px.huixiangedu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ow.jianghongdianzi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://oz.shxzskj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mp.hahajie.cn

【文件统计】
来源：http://vd.bookmarksfly.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yz.nszjky.cn

--------------------------------------------------------------------------------
来源：http://qi.9csxet.cn

目  录
来源：http://yw.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://lc.bookmarksfly.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rd.szsharing.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ee.chemitech.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tm.jctech888.com.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ou.lnxyls.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fi.hahajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jl.asd995.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://su.gzmigu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yx.huixinmuqiang.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mr.huanxung.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vd.jianghongdianzi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rm.521024.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wd.yuntaijiaju.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lg.szsharing.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jy.9csxet.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sj.szsharing.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cr.muxihuayi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tl.gzmigu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://me.gzmigu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hg.lnxyls.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fg.szsharing.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mr.huixinmuqiang.cn

================================================================================
来源：http://ux.jctech888.com.cn

A. 基础语法与类型
来源：http://un.asd995.cn

================================================================================
来源：http://bu.asd995.cn

[A01] Hello World
来源：http://iy.huixiangedu.cn

Py:   print("Hello, World!")
来源：http://ss.nicolike.cn

PHP:  echo "Hello, World!";
来源：http://ei.asd995.cn

JS:   console.log("Hello, World!");
来源：http://tn.yuexingan06.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mo.nicolike.cn

Java: System.out.println("Hello, World!");
来源：http://oc.lnxyls.cn

Go:   fmt.Println("Hello, World!")
来源：http://rp.shxzskj.cn

Ruby: puts "Hello, World!"
来源：http://ym.jctech888.com.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://mg.asd995.cn

[A02] 变量声明与赋值
来源：http://ug.lnxyls.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bg.shtwfgs.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://fg.lnxyls.cn

JS:   let name = "Alex"; const age = 20;
来源：http://cj.huixiangedu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wa.hahajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://rm.shxzukj.cn

Go:   name := "Alex"; age := 20
来源：http://mj.shtwfgs.cn

Ruby: name = "Alex"; age = 20
来源：http://ti.nicolike.cn

C#:   string name = "Alex"; int age = 20;
来源：http://vo.haigaiapp.cn

[A03] 常量定义
来源：http://hi.hahajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qc.asd995.cn

PHP:  const PI = 3.14159;
来源：http://sv.chemitech.net.cn

JS:   const PI = 3.14159;
来源：http://et.chemitech.net.cn

TS:   const PI: number = 3.14159;
来源：http://fp.521024.cn

Java: static final double PI = 3.14159;
来源：http://rv.shxzukj.cn

Go:   const PI = 3.14159
来源：http://od.huanxung.cn

Ruby: PI = 3.14159
来源：http://lh.shxzskj.cn

C#:   const double PI = 3.14159;
来源：http://ik.521024.cn

[A04] 判断变量类型
来源：http://de.nszjky.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://zl.szxytkj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yp.szsharing.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xu.nicolike.cn

TS:   typeof x; x instanceof Date
来源：http://bz.jctech888.com.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gp.9csxet.cn


<!-- 参考信息 -->