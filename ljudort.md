代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://sd.bjjhwx.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dd.szsharing.cn

[U42] PHP：PSR-4 自动加载
来源：http://by.521024.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hl.panjiajie.cn

[U43] PHP：声明命名空间
来源：http://nt.jctech888.com.cn

namespace App\Http;
来源：http://rh.huixinmuqiang.cn

[U44] PHP：开启严格类型
来源：http://jn.bjjhwx.cn

declare(strict_types=1);
来源：http://it.haigaiapp.cn

[U45] PHP：类型声明与返回类型
来源：http://bu.colortex.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ij.521024.cn

[U46] PHP：可空类型
来源：http://ca.bookmarksfly.cn

?string $name = null
来源：http://oi.panjiajie.cn

[U47] PHP：联合类型
来源：http://ee.bookmarksfly.cn

int|string $id
来源：http://fv.muxihuayi.cn

[U48] PHP：纯枚举
来源：http://nq.9csxet.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nl.wgjwhj.cn

[U49] PHP：只读属性
来源：http://nb.chemitech.net.cn

public readonly string $name
来源：http://hz.yuexingan06.cn

[U50] PHP：构造器属性提升
来源：http://ge.shxzskj.cn

public function __construct(private int $id) {}
来源：http://ed.nszjky.cn

[U51] PHP：数组解构
来源：http://ry.shxzukj.cn

[$a, $b] = $arr;
来源：http://al.bjjhwx.cn

[U52] PHP：箭头函数
来源：http://xu.huixiangedu.cn

$double = fn($x) => $x * 2;
来源：http://nj.muxihuayi.cn

[U53] PHP：空合并运算符
来源：http://hd.szsharing.cn

$v = $a ?? $b ?? "default";
来源：http://dj.yuntaijiaju.cn

[U54] PHP：空安全调用
来源：http://wq.nicolike.cn

$obj?->method()
来源：http://vh.huixinmuqiang.cn

[U55] PHP：match 表达式
来源：http://xv.shtwfgs.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://by.wgjwhj.cn

[U56] PHP：命名参数
来源：http://fk.bookmarksfly.cn

f(a: 1, b: 2)
来源：http://sd.jianghongdianzi.cn

[U57] PHP：字符串插值
来源：http://wv.szsharing.cn

"值: {$a}"
来源：http://sa.wgjwhj.cn

[U58] PHP：数组三件套
来源：http://hw.colortex.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wc.newstarts.cn

[U59] PHP：自定义排序
来源：http://bh.muxihuayi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qm.shxzskj.cn

[U60] PHP：JSON 编解码
来源：http://dp.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://us.chemitech.net.cn

[U61] PHP：正则
来源：http://dm.haigaiapp.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ju.panjiajie.cn

[U62] PHP：日期对象
来源：http://ah.panjiajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zv.colortex.cn

[U63] PHP：文件读写
来源：http://iv.szxytkj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wr.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://ys.szsharing.cn

glob("dir/*.php");  scandir("dir");
来源：http://vq.newstarts.cn

[U65] PHP：会话
来源：http://xs.521024.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xh.huanxung.cn

[U66] PHP：设置 Cookie
来源：http://cf.yuexingan06.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://eo.huixiangedu.cn

[U67] PHP：处理文件上传
来源：http://sj.colortex.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zz.shxzskj.cn

[U68] PHP：PDO 连接
来源：http://nu.chemitech.net.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uv.shxzskj.cn

[U69] PHP：PDO 预处理
来源：http://gi.yuntaijiaju.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hm.hnjuh.cn

[U70] PHP：PDO 事务
来源：http://ca.hahajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xu.hahajie.cn

[U71] PHP：抛出异常
来源：http://sy.haigaiapp.cn

throw new RuntimeException("失败", 500);
来源：http://ex.hahajie.cn

[U72] PHP：写错误日志
来源：http://ir.yuntaijiaju.cn

error_log("失败: " . $e->getMessage());
来源：http://bw.bookmarksfly.cn

[U73] PHP：读取 ini 配置
来源：http://ji.9csxet.cn

parse_ini_file("config.ini", true)
来源：http://ok.9csxet.cn

[U74] PHP：读取环境变量
来源：http://py.shxzukj.cn

