代发 wailian999

[U43] PHP：声明命名空间
来源：http://uo.bjjhwx.cn

namespace App\Http;
来源：http://fs.szsharing.cn

[U44] PHP：开启严格类型
来源：http://on.nicolike.cn

declare(strict_types=1);
来源：http://yf.shtwfgs.cn

[U45] PHP：类型声明与返回类型
来源：http://ss.shtwfgs.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://nz.bookmarksfly.cn

[U46] PHP：可空类型
来源：http://ix.huixinmuqiang.cn

?string $name = null
来源：http://bm.521024.cn

[U47] PHP：联合类型
来源：http://aq.szsharing.cn

int|string $id
来源：http://fd.szsharing.cn

[U48] PHP：纯枚举
来源：http://ib.hahajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vv.huixiangedu.cn

[U49] PHP：只读属性
来源：http://ms.9csxet.cn

public readonly string $name
来源：http://ll.colortex.cn

[U50] PHP：构造器属性提升
来源：http://vr.panjiajie.cn

public function __construct(private int $id) {}
来源：http://wb.jianghongdianzi.cn

[U51] PHP：数组解构
来源：http://fa.colortex.cn

[$a, $b] = $arr;
来源：http://hz.9csxet.cn

[U52] PHP：箭头函数
来源：http://np.shxzskj.cn

$double = fn($x) => $x * 2;
来源：http://vl.wgjwhj.cn

[U53] PHP：空合并运算符
来源：http://sn.nicolike.cn

$v = $a ?? $b ?? "default";
来源：http://gr.hnjuh.cn

[U54] PHP：空安全调用
来源：http://tv.shxzukj.cn

$obj?->method()
来源：http://zc.panjiajie.cn

[U55] PHP：match 表达式
来源：http://tu.huixinmuqiang.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bt.lnxyls.cn

[U56] PHP：命名参数
来源：http://vp.9csxet.cn

f(a: 1, b: 2)
来源：http://ir.hnjuh.cn

[U57] PHP：字符串插值
来源：http://kr.nszjky.cn

"值: {$a}"
来源：http://xq.colortex.cn

[U58] PHP：数组三件套
来源：http://yj.521024.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jr.asd995.cn

[U59] PHP：自定义排序
来源：http://ux.shtwfgs.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qp.bjjhwx.cn

[U60] PHP：JSON 编解码
来源：http://bw.wgjwhj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gc.huanxung.cn

[U61] PHP：正则
来源：http://ex.wgjwhj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://de.521024.cn

[U62] PHP：日期对象
来源：http://el.lnxyls.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ae.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://mc.newstarts.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ji.lnxyls.cn

[U64] PHP：目录遍历
来源：http://pa.shxzskj.cn

glob("dir/*.php");  scandir("dir");
来源：http://uy.newstarts.cn

[U65] PHP：会话
来源：http://fw.haigaiapp.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sc.shtwfgs.cn

[U66] PHP：设置 Cookie
来源：http://vs.shxzukj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pb.9csxet.cn

[U67] PHP：处理文件上传
来源：http://vj.huanxung.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bm.bookmarksfly.cn

[U68] PHP：PDO 连接
来源：http://yj.shtwfgs.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nx.szxytkj.cn

[U69] PHP：PDO 预处理
来源：http://fa.shxzskj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gp.shxzskj.cn

[U70] PHP：PDO 事务
来源：http://aa.szsharing.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://da.nszjky.cn

[U71] PHP：抛出异常
来源：http://yk.nszjky.cn

throw new RuntimeException("失败", 500);
来源：http://qc.gzmigu.cn

[U72] PHP：写错误日志
来源：http://zo.shxzskj.cn

error_log("失败: " . $e->getMessage());
来源：http://he.521024.cn

[U73] PHP：读取 ini 配置
来源：http://zl.colortex.cn

parse_ini_file("config.ini", true)
来源：http://yw.shxzukj.cn

[U74] PHP：读取环境变量
来源：http://ts.szxytkj.cn

getenv("APP_ENV") ?: "production"
来源：http://fk.521024.cn

[U75] PHP：依赖注入
来源：http://zm.bjjhwx.cn

composer require psr/container
来源：http://xf.huanxung.cn

[U76] PHP：简单路由
来源：http://pr.szsharing.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nv.9csxet.cn

