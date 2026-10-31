代发 wailian999

[U37] Py：读写 Excel
来源：http://rc.shxzukj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vx.hnjuh.cn

[U38] Py：获取脚本所在目录
来源：http://hx.huixinmuqiang.cn

Path(__file__).resolve().parent
来源：http://yc.asd995.cn

[U39] Py：判断是否在交互环境
来源：http://na.muxihuayi.cn

sys.stdout.isatty()
来源：http://di.wgjwhj.cn

[U40] Py：打印到标准错误
来源：http://xz.colortex.cn

print("err", file=sys.stderr)
来源：http://ku.hnjuh.cn

[U41] PHP：初始化 Composer 项目
来源：http://lc.muxihuayi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mp.shxzukj.cn

[U42] PHP：PSR-4 自动加载
来源：http://vc.huixinmuqiang.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xv.jianghongdianzi.cn

[U43] PHP：声明命名空间
来源：http://fl.shxzskj.cn

namespace App\Http;
来源：http://gq.colortex.cn

[U44] PHP：开启严格类型
来源：http://rz.521024.cn

declare(strict_types=1);
来源：http://ef.szsharing.cn

[U45] PHP：类型声明与返回类型
来源：http://op.jctech888.com.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tj.shxzukj.cn

[U46] PHP：可空类型
来源：http://se.shxzskj.cn

?string $name = null
来源：http://jc.jctech888.com.cn

[U47] PHP：联合类型
来源：http://ty.huixinmuqiang.cn

int|string $id
来源：http://cj.huixiangedu.cn

[U48] PHP：纯枚举
来源：http://fb.hnjuh.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ok.wgjwhj.cn

[U49] PHP：只读属性
来源：http://zx.chemitech.net.cn

public readonly string $name
来源：http://ji.asd995.cn

[U50] PHP：构造器属性提升
来源：http://pc.shxzskj.cn

public function __construct(private int $id) {}
来源：http://hd.yuexingan06.cn

[U51] PHP：数组解构
来源：http://lq.bookmarksfly.cn

[$a, $b] = $arr;
来源：http://hh.huixiangedu.cn

[U52] PHP：箭头函数
来源：http://fy.shtwfgs.cn

$double = fn($x) => $x * 2;
来源：http://cn.jctech888.com.cn

[U53] PHP：空合并运算符
来源：http://wg.jianghongdianzi.cn

$v = $a ?? $b ?? "default";
来源：http://fd.jianghongdianzi.cn

[U54] PHP：空安全调用
来源：http://wl.muxihuayi.cn

$obj?->method()
来源：http://xr.muxihuayi.cn

[U55] PHP：match 表达式
来源：http://ib.gzmigu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ni.jianghongdianzi.cn

[U56] PHP：命名参数
来源：http://fi.nszjky.cn

f(a: 1, b: 2)
来源：http://up.chemitech.net.cn

[U57] PHP：字符串插值
来源：http://ls.wgjwhj.cn

"值: {$a}"
来源：http://qq.chemitech.net.cn

[U58] PHP：数组三件套
来源：http://cf.huanxung.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ou.nszjky.cn

[U59] PHP：自定义排序
来源：http://mk.bookmarksfly.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zq.hnjuh.cn

[U60] PHP：JSON 编解码
来源：http://pv.lnxyls.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://de.lnxyls.cn

[U61] PHP：正则
来源：http://lw.jianghongdianzi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nz.yuntaijiaju.cn

[U62] PHP：日期对象
来源：http://sb.haigaiapp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ka.colortex.cn

[U63] PHP：文件读写
来源：http://yo.shxzukj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cn.szxytkj.cn

[U64] PHP：目录遍历
来源：http://gu.jctech888.com.cn

glob("dir/*.php");  scandir("dir");
来源：http://tp.521024.cn

[U65] PHP：会话
来源：http://qt.bjjhwx.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ne.panjiajie.cn

[U66] PHP：设置 Cookie
来源：http://xp.nszjky.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dv.jctech888.com.cn

[U67] PHP：处理文件上传
来源：http://cw.gzmigu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rd.wgjwhj.cn

[U68] PHP：PDO 连接
来源：http://ub.wgjwhj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ut.haigaiapp.cn

[U69] PHP：PDO 预处理
来源：http://rd.hahajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mk.asd995.cn

