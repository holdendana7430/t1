代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://oo.bookmarksfly.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://sj.asd995.cn

[U46] PHP：可空类型
来源：http://qc.wgjwhj.cn

?string $name = null
来源：http://aw.bookmarksfly.cn

[U47] PHP：联合类型
来源：http://ve.jctech888.com.cn

int|string $id
来源：http://ji.colortex.cn

[U48] PHP：纯枚举
来源：http://mh.gzmigu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ix.chemitech.net.cn

[U49] PHP：只读属性
来源：http://fe.szsharing.cn

public readonly string $name
来源：http://ro.colortex.cn

[U50] PHP：构造器属性提升
来源：http://gk.gzmigu.cn

public function __construct(private int $id) {}
来源：http://eo.lnxyls.cn

[U51] PHP：数组解构
来源：http://am.yuntaijiaju.cn

[$a, $b] = $arr;
来源：http://oo.lnxyls.cn

[U52] PHP：箭头函数
来源：http://pg.asd995.cn

$double = fn($x) => $x * 2;
来源：http://er.yuntaijiaju.cn

[U53] PHP：空合并运算符
来源：http://zx.asd995.cn

$v = $a ?? $b ?? "default";
来源：http://bm.wgjwhj.cn

[U54] PHP：空安全调用
来源：http://lw.nszjky.cn

$obj?->method()
来源：http://fo.nszjky.cn

[U55] PHP：match 表达式
来源：http://uq.wgjwhj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://in.panjiajie.cn

[U56] PHP：命名参数
来源：http://lf.nicolike.cn

f(a: 1, b: 2)
来源：http://bo.panjiajie.cn

[U57] PHP：字符串插值
来源：http://qp.panjiajie.cn

"值: {$a}"
来源：http://jz.newstarts.cn

[U58] PHP：数组三件套
来源：http://hb.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lu.huanxung.cn

[U59] PHP：自定义排序
来源：http://ps.521024.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yy.jctech888.com.cn

[U60] PHP：JSON 编解码
来源：http://dl.shtwfgs.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://we.huanxung.cn

[U61] PHP：正则
来源：http://nj.jctech888.com.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://iz.panjiajie.cn

[U62] PHP：日期对象
来源：http://jq.colortex.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xw.newstarts.cn

[U63] PHP：文件读写
来源：http://jg.shxzskj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ic.muxihuayi.cn

[U64] PHP：目录遍历
来源：http://sg.bjjhwx.cn

glob("dir/*.php");  scandir("dir");
来源：http://sm.panjiajie.cn

[U65] PHP：会话
来源：http://ow.huanxung.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bp.521024.cn

[U66] PHP：设置 Cookie
来源：http://eh.panjiajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wn.asd995.cn

[U67] PHP：处理文件上传
来源：http://iy.haigaiapp.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://di.szxytkj.cn

[U68] PHP：PDO 连接
来源：http://yz.shxzukj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tk.yuexingan06.cn

[U69] PHP：PDO 预处理
来源：http://ce.haigaiapp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tj.bookmarksfly.cn

[U70] PHP：PDO 事务
来源：http://vp.yuexingan06.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ra.9csxet.cn

[U71] PHP：抛出异常
来源：http://cr.yuntaijiaju.cn

throw new RuntimeException("失败", 500);
来源：http://dp.huixinmuqiang.cn

[U72] PHP：写错误日志
来源：http://le.szxytkj.cn

error_log("失败: " . $e->getMessage());
来源：http://bd.bookmarksfly.cn

[U73] PHP：读取 ini 配置
来源：http://ss.nicolike.cn

parse_ini_file("config.ini", true)
来源：http://ga.jctech888.com.cn

[U74] PHP：读取环境变量
来源：http://qn.wgjwhj.cn

getenv("APP_ENV") ?: "production"
来源：http://iv.szxytkj.cn

[U75] PHP：依赖注入
来源：http://ha.nicolike.cn

composer require psr/container
来源：http://ku.bjjhwx.cn

[U76] PHP：简单路由
来源：http://ny.yuexingan06.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dv.jctech888.com.cn

[U77] PHP：模板渲染
来源：http://il.huanxung.cn

