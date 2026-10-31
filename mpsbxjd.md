代发 wailian999

[U49] PHP：只读属性
来源：http://ma.huanxung.cn

public readonly string $name
来源：http://dm.asd995.cn

[U50] PHP：构造器属性提升
来源：http://gz.hnjuh.cn

public function __construct(private int $id) {}
来源：http://if.hnjuh.cn

[U51] PHP：数组解构
来源：http://re.bjjhwx.cn

[$a, $b] = $arr;
来源：http://ud.huanxung.cn

[U52] PHP：箭头函数
来源：http://ap.huixiangedu.cn

$double = fn($x) => $x * 2;
来源：http://iy.yuntaijiaju.cn

[U53] PHP：空合并运算符
来源：http://ko.colortex.cn

$v = $a ?? $b ?? "default";
来源：http://ow.huanxung.cn

[U54] PHP：空安全调用
来源：http://hi.wgjwhj.cn

$obj?->method()
来源：http://hg.huixiangedu.cn

[U55] PHP：match 表达式
来源：http://kn.shxzskj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qk.huixinmuqiang.cn

[U56] PHP：命名参数
来源：http://bg.haigaiapp.cn

f(a: 1, b: 2)
来源：http://ex.panjiajie.cn

[U57] PHP：字符串插值
来源：http://wp.szxytkj.cn

"值: {$a}"
来源：http://xl.panjiajie.cn

[U58] PHP：数组三件套
来源：http://pz.huanxung.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jv.haigaiapp.cn

[U59] PHP：自定义排序
来源：http://ch.shtwfgs.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://io.haigaiapp.cn

[U60] PHP：JSON 编解码
来源：http://ax.shxzskj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mq.lnxyls.cn

[U61] PHP：正则
来源：http://iw.hahajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fy.newstarts.cn

[U62] PHP：日期对象
来源：http://xx.asd995.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gt.yuexingan06.cn

[U63] PHP：文件读写
来源：http://fe.szxytkj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tx.shtwfgs.cn

[U64] PHP：目录遍历
来源：http://sb.bjjhwx.cn

glob("dir/*.php");  scandir("dir");
来源：http://xf.521024.cn

[U65] PHP：会话
来源：http://fz.yuexingan06.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wl.panjiajie.cn

[U66] PHP：设置 Cookie
来源：http://tr.szsharing.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ye.shxzukj.cn

[U67] PHP：处理文件上传
来源：http://wn.colortex.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tg.huixiangedu.cn

[U68] PHP：PDO 连接
来源：http://gz.panjiajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yy.asd995.cn

[U69] PHP：PDO 预处理
来源：http://je.jctech888.com.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qv.huanxung.cn

[U70] PHP：PDO 事务
来源：http://nc.chemitech.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://po.jctech888.com.cn

[U71] PHP：抛出异常
来源：http://zs.shxzskj.cn

throw new RuntimeException("失败", 500);
来源：http://pf.panjiajie.cn

[U72] PHP：写错误日志
来源：http://ha.asd995.cn

error_log("失败: " . $e->getMessage());
来源：http://en.9csxet.cn

[U73] PHP：读取 ini 配置
来源：http://bt.hahajie.cn

parse_ini_file("config.ini", true)
来源：http://pk.shxzukj.cn

[U74] PHP：读取环境变量
来源：http://tk.gzmigu.cn

getenv("APP_ENV") ?: "production"
来源：http://lg.shxzukj.cn

[U75] PHP：依赖注入
来源：http://mj.chemitech.net.cn

composer require psr/container
来源：http://zb.nszjky.cn

[U76] PHP：简单路由
来源：http://pe.shxzskj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vs.haigaiapp.cn

[U77] PHP：模板渲染
来源：http://mw.wgjwhj.cn

composer require twig/twig
来源：http://cr.lnxyls.cn

[U78] PHP：单元测试
来源：http://by.huanxung.cn

composer require --dev phpunit/phpunit
来源：http://yx.hnjuh.cn

[U79] PHP：静态分析
来源：http://ug.shtwfgs.cn

composer require --dev phpstan/phpstan
来源：http://ql.shxzskj.cn

[U80] PHP：代码规范修复
来源：http://vp.jctech888.com.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://lz.wgjwhj.cn

