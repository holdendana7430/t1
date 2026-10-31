代发 wailian999

[U29] Py：属性校验
来源：http://md.9csxet.cn

@property 与 @x.setter 配合
来源：http://ex.lnxyls.cn

[U30] Py：数据类
来源：http://lw.9csxet.cn

@dataclass(slots=True)
来源：http://yx.shxzukj.cn

[U31] Py：单测
来源：http://lv.shxzukj.cn

python -m pytest -q
来源：http://ma.colortex.cn

[U32] Py：代码格式化
来源：http://az.asd995.cn

ruff format . && ruff check --fix .
来源：http://vq.nszjky.cn

[U33] Py：打包发布
来源：http://wz.wgjwhj.cn

python -m build  （依赖 pyproject.toml）
来源：http://lu.wgjwhj.cn

[U34] Py：判断编码
来源：http://nt.shxzukj.cn

chardet.detect(raw)
来源：http://uq.huixinmuqiang.cn

[U35] Py：发送邮件
来源：http://ik.muxihuayi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tp.bjjhwx.cn

[U36] Py：定时任务
来源：http://yf.szxytkj.cn

schedule.every(10).minutes.do(job)
来源：http://jh.hahajie.cn

[U37] Py：读写 Excel
来源：http://yi.panjiajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ou.shxzskj.cn

[U38] Py：获取脚本所在目录
来源：http://iw.szxytkj.cn

Path(__file__).resolve().parent
来源：http://pr.yuntaijiaju.cn

[U39] Py：判断是否在交互环境
来源：http://bn.shxzskj.cn

sys.stdout.isatty()
来源：http://jd.521024.cn

[U40] Py：打印到标准错误
来源：http://we.huanxung.cn

print("err", file=sys.stderr)
来源：http://xv.521024.cn

[U41] PHP：初始化 Composer 项目
来源：http://in.huixiangedu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ru.asd995.cn

[U42] PHP：PSR-4 自动加载
来源：http://jv.jianghongdianzi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nt.521024.cn

[U43] PHP：声明命名空间
来源：http://cl.yuexingan06.cn

namespace App\Http;
来源：http://yo.yuexingan06.cn

[U44] PHP：开启严格类型
来源：http://do.chemitech.net.cn

declare(strict_types=1);
来源：http://ua.nicolike.cn

[U45] PHP：类型声明与返回类型
来源：http://en.shxzukj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://af.lnxyls.cn

[U46] PHP：可空类型
来源：http://cs.gzmigu.cn

?string $name = null
来源：http://fb.muxihuayi.cn

[U47] PHP：联合类型
来源：http://qq.shxzskj.cn

int|string $id
来源：http://bz.nicolike.cn

[U48] PHP：纯枚举
来源：http://zh.yuntaijiaju.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pf.yuexingan06.cn

[U49] PHP：只读属性
来源：http://jq.panjiajie.cn

public readonly string $name
来源：http://oi.chemitech.net.cn

[U50] PHP：构造器属性提升
来源：http://ge.yuntaijiaju.cn

public function __construct(private int $id) {}
来源：http://va.yuntaijiaju.cn

[U51] PHP：数组解构
来源：http://wk.muxihuayi.cn

[$a, $b] = $arr;
来源：http://am.haigaiapp.cn

[U52] PHP：箭头函数
来源：http://sn.gzmigu.cn

$double = fn($x) => $x * 2;
来源：http://zm.hnjuh.cn

[U53] PHP：空合并运算符
来源：http://my.shxzukj.cn

$v = $a ?? $b ?? "default";
来源：http://sx.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://yr.bookmarksfly.cn

$obj?->method()
来源：http://qd.colortex.cn

[U55] PHP：match 表达式
来源：http://vm.jctech888.com.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ir.nszjky.cn

[U56] PHP：命名参数
来源：http://ek.colortex.cn

f(a: 1, b: 2)
来源：http://ig.bjjhwx.cn

[U57] PHP：字符串插值
来源：http://fm.asd995.cn

"值: {$a}"
来源：http://oo.szxytkj.cn

[U58] PHP：数组三件套
来源：http://lf.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zp.9csxet.cn

[U59] PHP：自定义排序
来源：http://ot.hnjuh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fx.huixiangedu.cn

[U60] PHP：JSON 编解码
来源：http://sv.muxihuayi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cd.jctech888.com.cn

