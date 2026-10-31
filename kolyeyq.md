代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://vs.huixinmuqiang.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://kj.hahajie.cn

[U46] PHP：可空类型
来源：http://sa.lnxyls.cn

?string $name = null
来源：http://ih.nszjky.cn

[U47] PHP：联合类型
来源：http://wj.hahajie.cn

int|string $id
来源：http://ix.hnjuh.cn

[U48] PHP：纯枚举
来源：http://up.521024.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kp.bjjhwx.cn

[U49] PHP：只读属性
来源：http://zf.hnjuh.cn

public readonly string $name
来源：http://od.hnjuh.cn

[U50] PHP：构造器属性提升
来源：http://sh.chemitech.net.cn

public function __construct(private int $id) {}
来源：http://on.jctech888.com.cn

[U51] PHP：数组解构
来源：http://uc.bjjhwx.cn

[$a, $b] = $arr;
来源：http://dv.haigaiapp.cn

[U52] PHP：箭头函数
来源：http://ki.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://kk.hnjuh.cn

[U53] PHP：空合并运算符
来源：http://jc.bjjhwx.cn

$v = $a ?? $b ?? "default";
来源：http://nr.lnxyls.cn

[U54] PHP：空安全调用
来源：http://xz.huanxung.cn

$obj?->method()
来源：http://qw.hnjuh.cn

[U55] PHP：match 表达式
来源：http://xj.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zm.gzmigu.cn

[U56] PHP：命名参数
来源：http://ko.huixiangedu.cn

f(a: 1, b: 2)
来源：http://ap.huixinmuqiang.cn

[U57] PHP：字符串插值
来源：http://yr.9csxet.cn

"值: {$a}"
来源：http://kr.bookmarksfly.cn

[U58] PHP：数组三件套
来源：http://if.shtwfgs.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ym.lnxyls.cn

[U59] PHP：自定义排序
来源：http://kc.yuexingan06.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ke.jianghongdianzi.cn

[U60] PHP：JSON 编解码
来源：http://mb.szxytkj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mw.asd995.cn

[U61] PHP：正则
来源：http://at.gzmigu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://iq.panjiajie.cn

[U62] PHP：日期对象
来源：http://zt.chemitech.net.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ma.wgjwhj.cn

[U63] PHP：文件读写
来源：http://ef.huixinmuqiang.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vj.shtwfgs.cn

[U64] PHP：目录遍历
来源：http://dx.asd995.cn

glob("dir/*.php");  scandir("dir");
来源：http://yh.bookmarksfly.cn

[U65] PHP：会话
来源：http://pb.gzmigu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sk.chemitech.net.cn

[U66] PHP：设置 Cookie
来源：http://fv.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kj.jianghongdianzi.cn

[U67] PHP：处理文件上传
来源：http://bf.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://iy.9csxet.cn

[U68] PHP：PDO 连接
来源：http://us.newstarts.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kw.bjjhwx.cn

[U69] PHP：PDO 预处理
来源：http://zk.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ln.shtwfgs.cn

[U70] PHP：PDO 事务
来源：http://rq.yuntaijiaju.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ux.gzmigu.cn

[U71] PHP：抛出异常
来源：http://ho.gzmigu.cn

throw new RuntimeException("失败", 500);
来源：http://fx.chemitech.net.cn

[U72] PHP：写错误日志
来源：http://td.hahajie.cn

error_log("失败: " . $e->getMessage());
来源：http://jv.shxzukj.cn

[U73] PHP：读取 ini 配置
来源：http://gt.shxzskj.cn

parse_ini_file("config.ini", true)
来源：http://ij.nszjky.cn

[U74] PHP：读取环境变量
来源：http://gf.jctech888.com.cn

getenv("APP_ENV") ?: "production"
来源：http://hj.wgjwhj.cn

[U75] PHP：依赖注入
来源：http://lm.muxihuayi.cn

composer require psr/container
来源：http://fp.shtwfgs.cn

[U76] PHP：简单路由
来源：http://df.huixiangedu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xf.szxytkj.cn

[U77] PHP：模板渲染
来源：http://qg.521024.cn

composer require twig/twig
来源：http://mw.bjjhwx.cn

