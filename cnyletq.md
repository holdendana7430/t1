代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://nj.hnjuh.cn

sys.stdout.isatty()
来源：http://qv.nicolike.cn

[U40] Py：打印到标准错误
来源：http://us.shtwfgs.cn

print("err", file=sys.stderr)
来源：http://lj.hnjuh.cn

[U41] PHP：初始化 Composer 项目
来源：http://sa.shxzskj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rq.gzmigu.cn

[U42] PHP：PSR-4 自动加载
来源：http://mr.wgjwhj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://up.jianghongdianzi.cn

[U43] PHP：声明命名空间
来源：http://ji.nszjky.cn

namespace App\Http;
来源：http://bq.bjjhwx.cn

[U44] PHP：开启严格类型
来源：http://bt.shtwfgs.cn

declare(strict_types=1);
来源：http://rs.asd995.cn

[U45] PHP：类型声明与返回类型
来源：http://rr.shxzukj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qk.colortex.cn

[U46] PHP：可空类型
来源：http://re.nicolike.cn

?string $name = null
来源：http://ls.asd995.cn

[U47] PHP：联合类型
来源：http://je.panjiajie.cn

int|string $id
来源：http://wx.gzmigu.cn

[U48] PHP：纯枚举
来源：http://ki.521024.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://in.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://gy.yuntaijiaju.cn

public readonly string $name
来源：http://ht.shxzskj.cn

[U50] PHP：构造器属性提升
来源：http://yk.bookmarksfly.cn

public function __construct(private int $id) {}
来源：http://zc.jianghongdianzi.cn

[U51] PHP：数组解构
来源：http://hw.hnjuh.cn

[$a, $b] = $arr;
来源：http://qa.huixinmuqiang.cn

[U52] PHP：箭头函数
来源：http://nk.nszjky.cn

$double = fn($x) => $x * 2;
来源：http://fo.gzmigu.cn

[U53] PHP：空合并运算符
来源：http://iq.bjjhwx.cn

$v = $a ?? $b ?? "default";
来源：http://jo.asd995.cn

[U54] PHP：空安全调用
来源：http://ub.newstarts.cn

$obj?->method()
来源：http://gc.asd995.cn

[U55] PHP：match 表达式
来源：http://bp.9csxet.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xn.521024.cn

[U56] PHP：命名参数
来源：http://bp.bjjhwx.cn

f(a: 1, b: 2)
来源：http://yx.huanxung.cn

[U57] PHP：字符串插值
来源：http://uy.shxzskj.cn

"值: {$a}"
来源：http://lk.haigaiapp.cn

[U58] PHP：数组三件套
来源：http://qr.szxytkj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bw.chemitech.net.cn

[U59] PHP：自定义排序
来源：http://he.yuexingan06.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ik.bookmarksfly.cn

[U60] PHP：JSON 编解码
来源：http://qb.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ao.gzmigu.cn

[U61] PHP：正则
来源：http://gt.nszjky.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yg.szxytkj.cn

[U62] PHP：日期对象
来源：http://pr.yuntaijiaju.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://is.jctech888.com.cn

[U63] PHP：文件读写
来源：http://sf.huixiangedu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tb.newstarts.cn

[U64] PHP：目录遍历
来源：http://vj.newstarts.cn

glob("dir/*.php");  scandir("dir");
来源：http://il.nicolike.cn

[U65] PHP：会话
来源：http://fp.hnjuh.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://nt.shxzukj.cn

[U66] PHP：设置 Cookie
来源：http://vw.haigaiapp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zi.hnjuh.cn

[U67] PHP：处理文件上传
来源：http://po.panjiajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dn.chemitech.net.cn

[U68] PHP：PDO 连接
来源：http://jp.huixiangedu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sz.szxytkj.cn

[U69] PHP：PDO 预处理
来源：http://qt.huixiangedu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mt.yuexingan06.cn

[U70] PHP：PDO 事务
来源：http://pf.colortex.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xv.yuntaijiaju.cn

[U71] PHP：抛出异常
来源：http://tf.newstarts.cn

throw new RuntimeException("失败", 500);
来源：http://bn.jctech888.com.cn

[U72] PHP：写错误日志
来源：http://wm.newstarts.cn

