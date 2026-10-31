代发 wailian999

[U43] PHP：声明命名空间
来源：http://ot.huanxung.cn

namespace App\Http;
来源：http://xk.nszjky.cn

[U44] PHP：开启严格类型
来源：http://oa.jctech888.com.cn

declare(strict_types=1);
来源：http://zr.nszjky.cn

[U45] PHP：类型声明与返回类型
来源：http://ex.colortex.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ca.wgjwhj.cn

[U46] PHP：可空类型
来源：http://dj.huixiangedu.cn

?string $name = null
来源：http://mi.shxzukj.cn

[U47] PHP：联合类型
来源：http://mr.huanxung.cn

int|string $id
来源：http://wm.521024.cn

[U48] PHP：纯枚举
来源：http://xp.chemitech.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://od.shxzukj.cn

[U49] PHP：只读属性
来源：http://yu.asd995.cn

public readonly string $name
来源：http://km.yuntaijiaju.cn

[U50] PHP：构造器属性提升
来源：http://ko.newstarts.cn

public function __construct(private int $id) {}
来源：http://cp.521024.cn

[U51] PHP：数组解构
来源：http://wr.panjiajie.cn

[$a, $b] = $arr;
来源：http://qz.colortex.cn

[U52] PHP：箭头函数
来源：http://qw.521024.cn

$double = fn($x) => $x * 2;
来源：http://vz.gzmigu.cn

[U53] PHP：空合并运算符
来源：http://kw.lnxyls.cn

$v = $a ?? $b ?? "default";
来源：http://rz.bookmarksfly.cn

[U54] PHP：空安全调用
来源：http://qx.bjjhwx.cn

$obj?->method()
来源：http://lz.bjjhwx.cn

[U55] PHP：match 表达式
来源：http://mj.hnjuh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nu.muxihuayi.cn

[U56] PHP：命名参数
来源：http://wc.nicolike.cn

f(a: 1, b: 2)
来源：http://xs.lnxyls.cn

[U57] PHP：字符串插值
来源：http://qs.szsharing.cn

"值: {$a}"
来源：http://pn.jctech888.com.cn

[U58] PHP：数组三件套
来源：http://cs.colortex.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sb.gzmigu.cn

[U59] PHP：自定义排序
来源：http://oq.szsharing.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bk.newstarts.cn

[U60] PHP：JSON 编解码
来源：http://xz.shxzskj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jo.shtwfgs.cn

[U61] PHP：正则
来源：http://ub.hnjuh.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ku.wgjwhj.cn

[U62] PHP：日期对象
来源：http://bj.shtwfgs.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fl.shtwfgs.cn

[U63] PHP：文件读写
来源：http://oq.asd995.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ue.hnjuh.cn

[U64] PHP：目录遍历
来源：http://id.huixiangedu.cn

glob("dir/*.php");  scandir("dir");
来源：http://fj.asd995.cn

[U65] PHP：会话
来源：http://fo.jianghongdianzi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zi.asd995.cn

[U66] PHP：设置 Cookie
来源：http://rk.muxihuayi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qe.shxzskj.cn

[U67] PHP：处理文件上传
来源：http://op.shxzukj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ee.muxihuayi.cn

[U68] PHP：PDO 连接
来源：http://zy.nszjky.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ll.muxihuayi.cn

[U69] PHP：PDO 预处理
来源：http://kt.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xl.huixinmuqiang.cn

[U70] PHP：PDO 事务
来源：http://pa.newstarts.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sk.panjiajie.cn

[U71] PHP：抛出异常
来源：http://mp.jianghongdianzi.cn

throw new RuntimeException("失败", 500);
来源：http://pi.asd995.cn

[U72] PHP：写错误日志
来源：http://rb.yuntaijiaju.cn

error_log("失败: " . $e->getMessage());
来源：http://uk.colortex.cn

[U73] PHP：读取 ini 配置
来源：http://sl.muxihuayi.cn

parse_ini_file("config.ini", true)
来源：http://ao.nicolike.cn

[U74] PHP：读取环境变量
来源：http://px.lnxyls.cn

getenv("APP_ENV") ?: "production"
来源：http://yt.lnxyls.cn

[U75] PHP：依赖注入
来源：http://to.bjjhwx.cn