[U77] PHP：模板渲染
来源：http://rk.bjjhwx.cn

composer require twig/twig
来源：http://yv.huanxung.cn

[U78] PHP：单元测试
来源：http://qh.bookmarksfly.cn

composer require --dev phpunit/phpunit
来源：http://az.colortex.cn

[U79] PHP：静态分析
来源：http://lq.nicolike.cn

composer require --dev phpstan/phpstan
来源：http://ga.colortex.cn

[U80] PHP：代码规范修复
来源：http://zo.lnxyls.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ud.shtwfgs.cn

[U81] JS：初始化项目
来源：http://fb.yuntaijiaju.cn

npm init -y;  npm i express
来源：http://uv.shxzskj.cn

[U82] JS：package.json 脚本
来源：http://bb.wgjwhj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nx.521024.cn

[U83] JS：ES Module 导入导出
来源：http://fz.huanxung.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tk.hahajie.cn

[U84] JS：CommonJS 写法
来源：http://jo.9csxet.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hl.panjiajie.cn

[U85] JS：可选链
来源：http://gl.gzmigu.cn

a?.b?.c
来源：http://th.shtwfgs.cn

[U86] JS：空值合并
来源：http://nr.wgjwhj.cn

a ?? b
来源：http://gb.huanxung.cn

[U87] JS：解构默认值
来源：http://ib.shtwfgs.cn

const { a = 1, b = 2 } = obj;
来源：http://fh.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://fc.hnjuh.cn

{ ...a, ...b }
来源：http://tj.huixiangedu.cn

[U89] JS：数组去重
来源：http://xv.nszjky.cn

[...new Set(arr)]
来源：http://ie.gzmigu.cn

[U90] JS：数字数组排序
来源：http://ff.9csxet.cn

[...arr].sort((a, b) => a - b)
来源：http://jj.szxytkj.cn

[U91] JS：对象键值遍历
来源：http://fn.jctech888.com.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zi.shtwfgs.cn

[U92] JS：深拷贝
来源：http://rm.yuntaijiaju.cn

structuredClone(obj)
来源：http://lt.asd995.cn

[U93] JS：模板字符串
来源：http://sg.huanxung.cn

`共 ${n} 条`
来源：http://fk.hahajie.cn

[U94] JS：箭头函数
来源：http://ml.yuntaijiaju.cn

const double = x => x * 2;
来源：http://fd.panjiajie.cn

[U95] JS：Promise 包装
来源：http://jb.jctech888.com.cn

new Promise((resolve, reject) => {})
来源：http://yz.bjjhwx.cn

[U96] JS：async/await 与异常
来源：http://cm.panjiajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ml.shxzskj.cn

[U97] JS：并发请求
来源：http://hz.huixinmuqiang.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qu.shxzukj.cn

[U98] JS：fetch 带 JSON
来源：http://kf.yuntaijiaju.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://au.shxzukj.cn

[U99] JS：事件监听
来源：http://xw.yuntaijiaju.cn

el.addEventListener("click", e => {})
来源：http://ec.521024.cn

[U100] JS：DOM 查询
来源：http://ib.asd995.cn

document.querySelector(".item")
来源：http://eu.wgjwhj.cn

[U101] JS：classList 操作
来源：http://va.hnjuh.cn

el.classList.toggle("active")
来源：http://qm.szxytkj.cn

[U102] JS：本地存储
来源：http://aj.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ml.muxihuayi.cn

[U103] JS：定时器
来源：http://cr.yuexingan06.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ia.asd995.cn

[U104] JS：防抖
来源：http://la.bookmarksfly.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mu.panjiajie.cn

[U105] JS：节流
来源：http://lu.hnjuh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://je.haigaiapp.cn

[U106] JS：日期格式化
来源：http://gf.9csxet.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qj.hnjuh.cn

[U107] JS：数字千分位
来源：http://zd.shxzskj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://er.nicolike.cn

[U108] JS：随机整数
来源：http://av.9csxet.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kf.chemitech.net.cn

[U109] JS：数组分组
来源：http://sf.huixinmuqiang.cn

Object.groupBy(arr, x => x.type)
来源：http://az.szxytkj.cn

[U110] JS：数组分块
来源：http://ry.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qf.panjiajie.cn

