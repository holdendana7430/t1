代发 wailian999

[U43] PHP：声明命名空间
来源：http://ru.huixiangedu.cn

namespace App\Http;
来源：http://tb.shxzskj.cn

[U44] PHP：开启严格类型
来源：http://tw.chemitech.net.cn

declare(strict_types=1);
来源：http://dn.szsharing.cn

[U45] PHP：类型声明与返回类型
来源：http://lh.gzmigu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://nq.huixinmuqiang.cn

[U46] PHP：可空类型
来源：http://rf.huixinmuqiang.cn

?string $name = null
来源：http://ck.jctech888.com.cn

[U47] PHP：联合类型
来源：http://or.yuntaijiaju.cn

int|string $id
来源：http://xa.nicolike.cn

[U48] PHP：纯枚举
来源：http://kk.9csxet.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hd.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://ir.nicolike.cn

public readonly string $name
来源：http://si.bookmarksfly.cn

[U50] PHP：构造器属性提升
来源：http://su.lnxyls.cn

public function __construct(private int $id) {}
来源：http://sc.newstarts.cn

[U51] PHP：数组解构
来源：http://jk.muxihuayi.cn

[$a, $b] = $arr;
来源：http://jq.huixiangedu.cn

[U52] PHP：箭头函数
来源：http://lm.wgjwhj.cn

$double = fn($x) => $x * 2;
来源：http://gi.muxihuayi.cn

[U53] PHP：空合并运算符
来源：http://yi.shxzskj.cn

$v = $a ?? $b ?? "default";
来源：http://lj.nszjky.cn

[U54] PHP：空安全调用
来源：http://sc.jctech888.com.cn

$obj?->method()
来源：http://nd.haigaiapp.cn

[U55] PHP：match 表达式
来源：http://lg.lnxyls.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jd.jianghongdianzi.cn

[U56] PHP：命名参数
来源：http://pu.9csxet.cn

f(a: 1, b: 2)
来源：http://hc.yuexingan06.cn

[U57] PHP：字符串插值
来源：http://ye.jctech888.com.cn

"值: {$a}"
来源：http://tu.nicolike.cn

[U58] PHP：数组三件套
来源：http://vj.bjjhwx.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yc.nicolike.cn

[U59] PHP：自定义排序
来源：http://mb.panjiajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bk.huanxung.cn

[U60] PHP：JSON 编解码
来源：http://xg.newstarts.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tn.yuexingan06.cn

[U61] PHP：正则
来源：http://rv.wgjwhj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ip.bookmarksfly.cn

[U62] PHP：日期对象
来源：http://ga.huanxung.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uy.szxytkj.cn

[U63] PHP：文件读写
来源：http://da.wgjwhj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fp.yuexingan06.cn

[U64] PHP：目录遍历
来源：http://xt.jctech888.com.cn

glob("dir/*.php");  scandir("dir");
来源：http://dx.huanxung.cn

[U65] PHP：会话
来源：http://mx.shxzskj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bs.shtwfgs.cn

[U66] PHP：设置 Cookie
来源：http://lu.colortex.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xt.huanxung.cn

[U67] PHP：处理文件上传
来源：http://gt.shtwfgs.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kl.lnxyls.cn

[U68] PHP：PDO 连接
来源：http://qt.gzmigu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cm.gzmigu.cn

[U69] PHP：PDO 预处理
来源：http://tt.szsharing.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://om.yuexingan06.cn

[U70] PHP：PDO 事务
来源：http://at.szxytkj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fk.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://cl.bookmarksfly.cn

throw new RuntimeException("失败", 500);
来源：http://dw.huanxung.cn

[U72] PHP：写错误日志
来源：http://uh.yuexingan06.cn

error_log("失败: " . $e->getMessage());
来源：http://iv.huixiangedu.cn

[U73] PHP：读取 ini 配置
来源：http://gv.panjiajie.cn

parse_ini_file("config.ini", true)
来源：http://dw.yuntaijiaju.cn

[U74] PHP：读取环境变量
来源：http://ib.shtwfgs.cn

getenv("APP_ENV") ?: "production"
来源：http://hp.nszjky.cn

[U75] PHP：依赖注入
来源：http://dx.nszjky.cn

composer require psr/container
来源：http://av.huanxung.cn