[U70] PHP：PDO 事务
来源：http://tv.9csxet.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mo.jianghongdianzi.cn

[U71] PHP：抛出异常
来源：http://sy.wgjwhj.cn

throw new RuntimeException("失败", 500);
来源：http://no.hahajie.cn

[U72] PHP：写错误日志
来源：http://kx.yuntaijiaju.cn

error_log("失败: " . $e->getMessage());
来源：http://bg.huixiangedu.cn

[U73] PHP：读取 ini 配置
来源：http://zj.521024.cn

parse_ini_file("config.ini", true)
来源：http://iz.jctech888.com.cn

[U74] PHP：读取环境变量
来源：http://ah.gzmigu.cn

getenv("APP_ENV") ?: "production"
来源：http://ol.lnxyls.cn

[U75] PHP：依赖注入
来源：http://jt.asd995.cn

composer require psr/container
来源：http://gl.panjiajie.cn

[U76] PHP：简单路由
来源：http://zx.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ys.asd995.cn

[U77] PHP：模板渲染
来源：http://rs.newstarts.cn

composer require twig/twig
来源：http://jn.shxzskj.cn

[U78] PHP：单元测试
来源：http://hm.yuexingan06.cn

composer require --dev phpunit/phpunit
来源：http://yg.gzmigu.cn

[U79] PHP：静态分析
来源：http://cj.hahajie.cn

composer require --dev phpstan/phpstan
来源：http://wd.521024.cn

[U80] PHP：代码规范修复
来源：http://oz.huixiangedu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://og.asd995.cn

[U81] JS：初始化项目
来源：http://ki.muxihuayi.cn

npm init -y;  npm i express
来源：http://ul.nszjky.cn

[U82] JS：package.json 脚本
来源：http://yr.chemitech.net.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zi.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://bh.hahajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://oy.nszjky.cn

[U84] JS：CommonJS 写法
来源：http://se.hnjuh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zq.nicolike.cn

[U85] JS：可选链
来源：http://xt.huanxung.cn

a?.b?.c
来源：http://ce.wgjwhj.cn

[U86] JS：空值合并
来源：http://bc.nszjky.cn

a ?? b
来源：http://rr.wgjwhj.cn

[U87] JS：解构默认值
来源：http://fi.yuntaijiaju.cn

const { a = 1, b = 2 } = obj;
来源：http://zh.lnxyls.cn

[U88] JS：对象展开合并
来源：http://yo.gzmigu.cn

{ ...a, ...b }
来源：http://xw.hnjuh.cn

[U89] JS：数组去重
来源：http://yt.shxzskj.cn

[...new Set(arr)]
来源：http://qn.huixiangedu.cn

[U90] JS：数字数组排序
来源：http://ha.shxzukj.cn

[...arr].sort((a, b) => a - b)
来源：http://ca.bookmarksfly.cn

[U91] JS：对象键值遍历
来源：http://of.nszjky.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lt.bookmarksfly.cn

[U92] JS：深拷贝
来源：http://ep.chemitech.net.cn

structuredClone(obj)
来源：http://hx.chemitech.net.cn

[U93] JS：模板字符串
来源：http://db.muxihuayi.cn

`共 ${n} 条`
来源：http://je.gzmigu.cn

[U94] JS：箭头函数
来源：http://lh.chemitech.net.cn

const double = x => x * 2;
来源：http://gi.wgjwhj.cn

[U95] JS：Promise 包装
来源：http://ze.panjiajie.cn

new Promise((resolve, reject) => {})
来源：http://su.hnjuh.cn

[U96] JS：async/await 与异常
来源：http://tx.huixinmuqiang.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sk.huixiangedu.cn

[U97] JS：并发请求
来源：http://yq.jianghongdianzi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://wn.newstarts.cn

[U98] JS：fetch 带 JSON
来源：http://rh.szxytkj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bm.panjiajie.cn

[U99] JS：事件监听
来源：http://pi.huixinmuqiang.cn

el.addEventListener("click", e => {})
来源：http://ou.lnxyls.cn

[U100] JS：DOM 查询
来源：http://yd.hnjuh.cn

document.querySelector(".item")
来源：http://cs.shtwfgs.cn

[U101] JS：classList 操作
来源：http://vw.gzmigu.cn

el.classList.toggle("active")
来源：http://mh.nicolike.cn

