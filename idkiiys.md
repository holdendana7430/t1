代发 wailian999

[U37] Py：读写 Excel
来源：http://fu.haigaiapp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fi.wgjwhj.cn

[U38] Py：获取脚本所在目录
来源：http://cp.jctech888.com.cn

Path(__file__).resolve().parent
来源：http://dg.nszjky.cn

[U39] Py：判断是否在交互环境
来源：http://qg.shtwfgs.cn

sys.stdout.isatty()
来源：http://vn.521024.cn

[U40] Py：打印到标准错误
来源：http://pz.hnjuh.cn

print("err", file=sys.stderr)
来源：http://lt.hnjuh.cn

[U41] PHP：初始化 Composer 项目
来源：http://iy.shxzskj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://nv.huixinmuqiang.cn

[U42] PHP：PSR-4 自动加载
来源：http://mz.lnxyls.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ef.chemitech.net.cn

[U43] PHP：声明命名空间
来源：http://ns.yuexingan06.cn

namespace App\Http;
来源：http://hx.huixiangedu.cn

[U44] PHP：开启严格类型
来源：http://qk.shtwfgs.cn

declare(strict_types=1);
来源：http://xh.9csxet.cn

[U45] PHP：类型声明与返回类型
来源：http://dh.lnxyls.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://kz.shtwfgs.cn

[U46] PHP：可空类型
来源：http://rk.nszjky.cn

?string $name = null
来源：http://ok.colortex.cn

[U47] PHP：联合类型
来源：http://jf.shxzukj.cn

int|string $id
来源：http://dz.gzmigu.cn

[U48] PHP：纯枚举
来源：http://me.nszjky.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lo.newstarts.cn

[U49] PHP：只读属性
来源：http://wt.nszjky.cn

public readonly string $name
来源：http://mh.hahajie.cn

[U50] PHP：构造器属性提升
来源：http://bj.521024.cn

public function __construct(private int $id) {}
来源：http://pz.shxzskj.cn

[U51] PHP：数组解构
来源：http://uf.jianghongdianzi.cn

[$a, $b] = $arr;
来源：http://ve.jianghongdianzi.cn

[U52] PHP：箭头函数
来源：http://ql.huixinmuqiang.cn

$double = fn($x) => $x * 2;
来源：http://ev.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://pe.bjjhwx.cn

$v = $a ?? $b ?? "default";
来源：http://mt.muxihuayi.cn

[U54] PHP：空安全调用
来源：http://pv.hnjuh.cn

$obj?->method()
来源：http://py.9csxet.cn

[U55] PHP：match 表达式
来源：http://hx.huixinmuqiang.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xg.asd995.cn

[U56] PHP：命名参数
来源：http://sr.bjjhwx.cn

f(a: 1, b: 2)
来源：http://bo.colortex.cn

[U57] PHP：字符串插值
来源：http://bx.hnjuh.cn

"值: {$a}"
来源：http://su.huixiangedu.cn

[U58] PHP：数组三件套
来源：http://uy.huixinmuqiang.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rg.shtwfgs.cn

[U59] PHP：自定义排序
来源：http://wy.nicolike.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dk.haigaiapp.cn

[U60] PHP：JSON 编解码
来源：http://sb.panjiajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jx.colortex.cn

[U61] PHP：正则
来源：http://mr.muxihuayi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ln.muxihuayi.cn

[U62] PHP：日期对象
来源：http://ji.gzmigu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sb.nszjky.cn

[U63] PHP：文件读写
来源：http://zu.colortex.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yn.asd995.cn

[U64] PHP：目录遍历
来源：http://wd.jctech888.com.cn

glob("dir/*.php");  scandir("dir");
来源：http://aw.wgjwhj.cn

[U65] PHP：会话
来源：http://as.bjjhwx.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dd.chemitech.net.cn

[U66] PHP：设置 Cookie
来源：http://vn.szxytkj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kj.yuntaijiaju.cn

[U67] PHP：处理文件上传
来源：http://on.lnxyls.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vl.huixinmuqiang.cn

[U68] PHP：PDO 连接
来源：http://vr.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jp.jctech888.com.cn

[U69] PHP：PDO 预处理
来源：http://yq.chemitech.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ho.asd995.cn

