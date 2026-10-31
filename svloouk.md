代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://la.yuexingan06.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vf.newstarts.cn

[U46] PHP：可空类型
来源：http://bn.bookmarksfly.cn

?string $name = null
来源：http://tw.jctech888.com.cn

[U47] PHP：联合类型
来源：http://nt.yuntaijiaju.cn

int|string $id
来源：http://nb.hnjuh.cn

[U48] PHP：纯枚举
来源：http://ud.yuntaijiaju.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qk.muxihuayi.cn

[U49] PHP：只读属性
来源：http://wc.muxihuayi.cn

public readonly string $name
来源：http://ph.nicolike.cn

[U50] PHP：构造器属性提升
来源：http://fi.szxytkj.cn

public function __construct(private int $id) {}
来源：http://ox.colortex.cn

[U51] PHP：数组解构
来源：http://ul.huixiangedu.cn

[$a, $b] = $arr;
来源：http://ek.shxzskj.cn

[U52] PHP：箭头函数
来源：http://wp.shxzskj.cn

$double = fn($x) => $x * 2;
来源：http://fl.9csxet.cn

[U53] PHP：空合并运算符
来源：http://pp.521024.cn

$v = $a ?? $b ?? "default";
来源：http://et.asd995.cn

[U54] PHP：空安全调用
来源：http://nj.szxytkj.cn

$obj?->method()
来源：http://qi.huanxung.cn

[U55] PHP：match 表达式
来源：http://cm.huanxung.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dm.chemitech.net.cn

[U56] PHP：命名参数
来源：http://wl.nicolike.cn

f(a: 1, b: 2)
来源：http://iy.asd995.cn

[U57] PHP：字符串插值
来源：http://pd.jianghongdianzi.cn

"值: {$a}"
来源：http://lm.chemitech.net.cn

[U58] PHP：数组三件套
来源：http://ql.hnjuh.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gt.szxytkj.cn

[U59] PHP：自定义排序
来源：http://ma.asd995.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oa.colortex.cn

[U60] PHP：JSON 编解码
来源：http://pv.jctech888.com.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://el.jianghongdianzi.cn

[U61] PHP：正则
来源：http://gb.haigaiapp.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xv.nicolike.cn

[U62] PHP：日期对象
来源：http://mw.asd995.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zm.bjjhwx.cn

[U63] PHP：文件读写
来源：http://tm.huixiangedu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yg.9csxet.cn

[U64] PHP：目录遍历
来源：http://cz.yuntaijiaju.cn

glob("dir/*.php");  scandir("dir");
来源：http://yq.asd995.cn

[U65] PHP：会话
来源：http://pb.chemitech.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ny.yuexingan06.cn

[U66] PHP：设置 Cookie
来源：http://yv.521024.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pt.haigaiapp.cn

[U67] PHP：处理文件上传
来源：http://ay.shxzukj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ht.nicolike.cn

[U68] PHP：PDO 连接
来源：http://gl.huixiangedu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ne.chemitech.net.cn

[U69] PHP：PDO 预处理
来源：http://pw.muxihuayi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kc.nicolike.cn

[U70] PHP：PDO 事务
来源：http://xz.hahajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://np.9csxet.cn

[U71] PHP：抛出异常
来源：http://yx.colortex.cn

throw new RuntimeException("失败", 500);
来源：http://nj.huanxung.cn

[U72] PHP：写错误日志
来源：http://nc.huixiangedu.cn

error_log("失败: " . $e->getMessage());
来源：http://jq.panjiajie.cn

[U73] PHP：读取 ini 配置
来源：http://nx.nszjky.cn

parse_ini_file("config.ini", true)
来源：http://to.shxzukj.cn

[U74] PHP：读取环境变量
来源：http://gk.bjjhwx.cn

getenv("APP_ENV") ?: "production"
来源：http://tn.nszjky.cn

[U75] PHP：依赖注入
来源：http://np.jianghongdianzi.cn

composer require psr/container
来源：http://bx.nszjky.cn

[U76] PHP：简单路由
来源：http://st.huixiangedu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wj.newstarts.cn

[U77] PHP：模板渲染
来源：http://ef.bjjhwx.cn

composer require twig/twig
来源：http://jk.bookmarksfly.cn