composer require twig/twig
来源：http://ha.wgjwhj.cn

[U78] PHP：单元测试
来源：http://xn.panjiajie.cn

composer require --dev phpunit/phpunit
来源：http://pa.hahajie.cn

[U79] PHP：静态分析
来源：http://ll.szxytkj.cn

composer require --dev phpstan/phpstan
来源：http://rj.nicolike.cn

[U80] PHP：代码规范修复
来源：http://tm.wgjwhj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://av.gzmigu.cn

[U81] JS：初始化项目
来源：http://jd.bookmarksfly.cn

npm init -y;  npm i express
来源：http://vb.newstarts.cn

[U82] JS：package.json 脚本
来源：http://lq.wgjwhj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nx.shtwfgs.cn

[U83] JS：ES Module 导入导出
来源：http://ap.muxihuayi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bv.haigaiapp.cn

[U84] JS：CommonJS 写法
来源：http://kd.colortex.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ii.newstarts.cn

[U85] JS：可选链
来源：http://wl.yuexingan06.cn

a?.b?.c
来源：http://gf.bookmarksfly.cn

[U86] JS：空值合并
来源：http://yp.newstarts.cn

a ?? b
来源：http://ew.hnjuh.cn

[U87] JS：解构默认值
来源：http://xi.huanxung.cn

const { a = 1, b = 2 } = obj;
来源：http://uz.wgjwhj.cn

[U88] JS：对象展开合并
来源：http://qq.haigaiapp.cn

{ ...a, ...b }
来源：http://yi.521024.cn

[U89] JS：数组去重
来源：http://an.hnjuh.cn

[...new Set(arr)]
来源：http://pm.colortex.cn

[U90] JS：数字数组排序
来源：http://ie.colortex.cn

[...arr].sort((a, b) => a - b)
来源：http://hh.lnxyls.cn

[U91] JS：对象键值遍历
来源：http://sr.wgjwhj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wu.jianghongdianzi.cn

[U92] JS：深拷贝
来源：http://mp.nszjky.cn

structuredClone(obj)
来源：http://hf.huixiangedu.cn

[U93] JS：模板字符串
来源：http://re.jctech888.com.cn

`共 ${n} 条`
来源：http://ws.newstarts.cn

[U94] JS：箭头函数
来源：http://vl.szxytkj.cn

const double = x => x * 2;
来源：http://oz.9csxet.cn

[U95] JS：Promise 包装
来源：http://of.lnxyls.cn

new Promise((resolve, reject) => {})
来源：http://ie.shxzskj.cn

[U96] JS：async/await 与异常
来源：http://ua.hnjuh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kj.hahajie.cn

[U97] JS：并发请求
来源：http://zf.gzmigu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://up.nicolike.cn

[U98] JS：fetch 带 JSON
来源：http://iv.lnxyls.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rc.bookmarksfly.cn

[U99] JS：事件监听
来源：http://bv.yuexingan06.cn

el.addEventListener("click", e => {})
来源：http://wh.huanxung.cn

[U100] JS：DOM 查询
来源：http://iv.newstarts.cn

document.querySelector(".item")
来源：http://fo.9csxet.cn

[U101] JS：classList 操作
来源：http://js.panjiajie.cn

el.classList.toggle("active")
来源：http://so.hahajie.cn

[U102] JS：本地存储
来源：http://gc.huanxung.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xj.hahajie.cn

[U103] JS：定时器
来源：http://bc.jianghongdianzi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://za.colortex.cn

[U104] JS：防抖
来源：http://sk.yuexingan06.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://du.jctech888.com.cn

[U105] JS：节流
来源：http://my.szxytkj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gf.jctech888.com.cn

[U106] JS：日期格式化
来源：http://rr.shtwfgs.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hh.bookmarksfly.cn

[U107] JS：数字千分位
来源：http://bh.newstarts.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lb.huanxung.cn

[U108] JS：随机整数
来源：http://cy.shtwfgs.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vf.9csxet.cn

[U109] JS：数组分组
来源：http://og.lnxyls.cn

Object.groupBy(arr, x => x.type)
来源：http://og.jctech888.com.cn

[U110] JS：数组分块
来源：http://wm.bookmarksfly.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mh.521024.cn