error_log("失败: " . $e->getMessage());
来源：http://fm.hahajie.cn

[U73] PHP：读取 ini 配置
来源：http://nj.wgjwhj.cn

parse_ini_file("config.ini", true)
来源：http://is.panjiajie.cn

[U74] PHP：读取环境变量
来源：http://mk.jianghongdianzi.cn

getenv("APP_ENV") ?: "production"
来源：http://wm.shxzskj.cn

[U75] PHP：依赖注入
来源：http://pm.hnjuh.cn

composer require psr/container
来源：http://gs.wgjwhj.cn

[U76] PHP：简单路由
来源：http://sc.newstarts.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tc.jianghongdianzi.cn

[U77] PHP：模板渲染
来源：http://bu.521024.cn

composer require twig/twig
来源：http://xw.yuntaijiaju.cn

[U78] PHP：单元测试
来源：http://ar.bjjhwx.cn

composer require --dev phpunit/phpunit
来源：http://cq.yuntaijiaju.cn

[U79] PHP：静态分析
来源：http://dm.hahajie.cn

composer require --dev phpstan/phpstan
来源：http://lu.huixinmuqiang.cn

[U80] PHP：代码规范修复
来源：http://cs.9csxet.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ts.bookmarksfly.cn

[U81] JS：初始化项目
来源：http://cj.nszjky.cn

npm init -y;  npm i express
来源：http://dv.haigaiapp.cn

[U82] JS：package.json 脚本
来源：http://mk.shtwfgs.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jd.hahajie.cn

[U83] JS：ES Module 导入导出
来源：http://ch.huixiangedu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ej.yuexingan06.cn

[U84] JS：CommonJS 写法
来源：http://fj.bookmarksfly.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gd.shxzukj.cn

[U85] JS：可选链
来源：http://nm.hahajie.cn

a?.b?.c
来源：http://ox.hahajie.cn

[U86] JS：空值合并
来源：http://ov.yuexingan06.cn

a ?? b
来源：http://cr.huanxung.cn

[U87] JS：解构默认值
来源：http://ja.yuexingan06.cn

const { a = 1, b = 2 } = obj;
来源：http://my.szxytkj.cn

[U88] JS：对象展开合并
来源：http://wq.nszjky.cn

{ ...a, ...b }
来源：http://uk.shxzskj.cn

[U89] JS：数组去重
来源：http://iv.asd995.cn

[...new Set(arr)]
来源：http://dv.nicolike.cn

[U90] JS：数字数组排序
来源：http://zl.huixinmuqiang.cn

[...arr].sort((a, b) => a - b)
来源：http://nj.shxzukj.cn

[U91] JS：对象键值遍历
来源：http://ju.haigaiapp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nh.hnjuh.cn

[U92] JS：深拷贝
来源：http://hs.hnjuh.cn

structuredClone(obj)
来源：http://ku.gzmigu.cn

[U93] JS：模板字符串
来源：http://er.panjiajie.cn

`共 ${n} 条`
来源：http://xv.nicolike.cn

[U94] JS：箭头函数
来源：http://yp.9csxet.cn

const double = x => x * 2;
来源：http://tu.jctech888.com.cn

[U95] JS：Promise 包装
来源：http://vv.gzmigu.cn

new Promise((resolve, reject) => {})
来源：http://kr.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://ka.newstarts.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kg.newstarts.cn

[U97] JS：并发请求
来源：http://on.chemitech.net.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://sc.gzmigu.cn

[U98] JS：fetch 带 JSON
来源：http://mr.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pb.gzmigu.cn

[U99] JS：事件监听
来源：http://hz.newstarts.cn

el.addEventListener("click", e => {})
来源：http://om.colortex.cn

[U100] JS：DOM 查询
来源：http://vi.szsharing.cn

document.querySelector(".item")
来源：http://ad.bookmarksfly.cn

[U101] JS：classList 操作
来源：http://na.huixiangedu.cn

el.classList.toggle("active")
来源：http://bn.szsharing.cn

[U102] JS：本地存储
来源：http://uk.bjjhwx.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://uw.newstarts.cn

[U103] JS：定时器
来源：http://ag.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vr.chemitech.net.cn

[U104] JS：防抖
来源：http://hf.9csxet.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nr.nicolike.cn

