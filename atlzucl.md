代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://wa.szxytkj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://id.521024.cn

[U42] PHP：PSR-4 自动加载
来源：http://kl.nicolike.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yp.9csxet.cn

[U43] PHP：声明命名空间
来源：http://hs.shtwfgs.cn

namespace App\Http;
来源：http://rx.bjjhwx.cn

[U44] PHP：开启严格类型
来源：http://ic.jctech888.com.cn

declare(strict_types=1);
来源：http://dc.nszjky.cn

[U45] PHP：类型声明与返回类型
来源：http://li.521024.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zx.9csxet.cn

[U46] PHP：可空类型
来源：http://dq.shtwfgs.cn

?string $name = null
来源：http://oc.9csxet.cn

[U47] PHP：联合类型
来源：http://xe.asd995.cn

int|string $id
来源：http://if.huanxung.cn

[U48] PHP：纯枚举
来源：http://zz.nicolike.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qp.huixinmuqiang.cn

[U49] PHP：只读属性
来源：http://lq.yuntaijiaju.cn

public readonly string $name
来源：http://if.lnxyls.cn

[U50] PHP：构造器属性提升
来源：http://ig.panjiajie.cn

public function __construct(private int $id) {}
来源：http://kr.bookmarksfly.cn

[U51] PHP：数组解构
来源：http://hl.gzmigu.cn

[$a, $b] = $arr;
来源：http://qx.nicolike.cn

[U52] PHP：箭头函数
来源：http://lu.lnxyls.cn

$double = fn($x) => $x * 2;
来源：http://nh.muxihuayi.cn

[U53] PHP：空合并运算符
来源：http://te.chemitech.net.cn

$v = $a ?? $b ?? "default";
来源：http://nd.yuntaijiaju.cn

[U54] PHP：空安全调用
来源：http://jd.hahajie.cn

$obj?->method()
来源：http://vp.yuexingan06.cn

[U55] PHP：match 表达式
来源：http://uh.newstarts.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zm.chemitech.net.cn

[U56] PHP：命名参数
来源：http://qn.hahajie.cn

f(a: 1, b: 2)
来源：http://ia.bjjhwx.cn

[U57] PHP：字符串插值
来源：http://xf.shxzukj.cn

"值: {$a}"
来源：http://dr.shtwfgs.cn

[U58] PHP：数组三件套
来源：http://pj.panjiajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ps.bjjhwx.cn

[U59] PHP：自定义排序
来源：http://zo.huanxung.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kd.nszjky.cn

[U60] PHP：JSON 编解码
来源：http://kz.hnjuh.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://he.hahajie.cn

[U61] PHP：正则
来源：http://vw.shtwfgs.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nk.bookmarksfly.cn

[U62] PHP：日期对象
来源：http://pj.chemitech.net.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ia.shxzukj.cn

[U63] PHP：文件读写
来源：http://wc.jctech888.com.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nq.lnxyls.cn

[U64] PHP：目录遍历
来源：http://yh.jianghongdianzi.cn

glob("dir/*.php");  scandir("dir");
来源：http://qf.shxzskj.cn

[U65] PHP：会话
来源：http://ow.chemitech.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wj.shxzskj.cn

[U66] PHP：设置 Cookie
来源：http://bb.szsharing.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bc.muxihuayi.cn

[U67] PHP：处理文件上传
来源：http://dx.bjjhwx.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ib.colortex.cn

[U68] PHP：PDO 连接
来源：http://ua.lnxyls.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mj.huanxung.cn

[U69] PHP：PDO 预处理
来源：http://zx.szsharing.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nd.szxytkj.cn

[U70] PHP：PDO 事务
来源：http://xo.huanxung.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nl.newstarts.cn

[U71] PHP：抛出异常
来源：http://jj.yuntaijiaju.cn

throw new RuntimeException("失败", 500);
来源：http://mj.huixinmuqiang.cn

[U72] PHP：写错误日志
来源：http://jn.newstarts.cn

error_log("失败: " . $e->getMessage());
来源：http://de.jctech888.com.cn

[U73] PHP：读取 ini 配置
来源：http://gu.shtwfgs.cn

parse_ini_file("config.ini", true)
来源：http://rr.muxihuayi.cn

[U74] PHP：读取环境变量
来源：http://gc.bjjhwx.cn

