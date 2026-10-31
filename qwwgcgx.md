代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://pv.yuexingan06.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hd.yuntaijiaju.cn

[U46] PHP：可空类型
来源：http://zi.hahajie.cn

?string $name = null
来源：http://mg.yuexingan06.cn

[U47] PHP：联合类型
来源：http://vz.521024.cn

int|string $id
来源：http://yb.chemitech.net.cn

[U48] PHP：纯枚举
来源：http://by.jctech888.com.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ik.hnjuh.cn

[U49] PHP：只读属性
来源：http://hr.chemitech.net.cn

public readonly string $name
来源：http://zy.szsharing.cn

[U50] PHP：构造器属性提升
来源：http://zf.9csxet.cn

public function __construct(private int $id) {}
来源：http://ry.nicolike.cn

[U51] PHP：数组解构
来源：http://mv.panjiajie.cn

[$a, $b] = $arr;
来源：http://iq.muxihuayi.cn

[U52] PHP：箭头函数
来源：http://ck.bookmarksfly.cn

$double = fn($x) => $x * 2;
来源：http://fw.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://vw.shxzskj.cn

$v = $a ?? $b ?? "default";
来源：http://sk.bookmarksfly.cn

[U54] PHP：空安全调用
来源：http://ri.yuexingan06.cn

$obj?->method()
来源：http://mg.panjiajie.cn

[U55] PHP：match 表达式
来源：http://bf.panjiajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qm.9csxet.cn

[U56] PHP：命名参数
来源：http://xf.asd995.cn

f(a: 1, b: 2)
来源：http://zk.szsharing.cn

[U57] PHP：字符串插值
来源：http://im.shxzukj.cn

"值: {$a}"
来源：http://kx.hahajie.cn

[U58] PHP：数组三件套
来源：http://uq.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cw.wgjwhj.cn

[U59] PHP：自定义排序
来源：http://ny.chemitech.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iz.bookmarksfly.cn

[U60] PHP：JSON 编解码
来源：http://qf.521024.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gr.hnjuh.cn

[U61] PHP：正则
来源：http://qb.panjiajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xb.huixinmuqiang.cn

[U62] PHP：日期对象
来源：http://br.yuexingan06.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://iq.wgjwhj.cn

[U63] PHP：文件读写
来源：http://tt.shxzukj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yr.szsharing.cn

[U64] PHP：目录遍历
来源：http://ff.huixinmuqiang.cn

glob("dir/*.php");  scandir("dir");
来源：http://qb.shxzskj.cn

[U65] PHP：会话
来源：http://cu.newstarts.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zs.huixiangedu.cn

[U66] PHP：设置 Cookie
来源：http://qf.asd995.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dp.asd995.cn

[U67] PHP：处理文件上传
来源：http://ef.colortex.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ev.shxzskj.cn

[U68] PHP：PDO 连接
来源：http://tp.chemitech.net.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ok.shxzskj.cn

[U69] PHP：PDO 预处理
来源：http://sd.nicolike.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ix.szxytkj.cn

[U70] PHP：PDO 事务
来源：http://gu.bookmarksfly.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hm.gzmigu.cn

[U71] PHP：抛出异常
来源：http://xp.jianghongdianzi.cn

throw new RuntimeException("失败", 500);
来源：http://fx.chemitech.net.cn

[U72] PHP：写错误日志
来源：http://dc.haigaiapp.cn

error_log("失败: " . $e->getMessage());
来源：http://iv.huixiangedu.cn

[U73] PHP：读取 ini 配置
来源：http://ep.9csxet.cn

parse_ini_file("config.ini", true)
来源：http://ni.newstarts.cn

[U74] PHP：读取环境变量
来源：http://cv.colortex.cn

getenv("APP_ENV") ?: "production"
来源：http://dg.wgjwhj.cn

[U75] PHP：依赖注入
来源：http://vx.newstarts.cn

composer require psr/container
来源：http://ti.jctech888.com.cn

[U76] PHP：简单路由
来源：http://rx.bjjhwx.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bw.nicolike.cn

[U77] PHP：模板渲染
来源：http://zt.yuntaijiaju.cn