composer require psr/container
来源：http://mz.shxzskj.cn

[U76] PHP：简单路由
来源：http://vd.yuexingan06.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ru.haigaiapp.cn

[U77] PHP：模板渲染
来源：http://lh.bookmarksfly.cn

composer require twig/twig
来源：http://pz.asd995.cn

[U78] PHP：单元测试
来源：http://he.gzmigu.cn

composer require --dev phpunit/phpunit
来源：http://fb.colortex.cn

[U79] PHP：静态分析
来源：http://vz.asd995.cn

composer require --dev phpstan/phpstan
来源：http://qh.muxihuayi.cn

[U80] PHP：代码规范修复
来源：http://wr.521024.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kt.huanxung.cn

[U81] JS：初始化项目
来源：http://as.huixiangedu.cn

npm init -y;  npm i express
来源：http://jd.wgjwhj.cn

[U82] JS：package.json 脚本
来源：http://xl.huanxung.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cz.jianghongdianzi.cn

[U83] JS：ES Module 导入导出
来源：http://hj.yuexingan06.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vk.bookmarksfly.cn

[U84] JS：CommonJS 写法
来源：http://tp.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xq.asd995.cn

[U85] JS：可选链
来源：http://bq.wgjwhj.cn

a?.b?.c
来源：http://rw.colortex.cn

[U86] JS：空值合并
来源：http://ma.wgjwhj.cn

a ?? b
来源：http://ls.szxytkj.cn

[U87] JS：解构默认值
来源：http://uy.szxytkj.cn

const { a = 1, b = 2 } = obj;
来源：http://ss.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://wj.nicolike.cn

{ ...a, ...b }
来源：http://xs.haigaiapp.cn

[U89] JS：数组去重
来源：http://ks.huanxung.cn

[...new Set(arr)]
来源：http://wg.colortex.cn

[U90] JS：数字数组排序
来源：http://eg.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://lt.szxytkj.cn

[U91] JS：对象键值遍历
来源：http://dm.bookmarksfly.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sw.panjiajie.cn

[U92] JS：深拷贝
来源：http://it.huanxung.cn

structuredClone(obj)
来源：http://of.szsharing.cn

[U93] JS：模板字符串
来源：http://ts.asd995.cn

`共 ${n} 条`
来源：http://zg.muxihuayi.cn

[U94] JS：箭头函数
来源：http://xh.newstarts.cn

const double = x => x * 2;
来源：http://bl.wgjwhj.cn

[U95] JS：Promise 包装
来源：http://tv.gzmigu.cn

new Promise((resolve, reject) => {})
来源：http://zj.haigaiapp.cn

[U96] JS：async/await 与异常
来源：http://ib.shxzukj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cg.bookmarksfly.cn

[U97] JS：并发请求
来源：http://gt.yuntaijiaju.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://uz.shxzskj.cn

[U98] JS：fetch 带 JSON
来源：http://pd.muxihuayi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zg.szsharing.cn

[U99] JS：事件监听
来源：http://zv.bookmarksfly.cn

el.addEventListener("click", e => {})
来源：http://im.shxzskj.cn

[U100] JS：DOM 查询
来源：http://cz.jianghongdianzi.cn

document.querySelector(".item")
来源：http://yt.huixiangedu.cn

[U101] JS：classList 操作
来源：http://hs.bookmarksfly.cn

el.classList.toggle("active")
来源：http://mq.shxzukj.cn

[U102] JS：本地存储
来源：http://mt.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bo.bjjhwx.cn

[U103] JS：定时器
来源：http://xp.szxytkj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qk.asd995.cn

[U104] JS：防抖
来源：http://jp.shtwfgs.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ry.hnjuh.cn

[U105] JS：节流
来源：http://gk.shtwfgs.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mv.gzmigu.cn

[U106] JS：日期格式化
来源：http://qy.haigaiapp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://my.szxytkj.cn

[U107] JS：数字千分位
来源：http://yj.shtwfgs.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://va.gzmigu.cn

[U108] JS：随机整数
来源：http://yw.chemitech.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ro.bjjhwx.cn

[U109] JS：数组分组
来源：http://wq.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://ed.shxzukj.cn