[U76] PHP：简单路由
来源：http://db.yuntaijiaju.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://av.hahajie.cn

[U77] PHP：模板渲染
来源：http://ur.asd995.cn

composer require twig/twig
来源：http://tv.asd995.cn

[U78] PHP：单元测试
来源：http://yk.chemitech.net.cn

composer require --dev phpunit/phpunit
来源：http://km.newstarts.cn

[U79] PHP：静态分析
来源：http://kw.asd995.cn

composer require --dev phpstan/phpstan
来源：http://tj.shxzskj.cn

[U80] PHP：代码规范修复
来源：http://wx.huixinmuqiang.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://se.yuntaijiaju.cn

[U81] JS：初始化项目
来源：http://kp.szsharing.cn

npm init -y;  npm i express
来源：http://cg.nszjky.cn

[U82] JS：package.json 脚本
来源：http://lg.shxzukj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mw.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://mj.bjjhwx.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fp.huanxung.cn

[U84] JS：CommonJS 写法
来源：http://gp.yuexingan06.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ks.gzmigu.cn

[U85] JS：可选链
来源：http://jf.huixiangedu.cn

a?.b?.c
来源：http://uf.newstarts.cn

[U86] JS：空值合并
来源：http://js.huanxung.cn

a ?? b
来源：http://ut.huanxung.cn

[U87] JS：解构默认值
来源：http://nc.hahajie.cn

const { a = 1, b = 2 } = obj;
来源：http://bj.wgjwhj.cn

[U88] JS：对象展开合并
来源：http://cj.huixinmuqiang.cn

{ ...a, ...b }
来源：http://py.huixinmuqiang.cn

[U89] JS：数组去重
来源：http://hf.hnjuh.cn

[...new Set(arr)]
来源：http://pe.gzmigu.cn

[U90] JS：数字数组排序
来源：http://pr.bookmarksfly.cn

[...arr].sort((a, b) => a - b)
来源：http://gd.jctech888.com.cn

[U91] JS：对象键值遍历
来源：http://cv.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wm.jctech888.com.cn

[U92] JS：深拷贝
来源：http://pq.lnxyls.cn

structuredClone(obj)
来源：http://jk.shxzukj.cn

[U93] JS：模板字符串
来源：http://ev.lnxyls.cn

`共 ${n} 条`
来源：http://gw.jctech888.com.cn

[U94] JS：箭头函数
来源：http://iu.huixinmuqiang.cn

const double = x => x * 2;
来源：http://eq.yuntaijiaju.cn

[U95] JS：Promise 包装
来源：http://rg.bookmarksfly.cn

new Promise((resolve, reject) => {})
来源：http://jy.hahajie.cn

[U96] JS：async/await 与异常
来源：http://lk.yuexingan06.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://iu.hnjuh.cn

[U97] JS：并发请求
来源：http://zh.shtwfgs.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://gm.nicolike.cn

[U98] JS：fetch 带 JSON
来源：http://jz.hahajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nr.nszjky.cn

[U99] JS：事件监听
来源：http://vs.bjjhwx.cn

el.addEventListener("click", e => {})
来源：http://sw.9csxet.cn

[U100] JS：DOM 查询
来源：http://um.huixiangedu.cn

document.querySelector(".item")
来源：http://ak.shxzskj.cn

[U101] JS：classList 操作
来源：http://hv.nszjky.cn

el.classList.toggle("active")
来源：http://gp.shtwfgs.cn

[U102] JS：本地存储
来源：http://od.huixiangedu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xl.shxzukj.cn

[U103] JS：定时器
来源：http://am.jctech888.com.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xf.haigaiapp.cn

[U104] JS：防抖
来源：http://qi.wgjwhj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ex.9csxet.cn

[U105] JS：节流
来源：http://zt.huixiangedu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ri.asd995.cn

[U106] JS：日期格式化
来源：http://dm.yuntaijiaju.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://is.haigaiapp.cn

[U107] JS：数字千分位
来源：http://jf.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mm.huanxung.cn

[U108] JS：随机整数
来源：http://jf.szsharing.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vj.huixiangedu.cn

[U109] JS：数组分组
来源：http://yk.shxzukj.cn

Object.groupBy(arr, x => x.type)
来源：http://hm.szsharing.cn