composer require twig/twig
来源：http://df.yuexingan06.cn

[U78] PHP：单元测试
来源：http://nm.hahajie.cn

composer require --dev phpunit/phpunit
来源：http://rz.szsharing.cn

[U79] PHP：静态分析
来源：http://ay.muxihuayi.cn

composer require --dev phpstan/phpstan
来源：http://ze.521024.cn

[U80] PHP：代码规范修复
来源：http://ah.muxihuayi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kd.colortex.cn

[U81] JS：初始化项目
来源：http://wl.jianghongdianzi.cn

npm init -y;  npm i express
来源：http://sc.szxytkj.cn

[U82] JS：package.json 脚本
来源：http://ai.jianghongdianzi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://br.muxihuayi.cn

[U83] JS：ES Module 导入导出
来源：http://fe.nicolike.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jm.521024.cn

[U84] JS：CommonJS 写法
来源：http://tb.chemitech.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ua.szxytkj.cn

[U85] JS：可选链
来源：http://ox.asd995.cn

a?.b?.c
来源：http://zz.colortex.cn

[U86] JS：空值合并
来源：http://ze.9csxet.cn

a ?? b
来源：http://br.szxytkj.cn

[U87] JS：解构默认值
来源：http://ik.shxzskj.cn

const { a = 1, b = 2 } = obj;
来源：http://wr.nicolike.cn

[U88] JS：对象展开合并
来源：http://ym.huixinmuqiang.cn

{ ...a, ...b }
来源：http://tn.huanxung.cn

[U89] JS：数组去重
来源：http://ur.nszjky.cn

[...new Set(arr)]
来源：http://cr.nszjky.cn

[U90] JS：数字数组排序
来源：http://ld.521024.cn

[...arr].sort((a, b) => a - b)
来源：http://gw.nszjky.cn

[U91] JS：对象键值遍历
来源：http://kb.9csxet.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ar.hnjuh.cn

[U92] JS：深拷贝
来源：http://yg.bookmarksfly.cn

structuredClone(obj)
来源：http://yw.gzmigu.cn

[U93] JS：模板字符串
来源：http://ev.panjiajie.cn

`共 ${n} 条`
来源：http://tn.huanxung.cn

[U94] JS：箭头函数
来源：http://tx.lnxyls.cn

const double = x => x * 2;
来源：http://ll.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://kb.shtwfgs.cn

new Promise((resolve, reject) => {})
来源：http://wb.bjjhwx.cn

[U96] JS：async/await 与异常
来源：http://pr.haigaiapp.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vf.bookmarksfly.cn

[U97] JS：并发请求
来源：http://or.bookmarksfly.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jc.shtwfgs.cn

[U98] JS：fetch 带 JSON
来源：http://gk.521024.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uf.jianghongdianzi.cn

[U99] JS：事件监听
来源：http://pm.gzmigu.cn

el.addEventListener("click", e => {})
来源：http://cw.chemitech.net.cn

[U100] JS：DOM 查询
来源：http://dr.nszjky.cn

document.querySelector(".item")
来源：http://pr.hahajie.cn

[U101] JS：classList 操作
来源：http://sn.hnjuh.cn

el.classList.toggle("active")
来源：http://zm.yuntaijiaju.cn

[U102] JS：本地存储
来源：http://rx.nszjky.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mh.bjjhwx.cn

[U103] JS：定时器
来源：http://xr.gzmigu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ua.wgjwhj.cn

[U104] JS：防抖
来源：http://bb.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qt.jctech888.com.cn

[U105] JS：节流
来源：http://vt.panjiajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ra.9csxet.cn

[U106] JS：日期格式化
来源：http://cz.lnxyls.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ys.lnxyls.cn

[U107] JS：数字千分位
来源：http://pw.nszjky.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ml.newstarts.cn

[U108] JS：随机整数
来源：http://zm.chemitech.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dk.wgjwhj.cn

[U109] JS：数组分组
来源：http://he.9csxet.cn

Object.groupBy(arr, x => x.type)
来源：http://dz.muxihuayi.cn

[U110] JS：数组分块
来源：http://nd.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://im.nszjky.cn

