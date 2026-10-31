代发 wailian999

[U43] PHP：声明命名空间
来源：http://ni.haigaiapp.cn

namespace App\Http;
来源：http://ty.hnjuh.cn

[U44] PHP：开启严格类型
来源：http://ga.haigaiapp.cn

declare(strict_types=1);
来源：http://xw.asd995.cn

[U45] PHP：类型声明与返回类型
来源：http://gx.huixinmuqiang.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ov.jctech888.com.cn

[U46] PHP：可空类型
来源：http://mj.bookmarksfly.cn

?string $name = null
来源：http://pf.lnxyls.cn

[U47] PHP：联合类型
来源：http://xz.newstarts.cn

int|string $id
来源：http://rw.9csxet.cn

[U48] PHP：纯枚举
来源：http://ca.muxihuayi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nj.shtwfgs.cn

[U49] PHP：只读属性
来源：http://jy.gzmigu.cn

public readonly string $name
来源：http://db.nicolike.cn

[U50] PHP：构造器属性提升
来源：http://ex.hnjuh.cn

public function __construct(private int $id) {}
来源：http://cq.shtwfgs.cn

[U51] PHP：数组解构
来源：http://km.colortex.cn

[$a, $b] = $arr;
来源：http://uy.chemitech.net.cn

[U52] PHP：箭头函数
来源：http://ir.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://gx.chemitech.net.cn

[U53] PHP：空合并运算符
来源：http://ha.nicolike.cn

$v = $a ?? $b ?? "default";
来源：http://ay.colortex.cn

[U54] PHP：空安全调用
来源：http://wz.nszjky.cn

$obj?->method()
来源：http://mn.haigaiapp.cn

[U55] PHP：match 表达式
来源：http://ib.yuexingan06.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ch.shxzukj.cn

[U56] PHP：命名参数
来源：http://ef.jctech888.com.cn

f(a: 1, b: 2)
来源：http://hl.jianghongdianzi.cn

[U57] PHP：字符串插值
来源：http://mm.muxihuayi.cn

"值: {$a}"
来源：http://xv.huixinmuqiang.cn

[U58] PHP：数组三件套
来源：http://af.haigaiapp.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ga.gzmigu.cn

[U59] PHP：自定义排序
来源：http://ky.9csxet.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uj.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://nv.colortex.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fg.9csxet.cn

[U61] PHP：正则
来源：http://nk.shxzskj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xt.wgjwhj.cn

[U62] PHP：日期对象
来源：http://yl.jianghongdianzi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ng.szxytkj.cn

[U63] PHP：文件读写
来源：http://zn.huanxung.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ds.shxzukj.cn

[U64] PHP：目录遍历
来源：http://qk.muxihuayi.cn

glob("dir/*.php");  scandir("dir");
来源：http://ar.wgjwhj.cn

[U65] PHP：会话
来源：http://sz.hahajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cm.yuexingan06.cn

[U66] PHP：设置 Cookie
来源：http://mi.shxzskj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zw.yuntaijiaju.cn

[U67] PHP：处理文件上传
来源：http://gn.nszjky.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rc.521024.cn

[U68] PHP：PDO 连接
来源：http://wv.shxzskj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rw.panjiajie.cn

[U69] PHP：PDO 预处理
来源：http://bg.huixinmuqiang.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cl.huanxung.cn

[U70] PHP：PDO 事务
来源：http://bc.szsharing.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ly.9csxet.cn

[U71] PHP：抛出异常
来源：http://in.szsharing.cn

throw new RuntimeException("失败", 500);
来源：http://ni.yuexingan06.cn

[U72] PHP：写错误日志
来源：http://pp.lnxyls.cn

error_log("失败: " . $e->getMessage());
来源：http://vd.shxzskj.cn

[U73] PHP：读取 ini 配置
来源：http://gt.lnxyls.cn

parse_ini_file("config.ini", true)
来源：http://ro.colortex.cn

[U74] PHP：读取环境变量
来源：http://ym.521024.cn

getenv("APP_ENV") ?: "production"
来源：http://oj.szsharing.cn

[U75] PHP：依赖注入
来源：http://bs.521024.cn

composer require psr/container
来源：http://kt.yuexingan06.cn