[U111] JS：对象转 Map
来源：http://oy.szsharing.cn

new Map(Object.entries(obj))
来源：http://lh.shtwfgs.cn

[U112] JS：字符串补位
来源：http://uj.asd995.cn

"7".padStart(3, "0")
来源：http://bp.szxytkj.cn

[U113] JS：正则替换全部
来源：http://nd.muxihuayi.cn

s.replaceAll("a", "b")
来源：http://yh.nicolike.cn

[U114] JS：JSON 深比较
来源：http://um.haigaiapp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jf.muxihuayi.cn

[U115] JS：生成 UUID
来源：http://bk.huixinmuqiang.cn

crypto.randomUUID()
来源：http://ep.huanxung.cn

[U116] JS：类型检查（JSDoc）
来源：http://gl.newstarts.cn

/** @param {string} name */ function f(name) {}
来源：http://sx.szxytkj.cn

[U117] JS：单元测试
来源：http://hn.szxytkj.cn

npm i -D vitest;  npx vitest
来源：http://lr.huanxung.cn

[U118] JS：开发服务器
来源：http://kj.colortex.cn

npm i -D vite;  npx vite
来源：http://tv.panjiajie.cn

[U119] JS：生产构建
来源：http://tv.bjjhwx.cn

npx vite build
来源：http://yo.asd995.cn

[U120] JS：读取环境变量（Vite）
来源：http://iw.asd995.cn

import.meta.env.VITE_API_URL
来源：http://ra.szxytkj.cn

================================================================================
来源：http://cg.hnjuh.cn

统计汇总
来源：http://gr.bookmarksfly.cn

================================================================================
来源：http://td.shxzskj.cn

按语言统计（条）：
来源：http://cl.gzmigu.cn

Python ......... 252
来源：http://yf.bjjhwx.cn

PHP ............ 252
来源：http://tz.asd995.cn

JavaScript ..... 252
来源：http://gl.nicolike.cn

TypeScript ..... 212
来源：http://nc.shxzukj.cn

Java ........... 212
来源：http://yk.muxihuayi.cn

Go ............. 212
来源：http://um.huixiangedu.cn

Ruby ........... 212
来源：http://qk.szxytkj.cn

C# ............. 212
来源：http://cc.huixiangedu.cn

C .............. 30
来源：http://lc.bookmarksfly.cn

C++ ............ 30
来源：http://gh.muxihuayi.cn

SQL ............ 90
来源：http://tr.lnxyls.cn

Bash ........... 80
来源：http://il.chemitech.net.cn

Kotlin ......... 15
来源：http://wn.yuntaijiaju.cn

Swift .......... 15
来源：http://hb.hahajie.cn

Lua ............ 10
来源：http://gu.bjjhwx.cn

Perl ........... 10
来源：http://ra.jctech888.com.cn

Scala .......... 10
来源：http://lq.chemitech.net.cn

------------------------------------
来源：http://tz.9csxet.cn

合计 ........... 2106 条
来源：http://sf.muxihuayi.cn

按章节统计：
来源：http://lj.chemitech.net.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tl.asd995.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tv.colortex.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ev.chemitech.net.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ev.chemitech.net.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yr.shxzskj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kk.haigaiapp.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xg.nicolike.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sy.gzmigu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fy.asd995.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ok.jctech888.com.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ae.newstarts.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gx.asd995.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vv.shtwfgs.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ly.yuntaijiaju.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://en.huixiangedu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://iy.huanxung.cn

Q SQL 专题                              90
来源：http://rf.szxytkj.cn

R Bash 专题                             80
来源：http://bs.gzmigu.cn

S C / C++ 专题                          60
来源：http://cs.colortex.cn

T 其他语言补充                          60
来源：http://pc.shxzskj.cn

U 高频实用片段                         120
来源：http://rt.yuntaijiaju.cn

------------------------------------
来源：http://jn.gzmigu.cn

合计                                  2106 条
来源：http://qg.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://il.haigaiapp.cn

使用提醒
来源：http://fv.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://th.szsharing.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xf.shtwfgs.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://op.chemitech.net.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wi.gzmigu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://mn.newstarts.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ro.szsharing.cn

—— 文件结束 ——
来源：http://cg.wgjwhj.cn

================================================================================
来源：http://rl.wgjwhj.cn