[U111] JS：对象转 Map
来源：http://wd.szsharing.cn

new Map(Object.entries(obj))
来源：http://xp.huixinmuqiang.cn

[U112] JS：字符串补位
来源：http://cm.bjjhwx.cn

"7".padStart(3, "0")
来源：http://fm.nszjky.cn

[U113] JS：正则替换全部
来源：http://ot.wgjwhj.cn

s.replaceAll("a", "b")
来源：http://iv.wgjwhj.cn

[U114] JS：JSON 深比较
来源：http://fi.jianghongdianzi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mn.jctech888.com.cn

[U115] JS：生成 UUID
来源：http://gq.nicolike.cn

crypto.randomUUID()
来源：http://vy.panjiajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://le.bjjhwx.cn

/** @param {string} name */ function f(name) {}
来源：http://ij.huixinmuqiang.cn

[U117] JS：单元测试
来源：http://ph.panjiajie.cn

npm i -D vitest;  npx vitest
来源：http://ai.huanxung.cn

[U118] JS：开发服务器
来源：http://xa.huanxung.cn

npm i -D vite;  npx vite
来源：http://uv.lnxyls.cn

[U119] JS：生产构建
来源：http://up.nicolike.cn

npx vite build
来源：http://vu.hnjuh.cn

[U120] JS：读取环境变量（Vite）
来源：http://xq.yuntaijiaju.cn

import.meta.env.VITE_API_URL
来源：http://tt.newstarts.cn

================================================================================
来源：http://ol.hnjuh.cn

统计汇总
来源：http://gz.bjjhwx.cn

================================================================================
来源：http://my.9csxet.cn

按语言统计（条）：
来源：http://vi.jianghongdianzi.cn

Python ......... 252
来源：http://bv.nszjky.cn

PHP ............ 252
来源：http://fq.lnxyls.cn

JavaScript ..... 252
来源：http://aa.nszjky.cn

TypeScript ..... 212
来源：http://bs.jianghongdianzi.cn

Java ........... 212
来源：http://pr.nszjky.cn

Go ............. 212
来源：http://uo.bjjhwx.cn

Ruby ........... 212
来源：http://sp.szsharing.cn

C# ............. 212
来源：http://ev.wgjwhj.cn

C .............. 30
来源：http://ro.shxzukj.cn

C++ ............ 30
来源：http://mi.haigaiapp.cn

SQL ............ 90
来源：http://db.nszjky.cn

Bash ........... 80
来源：http://dc.chemitech.net.cn

Kotlin ......... 15
来源：http://ft.jctech888.com.cn

Swift .......... 15
来源：http://uq.shxzukj.cn

Lua ............ 10
来源：http://wj.lnxyls.cn

Perl ........... 10
来源：http://xp.shxzskj.cn

Scala .......... 10
来源：http://tt.huixiangedu.cn

------------------------------------
来源：http://qz.shxzskj.cn

合计 ........... 2106 条
来源：http://eg.szsharing.cn

按章节统计：
来源：http://nk.shxzskj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zo.huixinmuqiang.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ag.newstarts.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gk.hahajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pb.hahajie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://il.szxytkj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rs.9csxet.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rh.shxzukj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xd.huanxung.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nb.haigaiapp.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tg.bookmarksfly.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ti.panjiajie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ft.jianghongdianzi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rv.chemitech.net.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bu.chemitech.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hu.chemitech.net.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cc.huixiangedu.cn

Q SQL 专题                              90
来源：http://rf.hahajie.cn

R Bash 专题                             80
来源：http://tk.asd995.cn

S C / C++ 专题                          60
来源：http://br.nszjky.cn

T 其他语言补充                          60
来源：http://ms.yuntaijiaju.cn

U 高频实用片段                         120
来源：http://mp.nicolike.cn

------------------------------------
来源：http://hd.chemitech.net.cn

合计                                  2106 条
来源：http://bc.asd995.cn

--------------------------------------------------------------------------------
来源：http://gs.asd995.cn

使用提醒
来源：http://jt.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://hl.lnxyls.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yh.hahajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://le.jctech888.com.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zt.nicolike.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ck.muxihuayi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nh.huixiangedu.cn