[U70] PHP：PDO 事务
来源：http://ik.gzmigu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ld.wgjwhj.cn

[U71] PHP：抛出异常
来源：http://nj.bjjhwx.cn

throw new RuntimeException("失败", 500);
来源：http://fc.panjiajie.cn

[U72] PHP：写错误日志
来源：http://hl.9csxet.cn

error_log("失败: " . $e->getMessage());
来源：http://wr.bjjhwx.cn

[U73] PHP：读取 ini 配置
来源：http://jv.shxzukj.cn

parse_ini_file("config.ini", true)
来源：http://tl.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://os.jctech888.com.cn

getenv("APP_ENV") ?: "production"
来源：http://sk.hahajie.cn

[U75] PHP：依赖注入
来源：http://ua.gzmigu.cn

composer require psr/container
来源：http://zk.huixiangedu.cn

[U76] PHP：简单路由
来源：http://qe.huanxung.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pu.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://io.lnxyls.cn

composer require twig/twig
来源：http://ng.newstarts.cn

[U78] PHP：单元测试
来源：http://gw.yuntaijiaju.cn

composer require --dev phpunit/phpunit
来源：http://nv.muxihuayi.cn

[U79] PHP：静态分析
来源：http://gu.nicolike.cn

composer require --dev phpstan/phpstan
来源：http://jk.szxytkj.cn

[U80] PHP：代码规范修复
来源：http://ya.asd995.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bw.chemitech.net.cn

[U81] JS：初始化项目
来源：http://ms.newstarts.cn

npm init -y;  npm i express
来源：http://wt.nszjky.cn

[U82] JS：package.json 脚本
来源：http://gb.hahajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nb.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://zn.shtwfgs.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ay.yuexingan06.cn

[U84] JS：CommonJS 写法
来源：http://uz.hnjuh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bp.yuexingan06.cn

[U85] JS：可选链
来源：http://vc.huanxung.cn

a?.b?.c
来源：http://af.jctech888.com.cn

[U86] JS：空值合并
来源：http://cg.gzmigu.cn

a ?? b
来源：http://ps.yuexingan06.cn

[U87] JS：解构默认值
来源：http://fp.szsharing.cn

const { a = 1, b = 2 } = obj;
来源：http://uh.asd995.cn

[U88] JS：对象展开合并
来源：http://jx.hnjuh.cn

{ ...a, ...b }
来源：http://gj.lnxyls.cn

[U89] JS：数组去重
来源：http://jp.haigaiapp.cn

[...new Set(arr)]
来源：http://zp.colortex.cn

[U90] JS：数字数组排序
来源：http://gb.huixinmuqiang.cn

[...arr].sort((a, b) => a - b)
来源：http://ah.haigaiapp.cn

[U91] JS：对象键值遍历
来源：http://az.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jk.muxihuayi.cn

[U92] JS：深拷贝
来源：http://nj.lnxyls.cn

structuredClone(obj)
来源：http://zw.colortex.cn

[U93] JS：模板字符串
来源：http://tc.shtwfgs.cn

`共 ${n} 条`
来源：http://ye.shtwfgs.cn

[U94] JS：箭头函数
来源：http://jv.hnjuh.cn

const double = x => x * 2;
来源：http://fp.jctech888.com.cn

[U95] JS：Promise 包装
来源：http://ht.521024.cn

new Promise((resolve, reject) => {})
来源：http://lc.huixiangedu.cn

[U96] JS：async/await 与异常
来源：http://ht.nicolike.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zn.bookmarksfly.cn

[U97] JS：并发请求
来源：http://nt.yuexingan06.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ag.521024.cn

[U98] JS：fetch 带 JSON
来源：http://fn.huixiangedu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wv.shtwfgs.cn

[U99] JS：事件监听
来源：http://ja.jctech888.com.cn

el.addEventListener("click", e => {})
来源：http://hs.szxytkj.cn

[U100] JS：DOM 查询
来源：http://hc.bjjhwx.cn

document.querySelector(".item")
来源：http://zd.panjiajie.cn

[U101] JS：classList 操作
来源：http://ym.wgjwhj.cn

el.classList.toggle("active")
来源：http://jc.lnxyls.cn

[U102] JS：本地存储
来源：http://co.haigaiapp.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jj.asd995.cn