[U61] PHP：正则
来源：http://sr.muxihuayi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vk.gzmigu.cn

[U62] PHP：日期对象
来源：http://of.huixiangedu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gd.shtwfgs.cn

[U63] PHP：文件读写
来源：http://uw.hahajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://iw.yuntaijiaju.cn

[U64] PHP：目录遍历
来源：http://yz.haigaiapp.cn

glob("dir/*.php");  scandir("dir");
来源：http://ou.asd995.cn

[U65] PHP：会话
来源：http://mx.jctech888.com.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xp.shtwfgs.cn

[U66] PHP：设置 Cookie
来源：http://mv.lnxyls.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ej.gzmigu.cn

[U67] PHP：处理文件上传
来源：http://lm.9csxet.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ys.huixinmuqiang.cn

[U68] PHP：PDO 连接
来源：http://xr.nicolike.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lr.shxzukj.cn

[U69] PHP：PDO 预处理
来源：http://za.gzmigu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nv.lnxyls.cn

[U70] PHP：PDO 事务
来源：http://mr.yuntaijiaju.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://an.szsharing.cn

[U71] PHP：抛出异常
来源：http://iq.shxzukj.cn

throw new RuntimeException("失败", 500);
来源：http://yt.hahajie.cn

[U72] PHP：写错误日志
来源：http://cp.shtwfgs.cn

error_log("失败: " . $e->getMessage());
来源：http://ko.yuexingan06.cn

[U73] PHP：读取 ini 配置
来源：http://go.nicolike.cn

parse_ini_file("config.ini", true)
来源：http://ze.jianghongdianzi.cn

[U74] PHP：读取环境变量
来源：http://go.nszjky.cn

getenv("APP_ENV") ?: "production"
来源：http://te.jctech888.com.cn

[U75] PHP：依赖注入
来源：http://hj.muxihuayi.cn

composer require psr/container
来源：http://kb.lnxyls.cn

[U76] PHP：简单路由
来源：http://mp.shxzukj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kv.shtwfgs.cn

[U77] PHP：模板渲染
来源：http://cy.szsharing.cn

composer require twig/twig
来源：http://kh.jctech888.com.cn

[U78] PHP：单元测试
来源：http://sq.jctech888.com.cn

composer require --dev phpunit/phpunit
来源：http://pa.shxzskj.cn

[U79] PHP：静态分析
来源：http://fg.jctech888.com.cn

composer require --dev phpstan/phpstan
来源：http://vg.huixiangedu.cn

[U80] PHP：代码规范修复
来源：http://lc.szsharing.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ya.newstarts.cn

[U81] JS：初始化项目
来源：http://ur.colortex.cn

npm init -y;  npm i express
来源：http://eo.asd995.cn

[U82] JS：package.json 脚本
来源：http://ws.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://km.521024.cn

[U83] JS：ES Module 导入导出
来源：http://oq.yuntaijiaju.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vi.jctech888.com.cn

[U84] JS：CommonJS 写法
来源：http://dq.shxzukj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gt.yuntaijiaju.cn

[U85] JS：可选链
来源：http://se.wgjwhj.cn

a?.b?.c
来源：http://sn.521024.cn

[U86] JS：空值合并
来源：http://uf.muxihuayi.cn

a ?? b
来源：http://qj.chemitech.net.cn

[U87] JS：解构默认值
来源：http://sg.huixiangedu.cn

const { a = 1, b = 2 } = obj;
来源：http://it.yuexingan06.cn

[U88] JS：对象展开合并
来源：http://ql.jctech888.com.cn

{ ...a, ...b }
来源：http://qc.shxzskj.cn

[U89] JS：数组去重
来源：http://ay.hnjuh.cn

[...new Set(arr)]
来源：http://vm.huixinmuqiang.cn

[U90] JS：数字数组排序
来源：http://eb.huanxung.cn

[...arr].sort((a, b) => a - b)
来源：http://lw.9csxet.cn

[U91] JS：对象键值遍历
来源：http://zs.hnjuh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yb.shxzukj.cn

[U92] JS：深拷贝
来源：http://kx.hnjuh.cn

structuredClone(obj)
来源：http://lb.yuntaijiaju.cn

[U93] JS：模板字符串
来源：http://ly.haigaiapp.cn

`共 ${n} 条`
来源：http://fr.asd995.cn

[U94] JS：箭头函数
来源：http://bo.hnjuh.cn