[U76] PHP：简单路由
来源：http://fx.szxytkj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gb.panjiajie.cn

[U77] PHP：模板渲染
来源：http://qu.chemitech.net.cn

composer require twig/twig
来源：http://ia.newstarts.cn

[U78] PHP：单元测试
来源：http://ld.huanxung.cn

composer require --dev phpunit/phpunit
来源：http://wx.shxzukj.cn

[U79] PHP：静态分析
来源：http://qr.bjjhwx.cn

composer require --dev phpstan/phpstan
来源：http://yh.gzmigu.cn

[U80] PHP：代码规范修复
来源：http://hw.huixiangedu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ah.szxytkj.cn

[U81] JS：初始化项目
来源：http://au.huixiangedu.cn

npm init -y;  npm i express
来源：http://ul.newstarts.cn

[U82] JS：package.json 脚本
来源：http://oc.shxzukj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ct.panjiajie.cn

[U83] JS：ES Module 导入导出
来源：http://hi.shxzskj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lc.shxzukj.cn

[U84] JS：CommonJS 写法
来源：http://ne.gzmigu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hw.bookmarksfly.cn

[U85] JS：可选链
来源：http://oe.jctech888.com.cn

a?.b?.c
来源：http://tc.shxzskj.cn

[U86] JS：空值合并
来源：http://cd.521024.cn

a ?? b
来源：http://zi.nszjky.cn

[U87] JS：解构默认值
来源：http://iw.asd995.cn

const { a = 1, b = 2 } = obj;
来源：http://yy.jctech888.com.cn

[U88] JS：对象展开合并
来源：http://uz.hnjuh.cn

{ ...a, ...b }
来源：http://dr.szxytkj.cn

[U89] JS：数组去重
来源：http://ax.shtwfgs.cn

[...new Set(arr)]
来源：http://ko.gzmigu.cn

[U90] JS：数字数组排序
来源：http://iw.huixinmuqiang.cn

[...arr].sort((a, b) => a - b)
来源：http://oa.shxzskj.cn

[U91] JS：对象键值遍历
来源：http://cz.colortex.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mn.szxytkj.cn

[U92] JS：深拷贝
来源：http://hk.nicolike.cn

structuredClone(obj)
来源：http://nm.hahajie.cn

[U93] JS：模板字符串
来源：http://fz.szsharing.cn

`共 ${n} 条`
来源：http://pk.muxihuayi.cn

[U94] JS：箭头函数
来源：http://qn.hnjuh.cn

const double = x => x * 2;
来源：http://cz.shtwfgs.cn

[U95] JS：Promise 包装
来源：http://pd.szsharing.cn

new Promise((resolve, reject) => {})
来源：http://ff.panjiajie.cn

[U96] JS：async/await 与异常
来源：http://im.nszjky.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jr.jianghongdianzi.cn

[U97] JS：并发请求
来源：http://mf.szxytkj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jp.nicolike.cn

[U98] JS：fetch 带 JSON
来源：http://bk.nszjky.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ye.newstarts.cn

[U99] JS：事件监听
来源：http://hd.muxihuayi.cn

el.addEventListener("click", e => {})
来源：http://hu.shxzukj.cn

[U100] JS：DOM 查询
来源：http://qi.asd995.cn

document.querySelector(".item")
来源：http://rg.szxytkj.cn

[U101] JS：classList 操作
来源：http://dd.huixinmuqiang.cn

el.classList.toggle("active")
来源：http://tw.huixiangedu.cn

[U102] JS：本地存储
来源：http://zp.asd995.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wo.bjjhwx.cn

[U103] JS：定时器
来源：http://ur.muxihuayi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uq.jianghongdianzi.cn

[U104] JS：防抖
来源：http://oq.hnjuh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://md.jctech888.com.cn

[U105] JS：节流
来源：http://el.yuexingan06.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mw.bjjhwx.cn

[U106] JS：日期格式化
来源：http://wu.wgjwhj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hb.nicolike.cn

[U107] JS：数字千分位
来源：http://zr.szxytkj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dm.szsharing.cn

[U108] JS：随机整数
来源：http://rt.shxzukj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kf.colortex.cn

[U109] JS：数组分组
来源：http://jo.nicolike.cn

Object.groupBy(arr, x => x.type)
来源：http://lt.hnjuh.cn