[U103] JS：定时器
来源：http://ot.wgjwhj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uf.shtwfgs.cn

[U104] JS：防抖
来源：http://kb.shtwfgs.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eo.yuntaijiaju.cn

[U105] JS：节流
来源：http://ur.newstarts.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lh.chemitech.net.cn

[U106] JS：日期格式化
来源：http://vo.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zb.szxytkj.cn

[U107] JS：数字千分位
来源：http://xg.lnxyls.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qp.gzmigu.cn

[U108] JS：随机整数
来源：http://kn.haigaiapp.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sl.bookmarksfly.cn

[U109] JS：数组分组
来源：http://dd.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://zh.szxytkj.cn

[U110] JS：数组分块
来源：http://hs.jctech888.com.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bc.jctech888.com.cn

[U111] JS：对象转 Map
来源：http://mb.haigaiapp.cn

new Map(Object.entries(obj))
来源：http://nj.szsharing.cn

[U112] JS：字符串补位
来源：http://rk.muxihuayi.cn

"7".padStart(3, "0")
来源：http://pc.hahajie.cn

[U113] JS：正则替换全部
来源：http://pn.521024.cn

s.replaceAll("a", "b")
来源：http://qq.nszjky.cn

[U114] JS：JSON 深比较
来源：http://tm.muxihuayi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vz.szsharing.cn

[U115] JS：生成 UUID
来源：http://fu.chemitech.net.cn

crypto.randomUUID()
来源：http://si.jianghongdianzi.cn

[U116] JS：类型检查（JSDoc）
来源：http://vd.hahajie.cn

/** @param {string} name */ function f(name) {}
来源：http://wg.chemitech.net.cn

[U117] JS：单元测试
来源：http://yx.wgjwhj.cn

npm i -D vitest;  npx vitest
来源：http://xz.huixinmuqiang.cn

[U118] JS：开发服务器
来源：http://yk.wgjwhj.cn

npm i -D vite;  npx vite
来源：http://fw.jianghongdianzi.cn

[U119] JS：生产构建
来源：http://bc.huixinmuqiang.cn

npx vite build
来源：http://ys.9csxet.cn

[U120] JS：读取环境变量（Vite）
来源：http://jz.muxihuayi.cn

import.meta.env.VITE_API_URL
来源：http://id.panjiajie.cn

================================================================================
来源：http://rw.chemitech.net.cn

统计汇总
来源：http://ga.lnxyls.cn

================================================================================
来源：http://tc.shtwfgs.cn

按语言统计（条）：
来源：http://eb.jianghongdianzi.cn

Python ......... 252
来源：http://cy.bookmarksfly.cn

PHP ............ 252
来源：http://ed.nszjky.cn

JavaScript ..... 252
来源：http://fh.lnxyls.cn

TypeScript ..... 212
来源：http://iw.newstarts.cn

Java ........... 212
来源：http://qi.shxzukj.cn

Go ............. 212
来源：http://cj.shxzskj.cn

Ruby ........... 212
来源：http://jj.jctech888.com.cn

C# ............. 212
来源：http://mz.shxzukj.cn

C .............. 30
来源：http://ij.huixiangedu.cn

C++ ............ 30
来源：http://nj.huanxung.cn

SQL ............ 90
来源：http://fa.yuexingan06.cn

Bash ........... 80
来源：http://eg.bjjhwx.cn

Kotlin ......... 15
来源：http://hs.wgjwhj.cn

Swift .......... 15
来源：http://bc.shxzskj.cn

Lua ............ 10
来源：http://ks.huixinmuqiang.cn

Perl ........... 10
来源：http://we.haigaiapp.cn

Scala .......... 10
来源：http://mg.hahajie.cn

------------------------------------
来源：http://fu.huixiangedu.cn

合计 ........... 2106 条
来源：http://jb.lnxyls.cn

按章节统计：
来源：http://ic.9csxet.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ls.nszjky.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ib.jctech888.com.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ma.muxihuayi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ob.colortex.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jz.jctech888.com.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nw.wgjwhj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gc.szsharing.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tz.muxihuayi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rh.wgjwhj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cl.huixiangedu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fe.gzmigu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rg.nicolike.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wx.yuexingan06.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wh.huanxung.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://if.wgjwhj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pc.hnjuh.cn