[U102] JS：本地存储
来源：http://gn.yuexingan06.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ie.bjjhwx.cn

[U103] JS：定时器
来源：http://eq.huixinmuqiang.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hd.huixiangedu.cn

[U104] JS：防抖
来源：http://dq.bookmarksfly.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://td.hahajie.cn

[U105] JS：节流
来源：http://iq.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ak.shxzukj.cn

[U106] JS：日期格式化
来源：http://sk.hahajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vm.shxzskj.cn

[U107] JS：数字千分位
来源：http://if.shxzukj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ze.shtwfgs.cn

[U108] JS：随机整数
来源：http://rx.lnxyls.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mv.huanxung.cn

[U109] JS：数组分组
来源：http://ie.shtwfgs.cn

Object.groupBy(arr, x => x.type)
来源：http://ze.haigaiapp.cn

[U110] JS：数组分块
来源：http://zg.szxytkj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nc.yuexingan06.cn

[U111] JS：对象转 Map
来源：http://jg.nszjky.cn

new Map(Object.entries(obj))
来源：http://yj.shtwfgs.cn

[U112] JS：字符串补位
来源：http://wg.yuexingan06.cn

"7".padStart(3, "0")
来源：http://qn.haigaiapp.cn

[U113] JS：正则替换全部
来源：http://et.hnjuh.cn

s.replaceAll("a", "b")
来源：http://bf.nicolike.cn

[U114] JS：JSON 深比较
来源：http://ja.bookmarksfly.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vg.nszjky.cn

[U115] JS：生成 UUID
来源：http://hk.nszjky.cn

crypto.randomUUID()
来源：http://pw.shtwfgs.cn

[U116] JS：类型检查（JSDoc）
来源：http://jz.gzmigu.cn

/** @param {string} name */ function f(name) {}
来源：http://yp.gzmigu.cn

[U117] JS：单元测试
来源：http://rt.lnxyls.cn

npm i -D vitest;  npx vitest
来源：http://kt.huixiangedu.cn

[U118] JS：开发服务器
来源：http://ai.newstarts.cn

npm i -D vite;  npx vite
来源：http://by.muxihuayi.cn

[U119] JS：生产构建
来源：http://tw.hnjuh.cn

npx vite build
来源：http://qe.hahajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://er.colortex.cn

import.meta.env.VITE_API_URL
来源：http://xi.haigaiapp.cn

================================================================================
来源：http://fj.panjiajie.cn

统计汇总
来源：http://xo.jctech888.com.cn

================================================================================
来源：http://yg.gzmigu.cn

按语言统计（条）：
来源：http://wz.yuntaijiaju.cn

Python ......... 252
来源：http://mt.muxihuayi.cn

PHP ............ 252
来源：http://ds.nszjky.cn

JavaScript ..... 252
来源：http://ln.jianghongdianzi.cn

TypeScript ..... 212
来源：http://sv.shtwfgs.cn

Java ........... 212
来源：http://sb.muxihuayi.cn

Go ............. 212
来源：http://dy.shxzukj.cn

Ruby ........... 212
来源：http://ml.huixinmuqiang.cn

C# ............. 212
来源：http://dz.shtwfgs.cn

C .............. 30
来源：http://mb.yuexingan06.cn

C++ ............ 30
来源：http://jr.9csxet.cn

SQL ............ 90
来源：http://vu.nicolike.cn

Bash ........... 80
来源：http://ad.9csxet.cn

Kotlin ......... 15
来源：http://yk.newstarts.cn

Swift .......... 15
来源：http://eg.hahajie.cn

Lua ............ 10
来源：http://sy.chemitech.net.cn

Perl ........... 10
来源：http://nv.colortex.cn

Scala .......... 10
来源：http://hw.jctech888.com.cn

------------------------------------
来源：http://ob.9csxet.cn

合计 ........... 2106 条
来源：http://dr.muxihuayi.cn

按章节统计：
来源：http://ww.nicolike.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mf.shxzskj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gt.huanxung.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lm.yuexingan06.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sn.asd995.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dy.huanxung.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://am.bjjhwx.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ng.shxzskj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://uh.bjjhwx.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ch.lnxyls.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://av.lnxyls.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hx.newstarts.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ed.521024.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ub.yuntaijiaju.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zc.shxzskj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vf.hnjuh.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://li.huixinmuqiang.cn