[U78] PHP：单元测试
来源：http://dm.lnxyls.cn

composer require --dev phpunit/phpunit
来源：http://yq.yuntaijiaju.cn

[U79] PHP：静态分析
来源：http://rx.huixiangedu.cn

composer require --dev phpstan/phpstan
来源：http://hj.shtwfgs.cn

[U80] PHP：代码规范修复
来源：http://if.yuntaijiaju.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dp.szsharing.cn

[U81] JS：初始化项目
来源：http://lq.jctech888.com.cn

npm init -y;  npm i express
来源：http://xm.muxihuayi.cn

[U82] JS：package.json 脚本
来源：http://yo.jianghongdianzi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dn.bjjhwx.cn

[U83] JS：ES Module 导入导出
来源：http://qa.colortex.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ac.hnjuh.cn

[U84] JS：CommonJS 写法
来源：http://xk.521024.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yi.szxytkj.cn

[U85] JS：可选链
来源：http://sl.shxzskj.cn

a?.b?.c
来源：http://bc.shtwfgs.cn

[U86] JS：空值合并
来源：http://kv.hahajie.cn

a ?? b
来源：http://oj.huixinmuqiang.cn

[U87] JS：解构默认值
来源：http://ho.huixinmuqiang.cn

const { a = 1, b = 2 } = obj;
来源：http://vi.haigaiapp.cn

[U88] JS：对象展开合并
来源：http://qx.szsharing.cn

{ ...a, ...b }
来源：http://tl.panjiajie.cn

[U89] JS：数组去重
来源：http://xp.9csxet.cn

[...new Set(arr)]
来源：http://zv.huixinmuqiang.cn

[U90] JS：数字数组排序
来源：http://uj.gzmigu.cn

[...arr].sort((a, b) => a - b)
来源：http://up.huanxung.cn

[U91] JS：对象键值遍历
来源：http://re.szsharing.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://to.hnjuh.cn

[U92] JS：深拷贝
来源：http://rc.bjjhwx.cn

structuredClone(obj)
来源：http://zh.shtwfgs.cn

[U93] JS：模板字符串
来源：http://dk.jianghongdianzi.cn

`共 ${n} 条`
来源：http://bh.huanxung.cn

[U94] JS：箭头函数
来源：http://ko.asd995.cn

const double = x => x * 2;
来源：http://ws.huanxung.cn

[U95] JS：Promise 包装
来源：http://yg.panjiajie.cn

new Promise((resolve, reject) => {})
来源：http://nq.muxihuayi.cn

[U96] JS：async/await 与异常
来源：http://ym.jctech888.com.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oo.huixiangedu.cn

[U97] JS：并发请求
来源：http://un.hnjuh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lj.newstarts.cn

[U98] JS：fetch 带 JSON
来源：http://st.newstarts.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vw.hahajie.cn

[U99] JS：事件监听
来源：http://no.shxzskj.cn

el.addEventListener("click", e => {})
来源：http://xc.521024.cn

[U100] JS：DOM 查询
来源：http://kg.szxytkj.cn

document.querySelector(".item")
来源：http://tl.gzmigu.cn

[U101] JS：classList 操作
来源：http://yw.nicolike.cn

el.classList.toggle("active")
来源：http://ew.shtwfgs.cn

[U102] JS：本地存储
来源：http://fw.lnxyls.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sf.huixinmuqiang.cn

[U103] JS：定时器
来源：http://oo.panjiajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qm.hahajie.cn

[U104] JS：防抖
来源：http://sp.shxzskj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hf.521024.cn

[U105] JS：节流
来源：http://ad.colortex.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ae.nszjky.cn

[U106] JS：日期格式化
来源：http://tu.9csxet.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ul.panjiajie.cn

[U107] JS：数字千分位
来源：http://gd.wgjwhj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fl.asd995.cn

[U108] JS：随机整数
来源：http://om.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://aa.shxzskj.cn

[U109] JS：数组分组
来源：http://sk.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://sk.hnjuh.cn

[U110] JS：数组分块
来源：http://ih.szsharing.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ye.wgjwhj.cn

[U111] JS：对象转 Map
来源：http://ek.jctech888.com.cn

new Map(Object.entries(obj))
来源：http://ph.szxytkj.cn