[U111] JS：对象转 Map
来源：http://fb.nszjky.cn

new Map(Object.entries(obj))
来源：http://ll.huixiangedu.cn

[U112] JS：字符串补位
来源：http://oq.shxzskj.cn

"7".padStart(3, "0")
来源：http://ma.shtwfgs.cn

[U113] JS：正则替换全部
来源：http://iw.nszjky.cn

s.replaceAll("a", "b")
来源：http://my.yuntaijiaju.cn

[U114] JS：JSON 深比较
来源：http://jl.nicolike.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jw.shxzskj.cn

[U115] JS：生成 UUID
来源：http://pd.huanxung.cn

crypto.randomUUID()
来源：http://iu.hnjuh.cn

[U116] JS：类型检查（JSDoc）
来源：http://xf.newstarts.cn

/** @param {string} name */ function f(name) {}
来源：http://ri.huixinmuqiang.cn

[U117] JS：单元测试
来源：http://gu.szxytkj.cn

npm i -D vitest;  npx vitest
来源：http://hm.lnxyls.cn

[U118] JS：开发服务器
来源：http://xy.shtwfgs.cn

npm i -D vite;  npx vite
来源：http://vn.asd995.cn

[U119] JS：生产构建
来源：http://re.wgjwhj.cn

npx vite build
来源：http://zv.bookmarksfly.cn

[U120] JS：读取环境变量（Vite）
来源：http://ia.szsharing.cn

import.meta.env.VITE_API_URL
来源：http://gl.haigaiapp.cn

================================================================================
来源：http://bz.9csxet.cn

统计汇总
来源：http://uz.asd995.cn

================================================================================
来源：http://zu.nszjky.cn

按语言统计（条）：
来源：http://il.shxzukj.cn

Python ......... 252
来源：http://zw.szsharing.cn

PHP ............ 252
来源：http://dv.colortex.cn

JavaScript ..... 252
来源：http://cl.lnxyls.cn

TypeScript ..... 212
来源：http://oq.haigaiapp.cn

Java ........... 212
来源：http://cs.shxzukj.cn

Go ............. 212
来源：http://ba.nszjky.cn

Ruby ........... 212
来源：http://sm.lnxyls.cn

C# ............. 212
来源：http://jz.yuntaijiaju.cn

C .............. 30
来源：http://ys.szsharing.cn

C++ ............ 30
来源：http://mt.jctech888.com.cn

SQL ............ 90
来源：http://el.haigaiapp.cn

Bash ........... 80
来源：http://vm.szxytkj.cn

Kotlin ......... 15
来源：http://em.hnjuh.cn

Swift .......... 15
来源：http://tm.asd995.cn

Lua ............ 10
来源：http://nd.chemitech.net.cn

Perl ........... 10
来源：http://nu.gzmigu.cn

Scala .......... 10
来源：http://wq.wgjwhj.cn

------------------------------------
来源：http://vs.szxytkj.cn

合计 ........... 2106 条
来源：http://hs.lnxyls.cn

按章节统计：
来源：http://ug.muxihuayi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ju.yuntaijiaju.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fy.newstarts.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gg.hnjuh.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vw.nicolike.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://it.huixiangedu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nx.521024.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ge.hahajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mc.lnxyls.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qj.521024.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fe.shtwfgs.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gp.chemitech.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rh.yuntaijiaju.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bf.asd995.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fg.nicolike.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://my.nicolike.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ey.wgjwhj.cn

Q SQL 专题                              90
来源：http://ue.huixiangedu.cn

R Bash 专题                             80
来源：http://zu.521024.cn

S C / C++ 专题                          60
来源：http://vl.gzmigu.cn

T 其他语言补充                          60
来源：http://kx.bookmarksfly.cn

U 高频实用片段                         120
来源：http://fm.521024.cn

------------------------------------
来源：http://dk.asd995.cn

合计                                  2106 条
来源：http://wb.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://kw.521024.cn

使用提醒
来源：http://ut.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://ht.shxzskj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://oc.panjiajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fy.huanxung.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cc.szsharing.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://sn.szsharing.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gv.muxihuayi.cn