[U110] JS：数组分块
来源：http://wx.huixiangedu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lu.muxihuayi.cn

[U111] JS：对象转 Map
来源：http://wd.muxihuayi.cn

new Map(Object.entries(obj))
来源：http://vi.lnxyls.cn

[U112] JS：字符串补位
来源：http://yt.shxzskj.cn

"7".padStart(3, "0")
来源：http://xg.shxzskj.cn

[U113] JS：正则替换全部
来源：http://af.yuexingan06.cn

s.replaceAll("a", "b")
来源：http://qs.huixinmuqiang.cn

[U114] JS：JSON 深比较
来源：http://lk.521024.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jv.muxihuayi.cn

[U115] JS：生成 UUID
来源：http://wj.huanxung.cn

crypto.randomUUID()
来源：http://km.jctech888.com.cn

[U116] JS：类型检查（JSDoc）
来源：http://ni.huanxung.cn

/** @param {string} name */ function f(name) {}
来源：http://ko.szxytkj.cn

[U117] JS：单元测试
来源：http://fv.huanxung.cn

npm i -D vitest;  npx vitest
来源：http://bn.nszjky.cn

[U118] JS：开发服务器
来源：http://eo.shxzskj.cn

npm i -D vite;  npx vite
来源：http://zb.muxihuayi.cn

[U119] JS：生产构建
来源：http://wy.szxytkj.cn

npx vite build
来源：http://yn.asd995.cn

[U120] JS：读取环境变量（Vite）
来源：http://yn.jianghongdianzi.cn

import.meta.env.VITE_API_URL
来源：http://ls.szxytkj.cn

================================================================================
来源：http://pp.yuexingan06.cn

统计汇总
来源：http://ua.shxzskj.cn

================================================================================
来源：http://qo.jianghongdianzi.cn

按语言统计（条）：
来源：http://wd.jctech888.com.cn

Python ......... 252
来源：http://rc.bookmarksfly.cn

PHP ............ 252
来源：http://bn.yuntaijiaju.cn

JavaScript ..... 252
来源：http://dx.szsharing.cn

TypeScript ..... 212
来源：http://me.nicolike.cn

Java ........... 212
来源：http://lo.shtwfgs.cn

Go ............. 212
来源：http://zi.nszjky.cn

Ruby ........... 212
来源：http://fz.chemitech.net.cn

C# ............. 212
来源：http://lk.chemitech.net.cn

C .............. 30
来源：http://om.chemitech.net.cn

C++ ............ 30
来源：http://fj.asd995.cn

SQL ............ 90
来源：http://uf.shtwfgs.cn

Bash ........... 80
来源：http://yk.szxytkj.cn

Kotlin ......... 15
来源：http://pv.521024.cn

Swift .......... 15
来源：http://gh.shxzskj.cn

Lua ............ 10
来源：http://rb.wgjwhj.cn

Perl ........... 10
来源：http://vw.bjjhwx.cn

Scala .......... 10
来源：http://sx.jctech888.com.cn

------------------------------------
来源：http://uz.521024.cn

合计 ........... 2106 条
来源：http://so.gzmigu.cn

按章节统计：
来源：http://qb.9csxet.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ky.lnxyls.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nu.colortex.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pd.shxzukj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vg.yuexingan06.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vu.shtwfgs.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ys.nicolike.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ov.newstarts.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ic.lnxyls.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fo.asd995.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jb.bookmarksfly.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hh.bjjhwx.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ro.newstarts.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zx.shxzskj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qr.hahajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://be.chemitech.net.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://oq.newstarts.cn

Q SQL 专题                              90
来源：http://lm.yuexingan06.cn

R Bash 专题                             80
来源：http://nu.huanxung.cn

S C / C++ 专题                          60
来源：http://au.jianghongdianzi.cn

T 其他语言补充                          60
来源：http://ms.wgjwhj.cn

U 高频实用片段                         120
来源：http://oa.huixinmuqiang.cn

------------------------------------
来源：http://hf.nicolike.cn

合计                                  2106 条
来源：http://zk.521024.cn

--------------------------------------------------------------------------------
来源：http://hz.muxihuayi.cn

使用提醒
来源：http://lm.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://ff.nicolike.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vh.shtwfgs.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ri.lnxyls.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yc.muxihuayi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://pc.colortex.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qm.haigaiapp.cn