Q SQL 专题                              90
来源：http://fg.lnxyls.cn

R Bash 专题                             80
来源：http://fd.hnjuh.cn

S C / C++ 专题                          60
来源：http://tp.shtwfgs.cn

T 其他语言补充                          60
来源：http://oz.521024.cn

U 高频实用片段                         120
来源：http://bt.yuntaijiaju.cn

------------------------------------
来源：http://le.lnxyls.cn

合计                                  2106 条
来源：http://en.nszjky.cn

--------------------------------------------------------------------------------
来源：http://jk.shxzukj.cn

使用提醒
来源：http://bt.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://uc.newstarts.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://up.shtwfgs.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vp.huanxung.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gz.muxihuayi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://li.szxytkj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fx.huanxung.cn

—— 文件结束 ——
来源：http://bc.yuntaijiaju.cn

================================================================================
来源：http://yh.shxzukj.cn

程序语言常见例子速查手册（2024 版）
来源：http://ea.shxzskj.cn

Common Programming Examples Cheat Book
来源：http://vf.haigaiapp.cn

================================================================================
来源：http://se.huanxung.cn

【收录内容】
来源：http://ea.muxihuayi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ky.hnjuh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ux.asd995.cn

SQL · Bash · C · C++
来源：http://sv.gzmigu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jb.521024.cn

【使用说明】
来源：http://ym.huixiangedu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tl.jctech888.com.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://sm.gzmigu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ha.jctech888.com.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wq.jianghongdianzi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ld.yuntaijiaju.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cf.chemitech.net.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ov.shxzskj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kk.hnjuh.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jh.newstarts.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lx.nicolike.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cd.yuexingan06.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pb.muxihuayi.cn

【文件统计】
来源：http://xs.szxytkj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cy.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://qo.hnjuh.cn

目  录
来源：http://vn.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://kp.chemitech.net.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pr.huixinmuqiang.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zc.newstarts.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ma.9csxet.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dd.bjjhwx.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zz.9csxet.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xw.521024.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fq.chemitech.net.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ex.hnjuh.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ei.jctech888.com.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rx.gzmigu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://cr.bookmarksfly.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ad.huixiangedu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ey.panjiajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qo.shxzukj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gy.muxihuayi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pa.muxihuayi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yq.jctech888.com.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://eh.wgjwhj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jo.colortex.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ec.lnxyls.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ju.haigaiapp.cn

================================================================================
来源：http://ji.colortex.cn

A. 基础语法与类型
来源：http://zo.shtwfgs.cn

================================================================================
来源：http://pu.9csxet.cn

[A01] Hello World
来源：http://hc.bjjhwx.cn

Py:   print("Hello, World!")
来源：http://hl.hahajie.cn

PHP:  echo "Hello, World!";
来源：http://qa.gzmigu.cn

JS:   console.log("Hello, World!");
来源：http://zi.newstarts.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ca.nszjky.cn

Java: System.out.println("Hello, World!");
来源：http://pv.hnjuh.cn

Go:   fmt.Println("Hello, World!")
来源：http://vw.yuntaijiaju.cn

Ruby: puts "Hello, World!"
来源：http://ji.huanxung.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://he.yuntaijiaju.cn

[A02] 变量声明与赋值
来源：http://sy.colortex.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qr.hahajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://cg.szxytkj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://yc.shxzskj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sz.asd995.cn

Java: String name = "Alex"; int age = 20;
来源：http://sk.haigaiapp.cn

Go:   name := "Alex"; age := 20
来源：http://vc.jianghongdianzi.cn

Ruby: name = "Alex"; age = 20
来源：http://eq.bjjhwx.cn

C#:   string name = "Alex"; int age = 20;
来源：http://xg.szxytkj.cn

[A03] 常量定义
来源：http://sy.yuntaijiaju.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ka.9csxet.cn

PHP:  const PI = 3.14159;
来源：http://hh.bookmarksfly.cn

JS:   const PI = 3.14159;
来源：http://gp.wgjwhj.cn

TS:   const PI: number = 3.14159;
来源：http://mo.hahajie.cn

Java: static final double PI = 3.14159;
来源：http://ip.shxzukj.cn

Go:   const PI = 3.14159
来源：http://fi.nicolike.cn


<!-- 参考信息 -->