[U105] JS：节流
来源：http://ky.huixiangedu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://md.muxihuayi.cn

[U106] JS：日期格式化
来源：http://ld.hnjuh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gn.huixinmuqiang.cn

[U107] JS：数字千分位
来源：http://xq.shtwfgs.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ig.shxzskj.cn

[U108] JS：随机整数
来源：http://zz.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://td.yuexingan06.cn

[U109] JS：数组分组
来源：http://ut.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://iw.huixiangedu.cn

[U110] JS：数组分块
来源：http://ej.haigaiapp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://st.asd995.cn

[U111] JS：对象转 Map
来源：http://ay.521024.cn

new Map(Object.entries(obj))
来源：http://oj.shtwfgs.cn

[U112] JS：字符串补位
来源：http://ca.9csxet.cn

"7".padStart(3, "0")
来源：http://kj.hahajie.cn

[U113] JS：正则替换全部
来源：http://ct.yuexingan06.cn

s.replaceAll("a", "b")
来源：http://xo.yuexingan06.cn

[U114] JS：JSON 深比较
来源：http://na.huixinmuqiang.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vx.huanxung.cn

[U115] JS：生成 UUID
来源：http://yt.huixinmuqiang.cn

crypto.randomUUID()
来源：http://tv.yuntaijiaju.cn

[U116] JS：类型检查（JSDoc）
来源：http://nl.gzmigu.cn

/** @param {string} name */ function f(name) {}
来源：http://lp.9csxet.cn

[U117] JS：单元测试
来源：http://zh.nszjky.cn

npm i -D vitest;  npx vitest
来源：http://wt.newstarts.cn

[U118] JS：开发服务器
来源：http://lv.wgjwhj.cn

npm i -D vite;  npx vite
来源：http://qj.shxzskj.cn

[U119] JS：生产构建
来源：http://ad.hnjuh.cn

npx vite build
来源：http://qa.521024.cn

[U120] JS：读取环境变量（Vite）
来源：http://ii.hahajie.cn

import.meta.env.VITE_API_URL
来源：http://zw.nicolike.cn

================================================================================
来源：http://ih.asd995.cn

统计汇总
来源：http://xz.yuexingan06.cn

================================================================================
来源：http://tq.huanxung.cn

按语言统计（条）：
来源：http://gh.gzmigu.cn

Python ......... 252
来源：http://er.jianghongdianzi.cn

PHP ............ 252
来源：http://ci.gzmigu.cn

JavaScript ..... 252
来源：http://bq.hahajie.cn

TypeScript ..... 212
来源：http://jt.521024.cn

Java ........... 212
来源：http://jm.huixinmuqiang.cn

Go ............. 212
来源：http://gh.shxzukj.cn

Ruby ........... 212
来源：http://co.huixiangedu.cn

C# ............. 212
来源：http://fz.huanxung.cn

C .............. 30
来源：http://ay.9csxet.cn

C++ ............ 30
来源：http://zb.bookmarksfly.cn

SQL ............ 90
来源：http://xx.muxihuayi.cn

Bash ........... 80
来源：http://tf.lnxyls.cn

Kotlin ......... 15
来源：http://lp.asd995.cn

Swift .......... 15
来源：http://jc.hahajie.cn

Lua ............ 10
来源：http://rr.bjjhwx.cn

Perl ........... 10
来源：http://kt.hahajie.cn

Scala .......... 10
来源：http://va.hnjuh.cn

------------------------------------
来源：http://bt.shxzskj.cn

合计 ........... 2106 条
来源：http://fa.gzmigu.cn

按章节统计：
来源：http://ua.hnjuh.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bz.colortex.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gn.jianghongdianzi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qm.muxihuayi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kp.szxytkj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nb.huixinmuqiang.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fz.521024.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yv.shxzukj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vu.shtwfgs.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gj.colortex.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xd.newstarts.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://om.wgjwhj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jq.yuexingan06.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nv.szsharing.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://py.jctech888.com.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yz.wgjwhj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://er.hahajie.cn

Q SQL 专题                              90
来源：http://nv.bjjhwx.cn

R Bash 专题                             80
来源：http://dd.panjiajie.cn

S C / C++ 专题                          60
来源：http://li.wgjwhj.cn

T 其他语言补充                          60
来源：http://qs.hnjuh.cn