const double = x => x * 2;
来源：http://mg.lnxyls.cn

[U95] JS：Promise 包装
来源：http://py.wgjwhj.cn

new Promise((resolve, reject) => {})
来源：http://xl.panjiajie.cn

[U96] JS：async/await 与异常
来源：http://xf.huixiangedu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rj.huixiangedu.cn

[U97] JS：并发请求
来源：http://gh.szsharing.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://cl.panjiajie.cn

[U98] JS：fetch 带 JSON
来源：http://ed.nszjky.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mz.shxzukj.cn

[U99] JS：事件监听
来源：http://lt.muxihuayi.cn

el.addEventListener("click", e => {})
来源：http://lz.newstarts.cn

[U100] JS：DOM 查询
来源：http://wu.bookmarksfly.cn

document.querySelector(".item")
来源：http://wb.chemitech.net.cn

[U101] JS：classList 操作
来源：http://uo.haigaiapp.cn

el.classList.toggle("active")
来源：http://tj.521024.cn

[U102] JS：本地存储
来源：http://ck.asd995.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jp.szxytkj.cn

[U103] JS：定时器
来源：http://dq.521024.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cm.gzmigu.cn

[U104] JS：防抖
来源：http://ci.shxzukj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wj.jctech888.com.cn

[U105] JS：节流
来源：http://mk.9csxet.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hq.chemitech.net.cn

[U106] JS：日期格式化
来源：http://ld.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cl.huanxung.cn

[U107] JS：数字千分位
来源：http://so.huixinmuqiang.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hw.yuntaijiaju.cn

[U108] JS：随机整数
来源：http://gp.yuexingan06.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vw.colortex.cn

[U109] JS：数组分组
来源：http://zy.huanxung.cn

Object.groupBy(arr, x => x.type)
来源：http://cc.lnxyls.cn

[U110] JS：数组分块
来源：http://aj.shxzukj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://aj.chemitech.net.cn

[U111] JS：对象转 Map
来源：http://iv.haigaiapp.cn

new Map(Object.entries(obj))
来源：http://zz.9csxet.cn

[U112] JS：字符串补位
来源：http://cy.bjjhwx.cn

"7".padStart(3, "0")
来源：http://jz.lnxyls.cn

[U113] JS：正则替换全部
来源：http://ud.shxzukj.cn

s.replaceAll("a", "b")
来源：http://db.hahajie.cn

[U114] JS：JSON 深比较
来源：http://ui.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xx.bookmarksfly.cn

[U115] JS：生成 UUID
来源：http://io.yuntaijiaju.cn

crypto.randomUUID()
来源：http://ck.gzmigu.cn

[U116] JS：类型检查（JSDoc）
来源：http://dw.hnjuh.cn

/** @param {string} name */ function f(name) {}
来源：http://ix.chemitech.net.cn

[U117] JS：单元测试
来源：http://zz.jianghongdianzi.cn

npm i -D vitest;  npx vitest
来源：http://zz.szsharing.cn

[U118] JS：开发服务器
来源：http://oi.bjjhwx.cn

npm i -D vite;  npx vite
来源：http://cp.yuntaijiaju.cn

[U119] JS：生产构建
来源：http://ho.chemitech.net.cn

npx vite build
来源：http://in.bookmarksfly.cn

[U120] JS：读取环境变量（Vite）
来源：http://qz.hahajie.cn

import.meta.env.VITE_API_URL
来源：http://bp.shxzskj.cn

================================================================================
来源：http://hm.9csxet.cn

统计汇总
来源：http://eu.hahajie.cn

================================================================================
来源：http://lc.bookmarksfly.cn

按语言统计（条）：
来源：http://au.szxytkj.cn

Python ......... 252
来源：http://sx.muxihuayi.cn

PHP ............ 252
来源：http://qr.yuexingan06.cn

JavaScript ..... 252
来源：http://jf.bjjhwx.cn

TypeScript ..... 212
来源：http://pw.bookmarksfly.cn

Java ........... 212
来源：http://ae.nicolike.cn

Go ............. 212
来源：http://vj.bookmarksfly.cn

Ruby ........... 212
来源：http://ng.yuexingan06.cn

C# ............. 212
来源：http://cb.yuexingan06.cn

C .............. 30
来源：http://dk.lnxyls.cn

C++ ............ 30
来源：http://mj.nicolike.cn

