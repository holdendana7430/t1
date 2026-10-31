代发 wailian999

[U43] PHP：声明命名空间
来源：http://wu.shxzskj.cn

namespace App\Http;
来源：http://hf.chemitech.net.cn

[U44] PHP：开启严格类型
来源：http://pl.shxzskj.cn

declare(strict_types=1);
来源：http://ed.shtwfgs.cn

[U45] PHP：类型声明与返回类型
来源：http://po.chemitech.net.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://kj.huanxung.cn

[U46] PHP：可空类型
来源：http://im.hahajie.cn

?string $name = null
来源：http://ms.huixinmuqiang.cn

[U47] PHP：联合类型
来源：http://cj.muxihuayi.cn

int|string $id
来源：http://fn.shxzskj.cn

[U48] PHP：纯枚举
来源：http://qx.chemitech.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xb.shxzskj.cn

[U49] PHP：只读属性
来源：http://ru.gzmigu.cn

public readonly string $name
来源：http://ek.szxytkj.cn

[U50] PHP：构造器属性提升
来源：http://jf.haigaiapp.cn

public function __construct(private int $id) {}
来源：http://pw.chemitech.net.cn

[U51] PHP：数组解构
来源：http://km.jctech888.com.cn

[$a, $b] = $arr;
来源：http://du.haigaiapp.cn

[U52] PHP：箭头函数
来源：http://to.jctech888.com.cn

$double = fn($x) => $x * 2;
来源：http://of.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://ri.hahajie.cn

$v = $a ?? $b ?? "default";
来源：http://yh.muxihuayi.cn

[U54] PHP：空安全调用
来源：http://hb.hahajie.cn

$obj?->method()
来源：http://rj.szsharing.cn

[U55] PHP：match 表达式
来源：http://fg.muxihuayi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ed.panjiajie.cn

[U56] PHP：命名参数
来源：http://ff.yuexingan06.cn

f(a: 1, b: 2)
来源：http://bh.yuntaijiaju.cn

[U57] PHP：字符串插值
来源：http://ao.hahajie.cn

"值: {$a}"
来源：http://lq.muxihuayi.cn

[U58] PHP：数组三件套
来源：http://tw.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mj.szsharing.cn

[U59] PHP：自定义排序
来源：http://fp.huanxung.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lr.jctech888.com.cn

[U60] PHP：JSON 编解码
来源：http://fg.shxzukj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hk.jianghongdianzi.cn

[U61] PHP：正则
来源：http://wx.bookmarksfly.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zj.szxytkj.cn

[U62] PHP：日期对象
来源：http://yi.asd995.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wz.muxihuayi.cn

[U63] PHP：文件读写
来源：http://bx.bookmarksfly.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ul.wgjwhj.cn

[U64] PHP：目录遍历
来源：http://wz.newstarts.cn

glob("dir/*.php");  scandir("dir");
来源：http://rz.lnxyls.cn

[U65] PHP：会话
来源：http://bc.gzmigu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hb.muxihuayi.cn

[U66] PHP：设置 Cookie
来源：http://xq.shtwfgs.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zu.jctech888.com.cn

[U67] PHP：处理文件上传
来源：http://fb.shtwfgs.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fs.bjjhwx.cn

[U68] PHP：PDO 连接
来源：http://oq.bjjhwx.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yl.hahajie.cn

[U69] PHP：PDO 预处理
来源：http://yd.521024.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vh.haigaiapp.cn

[U70] PHP：PDO 事务
来源：http://sm.9csxet.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qn.szsharing.cn

[U71] PHP：抛出异常
来源：http://dg.haigaiapp.cn

throw new RuntimeException("失败", 500);
来源：http://uf.bookmarksfly.cn

[U72] PHP：写错误日志
来源：http://ct.gzmigu.cn

error_log("失败: " . $e->getMessage());
来源：http://oj.gzmigu.cn

[U73] PHP：读取 ini 配置
来源：http://fe.szsharing.cn

parse_ini_file("config.ini", true)
来源：http://af.colortex.cn

[U74] PHP：读取环境变量
来源：http://ut.shtwfgs.cn

getenv("APP_ENV") ?: "production"
来源：http://jp.nicolike.cn

[U75] PHP：依赖注入
来源：http://tx.chemitech.net.cn

composer require psr/container
来源：http://lg.shxzskj.cn