U 高频实用片段                         120
来源：http://kx.chemitech.net.cn

------------------------------------
来源：http://dr.colortex.cn

合计                                  2106 条
来源：http://zi.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://ci.hahajie.cn

使用提醒
来源：http://om.521024.cn

--------------------------------------------------------------------------------
来源：http://xq.panjiajie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hr.muxihuayi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ev.huixiangedu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lc.huixinmuqiang.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ls.bjjhwx.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nj.gzmigu.cn

—— 文件结束 ——
来源：http://ym.yuexingan06.cn

================================================================================
来源：http://lp.hahajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://up.9csxet.cn

Common Programming Examples Cheat Book
来源：http://xi.9csxet.cn

================================================================================
来源：http://jr.lnxyls.cn

【收录内容】
来源：http://rl.shxzskj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://on.yuexingan06.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://po.yuexingan06.cn

SQL · Bash · C · C++
来源：http://li.nicolike.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fp.yuntaijiaju.cn

【使用说明】
来源：http://jx.muxihuayi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://og.jianghongdianzi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dx.huanxung.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vy.521024.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://su.newstarts.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xv.hnjuh.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qo.huixiangedu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vc.hnjuh.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ff.hahajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wd.szxytkj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dd.yuntaijiaju.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bw.shtwfgs.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zk.huixinmuqiang.cn

【文件统计】
来源：http://ed.hahajie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zl.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://bm.asd995.cn

目  录
来源：http://ar.nicolike.cn

--------------------------------------------------------------------------------
来源：http://os.wgjwhj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rw.hahajie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zu.newstarts.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mk.shtwfgs.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mp.521024.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gc.colortex.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ni.jianghongdianzi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ij.huixinmuqiang.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rh.szsharing.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://up.huanxung.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ba.huixinmuqiang.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://se.hahajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nv.asd995.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://oi.shtwfgs.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yg.nicolike.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mi.jctech888.com.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bf.newstarts.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bz.bjjhwx.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://fv.jctech888.com.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hx.jctech888.com.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cn.huixiangedu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cn.chemitech.net.cn

================================================================================
来源：http://kz.shxzukj.cn

A. 基础语法与类型
来源：http://ht.nicolike.cn

================================================================================
来源：http://nj.yuntaijiaju.cn

[A01] Hello World
来源：http://qr.shtwfgs.cn

Py:   print("Hello, World!")
来源：http://yn.jianghongdianzi.cn

PHP:  echo "Hello, World!";
来源：http://go.yuexingan06.cn

JS:   console.log("Hello, World!");
来源：http://sr.panjiajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bt.huixinmuqiang.cn

Java: System.out.println("Hello, World!");
来源：http://sd.lnxyls.cn

Go:   fmt.Println("Hello, World!")
来源：http://mz.lnxyls.cn

Ruby: puts "Hello, World!"
来源：http://id.hnjuh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://qa.yuntaijiaju.cn

[A02] 变量声明与赋值
来源：http://ga.shtwfgs.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wp.asd995.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://fd.panjiajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xh.jctech888.com.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ai.9csxet.cn

Java: String name = "Alex"; int age = 20;
来源：http://tf.szsharing.cn

Go:   name := "Alex"; age := 20
来源：http://qo.9csxet.cn

Ruby: name = "Alex"; age = 20
来源：http://nc.colortex.cn

C#:   string name = "Alex"; int age = 20;
来源：http://rw.hnjuh.cn

[A03] 常量定义
来源：http://lt.newstarts.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://oe.huanxung.cn

PHP:  const PI = 3.14159;
来源：http://az.521024.cn

JS:   const PI = 3.14159;
来源：http://xk.lnxyls.cn

TS:   const PI: number = 3.14159;
来源：http://zp.bjjhwx.cn

Java: static final double PI = 3.14159;
来源：http://hj.jctech888.com.cn

Go:   const PI = 3.14159
来源：http://zu.wgjwhj.cn

Ruby: PI = 3.14159
来源：http://im.hahajie.cn

C#:   const double PI = 3.14159;
来源：http://jt.shtwfgs.cn

[A04] 判断变量类型
来源：http://um.lnxyls.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://xr.lnxyls.cn


<!-- 参考信息 -->