[U78] PHP：单元测试
来源：http://au.bjjhwx.cn

composer require --dev phpunit/phpunit
来源：http://ot.muxihuayi.cn

[U79] PHP：静态分析
来源：http://xz.panjiajie.cn

composer require --dev phpstan/phpstan
来源：http://af.nicolike.cn

[U80] PHP：代码规范修复
来源：http://am.shxzukj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rt.lnxyls.cn

[U81] JS：初始化项目
来源：http://ds.gzmigu.cn

npm init -y;  npm i express
来源：http://to.shxzskj.cn

[U82] JS：package.json 脚本
来源：http://za.haigaiapp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fl.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://nf.haigaiapp.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wy.shxzukj.cn

[U84] JS：CommonJS 写法
来源：http://gg.hahajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://tt.bookmarksfly.cn

[U85] JS：可选链
来源：http://sm.szsharing.cn

a?.b?.c
来源：http://oo.shtwfgs.cn

[U86] JS：空值合并
来源：http://ii.jctech888.com.cn

a ?? b
来源：http://jt.newstarts.cn

[U87] JS：解构默认值
来源：http://bv.bookmarksfly.cn

const { a = 1, b = 2 } = obj;
来源：http://oo.huixinmuqiang.cn

[U88] JS：对象展开合并
来源：http://he.szsharing.cn

{ ...a, ...b }
来源：http://vs.jctech888.com.cn

[U89] JS：数组去重
来源：http://wq.shxzukj.cn

[...new Set(arr)]
来源：http://ut.yuexingan06.cn

[U90] JS：数字数组排序
来源：http://iy.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://kv.muxihuayi.cn

[U91] JS：对象键值遍历
来源：http://rt.521024.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pn.haigaiapp.cn

[U92] JS：深拷贝
来源：http://jz.shtwfgs.cn

structuredClone(obj)
来源：http://bk.huanxung.cn

[U93] JS：模板字符串
来源：http://dv.nicolike.cn

`共 ${n} 条`
来源：http://ng.shtwfgs.cn

[U94] JS：箭头函数
来源：http://tv.panjiajie.cn

const double = x => x * 2;
来源：http://dr.jianghongdianzi.cn

[U95] JS：Promise 包装
来源：http://wx.yuntaijiaju.cn

new Promise((resolve, reject) => {})
来源：http://ld.gzmigu.cn

[U96] JS：async/await 与异常
来源：http://lv.colortex.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rj.hnjuh.cn

[U97] JS：并发请求
来源：http://gg.shxzskj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hj.bjjhwx.cn

[U98] JS：fetch 带 JSON
来源：http://lg.szsharing.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vn.gzmigu.cn

[U99] JS：事件监听
来源：http://pu.panjiajie.cn

el.addEventListener("click", e => {})
来源：http://vg.yuntaijiaju.cn

[U100] JS：DOM 查询
来源：http://co.panjiajie.cn

document.querySelector(".item")
来源：http://pq.muxihuayi.cn

[U101] JS：classList 操作
来源：http://ee.nicolike.cn

el.classList.toggle("active")
来源：http://wq.shxzukj.cn

[U102] JS：本地存储
来源：http://sr.szxytkj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jn.yuntaijiaju.cn

[U103] JS：定时器
来源：http://kd.huixinmuqiang.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nm.9csxet.cn

[U104] JS：防抖
来源：http://yj.panjiajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ri.muxihuayi.cn

[U105] JS：节流
来源：http://gx.shtwfgs.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sq.hnjuh.cn

[U106] JS：日期格式化
来源：http://zx.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://oy.huixiangedu.cn

[U107] JS：数字千分位
来源：http://mq.shtwfgs.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ib.yuexingan06.cn

[U108] JS：随机整数
来源：http://hn.bookmarksfly.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yq.huixinmuqiang.cn

[U109] JS：数组分组
来源：http://xh.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://hw.shxzukj.cn

[U110] JS：数组分块
来源：http://nx.szxytkj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mh.521024.cn

[U111] JS：对象转 Map
来源：http://ou.bookmarksfly.cn

new Map(Object.entries(obj))
来源：http://sq.jianghongdianzi.cn