getenv("APP_ENV") ?: "production"
来源：http://ja.jctech888.com.cn

[U75] PHP：依赖注入
来源：http://ln.lnxyls.cn

composer require psr/container
来源：http://rn.szxytkj.cn

[U76] PHP：简单路由
来源：http://cd.jctech888.com.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://so.huixiangedu.cn

[U77] PHP：模板渲染
来源：http://hb.huanxung.cn

composer require twig/twig
来源：http://cq.9csxet.cn

[U78] PHP：单元测试
来源：http://lt.bookmarksfly.cn

composer require --dev phpunit/phpunit
来源：http://fr.huanxung.cn

[U79] PHP：静态分析
来源：http://sn.szxytkj.cn

composer require --dev phpstan/phpstan
来源：http://gj.nszjky.cn

[U80] PHP：代码规范修复
来源：http://ag.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mq.nszjky.cn

[U81] JS：初始化项目
来源：http://ac.huanxung.cn

npm init -y;  npm i express
来源：http://ml.gzmigu.cn

[U82] JS：package.json 脚本
来源：http://tb.521024.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xd.hnjuh.cn

[U83] JS：ES Module 导入导出
来源：http://hd.huanxung.cn

export const a = 1;  import { a } from "./m.js";
来源：http://sl.newstarts.cn

[U84] JS：CommonJS 写法
来源：http://js.asd995.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ho.jianghongdianzi.cn

[U85] JS：可选链
来源：http://nm.panjiajie.cn

a?.b?.c
来源：http://bh.hahajie.cn

[U86] JS：空值合并
来源：http://by.jctech888.com.cn

a ?? b
来源：http://ih.shxzukj.cn

[U87] JS：解构默认值
来源：http://sr.colortex.cn

const { a = 1, b = 2 } = obj;
来源：http://zg.shtwfgs.cn

[U88] JS：对象展开合并
来源：http://tl.panjiajie.cn

{ ...a, ...b }
来源：http://om.colortex.cn

[U89] JS：数组去重
来源：http://fx.szsharing.cn

[...new Set(arr)]
来源：http://av.huanxung.cn

[U90] JS：数字数组排序
来源：http://fb.asd995.cn

[...arr].sort((a, b) => a - b)
来源：http://sd.yuexingan06.cn

[U91] JS：对象键值遍历
来源：http://tz.panjiajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lv.szxytkj.cn

[U92] JS：深拷贝
来源：http://gt.bjjhwx.cn

structuredClone(obj)
来源：http://xn.shtwfgs.cn

[U93] JS：模板字符串
来源：http://yp.chemitech.net.cn

`共 ${n} 条`
来源：http://lr.shtwfgs.cn

[U94] JS：箭头函数
来源：http://vv.colortex.cn

const double = x => x * 2;
来源：http://po.muxihuayi.cn

[U95] JS：Promise 包装
来源：http://yl.bjjhwx.cn

new Promise((resolve, reject) => {})
来源：http://ei.newstarts.cn

[U96] JS：async/await 与异常
来源：http://au.huixinmuqiang.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hg.panjiajie.cn

[U97] JS：并发请求
来源：http://uq.hnjuh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lt.hnjuh.cn

[U98] JS：fetch 带 JSON
来源：http://py.hnjuh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cj.jianghongdianzi.cn

[U99] JS：事件监听
来源：http://lo.szxytkj.cn

el.addEventListener("click", e => {})
来源：http://vj.asd995.cn

[U100] JS：DOM 查询
来源：http://qq.huanxung.cn

document.querySelector(".item")
来源：http://ob.gzmigu.cn

[U101] JS：classList 操作
来源：http://tz.hahajie.cn

el.classList.toggle("active")
来源：http://zp.521024.cn

[U102] JS：本地存储
来源：http://mw.huixiangedu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sm.jianghongdianzi.cn

[U103] JS：定时器
来源：http://hs.muxihuayi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fr.asd995.cn

[U104] JS：防抖
来源：http://bc.nszjky.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://el.hahajie.cn

[U105] JS：节流
来源：http://ym.yuntaijiaju.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dj.jctech888.com.cn

[U106] JS：日期格式化
来源：http://ek.haigaiapp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lx.shtwfgs.cn

[U107] JS：数字千分位
来源：http://ue.hnjuh.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://eh.lnxyls.cn