[U112] JS：字符串补位
来源：http://vn.asd995.cn

"7".padStart(3, "0")
来源：http://bj.muxihuayi.cn

[U113] JS：正则替换全部
来源：http://fo.shxzskj.cn

s.replaceAll("a", "b")
来源：http://nw.shxzskj.cn

[U114] JS：JSON 深比较
来源：http://th.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hs.shtwfgs.cn

[U115] JS：生成 UUID
来源：http://lb.521024.cn

crypto.randomUUID()
来源：http://yk.jianghongdianzi.cn

[U116] JS：类型检查（JSDoc）
来源：http://ob.521024.cn

/** @param {string} name */ function f(name) {}
来源：http://og.yuntaijiaju.cn

[U117] JS：单元测试
来源：http://nr.huixinmuqiang.cn

npm i -D vitest;  npx vitest
来源：http://wc.bjjhwx.cn

[U118] JS：开发服务器
来源：http://qt.huixinmuqiang.cn

npm i -D vite;  npx vite
来源：http://nd.shtwfgs.cn

[U119] JS：生产构建
来源：http://qt.panjiajie.cn

npx vite build
来源：http://mg.szsharing.cn

[U120] JS：读取环境变量（Vite）
来源：http://ol.jctech888.com.cn

import.meta.env.VITE_API_URL
来源：http://tc.shxzukj.cn

================================================================================
来源：http://cg.jctech888.com.cn

统计汇总
来源：http://tp.9csxet.cn

================================================================================
来源：http://wt.shxzskj.cn

按语言统计（条）：
来源：http://er.jctech888.com.cn

Python ......... 252
来源：http://zs.gzmigu.cn

PHP ............ 252
来源：http://qf.hahajie.cn

JavaScript ..... 252
来源：http://zi.haigaiapp.cn

TypeScript ..... 212
来源：http://cu.yuexingan06.cn

Java ........... 212
来源：http://yq.yuexingan06.cn

Go ............. 212
来源：http://fn.wgjwhj.cn

Ruby ........... 212
来源：http://it.9csxet.cn

C# ............. 212
来源：http://wl.colortex.cn

C .............. 30
来源：http://dn.jctech888.com.cn

C++ ............ 30
来源：http://nd.panjiajie.cn

SQL ............ 90
来源：http://va.yuntaijiaju.cn

Bash ........... 80
来源：http://id.muxihuayi.cn

Kotlin ......... 15
来源：http://eh.huanxung.cn

Swift .......... 15
来源：http://yi.jianghongdianzi.cn

Lua ............ 10
来源：http://qt.9csxet.cn

Perl ........... 10
来源：http://wk.gzmigu.cn

Scala .......... 10
来源：http://kr.chemitech.net.cn

------------------------------------
来源：http://ar.shtwfgs.cn

合计 ........... 2106 条
来源：http://pt.hnjuh.cn

按章节统计：
来源：http://sb.lnxyls.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hw.yuntaijiaju.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zt.shxzskj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fq.shxzskj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xn.huixiangedu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wn.bookmarksfly.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dx.bookmarksfly.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fa.panjiajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gc.lnxyls.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nr.nicolike.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://af.colortex.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vd.hnjuh.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ue.szsharing.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jy.jctech888.com.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mk.szxytkj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rj.521024.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ry.nszjky.cn

Q SQL 专题                              90
来源：http://pv.bjjhwx.cn

R Bash 专题                             80
来源：http://me.yuntaijiaju.cn

S C / C++ 专题                          60
来源：http://ic.haigaiapp.cn

T 其他语言补充                          60
来源：http://uz.jctech888.com.cn

U 高频实用片段                         120
来源：http://tc.nszjky.cn

------------------------------------
来源：http://dh.huixinmuqiang.cn

合计                                  2106 条
来源：http://uc.newstarts.cn

--------------------------------------------------------------------------------
来源：http://ye.szsharing.cn

使用提醒
来源：http://sf.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://ys.szxytkj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fg.gzmigu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cz.jctech888.com.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nu.newstarts.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gf.hnjuh.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gu.nszjky.cn

—— 文件结束 ——
来源：http://ig.bjjhwx.cn

================================================================================
来源：http://cd.wgjwhj.cn