[U76] PHP：简单路由
来源：http://eg.haigaiapp.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mi.asd995.cn

[U77] PHP：模板渲染
来源：http://gf.asd995.cn

composer require twig/twig
来源：http://br.521024.cn

[U78] PHP：单元测试
来源：http://zy.hnjuh.cn

composer require --dev phpunit/phpunit
来源：http://wr.huixiangedu.cn

[U79] PHP：静态分析
来源：http://gx.jctech888.com.cn

composer require --dev phpstan/phpstan
来源：http://mz.huixinmuqiang.cn

[U80] PHP：代码规范修复
来源：http://ec.gzmigu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ou.haigaiapp.cn

[U81] JS：初始化项目
来源：http://zf.asd995.cn

npm init -y;  npm i express
来源：http://fs.szxytkj.cn

[U82] JS：package.json 脚本
来源：http://ef.hnjuh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rh.nszjky.cn

[U83] JS：ES Module 导入导出
来源：http://hs.521024.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ei.nszjky.cn

[U84] JS：CommonJS 写法
来源：http://ie.yuexingan06.cn

module.exports = { a };  const { a } = require("./m");
来源：http://eq.colortex.cn

[U85] JS：可选链
来源：http://vm.huixiangedu.cn

a?.b?.c
来源：http://kb.panjiajie.cn

[U86] JS：空值合并
来源：http://iq.521024.cn

a ?? b
来源：http://om.jianghongdianzi.cn

[U87] JS：解构默认值
来源：http://fr.bookmarksfly.cn

const { a = 1, b = 2 } = obj;
来源：http://ed.colortex.cn

[U88] JS：对象展开合并
来源：http://zd.yuntaijiaju.cn

{ ...a, ...b }
来源：http://sh.bookmarksfly.cn

[U89] JS：数组去重
来源：http://xz.shtwfgs.cn

[...new Set(arr)]
来源：http://ab.jianghongdianzi.cn

[U90] JS：数字数组排序
来源：http://ox.shxzskj.cn

[...arr].sort((a, b) => a - b)
来源：http://cm.shxzukj.cn

[U91] JS：对象键值遍历
来源：http://ac.yuexingan06.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ce.jctech888.com.cn

[U92] JS：深拷贝
来源：http://uw.shtwfgs.cn

structuredClone(obj)
来源：http://qj.asd995.cn

[U93] JS：模板字符串
来源：http://nl.jctech888.com.cn

`共 ${n} 条`
来源：http://kn.521024.cn

[U94] JS：箭头函数
来源：http://hd.newstarts.cn

const double = x => x * 2;
来源：http://cf.jctech888.com.cn

[U95] JS：Promise 包装
来源：http://ml.szsharing.cn

new Promise((resolve, reject) => {})
来源：http://rd.bookmarksfly.cn

[U96] JS：async/await 与异常
来源：http://ej.9csxet.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zm.asd995.cn

[U97] JS：并发请求
来源：http://gi.nicolike.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ro.szxytkj.cn

[U98] JS：fetch 带 JSON
来源：http://ti.hahajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sw.hnjuh.cn

[U99] JS：事件监听
来源：http://mr.shxzukj.cn

el.addEventListener("click", e => {})
来源：http://ca.colortex.cn

[U100] JS：DOM 查询
来源：http://xw.asd995.cn

document.querySelector(".item")
来源：http://om.huixinmuqiang.cn

[U101] JS：classList 操作
来源：http://vs.hahajie.cn

el.classList.toggle("active")
来源：http://rc.nicolike.cn

[U102] JS：本地存储
来源：http://yl.asd995.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://lq.haigaiapp.cn

[U103] JS：定时器
来源：http://zd.colortex.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rg.szxytkj.cn

[U104] JS：防抖
来源：http://ay.9csxet.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nc.shtwfgs.cn

[U105] JS：节流
来源：http://wr.muxihuayi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jc.szsharing.cn

[U106] JS：日期格式化
来源：http://mb.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fr.asd995.cn

[U107] JS：数字千分位
来源：http://qh.nszjky.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wo.muxihuayi.cn

[U108] JS：随机整数
来源：http://gj.hahajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zq.shxzukj.cn

[U109] JS：数组分组
来源：http://of.nszjky.cn

Object.groupBy(arr, x => x.type)
来源：http://vn.huixiangedu.cn