[U110] JS：数组分块
来源：http://gz.nicolike.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zf.asd995.cn

[U111] JS：对象转 Map
来源：http://ja.shxzskj.cn

new Map(Object.entries(obj))
来源：http://qn.colortex.cn

[U112] JS：字符串补位
来源：http://ku.wgjwhj.cn

"7".padStart(3, "0")
来源：http://xi.shxzskj.cn

[U113] JS：正则替换全部
来源：http://qr.jianghongdianzi.cn

s.replaceAll("a", "b")
来源：http://vi.huixinmuqiang.cn

[U114] JS：JSON 深比较
来源：http://vu.yuexingan06.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rv.shxzskj.cn

[U115] JS：生成 UUID
来源：http://vv.szsharing.cn

crypto.randomUUID()
来源：http://kk.yuntaijiaju.cn

[U116] JS：类型检查（JSDoc）
来源：http://oo.colortex.cn

/** @param {string} name */ function f(name) {}
来源：http://ta.szxytkj.cn

[U117] JS：单元测试
来源：http://im.huixiangedu.cn

npm i -D vitest;  npx vitest
来源：http://mg.bookmarksfly.cn

[U118] JS：开发服务器
来源：http://lz.jianghongdianzi.cn

npm i -D vite;  npx vite
来源：http://at.nszjky.cn

[U119] JS：生产构建
来源：http://wt.jianghongdianzi.cn

npx vite build
来源：http://if.nicolike.cn

[U120] JS：读取环境变量（Vite）
来源：http://ll.9csxet.cn

import.meta.env.VITE_API_URL
来源：http://jr.muxihuayi.cn

================================================================================
来源：http://mc.newstarts.cn

统计汇总
来源：http://ud.jianghongdianzi.cn

================================================================================
来源：http://bc.huixiangedu.cn

按语言统计（条）：
来源：http://yc.huanxung.cn

Python ......... 252
来源：http://fa.shxzukj.cn

PHP ............ 252
来源：http://re.bookmarksfly.cn

JavaScript ..... 252
来源：http://wk.szsharing.cn

TypeScript ..... 212
来源：http://vj.shxzskj.cn

Java ........... 212
来源：http://nv.nicolike.cn

Go ............. 212
来源：http://pa.jctech888.com.cn

Ruby ........... 212
来源：http://mk.nicolike.cn

C# ............. 212
来源：http://sw.yuexingan06.cn

C .............. 30
来源：http://tn.nicolike.cn

C++ ............ 30
来源：http://wy.panjiajie.cn

SQL ............ 90
来源：http://xr.lnxyls.cn

Bash ........... 80
来源：http://jc.nicolike.cn

Kotlin ......... 15
来源：http://ym.huanxung.cn

Swift .......... 15
来源：http://cs.yuexingan06.cn

Lua ............ 10
来源：http://lz.shtwfgs.cn

Perl ........... 10
来源：http://vr.huixinmuqiang.cn

Scala .......... 10
来源：http://fn.huixinmuqiang.cn

------------------------------------
来源：http://sk.9csxet.cn

合计 ........... 2106 条
来源：http://eh.lnxyls.cn

按章节统计：
来源：http://ff.asd995.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://os.nicolike.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://df.nszjky.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uy.yuexingan06.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pm.jctech888.com.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vs.nicolike.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xi.colortex.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://oc.gzmigu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xr.wgjwhj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sj.shxzukj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ch.asd995.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ea.shxzskj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sf.szxytkj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zi.panjiajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dy.9csxet.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mw.huixinmuqiang.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wv.nicolike.cn

Q SQL 专题                              90
来源：http://vo.bookmarksfly.cn

R Bash 专题                             80
来源：http://dy.huanxung.cn

S C / C++ 专题                          60
来源：http://nk.hahajie.cn

T 其他语言补充                          60
来源：http://qj.hahajie.cn

U 高频实用片段                         120
来源：http://dn.hnjuh.cn

------------------------------------
来源：http://pp.jctech888.com.cn

合计                                  2106 条
来源：http://dp.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://iq.jianghongdianzi.cn

使用提醒
来源：http://wi.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://ou.huixinmuqiang.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zc.yuexingan06.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://eu.huanxung.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://aa.shxzskj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://nk.gzmigu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tb.shtwfgs.cn