[U81] JS：初始化项目
来源：http://vu.9csxet.cn

npm init -y;  npm i express
来源：http://at.muxihuayi.cn

[U82] JS：package.json 脚本
来源：http://xc.bookmarksfly.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sd.shxzukj.cn

[U83] JS：ES Module 导入导出
来源：http://ht.szxytkj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://in.chemitech.net.cn

[U84] JS：CommonJS 写法
来源：http://nk.jianghongdianzi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://tj.jianghongdianzi.cn

[U85] JS：可选链
来源：http://ys.chemitech.net.cn

a?.b?.c
来源：http://hn.szsharing.cn

[U86] JS：空值合并
来源：http://jy.jctech888.com.cn

a ?? b
来源：http://nf.asd995.cn

[U87] JS：解构默认值
来源：http://hp.yuexingan06.cn

const { a = 1, b = 2 } = obj;
来源：http://ar.jctech888.com.cn

[U88] JS：对象展开合并
来源：http://tf.szxytkj.cn

{ ...a, ...b }
来源：http://nk.nicolike.cn

[U89] JS：数组去重
来源：http://pm.newstarts.cn

[...new Set(arr)]
来源：http://li.shxzukj.cn

[U90] JS：数字数组排序
来源：http://ao.nszjky.cn

[...arr].sort((a, b) => a - b)
来源：http://cy.haigaiapp.cn

[U91] JS：对象键值遍历
来源：http://ys.yuexingan06.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ee.wgjwhj.cn

[U92] JS：深拷贝
来源：http://vp.huanxung.cn

structuredClone(obj)
来源：http://fc.wgjwhj.cn

[U93] JS：模板字符串
来源：http://br.muxihuayi.cn

`共 ${n} 条`
来源：http://cl.hnjuh.cn

[U94] JS：箭头函数
来源：http://ki.jctech888.com.cn

const double = x => x * 2;
来源：http://tj.gzmigu.cn

[U95] JS：Promise 包装
来源：http://zb.szsharing.cn

new Promise((resolve, reject) => {})
来源：http://bu.nszjky.cn

[U96] JS：async/await 与异常
来源：http://of.shxzukj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bn.shtwfgs.cn

[U97] JS：并发请求
来源：http://mo.9csxet.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qv.huixiangedu.cn

[U98] JS：fetch 带 JSON
来源：http://lu.bookmarksfly.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://iz.bookmarksfly.cn

[U99] JS：事件监听
来源：http://ut.szsharing.cn

el.addEventListener("click", e => {})
来源：http://jx.szsharing.cn

[U100] JS：DOM 查询
来源：http://mx.wgjwhj.cn

document.querySelector(".item")
来源：http://uc.szxytkj.cn

[U101] JS：classList 操作
来源：http://nr.szxytkj.cn

el.classList.toggle("active")
来源：http://it.9csxet.cn

[U102] JS：本地存储
来源：http://nk.521024.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mm.521024.cn

[U103] JS：定时器
来源：http://nh.bjjhwx.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tb.hahajie.cn

[U104] JS：防抖
来源：http://xm.asd995.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xo.wgjwhj.cn

[U105] JS：节流
来源：http://jq.9csxet.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vl.yuexingan06.cn

[U106] JS：日期格式化
来源：http://wi.hahajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://st.haigaiapp.cn

[U107] JS：数字千分位
来源：http://nw.nszjky.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tb.lnxyls.cn

[U108] JS：随机整数
来源：http://ej.jianghongdianzi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vm.521024.cn

[U109] JS：数组分组
来源：http://pe.521024.cn

Object.groupBy(arr, x => x.type)
来源：http://qq.haigaiapp.cn

[U110] JS：数组分块
来源：http://ek.521024.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ot.colortex.cn

[U111] JS：对象转 Map
来源：http://fp.szxytkj.cn

new Map(Object.entries(obj))
来源：http://gf.asd995.cn

[U112] JS：字符串补位
来源：http://zs.jianghongdianzi.cn

"7".padStart(3, "0")
来源：http://hm.yuexingan06.cn

[U113] JS：正则替换全部
来源：http://dr.gzmigu.cn

s.replaceAll("a", "b")
来源：http://ig.szsharing.cn