getenv("APP_ENV") ?: "production"
来源：http://sx.9csxet.cn

[U75] PHP：依赖注入
来源：http://ks.yuntaijiaju.cn

composer require psr/container
来源：http://te.szsharing.cn

[U76] PHP：简单路由
来源：http://wi.muxihuayi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ql.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://zx.huixinmuqiang.cn

composer require twig/twig
来源：http://bl.9csxet.cn

[U78] PHP：单元测试
来源：http://qa.jctech888.com.cn

composer require --dev phpunit/phpunit
来源：http://fc.lnxyls.cn

[U79] PHP：静态分析
来源：http://lt.nicolike.cn

composer require --dev phpstan/phpstan
来源：http://op.lnxyls.cn

[U80] PHP：代码规范修复
来源：http://rp.shtwfgs.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ds.bookmarksfly.cn

[U81] JS：初始化项目
来源：http://nv.newstarts.cn

npm init -y;  npm i express
来源：http://ot.nszjky.cn

[U82] JS：package.json 脚本
来源：http://wo.newstarts.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xi.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://bm.jianghongdianzi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://pm.nicolike.cn

[U84] JS：CommonJS 写法
来源：http://js.chemitech.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zq.yuexingan06.cn

[U85] JS：可选链
来源：http://mf.szsharing.cn

a?.b?.c
来源：http://og.shxzskj.cn

[U86] JS：空值合并
来源：http://hc.nicolike.cn

a ?? b
来源：http://fs.jianghongdianzi.cn

[U87] JS：解构默认值
来源：http://ro.9csxet.cn

const { a = 1, b = 2 } = obj;
来源：http://tv.haigaiapp.cn

[U88] JS：对象展开合并
来源：http://fh.shxzskj.cn

{ ...a, ...b }
来源：http://xq.9csxet.cn

[U89] JS：数组去重
来源：http://cg.lnxyls.cn

[...new Set(arr)]
来源：http://jy.hahajie.cn

[U90] JS：数字数组排序
来源：http://dm.jianghongdianzi.cn

[...arr].sort((a, b) => a - b)
来源：http://qx.muxihuayi.cn

[U91] JS：对象键值遍历
来源：http://nl.muxihuayi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://oj.panjiajie.cn

[U92] JS：深拷贝
来源：http://la.haigaiapp.cn

structuredClone(obj)
来源：http://qx.asd995.cn

[U93] JS：模板字符串
来源：http://kv.lnxyls.cn

`共 ${n} 条`
来源：http://ug.nicolike.cn

[U94] JS：箭头函数
来源：http://cy.bookmarksfly.cn

const double = x => x * 2;
来源：http://og.haigaiapp.cn

[U95] JS：Promise 包装
来源：http://ml.chemitech.net.cn

new Promise((resolve, reject) => {})
来源：http://zk.chemitech.net.cn

[U96] JS：async/await 与异常
来源：http://ae.chemitech.net.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cm.yuntaijiaju.cn

[U97] JS：并发请求
来源：http://bh.newstarts.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://fi.shxzukj.cn

[U98] JS：fetch 带 JSON
来源：http://ve.muxihuayi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fm.haigaiapp.cn

[U99] JS：事件监听
来源：http://ld.huixiangedu.cn

el.addEventListener("click", e => {})
来源：http://jf.szsharing.cn

[U100] JS：DOM 查询
来源：http://ir.szsharing.cn

document.querySelector(".item")
来源：http://my.shtwfgs.cn

[U101] JS：classList 操作
来源：http://nq.muxihuayi.cn

el.classList.toggle("active")
来源：http://at.shxzukj.cn

[U102] JS：本地存储
来源：http://pt.nicolike.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://lp.chemitech.net.cn

[U103] JS：定时器
来源：http://uh.newstarts.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ne.bookmarksfly.cn

[U104] JS：防抖
来源：http://jd.shtwfgs.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cv.muxihuayi.cn

[U105] JS：节流
来源：http://gt.huanxung.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://el.huanxung.cn

[U106] JS：日期格式化
来源：http://bj.9csxet.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ox.gzmigu.cn

[U107] JS：数字千分位
来源：http://zd.shtwfgs.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qi.hnjuh.cn

[U108] JS：随机整数
来源：http://lr.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uz.szsharing.cn