[U110] JS：数组分块
来源：http://cx.shxzskj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mu.jianghongdianzi.cn

[U111] JS：对象转 Map
来源：http://pt.bjjhwx.cn

new Map(Object.entries(obj))
来源：http://lo.szxytkj.cn

[U112] JS：字符串补位
来源：http://zz.hahajie.cn

"7".padStart(3, "0")
来源：http://vi.newstarts.cn

[U113] JS：正则替换全部
来源：http://ih.szxytkj.cn

s.replaceAll("a", "b")
来源：http://ls.szsharing.cn

[U114] JS：JSON 深比较
来源：http://yl.gzmigu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rq.shtwfgs.cn

[U115] JS：生成 UUID
来源：http://ts.haigaiapp.cn

crypto.randomUUID()
来源：http://ls.yuntaijiaju.cn

[U116] JS：类型检查（JSDoc）
来源：http://kq.szxytkj.cn

/** @param {string} name */ function f(name) {}
来源：http://gl.colortex.cn

[U117] JS：单元测试
来源：http://vp.shxzukj.cn

npm i -D vitest;  npx vitest
来源：http://ke.9csxet.cn

[U118] JS：开发服务器
来源：http://uo.jctech888.com.cn

npm i -D vite;  npx vite
来源：http://af.gzmigu.cn

[U119] JS：生产构建
来源：http://gf.hnjuh.cn

npx vite build
来源：http://pd.newstarts.cn

[U120] JS：读取环境变量（Vite）
来源：http://jg.szsharing.cn

import.meta.env.VITE_API_URL
来源：http://ue.521024.cn

================================================================================
来源：http://mv.9csxet.cn

统计汇总
来源：http://yz.shtwfgs.cn

================================================================================
来源：http://xr.huixinmuqiang.cn

按语言统计（条）：
来源：http://ls.shtwfgs.cn

Python ......... 252
来源：http://ud.colortex.cn

PHP ............ 252
来源：http://ha.gzmigu.cn

JavaScript ..... 252
来源：http://ey.yuntaijiaju.cn

TypeScript ..... 212
来源：http://hm.nszjky.cn

Java ........... 212
来源：http://up.bjjhwx.cn

Go ............. 212
来源：http://bv.hahajie.cn

Ruby ........... 212
来源：http://kb.panjiajie.cn

C# ............. 212
来源：http://ph.shxzskj.cn

C .............. 30
来源：http://pu.jctech888.com.cn

C++ ............ 30
来源：http://ea.shxzukj.cn

SQL ............ 90
来源：http://qp.szxytkj.cn

Bash ........... 80
来源：http://fo.gzmigu.cn

Kotlin ......... 15
来源：http://ho.shxzskj.cn

Swift .......... 15
来源：http://vk.521024.cn

Lua ............ 10
来源：http://ys.bookmarksfly.cn

Perl ........... 10
来源：http://ov.muxihuayi.cn

Scala .......... 10
来源：http://aj.huixiangedu.cn

------------------------------------
来源：http://qq.nszjky.cn

合计 ........... 2106 条
来源：http://vg.newstarts.cn

按章节统计：
来源：http://qe.bjjhwx.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wy.lnxyls.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lu.chemitech.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xp.lnxyls.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vs.chemitech.net.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yv.9csxet.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sb.shtwfgs.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qs.shxzskj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lf.huixiangedu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rp.gzmigu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vh.yuntaijiaju.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qn.jctech888.com.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nv.nicolike.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mk.huixinmuqiang.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hf.colortex.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rt.newstarts.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pc.nicolike.cn

Q SQL 专题                              90
来源：http://tn.nicolike.cn

R Bash 专题                             80
来源：http://oj.huixiangedu.cn

S C / C++ 专题                          60
来源：http://je.shtwfgs.cn

T 其他语言补充                          60
来源：http://zw.yuexingan06.cn

U 高频实用片段                         120
来源：http://sm.colortex.cn

------------------------------------
来源：http://oq.asd995.cn

合计                                  2106 条
来源：http://yw.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://dv.yuntaijiaju.cn

使用提醒
来源：http://et.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://oh.jianghongdianzi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ii.9csxet.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jf.haigaiapp.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hr.lnxyls.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zc.yuntaijiaju.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mo.yuntaijiaju.cn