[U110] JS：数组分块
来源：http://na.521024.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wg.shtwfgs.cn

[U111] JS：对象转 Map
来源：http://os.hnjuh.cn

new Map(Object.entries(obj))
来源：http://ew.szxytkj.cn

[U112] JS：字符串补位
来源：http://kh.colortex.cn

"7".padStart(3, "0")
来源：http://qb.shtwfgs.cn

[U113] JS：正则替换全部
来源：http://np.wgjwhj.cn

s.replaceAll("a", "b")
来源：http://dd.nicolike.cn

[U114] JS：JSON 深比较
来源：http://ut.jctech888.com.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jx.nszjky.cn

[U115] JS：生成 UUID
来源：http://ve.shxzskj.cn

crypto.randomUUID()
来源：http://mc.jctech888.com.cn

[U116] JS：类型检查（JSDoc）
来源：http://kn.szsharing.cn

/** @param {string} name */ function f(name) {}
来源：http://zr.shtwfgs.cn

[U117] JS：单元测试
来源：http://kb.hahajie.cn

npm i -D vitest;  npx vitest
来源：http://ms.panjiajie.cn

[U118] JS：开发服务器
来源：http://iq.yuexingan06.cn

npm i -D vite;  npx vite
来源：http://xu.lnxyls.cn

[U119] JS：生产构建
来源：http://wj.nicolike.cn

npx vite build
来源：http://cn.shtwfgs.cn

[U120] JS：读取环境变量（Vite）
来源：http://ri.szxytkj.cn

import.meta.env.VITE_API_URL
来源：http://gn.bookmarksfly.cn

================================================================================
来源：http://ob.wgjwhj.cn

统计汇总
来源：http://os.jctech888.com.cn

================================================================================
来源：http://ds.chemitech.net.cn

按语言统计（条）：
来源：http://jl.huixiangedu.cn

Python ......... 252
来源：http://wk.panjiajie.cn

PHP ............ 252
来源：http://uq.yuntaijiaju.cn

JavaScript ..... 252
来源：http://oa.szsharing.cn

TypeScript ..... 212
来源：http://fn.szsharing.cn

Java ........... 212
来源：http://dr.szsharing.cn

Go ............. 212
来源：http://bf.asd995.cn

Ruby ........... 212
来源：http://wx.nicolike.cn

C# ............. 212
来源：http://kd.yuexingan06.cn

C .............. 30
来源：http://cb.9csxet.cn

C++ ............ 30
来源：http://rj.panjiajie.cn

SQL ............ 90
来源：http://az.muxihuayi.cn

Bash ........... 80
来源：http://ov.jctech888.com.cn

Kotlin ......... 15
来源：http://ed.bookmarksfly.cn

Swift .......... 15
来源：http://un.bjjhwx.cn

Lua ............ 10
来源：http://tv.nszjky.cn

Perl ........... 10
来源：http://dv.hahajie.cn

Scala .......... 10
来源：http://rr.9csxet.cn

------------------------------------
来源：http://ur.szxytkj.cn

合计 ........... 2106 条
来源：http://ou.huixinmuqiang.cn

按章节统计：
来源：http://gq.huanxung.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wp.hnjuh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jm.haigaiapp.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uq.jianghongdianzi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vp.9csxet.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hb.bookmarksfly.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zd.wgjwhj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fy.shtwfgs.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ow.newstarts.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tb.shxzskj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fk.colortex.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://eq.szxytkj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dx.9csxet.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fz.asd995.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rn.haigaiapp.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yg.haigaiapp.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ct.nszjky.cn

Q SQL 专题                              90
来源：http://hr.9csxet.cn

R Bash 专题                             80
来源：http://ft.jianghongdianzi.cn

S C / C++ 专题                          60
来源：http://jq.hnjuh.cn

T 其他语言补充                          60
来源：http://kg.hnjuh.cn

U 高频实用片段                         120
来源：http://ar.muxihuayi.cn

------------------------------------
来源：http://mg.jianghongdianzi.cn

合计                                  2106 条
来源：http://ae.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://ty.lnxyls.cn

使用提醒
来源：http://ax.szsharing.cn

--------------------------------------------------------------------------------
来源：http://bd.lnxyls.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://iz.shxzukj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dn.huixiangedu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mg.huixiangedu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ir.szxytkj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://va.huanxung.cn