—— 文件结束 ——
来源：http://vs.panjiajie.cn

================================================================================
来源：http://zj.huanxung.cn

程序语言常见例子速查手册（2024 版）
来源：http://nm.shxzskj.cn

Common Programming Examples Cheat Book
来源：http://dj.hnjuh.cn

================================================================================
来源：http://ub.jctech888.com.cn

【收录内容】
来源：http://hu.9csxet.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://wa.hahajie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tu.huixiangedu.cn

SQL · Bash · C · C++
来源：http://or.yuntaijiaju.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://di.colortex.cn

【使用说明】
来源：http://qp.panjiajie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gr.huixinmuqiang.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cy.szsharing.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yr.szxytkj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gu.muxihuayi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://zo.shxzskj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uu.yuexingan06.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kt.yuntaijiaju.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mq.haigaiapp.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ka.nszjky.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cb.haigaiapp.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vd.asd995.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jh.bjjhwx.cn

【文件统计】
来源：http://zv.hnjuh.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ji.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://xt.shxzskj.cn

目  录
来源：http://nm.newstarts.cn

--------------------------------------------------------------------------------
来源：http://nf.szsharing.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zv.jctech888.com.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://oz.bookmarksfly.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rx.huixinmuqiang.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nz.gzmigu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xu.shxzskj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wk.shtwfgs.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wm.newstarts.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ep.jctech888.com.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pb.hnjuh.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hv.yuexingan06.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://px.nszjky.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://py.asd995.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gd.gzmigu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rk.colortex.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gk.huixiangedu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://uz.lnxyls.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://je.lnxyls.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://nf.gzmigu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fn.hahajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zy.nicolike.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vt.szsharing.cn

================================================================================
来源：http://si.muxihuayi.cn

A. 基础语法与类型
来源：http://ws.bjjhwx.cn

================================================================================
来源：http://dk.shtwfgs.cn

[A01] Hello World
来源：http://xm.jianghongdianzi.cn

Py:   print("Hello, World!")
来源：http://ir.asd995.cn

PHP:  echo "Hello, World!";
来源：http://ff.shxzskj.cn

JS:   console.log("Hello, World!");
来源：http://bk.wgjwhj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sv.szxytkj.cn

Java: System.out.println("Hello, World!");
来源：http://bu.newstarts.cn

Go:   fmt.Println("Hello, World!")
来源：http://gu.hnjuh.cn

Ruby: puts "Hello, World!"
来源：http://jg.huanxung.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://yh.lnxyls.cn

[A02] 变量声明与赋值
来源：http://cl.9csxet.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kn.nicolike.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rs.bjjhwx.cn

JS:   let name = "Alex"; const age = 20;
来源：http://pi.shxzukj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cg.bookmarksfly.cn

Java: String name = "Alex"; int age = 20;
来源：http://vz.chemitech.net.cn

Go:   name := "Alex"; age := 20
来源：http://fx.jianghongdianzi.cn

Ruby: name = "Alex"; age = 20
来源：http://du.szxytkj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ki.wgjwhj.cn

[A03] 常量定义
来源：http://xh.colortex.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ai.shtwfgs.cn

PHP:  const PI = 3.14159;
来源：http://dm.huixinmuqiang.cn

JS:   const PI = 3.14159;
来源：http://kq.lnxyls.cn

TS:   const PI: number = 3.14159;
来源：http://fo.szxytkj.cn

Java: static final double PI = 3.14159;
来源：http://of.colortex.cn

Go:   const PI = 3.14159
来源：http://qe.muxihuayi.cn

Ruby: PI = 3.14159
来源：http://pj.hnjuh.cn

C#:   const double PI = 3.14159;
来源：http://yf.shxzskj.cn

[A04] 判断变量类型
来源：http://rt.huixinmuqiang.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cq.9csxet.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://db.jctech888.com.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://es.shxzukj.cn

TS:   typeof x; x instanceof Date
来源：http://rv.gzmigu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tj.shxzskj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pa.521024.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ov.bookmarksfly.cn

C#:   x.GetType().Name; x is int
来源：http://uu.shxzukj.cn

[A05] 整数除法与取模
来源：http://gf.yuntaijiaju.cn


<!-- 参考信息 -->