—— 文件结束 ——
来源：http://yb.asd995.cn

================================================================================
来源：http://ge.521024.cn

程序语言常见例子速查手册（2024 版）
来源：http://yf.shxzukj.cn

Common Programming Examples Cheat Book
来源：http://op.szsharing.cn

================================================================================
来源：http://ae.shtwfgs.cn

【收录内容】
来源：http://zc.colortex.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qv.szxytkj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kq.nszjky.cn

SQL · Bash · C · C++
来源：http://ti.gzmigu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ux.jctech888.com.cn

【使用说明】
来源：http://uv.9csxet.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tv.panjiajie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ev.colortex.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ex.newstarts.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://an.huixiangedu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://od.panjiajie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cs.asd995.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nz.bookmarksfly.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bv.gzmigu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ye.chemitech.net.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://eh.huixiangedu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dm.szsharing.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://em.hahajie.cn

【文件统计】
来源：http://hn.wgjwhj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://iy.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://rs.9csxet.cn

目  录
来源：http://dk.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://ra.bjjhwx.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xg.shxzukj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sa.huixiangedu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mc.chemitech.net.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mt.huixinmuqiang.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mn.colortex.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gx.haigaiapp.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://so.shxzskj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ft.muxihuayi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vo.shxzukj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ad.asd995.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wx.asd995.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kx.yuexingan06.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xp.hnjuh.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nm.colortex.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vg.jctech888.com.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dx.asd995.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://by.lnxyls.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ie.521024.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pd.huanxung.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qr.szxytkj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gw.nicolike.cn

================================================================================
来源：http://by.hnjuh.cn

A. 基础语法与类型
来源：http://rw.shxzukj.cn

================================================================================
来源：http://au.nszjky.cn

[A01] Hello World
来源：http://qd.panjiajie.cn

Py:   print("Hello, World!")
来源：http://ys.panjiajie.cn

PHP:  echo "Hello, World!";
来源：http://dn.shtwfgs.cn

JS:   console.log("Hello, World!");
来源：http://xz.shtwfgs.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cm.chemitech.net.cn

Java: System.out.println("Hello, World!");
来源：http://ry.shxzskj.cn

Go:   fmt.Println("Hello, World!")
来源：http://xg.wgjwhj.cn

Ruby: puts "Hello, World!"
来源：http://vh.nszjky.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://im.haigaiapp.cn

[A02] 变量声明与赋值
来源：http://ma.szsharing.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://br.yuntaijiaju.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://zd.huixiangedu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ck.hnjuh.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pa.asd995.cn

Java: String name = "Alex"; int age = 20;
来源：http://vf.hahajie.cn

Go:   name := "Alex"; age := 20
来源：http://ld.hnjuh.cn

Ruby: name = "Alex"; age = 20
来源：http://hv.panjiajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://sn.huanxung.cn

[A03] 常量定义
来源：http://zk.yuexingan06.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yi.szxytkj.cn

PHP:  const PI = 3.14159;
来源：http://lc.shxzskj.cn

JS:   const PI = 3.14159;
来源：http://wg.haigaiapp.cn

TS:   const PI: number = 3.14159;
来源：http://ur.szsharing.cn

Java: static final double PI = 3.14159;
来源：http://ub.yuexingan06.cn

Go:   const PI = 3.14159
来源：http://pl.yuntaijiaju.cn

Ruby: PI = 3.14159
来源：http://ug.szsharing.cn

C#:   const double PI = 3.14159;
来源：http://yi.gzmigu.cn

[A04] 判断变量类型
来源：http://zf.hahajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://yn.bookmarksfly.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wr.521024.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://sv.shxzskj.cn

TS:   typeof x; x instanceof Date
来源：http://yu.jianghongdianzi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ap.hnjuh.cn

Go:   reflect.TypeOf(x).Name()
来源：http://zr.wgjwhj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yu.jianghongdianzi.cn

C#:   x.GetType().Name; x is int
来源：http://ja.yuexingan06.cn

[A05] 整数除法与取模
来源：http://vl.asd995.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yz.lnxyls.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://cf.hahajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hp.bookmarksfly.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://me.huixinmuqiang.cn


<!-- 参考信息 -->