程序语言常见例子速查手册（2024 版）
来源：http://qx.bookmarksfly.cn

Common Programming Examples Cheat Book
来源：http://gl.bookmarksfly.cn

================================================================================
来源：http://go.yuntaijiaju.cn

【收录内容】
来源：http://iv.haigaiapp.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://wi.szxytkj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zn.jianghongdianzi.cn

SQL · Bash · C · C++
来源：http://sz.9csxet.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uo.bookmarksfly.cn

【使用说明】
来源：http://ye.jctech888.com.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jd.panjiajie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fw.nszjky.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pd.bjjhwx.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cw.hahajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://nz.nicolike.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wn.huanxung.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jr.panjiajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lo.jctech888.com.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fl.shxzukj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gk.haigaiapp.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jn.nszjky.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qq.jianghongdianzi.cn

【文件统计】
来源：http://ka.hnjuh.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cj.nicolike.cn

--------------------------------------------------------------------------------
来源：http://gc.lnxyls.cn

目  录
来源：http://wc.colortex.cn

--------------------------------------------------------------------------------
来源：http://ta.huixinmuqiang.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jj.hahajie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xe.shxzskj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ha.haigaiapp.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vw.hahajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://if.yuntaijiaju.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://td.szxytkj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mk.jianghongdianzi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kq.yuexingan06.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kc.hahajie.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gh.lnxyls.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dc.nszjky.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bt.wgjwhj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yd.wgjwhj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lu.9csxet.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sh.huixiangedu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jt.nszjky.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nd.bookmarksfly.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://du.szsharing.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uh.muxihuayi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://am.jianghongdianzi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vp.bookmarksfly.cn

================================================================================
来源：http://sc.shxzskj.cn

A. 基础语法与类型
来源：http://eo.wgjwhj.cn

================================================================================
来源：http://rl.newstarts.cn

[A01] Hello World
来源：http://nf.huixinmuqiang.cn

Py:   print("Hello, World!")
来源：http://lz.shxzskj.cn

PHP:  echo "Hello, World!";
来源：http://yd.szxytkj.cn

JS:   console.log("Hello, World!");
来源：http://qy.hnjuh.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jg.gzmigu.cn

Java: System.out.println("Hello, World!");
来源：http://gb.shxzukj.cn

Go:   fmt.Println("Hello, World!")
来源：http://lq.wgjwhj.cn

Ruby: puts "Hello, World!"
来源：http://uj.haigaiapp.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://qy.yuexingan06.cn

[A02] 变量声明与赋值
来源：http://my.lnxyls.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ru.haigaiapp.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://di.yuntaijiaju.cn

JS:   let name = "Alex"; const age = 20;
来源：http://fh.szsharing.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zh.huanxung.cn

Java: String name = "Alex"; int age = 20;
来源：http://lo.shxzskj.cn

Go:   name := "Alex"; age := 20
来源：http://bf.szxytkj.cn

Ruby: name = "Alex"; age = 20
来源：http://rj.szsharing.cn

C#:   string name = "Alex"; int age = 20;
来源：http://xs.nszjky.cn

[A03] 常量定义
来源：http://oj.bjjhwx.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fy.hahajie.cn

PHP:  const PI = 3.14159;
来源：http://pc.szsharing.cn

JS:   const PI = 3.14159;
来源：http://sr.nicolike.cn

TS:   const PI: number = 3.14159;
来源：http://zm.chemitech.net.cn

Java: static final double PI = 3.14159;
来源：http://hq.huixiangedu.cn

Go:   const PI = 3.14159
来源：http://cn.huixinmuqiang.cn

Ruby: PI = 3.14159
来源：http://pb.wgjwhj.cn

C#:   const double PI = 3.14159;
来源：http://ih.gzmigu.cn

[A04] 判断变量类型
来源：http://sy.wgjwhj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://pc.panjiajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hm.huixinmuqiang.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ya.gzmigu.cn

TS:   typeof x; x instanceof Date
来源：http://pj.jctech888.com.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yh.shxzukj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://lb.chemitech.net.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://sm.yuexingan06.cn

C#:   x.GetType().Name; x is int
来源：http://vw.jctech888.com.cn

[A05] 整数除法与取模
来源：http://oh.huixiangedu.cn


<!-- 参考信息 -->