[U109] JS：数组分组
来源：http://cd.haigaiapp.cn

Object.groupBy(arr, x => x.type)
来源：http://ae.muxihuayi.cn

[U110] JS：数组分块
来源：http://fy.nicolike.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yg.huixinmuqiang.cn

[U111] JS：对象转 Map
来源：http://jb.jianghongdianzi.cn

new Map(Object.entries(obj))
来源：http://yw.yuntaijiaju.cn

[U112] JS：字符串补位
来源：http://fl.521024.cn

"7".padStart(3, "0")
来源：http://ih.muxihuayi.cn

[U113] JS：正则替换全部
来源：http://cr.9csxet.cn

s.replaceAll("a", "b")
来源：http://td.jctech888.com.cn

[U114] JS：JSON 深比较
来源：http://et.shxzskj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://py.shxzskj.cn

[U115] JS：生成 UUID
来源：http://hr.huanxung.cn

crypto.randomUUID()
来源：http://wx.panjiajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://ck.szxytkj.cn

/** @param {string} name */ function f(name) {}
来源：http://sw.521024.cn

[U117] JS：单元测试
来源：http://oo.nszjky.cn

npm i -D vitest;  npx vitest
来源：http://ud.521024.cn

[U118] JS：开发服务器
来源：http://es.lnxyls.cn

npm i -D vite;  npx vite
来源：http://pp.jianghongdianzi.cn

[U119] JS：生产构建
来源：http://cs.bjjhwx.cn

npx vite build
来源：http://je.panjiajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://vz.bookmarksfly.cn

import.meta.env.VITE_API_URL
来源：http://jj.shtwfgs.cn

================================================================================
来源：http://zo.huixinmuqiang.cn

统计汇总
来源：http://lo.chemitech.net.cn

================================================================================
来源：http://fi.9csxet.cn

按语言统计（条）：
来源：http://lm.yuntaijiaju.cn

Python ......... 252
来源：http://tz.chemitech.net.cn

PHP ............ 252
来源：http://kd.wgjwhj.cn

JavaScript ..... 252
来源：http://nx.szxytkj.cn

TypeScript ..... 212
来源：http://ti.chemitech.net.cn

Java ........... 212
来源：http://sq.chemitech.net.cn

Go ............. 212
来源：http://hc.bookmarksfly.cn

Ruby ........... 212
来源：http://hc.hahajie.cn

C# ............. 212
来源：http://cz.szxytkj.cn

C .............. 30
来源：http://ic.newstarts.cn

C++ ............ 30
来源：http://ou.chemitech.net.cn

SQL ............ 90
来源：http://ek.haigaiapp.cn

Bash ........... 80
来源：http://qj.shxzukj.cn

Kotlin ......... 15
来源：http://pi.9csxet.cn

Swift .......... 15
来源：http://ne.shtwfgs.cn

Lua ............ 10
来源：http://qj.lnxyls.cn

Perl ........... 10
来源：http://je.colortex.cn

Scala .......... 10
来源：http://gz.szsharing.cn

------------------------------------
来源：http://ee.jianghongdianzi.cn

合计 ........... 2106 条
来源：http://ea.huanxung.cn

按章节统计：
来源：http://wz.haigaiapp.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ra.yuexingan06.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ky.wgjwhj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cv.yuntaijiaju.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ix.newstarts.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ko.hnjuh.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wp.muxihuayi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ch.nszjky.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vp.huixinmuqiang.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tm.chemitech.net.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uz.nszjky.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ih.shxzukj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lf.yuntaijiaju.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ts.huixinmuqiang.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ne.hnjuh.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lr.huanxung.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yw.newstarts.cn

Q SQL 专题                              90
来源：http://ri.shxzskj.cn

R Bash 专题                             80
来源：http://zz.huanxung.cn

S C / C++ 专题                          60
来源：http://lx.521024.cn

T 其他语言补充                          60
来源：http://oo.szsharing.cn

U 高频实用片段                         120
来源：http://pt.yuntaijiaju.cn

------------------------------------
来源：http://ce.nszjky.cn

合计                                  2106 条
来源：http://wm.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://ce.szxytkj.cn

使用提醒
来源：http://hr.9csxet.cn