—— 文件结束 ——
来源：http://ww.9csxet.cn

================================================================================
来源：http://hp.muxihuayi.cn

程序语言常见例子速查手册（2024 版）
来源：http://cb.shtwfgs.cn

Common Programming Examples Cheat Book
来源：http://cq.huixinmuqiang.cn

================================================================================
来源：http://ia.521024.cn

【收录内容】
来源：http://ht.newstarts.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ja.yuexingan06.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ri.jctech888.com.cn

SQL · Bash · C · C++
来源：http://am.jianghongdianzi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sf.nicolike.cn

【使用说明】
来源：http://de.jianghongdianzi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qs.jianghongdianzi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hl.shtwfgs.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mp.shxzskj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lc.lnxyls.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://da.hnjuh.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sq.nszjky.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mp.haigaiapp.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hk.szxytkj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gt.panjiajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ae.yuexingan06.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zc.newstarts.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ho.colortex.cn

【文件统计】
来源：http://tq.huanxung.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gv.nszjky.cn

--------------------------------------------------------------------------------
来源：http://yr.hahajie.cn

目  录
来源：http://qk.nszjky.cn

--------------------------------------------------------------------------------
来源：http://sh.521024.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hy.jianghongdianzi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tz.nicolike.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://et.yuntaijiaju.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xr.wgjwhj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nb.shtwfgs.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mf.huanxung.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qv.yuntaijiaju.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bs.521024.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nz.bjjhwx.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hb.huixinmuqiang.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://va.haigaiapp.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zi.bjjhwx.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://id.haigaiapp.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://iv.gzmigu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zm.newstarts.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kb.chemitech.net.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jf.hahajie.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ap.jctech888.com.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uy.yuntaijiaju.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wl.hnjuh.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xw.hahajie.cn

================================================================================
来源：http://hw.asd995.cn

A. 基础语法与类型
来源：http://qx.bjjhwx.cn

================================================================================
来源：http://jm.szxytkj.cn

[A01] Hello World
来源：http://wy.shxzukj.cn

Py:   print("Hello, World!")
来源：http://fi.haigaiapp.cn

PHP:  echo "Hello, World!";
来源：http://gb.shtwfgs.cn

JS:   console.log("Hello, World!");
来源：http://ot.panjiajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ac.wgjwhj.cn

Java: System.out.println("Hello, World!");
来源：http://tc.szxytkj.cn

Go:   fmt.Println("Hello, World!")
来源：http://zp.jianghongdianzi.cn

Ruby: puts "Hello, World!"
来源：http://ea.521024.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ui.shxzskj.cn

[A02] 变量声明与赋值
来源：http://dk.chemitech.net.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ns.shxzukj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rg.hahajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ta.nicolike.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dg.newstarts.cn

Java: String name = "Alex"; int age = 20;
来源：http://bk.yuexingan06.cn

Go:   name := "Alex"; age := 20
来源：http://ng.lnxyls.cn

Ruby: name = "Alex"; age = 20
来源：http://py.yuexingan06.cn

C#:   string name = "Alex"; int age = 20;
来源：http://cx.chemitech.net.cn

[A03] 常量定义
来源：http://hu.huixiangedu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://oo.521024.cn

PHP:  const PI = 3.14159;
来源：http://kt.521024.cn

JS:   const PI = 3.14159;
来源：http://sm.hahajie.cn

TS:   const PI: number = 3.14159;
来源：http://qq.szxytkj.cn

Java: static final double PI = 3.14159;
来源：http://ta.bjjhwx.cn

Go:   const PI = 3.14159
来源：http://uu.jctech888.com.cn

Ruby: PI = 3.14159
来源：http://am.huixinmuqiang.cn

C#:   const double PI = 3.14159;
来源：http://wj.wgjwhj.cn

[A04] 判断变量类型
来源：http://az.szsharing.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dk.lnxyls.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ga.szxytkj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xm.yuntaijiaju.cn

TS:   typeof x; x instanceof Date
来源：http://dn.huixiangedu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zt.nicolike.cn

Go:   reflect.TypeOf(x).Name()
来源：http://xj.shxzukj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://el.hnjuh.cn

C#:   x.GetType().Name; x is int
来源：http://cp.shxzukj.cn

[A05] 整数除法与取模
来源：http://jj.muxihuayi.cn


<!-- 参考信息 -->