—— 文件结束 ——
来源：http://yy.colortex.cn

================================================================================
来源：http://xn.shtwfgs.cn

程序语言常见例子速查手册（2024 版）
来源：http://qp.huanxung.cn

Common Programming Examples Cheat Book
来源：http://lp.nszjky.cn

================================================================================
来源：http://mr.wgjwhj.cn

【收录内容】
来源：http://bp.hahajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://pj.asd995.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ns.gzmigu.cn

SQL · Bash · C · C++
来源：http://pc.jianghongdianzi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ax.9csxet.cn

【使用说明】
来源：http://ji.gzmigu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pm.nszjky.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zd.gzmigu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://am.yuexingan06.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rq.nicolike.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://hw.newstarts.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dz.hahajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tf.yuntaijiaju.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tk.huixinmuqiang.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fb.haigaiapp.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mi.nicolike.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://oo.panjiajie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xc.wgjwhj.cn

【文件统计】
来源：http://oa.chemitech.net.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mz.szsharing.cn

--------------------------------------------------------------------------------
来源：http://cz.asd995.cn

目  录
来源：http://zt.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://lz.yuntaijiaju.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ji.chemitech.net.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ua.muxihuayi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pn.muxihuayi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ba.shxzskj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://sw.jctech888.com.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vs.wgjwhj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ka.9csxet.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vt.nszjky.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nk.shxzukj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fe.nicolike.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ye.newstarts.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://be.szxytkj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ea.hahajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zm.wgjwhj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pp.gzmigu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://po.wgjwhj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fj.gzmigu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://rl.gzmigu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fv.yuntaijiaju.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pd.shxzukj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hc.yuexingan06.cn

================================================================================
来源：http://wu.jianghongdianzi.cn

A. 基础语法与类型
来源：http://br.hahajie.cn

================================================================================
来源：http://ya.asd995.cn

[A01] Hello World
来源：http://tw.nicolike.cn

Py:   print("Hello, World!")
来源：http://oa.lnxyls.cn

PHP:  echo "Hello, World!";
来源：http://mb.szsharing.cn

JS:   console.log("Hello, World!");
来源：http://je.yuntaijiaju.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ty.bjjhwx.cn

Java: System.out.println("Hello, World!");
来源：http://kl.panjiajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://ep.chemitech.net.cn

Ruby: puts "Hello, World!"
来源：http://ad.jctech888.com.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://qc.hnjuh.cn

[A02] 变量声明与赋值
来源：http://jl.huixinmuqiang.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ra.panjiajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://zw.jianghongdianzi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://eh.yuexingan06.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yv.lnxyls.cn

Java: String name = "Alex"; int age = 20;
来源：http://lx.shtwfgs.cn

Go:   name := "Alex"; age := 20
来源：http://ov.asd995.cn

Ruby: name = "Alex"; age = 20
来源：http://zf.chemitech.net.cn

C#:   string name = "Alex"; int age = 20;
来源：http://yq.wgjwhj.cn

[A03] 常量定义
来源：http://av.9csxet.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ao.jctech888.com.cn

PHP:  const PI = 3.14159;
来源：http://bj.panjiajie.cn

JS:   const PI = 3.14159;
来源：http://iq.shxzukj.cn

TS:   const PI: number = 3.14159;
来源：http://rs.bookmarksfly.cn

Java: static final double PI = 3.14159;
来源：http://ev.szsharing.cn

Go:   const PI = 3.14159
来源：http://br.gzmigu.cn

Ruby: PI = 3.14159
来源：http://im.yuexingan06.cn

C#:   const double PI = 3.14159;
来源：http://ax.shxzskj.cn

[A04] 判断变量类型
来源：http://yx.bjjhwx.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://aj.huixiangedu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://as.gzmigu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yj.shxzukj.cn

TS:   typeof x; x instanceof Date
来源：http://vr.newstarts.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ak.yuntaijiaju.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ls.wgjwhj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://go.shtwfgs.cn

C#:   x.GetType().Name; x is int
来源：http://se.chemitech.net.cn

[A05] 整数除法与取模
来源：http://qs.muxihuayi.cn


<!-- 参考信息 -->