[U114] JS：JSON 深比较
来源：http://vl.bjjhwx.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mv.muxihuayi.cn

[U115] JS：生成 UUID
来源：http://ex.bookmarksfly.cn

crypto.randomUUID()
来源：http://td.bjjhwx.cn

[U116] JS：类型检查（JSDoc）
来源：http://ut.muxihuayi.cn

/** @param {string} name */ function f(name) {}
来源：http://pj.nszjky.cn

[U117] JS：单元测试
来源：http://jz.nszjky.cn

npm i -D vitest;  npx vitest
来源：http://cq.szsharing.cn

[U118] JS：开发服务器
来源：http://fj.521024.cn

npm i -D vite;  npx vite
来源：http://xm.nicolike.cn

[U119] JS：生产构建
来源：http://db.newstarts.cn

npx vite build
来源：http://pv.nicolike.cn

[U120] JS：读取环境变量（Vite）
来源：http://je.huixiangedu.cn

import.meta.env.VITE_API_URL
来源：http://gz.yuexingan06.cn

================================================================================
来源：http://hn.bjjhwx.cn

统计汇总
来源：http://zk.colortex.cn

================================================================================
来源：http://qt.521024.cn

按语言统计（条）：
来源：http://lp.panjiajie.cn

Python ......... 252
来源：http://yk.gzmigu.cn

PHP ............ 252
来源：http://cj.newstarts.cn

JavaScript ..... 252
来源：http://zh.jctech888.com.cn

TypeScript ..... 212
来源：http://ku.521024.cn

Java ........... 212
来源：http://om.colortex.cn

Go ............. 212
来源：http://zd.newstarts.cn

Ruby ........... 212
来源：http://bh.shxzukj.cn

C# ............. 212
来源：http://jh.shtwfgs.cn

C .............. 30
来源：http://tq.szxytkj.cn

C++ ............ 30
来源：http://ya.lnxyls.cn

SQL ............ 90
来源：http://jk.gzmigu.cn

Bash ........... 80
来源：http://ps.chemitech.net.cn

Kotlin ......... 15
来源：http://wu.nszjky.cn

Swift .......... 15
来源：http://yr.bookmarksfly.cn

Lua ............ 10
来源：http://qi.haigaiapp.cn

Perl ........... 10
来源：http://zq.9csxet.cn

Scala .......... 10
来源：http://tx.yuexingan06.cn

------------------------------------
来源：http://xa.newstarts.cn

合计 ........... 2106 条
来源：http://sr.9csxet.cn

按章节统计：
来源：http://ez.muxihuayi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ro.9csxet.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zi.panjiajie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ms.521024.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qu.nicolike.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zw.huanxung.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gs.shxzukj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xg.asd995.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tj.gzmigu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://eb.shxzskj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hv.chemitech.net.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nw.jctech888.com.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ah.nszjky.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cw.huixinmuqiang.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tw.yuexingan06.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ts.asd995.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cg.shxzskj.cn

Q SQL 专题                              90
来源：http://df.szsharing.cn

R Bash 专题                             80
来源：http://mn.bookmarksfly.cn

S C / C++ 专题                          60
来源：http://rc.huixinmuqiang.cn

T 其他语言补充                          60
来源：http://na.hahajie.cn

U 高频实用片段                         120
来源：http://oy.9csxet.cn

------------------------------------
来源：http://zy.yuexingan06.cn

合计                                  2106 条
来源：http://db.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://by.chemitech.net.cn

使用提醒
来源：http://kr.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://ju.huixinmuqiang.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dx.jianghongdianzi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://iw.newstarts.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fo.nszjky.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://pp.shtwfgs.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rh.shxzukj.cn

—— 文件结束 ——
来源：http://jj.shtwfgs.cn

================================================================================
来源：http://li.yuexingan06.cn

程序语言常见例子速查手册（2024 版）
来源：http://sa.shxzukj.cn

Common Programming Examples Cheat Book
来源：http://ok.yuntaijiaju.cn

================================================================================
来源：http://yt.yuexingan06.cn

【收录内容】
来源：http://hs.wgjwhj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://yh.huanxung.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pz.wgjwhj.cn

SQL · Bash · C · C++
来源：http://zu.shxzukj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ju.bookmarksfly.cn