[U108] JS：随机整数
来源：http://zd.huanxung.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hf.shxzskj.cn

[U109] JS：数组分组
来源：http://qm.nszjky.cn

Object.groupBy(arr, x => x.type)
来源：http://ff.huixiangedu.cn

[U110] JS：数组分块
来源：http://th.muxihuayi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ka.521024.cn

[U111] JS：对象转 Map
来源：http://jj.huixiangedu.cn

new Map(Object.entries(obj))
来源：http://qy.huixiangedu.cn

[U112] JS：字符串补位
来源：http://ho.yuntaijiaju.cn

"7".padStart(3, "0")
来源：http://yg.jctech888.com.cn

[U113] JS：正则替换全部
来源：http://tx.muxihuayi.cn

s.replaceAll("a", "b")
来源：http://uq.hnjuh.cn

[U114] JS：JSON 深比较
来源：http://nm.szxytkj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ss.huixiangedu.cn

[U115] JS：生成 UUID
来源：http://hd.9csxet.cn

crypto.randomUUID()
来源：http://qb.bjjhwx.cn

[U116] JS：类型检查（JSDoc）
来源：http://gg.chemitech.net.cn

/** @param {string} name */ function f(name) {}
来源：http://jd.haigaiapp.cn

[U117] JS：单元测试
来源：http://us.wgjwhj.cn

npm i -D vitest;  npx vitest
来源：http://xm.colortex.cn

[U118] JS：开发服务器
来源：http://zd.szsharing.cn

npm i -D vite;  npx vite
来源：http://qd.chemitech.net.cn

[U119] JS：生产构建
来源：http://ib.shxzskj.cn

npx vite build
来源：http://bv.shtwfgs.cn

[U120] JS：读取环境变量（Vite）
来源：http://tq.jctech888.com.cn

import.meta.env.VITE_API_URL
来源：http://bn.lnxyls.cn

================================================================================
来源：http://cr.lnxyls.cn

统计汇总
来源：http://wr.szxytkj.cn

================================================================================
来源：http://oa.newstarts.cn

按语言统计（条）：
来源：http://ni.yuntaijiaju.cn

Python ......... 252
来源：http://nu.muxihuayi.cn

PHP ............ 252
来源：http://eg.huixinmuqiang.cn

JavaScript ..... 252
来源：http://sm.9csxet.cn

TypeScript ..... 212
来源：http://mh.huanxung.cn

Java ........... 212
来源：http://hh.shtwfgs.cn

Go ............. 212
来源：http://sn.nicolike.cn

Ruby ........... 212
来源：http://ln.521024.cn

C# ............. 212
来源：http://zs.yuexingan06.cn

C .............. 30
来源：http://mw.yuexingan06.cn

C++ ............ 30
来源：http://io.wgjwhj.cn

SQL ............ 90
来源：http://cw.jctech888.com.cn

Bash ........... 80
来源：http://rt.wgjwhj.cn

Kotlin ......... 15
来源：http://ny.wgjwhj.cn

Swift .......... 15
来源：http://sq.shxzukj.cn

Lua ............ 10
来源：http://jx.jianghongdianzi.cn

Perl ........... 10
来源：http://th.yuexingan06.cn

Scala .......... 10
来源：http://qj.521024.cn

------------------------------------
来源：http://ju.yuntaijiaju.cn

合计 ........... 2106 条
来源：http://qd.huanxung.cn

按章节统计：
来源：http://xg.haigaiapp.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hr.shxzukj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mc.yuexingan06.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nv.jianghongdianzi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://os.nicolike.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://al.lnxyls.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mx.huixiangedu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ec.nszjky.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nx.9csxet.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tz.huanxung.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ir.nszjky.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yd.haigaiapp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uf.shxzukj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qc.bookmarksfly.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wa.hahajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://iw.nicolike.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dd.bookmarksfly.cn

Q SQL 专题                              90
来源：http://vu.lnxyls.cn

R Bash 专题                             80
来源：http://zc.yuntaijiaju.cn

S C / C++ 专题                          60
来源：http://fm.haigaiapp.cn

T 其他语言补充                          60
来源：http://yh.bookmarksfly.cn

U 高频实用片段                         120
来源：http://tx.hnjuh.cn

------------------------------------
来源：http://um.gzmigu.cn