SQL ............ 90
来源：http://qd.shxzukj.cn

Bash ........... 80
来源：http://xz.hahajie.cn

Kotlin ......... 15
来源：http://gb.yuexingan06.cn

Swift .......... 15
来源：http://kq.hnjuh.cn

Lua ............ 10
来源：http://mh.wgjwhj.cn

Perl ........... 10
来源：http://am.521024.cn

Scala .......... 10
来源：http://pn.9csxet.cn

------------------------------------
来源：http://yu.gzmigu.cn

合计 ........... 2106 条
来源：http://xo.huanxung.cn

按章节统计：
来源：http://zz.gzmigu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://me.shxzskj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kt.wgjwhj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jd.panjiajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vy.shtwfgs.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gc.gzmigu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dn.muxihuayi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ot.shtwfgs.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hy.jctech888.com.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vd.jianghongdianzi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wg.colortex.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fi.chemitech.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zz.jctech888.com.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ta.gzmigu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cb.bjjhwx.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yl.bjjhwx.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://es.huixinmuqiang.cn

Q SQL 专题                              90
来源：http://tr.panjiajie.cn

R Bash 专题                             80
来源：http://ep.yuntaijiaju.cn

S C / C++ 专题                          60
来源：http://jh.nicolike.cn

T 其他语言补充                          60
来源：http://mm.huanxung.cn

U 高频实用片段                         120
来源：http://ti.haigaiapp.cn

------------------------------------
来源：http://uy.huanxung.cn

合计                                  2106 条
来源：http://gk.nicolike.cn

--------------------------------------------------------------------------------
来源：http://xe.jianghongdianzi.cn

使用提醒
来源：http://sn.szsharing.cn

--------------------------------------------------------------------------------
来源：http://ut.huixinmuqiang.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sx.bookmarksfly.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sh.colortex.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ib.nszjky.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qw.jctech888.com.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://co.szxytkj.cn

—— 文件结束 ——
来源：http://jp.shxzskj.cn

================================================================================
来源：http://vo.shxzskj.cn

程序语言常见例子速查手册（2024 版）
来源：http://ao.9csxet.cn

Common Programming Examples Cheat Book
来源：http://er.shxzukj.cn

================================================================================
来源：http://jy.521024.cn

【收录内容】
来源：http://qb.huanxung.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.colortex.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zd.yuntaijiaju.cn

SQL · Bash · C · C++
来源：http://ed.asd995.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wv.muxihuayi.cn

【使用说明】
来源：http://yi.szxytkj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yt.jctech888.com.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ms.huanxung.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vy.chemitech.net.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://en.shtwfgs.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://jy.wgjwhj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sa.panjiajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nm.colortex.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dz.bookmarksfly.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bf.wgjwhj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wf.bjjhwx.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fl.newstarts.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hu.huixinmuqiang.cn

【文件统计】
来源：http://aq.lnxyls.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yt.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://na.colortex.cn

目  录
来源：http://hd.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://ic.szsharing.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dh.haigaiapp.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ea.newstarts.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wc.colortex.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cm.huanxung.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fm.colortex.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qh.nicolike.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dq.szsharing.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nm.panjiajie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pm.wgjwhj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qj.chemitech.net.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://oe.jctech888.com.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bl.hahajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://km.bjjhwx.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hc.wgjwhj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://go.huixinmuqiang.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://be.521024.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://oa.gzmigu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gt.szxytkj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hv.szsharing.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yg.huixinmuqiang.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pq.szxytkj.cn

================================================================================
来源：http://bf.szxytkj.cn

A. 基础语法与类型
来源：http://ky.panjiajie.cn

================================================================================
来源：http://ov.shtwfgs.cn

[A01] Hello World
来源：http://od.colortex.cn

Py:   print("Hello, World!")
来源：http://gt.bookmarksfly.cn

PHP:  echo "Hello, World!";
来源：http://iv.bookmarksfly.cn

JS:   console.log("Hello, World!");
来源：http://wu.huixinmuqiang.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dv.panjiajie.cn

Java: System.out.println("Hello, World!");
来源：http://pl.gzmigu.cn

Go:   fmt.Println("Hello, World!")
来源：http://sm.newstarts.cn

Ruby: puts "Hello, World!"
来源：http://yy.bookmarksfly.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://sf.shxzskj.cn


<!-- 参考信息 -->