--------------------------------------------------------------------------------
来源：http://wo.colortex.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pq.huixinmuqiang.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dq.huanxung.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yk.521024.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://uv.9csxet.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cf.newstarts.cn

—— 文件结束 ——
来源：http://nu.huanxung.cn

================================================================================
来源：http://ja.muxihuayi.cn

程序语言常见例子速查手册（2024 版）
来源：http://km.nszjky.cn

Common Programming Examples Cheat Book
来源：http://jf.nszjky.cn

================================================================================
来源：http://om.wgjwhj.cn

【收录内容】
来源：http://qn.colortex.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ka.colortex.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jj.szsharing.cn

SQL · Bash · C · C++
来源：http://pn.chemitech.net.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://oz.newstarts.cn

【使用说明】
来源：http://kd.hahajie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yw.521024.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fc.shxzskj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ng.colortex.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://iv.nszjky.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://vm.shxzskj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qs.jctech888.com.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cj.colortex.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yw.nicolike.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vn.jianghongdianzi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lc.muxihuayi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tl.bjjhwx.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mh.szsharing.cn

【文件统计】
来源：http://nn.bjjhwx.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ln.huanxung.cn

--------------------------------------------------------------------------------
来源：http://vu.521024.cn

目  录
来源：http://mk.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://bu.szxytkj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gg.bookmarksfly.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nt.wgjwhj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cl.huixinmuqiang.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yf.yuntaijiaju.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xu.szxytkj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ns.newstarts.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://og.huixinmuqiang.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fv.yuntaijiaju.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ko.wgjwhj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qu.huixinmuqiang.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ka.nszjky.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://un.bjjhwx.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ye.9csxet.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pt.bjjhwx.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rd.newstarts.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tu.bookmarksfly.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kc.shxzskj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://qd.panjiajie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://js.nicolike.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xb.haigaiapp.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ru.521024.cn

================================================================================
来源：http://aq.jianghongdianzi.cn

A. 基础语法与类型
来源：http://tm.huixiangedu.cn

================================================================================
来源：http://da.9csxet.cn

[A01] Hello World
来源：http://xi.colortex.cn

Py:   print("Hello, World!")
来源：http://oq.muxihuayi.cn

PHP:  echo "Hello, World!";
来源：http://hr.521024.cn

JS:   console.log("Hello, World!");
来源：http://yo.haigaiapp.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rc.nicolike.cn

Java: System.out.println("Hello, World!");
来源：http://al.muxihuayi.cn

Go:   fmt.Println("Hello, World!")
来源：http://du.bookmarksfly.cn

Ruby: puts "Hello, World!"
来源：http://gw.haigaiapp.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ce.gzmigu.cn

[A02] 变量声明与赋值
来源：http://br.jctech888.com.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wq.jctech888.com.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://bw.bjjhwx.cn

JS:   let name = "Alex"; const age = 20;
来源：http://of.szsharing.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qh.bookmarksfly.cn

Java: String name = "Alex"; int age = 20;
来源：http://uk.huixiangedu.cn

Go:   name := "Alex"; age := 20
来源：http://ki.nszjky.cn

Ruby: name = "Alex"; age = 20
来源：http://hl.9csxet.cn

C#:   string name = "Alex"; int age = 20;
来源：http://vb.gzmigu.cn

[A03] 常量定义
来源：http://kk.yuexingan06.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tx.gzmigu.cn

PHP:  const PI = 3.14159;
来源：http://pm.newstarts.cn

JS:   const PI = 3.14159;
来源：http://tv.yuntaijiaju.cn

TS:   const PI: number = 3.14159;
来源：http://nw.szxytkj.cn

Java: static final double PI = 3.14159;
来源：http://db.wgjwhj.cn

Go:   const PI = 3.14159
来源：http://id.bookmarksfly.cn

Ruby: PI = 3.14159
来源：http://qo.shtwfgs.cn

C#:   const double PI = 3.14159;
来源：http://ew.panjiajie.cn

[A04] 判断变量类型
来源：http://qa.521024.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://jw.haigaiapp.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ml.shxzskj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qg.bjjhwx.cn

TS:   typeof x; x instanceof Date
来源：http://vx.9csxet.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ft.newstarts.cn


<!-- 参考信息 -->