[U112] JS：字符串补位
来源：http://al.hnjuh.cn

"7".padStart(3, "0")
来源：http://ev.muxihuayi.cn

[U113] JS：正则替换全部
来源：http://ic.bookmarksfly.cn

s.replaceAll("a", "b")
来源：http://qi.muxihuayi.cn

[U114] JS：JSON 深比较
来源：http://dc.chemitech.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://br.521024.cn

[U115] JS：生成 UUID
来源：http://ee.huixinmuqiang.cn

crypto.randomUUID()
来源：http://dt.colortex.cn

[U116] JS：类型检查（JSDoc）
来源：http://ru.hnjuh.cn

/** @param {string} name */ function f(name) {}
来源：http://po.panjiajie.cn

[U117] JS：单元测试
来源：http://uo.huixiangedu.cn

npm i -D vitest;  npx vitest
来源：http://ko.gzmigu.cn

[U118] JS：开发服务器
来源：http://xd.gzmigu.cn

npm i -D vite;  npx vite
来源：http://yi.yuntaijiaju.cn

[U119] JS：生产构建
来源：http://ab.shxzukj.cn

npx vite build
来源：http://pa.yuntaijiaju.cn

[U120] JS：读取环境变量（Vite）
来源：http://vm.colortex.cn

import.meta.env.VITE_API_URL
来源：http://jg.huanxung.cn

================================================================================
来源：http://jh.jctech888.com.cn

统计汇总
来源：http://fj.lnxyls.cn

================================================================================
来源：http://su.haigaiapp.cn

按语言统计（条）：
来源：http://yd.bjjhwx.cn

Python ......... 252
来源：http://ep.szxytkj.cn

PHP ............ 252
来源：http://zj.huixiangedu.cn

JavaScript ..... 252
来源：http://zy.shxzskj.cn

TypeScript ..... 212
来源：http://nr.nszjky.cn

Java ........... 212
来源：http://og.asd995.cn

Go ............. 212
来源：http://ca.9csxet.cn

Ruby ........... 212
来源：http://xu.nicolike.cn

C# ............. 212
来源：http://vc.jianghongdianzi.cn

C .............. 30
来源：http://tn.shxzukj.cn

C++ ............ 30
来源：http://ma.shxzukj.cn

SQL ............ 90
来源：http://tm.colortex.cn

Bash ........... 80
来源：http://bv.huixiangedu.cn

Kotlin ......... 15
来源：http://eu.szsharing.cn

Swift .......... 15
来源：http://su.yuntaijiaju.cn

Lua ............ 10
来源：http://rl.bookmarksfly.cn

Perl ........... 10
来源：http://zd.yuntaijiaju.cn

Scala .......... 10
来源：http://qm.nszjky.cn

------------------------------------
来源：http://tp.bjjhwx.cn

合计 ........... 2106 条
来源：http://oy.huixiangedu.cn

按章节统计：
来源：http://vk.panjiajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jz.bjjhwx.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hi.wgjwhj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lb.huixinmuqiang.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mr.521024.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ux.shxzukj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dw.muxihuayi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dd.shtwfgs.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ai.muxihuayi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jv.shtwfgs.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ox.shxzskj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://js.9csxet.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zw.yuntaijiaju.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jy.9csxet.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mx.huanxung.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ud.asd995.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://df.nicolike.cn

Q SQL 专题                              90
来源：http://ii.bjjhwx.cn

R Bash 专题                             80
来源：http://np.asd995.cn

S C / C++ 专题                          60
来源：http://ca.wgjwhj.cn

T 其他语言补充                          60
来源：http://ud.asd995.cn

U 高频实用片段                         120
来源：http://jv.colortex.cn

------------------------------------
来源：http://fp.nszjky.cn

合计                                  2106 条
来源：http://nz.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://gd.nicolike.cn

使用提醒
来源：http://cx.hahajie.cn

--------------------------------------------------------------------------------
来源：http://ag.asd995.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://db.chemitech.net.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dq.bjjhwx.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ik.huixiangedu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fa.bjjhwx.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tl.jctech888.com.cn

—— 文件结束 ——
来源：http://qm.szxytkj.cn