【使用说明】
来源：http://xh.szsharing.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nn.nicolike.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kr.nicolike.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tv.nicolike.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mh.shxzskj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qs.newstarts.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fv.shxzukj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cu.wgjwhj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sq.asd995.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mo.huixiangedu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kk.nicolike.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://os.wgjwhj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xr.shxzukj.cn

【文件统计】
来源：http://kj.wgjwhj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tk.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://zu.gzmigu.cn

目  录
来源：http://rt.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://ci.szsharing.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ph.huanxung.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jc.huixinmuqiang.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xz.muxihuayi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xb.hahajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ab.nszjky.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ao.yuntaijiaju.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://pd.shtwfgs.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gf.szsharing.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xy.szxytkj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ko.muxihuayi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dt.nicolike.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://an.colortex.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rc.huixinmuqiang.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://np.huanxung.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ay.hnjuh.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ug.shxzskj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mz.huanxung.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ml.lnxyls.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wf.chemitech.net.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ph.bjjhwx.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://um.9csxet.cn

================================================================================
来源：http://xj.9csxet.cn

A. 基础语法与类型
来源：http://yn.jctech888.com.cn

================================================================================
来源：http://sj.lnxyls.cn

[A01] Hello World
来源：http://vo.yuntaijiaju.cn

Py:   print("Hello, World!")
来源：http://gh.szxytkj.cn

PHP:  echo "Hello, World!";
来源：http://bl.lnxyls.cn

JS:   console.log("Hello, World!");
来源：http://fp.bookmarksfly.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mc.chemitech.net.cn

Java: System.out.println("Hello, World!");
来源：http://tz.bookmarksfly.cn

Go:   fmt.Println("Hello, World!")
来源：http://ta.hnjuh.cn

Ruby: puts "Hello, World!"
来源：http://ai.bookmarksfly.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://pl.nszjky.cn

[A02] 变量声明与赋值
来源：http://go.szxytkj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pl.bookmarksfly.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://yd.yuexingan06.cn

JS:   let name = "Alex"; const age = 20;
来源：http://gq.hnjuh.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bb.huixinmuqiang.cn

Java: String name = "Alex"; int age = 20;
来源：http://ly.jctech888.com.cn

Go:   name := "Alex"; age := 20
来源：http://ye.wgjwhj.cn

Ruby: name = "Alex"; age = 20
来源：http://pm.muxihuayi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://kq.bjjhwx.cn

[A03] 常量定义
来源：http://xa.hahajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sy.huanxung.cn

PHP:  const PI = 3.14159;
来源：http://vh.szsharing.cn

JS:   const PI = 3.14159;
来源：http://bx.huixinmuqiang.cn

TS:   const PI: number = 3.14159;
来源：http://jj.chemitech.net.cn

Java: static final double PI = 3.14159;
来源：http://zb.colortex.cn

Go:   const PI = 3.14159
来源：http://wx.szsharing.cn

Ruby: PI = 3.14159
来源：http://sf.asd995.cn

C#:   const double PI = 3.14159;
来源：http://rk.yuexingan06.cn

[A04] 判断变量类型
来源：http://yy.lnxyls.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://jj.asd995.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gg.hnjuh.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xn.hahajie.cn

TS:   typeof x; x instanceof Date
来源：http://hr.hahajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://da.yuexingan06.cn

Go:   reflect.TypeOf(x).Name()
来源：http://yk.huanxung.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://af.colortex.cn

C#:   x.GetType().Name; x is int
来源：http://wp.shtwfgs.cn

[A05] 整数除法与取模
来源：http://rm.asd995.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bq.jctech888.com.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://kl.muxihuayi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ms.huixiangedu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rg.bookmarksfly.cn

Java: 7 / 2; 7 % 2
来源：http://ze.521024.cn

Go:   7 / 2; 7 % 2
来源：http://bt.muxihuayi.cn

Ruby: 7 / 2; 7 % 2
来源：http://vu.szsharing.cn

C#:   7 / 2; 7 % 2
来源：http://bk.lnxyls.cn

[A06] 字符串转数字
来源：http://xc.jianghongdianzi.cn

Py:   int("42"); float("3.14")
来源：http://yn.jianghongdianzi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kp.521024.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ni.wgjwhj.cn


<!-- 参考信息 -->