—— 文件结束 ——
来源：http://ph.asd995.cn

================================================================================
来源：http://sb.chemitech.net.cn

程序语言常见例子速查手册（2024 版）
来源：http://dv.yuntaijiaju.cn

Common Programming Examples Cheat Book
来源：http://oy.shxzskj.cn

================================================================================
来源：http://uj.hnjuh.cn

【收录内容】
来源：http://fl.hnjuh.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vo.asd995.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ix.gzmigu.cn

SQL · Bash · C · C++
来源：http://bx.lnxyls.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xb.jianghongdianzi.cn

【使用说明】
来源：http://wk.asd995.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kx.nszjky.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bb.bjjhwx.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fd.szxytkj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://of.haigaiapp.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://dh.lnxyls.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kg.shxzukj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://iz.huixiangedu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lm.colortex.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cs.huixiangedu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bn.9csxet.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dx.521024.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qq.hahajie.cn

【文件统计】
来源：http://op.newstarts.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dy.newstarts.cn

--------------------------------------------------------------------------------
来源：http://nu.9csxet.cn

目  录
来源：http://pe.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://mo.shxzukj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hb.shxzukj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gt.yuntaijiaju.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sd.haigaiapp.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mf.yuexingan06.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jl.shxzukj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jl.wgjwhj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mm.huanxung.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ms.huixiangedu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ly.lnxyls.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vb.haigaiapp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tt.szsharing.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://og.szxytkj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yo.asd995.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nd.shxzukj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dc.shxzukj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ql.wgjwhj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://se.shxzukj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ip.jctech888.com.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sx.yuexingan06.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://sm.bookmarksfly.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://sk.gzmigu.cn

================================================================================
来源：http://zr.bjjhwx.cn

A. 基础语法与类型
来源：http://uz.nszjky.cn

================================================================================
来源：http://aj.lnxyls.cn

[A01] Hello World
来源：http://bh.shtwfgs.cn

Py:   print("Hello, World!")
来源：http://fb.huanxung.cn

PHP:  echo "Hello, World!";
来源：http://fr.521024.cn

JS:   console.log("Hello, World!");
来源：http://dl.shxzukj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://uo.muxihuayi.cn

Java: System.out.println("Hello, World!");
来源：http://an.shtwfgs.cn

Go:   fmt.Println("Hello, World!")
来源：http://kh.huixiangedu.cn

Ruby: puts "Hello, World!"
来源：http://xm.nicolike.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://od.bjjhwx.cn

[A02] 变量声明与赋值
来源：http://dm.nszjky.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zj.huixiangedu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ac.nicolike.cn

JS:   let name = "Alex"; const age = 20;
来源：http://jl.huixinmuqiang.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yc.nicolike.cn

Java: String name = "Alex"; int age = 20;
来源：http://lo.gzmigu.cn

Go:   name := "Alex"; age := 20
来源：http://lr.jctech888.com.cn

Ruby: name = "Alex"; age = 20
来源：http://dm.521024.cn

C#:   string name = "Alex"; int age = 20;
来源：http://pe.521024.cn

[A03] 常量定义
来源：http://vu.szxytkj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vq.wgjwhj.cn

PHP:  const PI = 3.14159;
来源：http://zb.9csxet.cn

JS:   const PI = 3.14159;
来源：http://xu.yuexingan06.cn

TS:   const PI: number = 3.14159;
来源：http://ry.hnjuh.cn

Java: static final double PI = 3.14159;
来源：http://qi.wgjwhj.cn

Go:   const PI = 3.14159
来源：http://iv.huixiangedu.cn

Ruby: PI = 3.14159
来源：http://ay.huixinmuqiang.cn

C#:   const double PI = 3.14159;
来源：http://lq.huanxung.cn

[A04] 判断变量类型
来源：http://tc.panjiajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cp.huixinmuqiang.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qj.huixinmuqiang.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://va.9csxet.cn

TS:   typeof x; x instanceof Date
来源：http://fx.shtwfgs.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jz.shtwfgs.cn

Go:   reflect.TypeOf(x).Name()
来源：http://yj.hahajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://sk.nszjky.cn

C#:   x.GetType().Name; x is int
来源：http://du.shxzukj.cn

[A05] 整数除法与取模
来源：http://pb.9csxet.cn


<!-- 参考信息 -->