================================================================================
来源：http://ak.nszjky.cn

程序语言常见例子速查手册（2024 版）
来源：http://oe.bjjhwx.cn

Common Programming Examples Cheat Book
来源：http://wr.szxytkj.cn

================================================================================
来源：http://ze.hahajie.cn

【收录内容】
来源：http://fd.gzmigu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://tt.bjjhwx.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://co.hnjuh.cn

SQL · Bash · C · C++
来源：http://gz.szxytkj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fi.9csxet.cn

【使用说明】
来源：http://gn.9csxet.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bk.nszjky.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://te.yuntaijiaju.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ea.nicolike.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tu.wgjwhj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://er.colortex.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xg.nicolike.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gd.nicolike.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wa.newstarts.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xt.nicolike.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pc.yuexingan06.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bm.huanxung.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qy.shtwfgs.cn

【文件统计】
来源：http://zr.huanxung.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ir.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://vh.nszjky.cn

目  录
来源：http://ov.asd995.cn

--------------------------------------------------------------------------------
来源：http://ll.gzmigu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ih.nszjky.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mq.lnxyls.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://us.huixinmuqiang.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zf.shtwfgs.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://em.chemitech.net.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mv.haigaiapp.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mf.huanxung.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qj.jianghongdianzi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xw.shtwfgs.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yx.yuexingan06.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hm.huanxung.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hi.szsharing.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bz.nicolike.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nj.huixinmuqiang.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kx.jianghongdianzi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zi.colortex.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ez.chemitech.net.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://mk.newstarts.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://is.521024.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://or.colortex.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://oc.bjjhwx.cn

================================================================================
来源：http://jn.newstarts.cn

A. 基础语法与类型
来源：http://xj.szsharing.cn

================================================================================
来源：http://li.521024.cn

[A01] Hello World
来源：http://gl.521024.cn

Py:   print("Hello, World!")
来源：http://wf.asd995.cn

PHP:  echo "Hello, World!";
来源：http://uv.shtwfgs.cn

JS:   console.log("Hello, World!");
来源：http://lz.gzmigu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ec.huixiangedu.cn

Java: System.out.println("Hello, World!");
来源：http://sb.shtwfgs.cn

Go:   fmt.Println("Hello, World!")
来源：http://cd.huixinmuqiang.cn

Ruby: puts "Hello, World!"
来源：http://to.colortex.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://nf.panjiajie.cn

[A02] 变量声明与赋值
来源：http://vk.lnxyls.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pt.huanxung.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://kl.jctech888.com.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vp.hahajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rs.9csxet.cn

Java: String name = "Alex"; int age = 20;
来源：http://jl.521024.cn

Go:   name := "Alex"; age := 20
来源：http://rf.jctech888.com.cn

Ruby: name = "Alex"; age = 20
来源：http://es.yuntaijiaju.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ji.huanxung.cn

[A03] 常量定义
来源：http://zy.shxzukj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dy.colortex.cn

PHP:  const PI = 3.14159;
来源：http://ft.521024.cn

JS:   const PI = 3.14159;
来源：http://yg.hnjuh.cn

TS:   const PI: number = 3.14159;
来源：http://fg.nszjky.cn

Java: static final double PI = 3.14159;
来源：http://gp.colortex.cn

Go:   const PI = 3.14159
来源：http://fb.9csxet.cn

Ruby: PI = 3.14159
来源：http://oe.muxihuayi.cn

C#:   const double PI = 3.14159;
来源：http://zv.yuntaijiaju.cn

[A04] 判断变量类型
来源：http://fy.hnjuh.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://wc.huixiangedu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ce.jianghongdianzi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qk.hnjuh.cn

TS:   typeof x; x instanceof Date
来源：http://xi.shxzukj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ud.lnxyls.cn

Go:   reflect.TypeOf(x).Name()
来源：http://dg.9csxet.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://fd.9csxet.cn

C#:   x.GetType().Name; x is int
来源：http://sf.hnjuh.cn

[A05] 整数除法与取模
来源：http://jj.jctech888.com.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ew.nszjky.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://lc.shtwfgs.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pe.huixiangedu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ho.shtwfgs.cn


<!-- 参考信息 -->