合计                                  2106 条
来源：http://kc.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://ho.huixinmuqiang.cn

使用提醒
来源：http://pc.colortex.cn

--------------------------------------------------------------------------------
来源：http://du.colortex.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vw.bookmarksfly.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ss.wgjwhj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wi.jctech888.com.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wu.shxzskj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://aw.hahajie.cn

—— 文件结束 ——
来源：http://hh.shxzukj.cn

================================================================================
来源：http://ri.shxzskj.cn

程序语言常见例子速查手册（2024 版）
来源：http://tz.haigaiapp.cn

Common Programming Examples Cheat Book
来源：http://ft.newstarts.cn

================================================================================
来源：http://je.lnxyls.cn

【收录内容】
来源：http://tk.nszjky.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://av.panjiajie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cc.huixinmuqiang.cn

SQL · Bash · C · C++
来源：http://zg.bjjhwx.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lv.lnxyls.cn

【使用说明】
来源：http://ba.bjjhwx.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nu.newstarts.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fr.huixiangedu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kn.nszjky.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ic.wgjwhj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://rv.hahajie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yb.521024.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ib.9csxet.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yz.nicolike.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kj.colortex.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gd.jctech888.com.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://iz.shxzskj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ib.bookmarksfly.cn

【文件统计】
来源：http://hi.hnjuh.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ad.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://co.bookmarksfly.cn

目  录
来源：http://jw.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://hk.wgjwhj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gw.szxytkj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cv.gzmigu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://aj.lnxyls.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://po.bjjhwx.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ce.bjjhwx.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://go.haigaiapp.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jd.hahajie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xd.shxzskj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ul.newstarts.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dg.yuntaijiaju.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xa.bookmarksfly.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://st.colortex.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://me.bookmarksfly.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yf.szxytkj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qu.gzmigu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://uy.hahajie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ym.huanxung.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://nq.huixinmuqiang.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pr.nszjky.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zt.lnxyls.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://du.lnxyls.cn

================================================================================
来源：http://ot.gzmigu.cn

A. 基础语法与类型
来源：http://um.hnjuh.cn

================================================================================
来源：http://dc.jctech888.com.cn

[A01] Hello World
来源：http://we.shxzskj.cn

Py:   print("Hello, World!")
来源：http://lp.bookmarksfly.cn

PHP:  echo "Hello, World!";
来源：http://da.hnjuh.cn

JS:   console.log("Hello, World!");
来源：http://gf.bjjhwx.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sx.hnjuh.cn

Java: System.out.println("Hello, World!");
来源：http://pm.shtwfgs.cn

Go:   fmt.Println("Hello, World!")
来源：http://wx.newstarts.cn

Ruby: puts "Hello, World!"
来源：http://iy.bookmarksfly.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ev.yuexingan06.cn

[A02] 变量声明与赋值
来源：http://cq.shtwfgs.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tb.huanxung.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.muxihuayi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://pq.521024.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jp.nszjky.cn

Java: String name = "Alex"; int age = 20;
来源：http://ne.newstarts.cn

Go:   name := "Alex"; age := 20
来源：http://hs.hahajie.cn

Ruby: name = "Alex"; age = 20
来源：http://sr.jctech888.com.cn

C#:   string name = "Alex"; int age = 20;
来源：http://sq.shxzskj.cn

[A03] 常量定义
来源：http://mg.shtwfgs.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://oz.jianghongdianzi.cn

PHP:  const PI = 3.14159;
来源：http://pu.haigaiapp.cn

JS:   const PI = 3.14159;
来源：http://gb.jianghongdianzi.cn

TS:   const PI: number = 3.14159;
来源：http://nv.bjjhwx.cn

Java: static final double PI = 3.14159;
来源：http://mo.haigaiapp.cn

Go:   const PI = 3.14159
来源：http://em.szxytkj.cn

Ruby: PI = 3.14159
来源：http://ve.gzmigu.cn

C#:   const double PI = 3.14159;
来源：http://gp.bookmarksfly.cn

[A04] 判断变量类型
来源：http://gu.gzmigu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://wv.jianghongdianzi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://am.yuntaijiaju.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zm.muxihuayi.cn

TS:   typeof x; x instanceof Date
来源：http://oz.yuexingan06.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bt.jianghongdianzi.cn


<!-- 参考信息 -->