Q SQL 专题                              90
来源：http://qj.hahajie.cn

R Bash 专题                             80
来源：http://zb.9csxet.cn

S C / C++ 专题                          60
来源：http://yp.jctech888.com.cn

T 其他语言补充                          60
来源：http://ht.newstarts.cn

U 高频实用片段                         120
来源：http://ej.521024.cn

------------------------------------
来源：http://lk.szxytkj.cn

合计                                  2106 条
来源：http://dd.asd995.cn

--------------------------------------------------------------------------------
来源：http://oa.huixinmuqiang.cn

使用提醒
来源：http://mx.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://ji.wgjwhj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ws.nicolike.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vh.gzmigu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hd.huixiangedu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://en.lnxyls.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rc.huanxung.cn

—— 文件结束 ——
来源：http://ic.shxzukj.cn

================================================================================
来源：http://mp.chemitech.net.cn

程序语言常见例子速查手册（2024 版）
来源：http://jw.nicolike.cn

Common Programming Examples Cheat Book
来源：http://vv.hnjuh.cn

================================================================================
来源：http://gn.bjjhwx.cn

【收录内容】
来源：http://ys.haigaiapp.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vb.hahajie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xe.yuexingan06.cn

SQL · Bash · C · C++
来源：http://lc.521024.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://os.nicolike.cn

【使用说明】
来源：http://bd.muxihuayi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xy.lnxyls.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gu.jianghongdianzi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://im.gzmigu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fm.nszjky.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://nr.hnjuh.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xo.nszjky.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://le.haigaiapp.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hd.colortex.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mu.nicolike.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gi.hnjuh.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ru.panjiajie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dh.nszjky.cn

【文件统计】
来源：http://ey.colortex.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hw.nszjky.cn

--------------------------------------------------------------------------------
来源：http://nh.shxzskj.cn

目  录
来源：http://wx.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://ra.huixiangedu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hy.newstarts.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://im.huanxung.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dx.wgjwhj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jb.muxihuayi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yc.panjiajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://af.colortex.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://pm.jctech888.com.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://on.521024.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vg.lnxyls.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vw.bookmarksfly.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://eu.huixinmuqiang.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sj.muxihuayi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vn.jctech888.com.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dh.asd995.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jr.bookmarksfly.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gf.newstarts.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cx.lnxyls.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://df.521024.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gg.huixiangedu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ct.asd995.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://am.muxihuayi.cn

================================================================================
来源：http://yb.bjjhwx.cn

A. 基础语法与类型
来源：http://mm.jctech888.com.cn

================================================================================
来源：http://ni.nszjky.cn

[A01] Hello World
来源：http://bh.hnjuh.cn

Py:   print("Hello, World!")
来源：http://wd.huixiangedu.cn

PHP:  echo "Hello, World!";
来源：http://cp.jianghongdianzi.cn

JS:   console.log("Hello, World!");
来源：http://rk.shtwfgs.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ld.yuntaijiaju.cn

Java: System.out.println("Hello, World!");
来源：http://tq.bjjhwx.cn

Go:   fmt.Println("Hello, World!")
来源：http://fb.yuexingan06.cn

Ruby: puts "Hello, World!"
来源：http://qt.gzmigu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://yj.hahajie.cn

[A02] 变量声明与赋值
来源：http://ir.newstarts.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dp.asd995.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hi.9csxet.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xu.newstarts.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rg.nicolike.cn

Java: String name = "Alex"; int age = 20;
来源：http://wu.szsharing.cn

Go:   name := "Alex"; age := 20
来源：http://fr.colortex.cn

Ruby: name = "Alex"; age = 20
来源：http://la.gzmigu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://dw.huixinmuqiang.cn

[A03] 常量定义
来源：http://tl.haigaiapp.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bi.nszjky.cn

PHP:  const PI = 3.14159;
来源：http://yg.lnxyls.cn

JS:   const PI = 3.14159;
来源：http://py.bjjhwx.cn

TS:   const PI: number = 3.14159;
来源：http://mh.huixiangedu.cn

Java: static final double PI = 3.14159;
来源：http://qs.shxzukj.cn

Go:   const PI = 3.14159
来源：http://ba.asd995.cn


<!-- 参考信息 -->