程序语言常见例子速查手册（2024 版）
来源：http://vi.asd995.cn

Common Programming Examples Cheat Book
来源：http://pk.newstarts.cn

================================================================================
来源：http://nm.huixinmuqiang.cn

【收录内容】
来源：http://fv.wgjwhj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://gt.huixinmuqiang.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gb.shxzskj.cn

SQL · Bash · C · C++
来源：http://sn.wgjwhj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kk.szsharing.cn

【使用说明】
来源：http://fr.muxihuayi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://az.chemitech.net.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ec.hnjuh.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bh.nszjky.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yv.colortex.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ia.bjjhwx.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ar.nicolike.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zn.jctech888.com.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mb.shxzskj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kt.newstarts.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qm.asd995.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dy.bookmarksfly.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://au.hahajie.cn

【文件统计】
来源：http://er.bjjhwx.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vh.colortex.cn

--------------------------------------------------------------------------------
来源：http://vx.chemitech.net.cn

目  录
来源：http://nu.newstarts.cn

--------------------------------------------------------------------------------
来源：http://jx.panjiajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://se.huixinmuqiang.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hf.colortex.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kb.haigaiapp.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vw.huanxung.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ss.muxihuayi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://sq.bjjhwx.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rt.jctech888.com.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cu.chemitech.net.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wi.jianghongdianzi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fw.szxytkj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hk.muxihuayi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gg.shxzskj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://eq.yuntaijiaju.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yu.panjiajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uf.bookmarksfly.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fp.shtwfgs.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jt.yuntaijiaju.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://jl.shxzskj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qb.hnjuh.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vb.chemitech.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jb.hnjuh.cn

================================================================================
来源：http://eu.haigaiapp.cn

A. 基础语法与类型
来源：http://ou.chemitech.net.cn

================================================================================
来源：http://hb.huixinmuqiang.cn

[A01] Hello World
来源：http://tb.9csxet.cn

Py:   print("Hello, World!")
来源：http://bu.chemitech.net.cn

PHP:  echo "Hello, World!";
来源：http://sm.haigaiapp.cn

JS:   console.log("Hello, World!");
来源：http://re.wgjwhj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cq.shxzukj.cn

Java: System.out.println("Hello, World!");
来源：http://ik.huanxung.cn

Go:   fmt.Println("Hello, World!")
来源：http://ad.chemitech.net.cn

Ruby: puts "Hello, World!"
来源：http://it.gzmigu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fw.bjjhwx.cn

[A02] 变量声明与赋值
来源：http://ue.hnjuh.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mp.nicolike.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://px.szsharing.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xd.huixiangedu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ga.521024.cn

Java: String name = "Alex"; int age = 20;
来源：http://mj.yuexingan06.cn

Go:   name := "Alex"; age := 20
来源：http://qd.jctech888.com.cn

Ruby: name = "Alex"; age = 20
来源：http://wt.colortex.cn

C#:   string name = "Alex"; int age = 20;
来源：http://na.muxihuayi.cn

[A03] 常量定义
来源：http://gg.lnxyls.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qg.szsharing.cn

PHP:  const PI = 3.14159;
来源：http://zs.panjiajie.cn

JS:   const PI = 3.14159;
来源：http://qt.bjjhwx.cn

TS:   const PI: number = 3.14159;
来源：http://ig.gzmigu.cn

Java: static final double PI = 3.14159;
来源：http://an.asd995.cn

Go:   const PI = 3.14159
来源：http://ml.shxzskj.cn

Ruby: PI = 3.14159
来源：http://uo.shxzskj.cn

C#:   const double PI = 3.14159;
来源：http://rs.bookmarksfly.cn

[A04] 判断变量类型
来源：http://bu.huanxung.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://tv.shxzukj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://it.shtwfgs.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yo.nicolike.cn

TS:   typeof x; x instanceof Date
来源：http://mj.szxytkj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pe.nszjky.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ss.asd995.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yr.521024.cn

C#:   x.GetType().Name; x is int
来源：http://gg.newstarts.cn

[A05] 整数除法与取模
来源：http://ns.jianghongdianzi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zy.9csxet.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zo.huanxung.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ub.hnjuh.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qb.shtwfgs.cn


<!-- 参考信息 -->