—— 文件结束 ——
来源：http://nl.wgjwhj.cn

================================================================================
来源：http://qo.bookmarksfly.cn

程序语言常见例子速查手册（2024 版）
来源：http://kw.gzmigu.cn

Common Programming Examples Cheat Book
来源：http://pr.lnxyls.cn

================================================================================
来源：http://nc.yuexingan06.cn

【收录内容】
来源：http://nw.nszjky.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ex.bookmarksfly.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://px.asd995.cn

SQL · Bash · C · C++
来源：http://jo.shtwfgs.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vo.yuexingan06.cn

【使用说明】
来源：http://fo.chemitech.net.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hp.shtwfgs.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yf.bjjhwx.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ap.shxzskj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bt.nicolike.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://vw.shxzskj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rg.haigaiapp.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fj.huixiangedu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jp.chemitech.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ij.yuntaijiaju.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vq.huanxung.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xt.muxihuayi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hb.bjjhwx.cn

【文件统计】
来源：http://qj.huanxung.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://to.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://po.hnjuh.cn

目  录
来源：http://jx.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://ox.bjjhwx.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wb.yuexingan06.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pp.wgjwhj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ou.hahajie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mi.newstarts.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://so.panjiajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ib.huanxung.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wy.lnxyls.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fe.9csxet.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rt.jctech888.com.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jw.nicolike.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ul.asd995.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://uh.muxihuayi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pu.yuexingan06.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ox.szsharing.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gs.nszjky.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hk.bookmarksfly.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xh.shtwfgs.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xe.szsharing.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lc.huixinmuqiang.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bi.haigaiapp.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nj.colortex.cn

================================================================================
来源：http://mq.colortex.cn

A. 基础语法与类型
来源：http://nr.bookmarksfly.cn

================================================================================
来源：http://vv.nszjky.cn

[A01] Hello World
来源：http://qc.bookmarksfly.cn

Py:   print("Hello, World!")
来源：http://zt.wgjwhj.cn

PHP:  echo "Hello, World!";
来源：http://wi.jianghongdianzi.cn

JS:   console.log("Hello, World!");
来源：http://wm.hnjuh.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lc.yuntaijiaju.cn

Java: System.out.println("Hello, World!");
来源：http://xs.chemitech.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://ny.chemitech.net.cn

Ruby: puts "Hello, World!"
来源：http://zn.szxytkj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fr.bjjhwx.cn

[A02] 变量声明与赋值
来源：http://jd.nszjky.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://am.chemitech.net.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ti.newstarts.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hl.hahajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dk.huanxung.cn

Java: String name = "Alex"; int age = 20;
来源：http://by.shxzukj.cn

Go:   name := "Alex"; age := 20
来源：http://dv.chemitech.net.cn

Ruby: name = "Alex"; age = 20
来源：http://gm.haigaiapp.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ac.521024.cn

[A03] 常量定义
来源：http://or.bjjhwx.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zk.szxytkj.cn

PHP:  const PI = 3.14159;
来源：http://pk.asd995.cn

JS:   const PI = 3.14159;
来源：http://au.hahajie.cn

TS:   const PI: number = 3.14159;
来源：http://uw.panjiajie.cn

Java: static final double PI = 3.14159;
来源：http://hc.bookmarksfly.cn

Go:   const PI = 3.14159
来源：http://zs.jianghongdianzi.cn

Ruby: PI = 3.14159
来源：http://si.panjiajie.cn

C#:   const double PI = 3.14159;
来源：http://bs.shxzukj.cn

[A04] 判断变量类型
来源：http://xd.jianghongdianzi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://gg.muxihuayi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ue.huixinmuqiang.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pu.colortex.cn

TS:   typeof x; x instanceof Date
来源：http://nz.nicolike.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ok.wgjwhj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://sq.shxzukj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://pn.huixinmuqiang.cn

C#:   x.GetType().Name; x is int
来源：http://yp.hnjuh.cn

[A05] 整数除法与取模
来源：http://xu.muxihuayi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pg.panjiajie.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xk.yuntaijiaju.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ra.shxzukj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yi.shxzskj.cn


<!-- 参考信息 -->