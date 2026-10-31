代发 wailian999

[U33] Py：打包发布
来源：http://nv.hnjuh.cn

python -m build  （依赖 pyproject.toml）
来源：http://ju.9csxet.cn

[U34] Py：判断编码
来源：http://cy.szxytkj.cn

chardet.detect(raw)
来源：http://uz.muxihuayi.cn

[U35] Py：发送邮件
来源：http://py.shtwfgs.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ed.hahajie.cn

[U36] Py：定时任务
来源：http://tz.bookmarksfly.cn

schedule.every(10).minutes.do(job)
来源：http://uw.wgjwhj.cn

[U37] Py：读写 Excel
来源：http://sq.521024.cn

pandas.read_excel / DataFrame.to_excel
来源：http://im.lnxyls.cn

[U38] Py：获取脚本所在目录
来源：http://fb.yuntaijiaju.cn

Path(__file__).resolve().parent
来源：http://cy.muxihuayi.cn

[U39] Py：判断是否在交互环境
来源：http://qo.lnxyls.cn

sys.stdout.isatty()
来源：http://yr.szxytkj.cn

[U40] Py：打印到标准错误
来源：http://yo.colortex.cn

print("err", file=sys.stderr)
来源：http://rp.asd995.cn

[U41] PHP：初始化 Composer 项目
来源：http://ka.yuexingan06.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cx.szxytkj.cn

[U42] PHP：PSR-4 自动加载
来源：http://ju.panjiajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fs.newstarts.cn

[U43] PHP：声明命名空间
来源：http://cc.hahajie.cn

namespace App\Http;
来源：http://ow.haigaiapp.cn

[U44] PHP：开启严格类型
来源：http://cw.yuntaijiaju.cn

declare(strict_types=1);
来源：http://rd.asd995.cn

[U45] PHP：类型声明与返回类型
来源：http://yy.haigaiapp.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zd.jctech888.com.cn

[U46] PHP：可空类型
来源：http://fr.huixinmuqiang.cn

?string $name = null
来源：http://vg.shtwfgs.cn

[U47] PHP：联合类型
来源：http://ty.newstarts.cn

int|string $id
来源：http://xq.shxzukj.cn

[U48] PHP：纯枚举
来源：http://tg.shxzskj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rs.lnxyls.cn

[U49] PHP：只读属性
来源：http://qz.panjiajie.cn

public readonly string $name
来源：http://de.haigaiapp.cn

[U50] PHP：构造器属性提升
来源：http://yd.shxzukj.cn

public function __construct(private int $id) {}
来源：http://ei.jianghongdianzi.cn

[U51] PHP：数组解构
来源：http://bv.yuexingan06.cn

[$a, $b] = $arr;
来源：http://wp.jctech888.com.cn

[U52] PHP：箭头函数
来源：http://ua.huixiangedu.cn

$double = fn($x) => $x * 2;
来源：http://ab.huanxung.cn

[U53] PHP：空合并运算符
来源：http://we.szxytkj.cn

$v = $a ?? $b ?? "default";
来源：http://vn.nszjky.cn

[U54] PHP：空安全调用
来源：http://mh.newstarts.cn

$obj?->method()
来源：http://oj.nszjky.cn

[U55] PHP：match 表达式
来源：http://mp.haigaiapp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cq.yuexingan06.cn

[U56] PHP：命名参数
来源：http://pc.jctech888.com.cn

f(a: 1, b: 2)
来源：http://ci.muxihuayi.cn

[U57] PHP：字符串插值
来源：http://wj.szxytkj.cn

"值: {$a}"
来源：http://nx.huanxung.cn

[U58] PHP：数组三件套
来源：http://lv.haigaiapp.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://or.yuntaijiaju.cn

[U59] PHP：自定义排序
来源：http://dn.9csxet.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ea.gzmigu.cn

[U60] PHP：JSON 编解码
来源：http://hg.hahajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pf.521024.cn

[U61] PHP：正则
来源：http://sh.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fy.muxihuayi.cn

[U62] PHP：日期对象
来源：http://on.nszjky.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ox.shtwfgs.cn

[U63] PHP：文件读写
来源：http://dg.szsharing.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lt.huixinmuqiang.cn

[U64] PHP：目录遍历
来源：http://ku.521024.cn

glob("dir/*.php");  scandir("dir");
来源：http://wk.9csxet.cn

[U65] PHP：会话
来源：http://zw.hahajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vi.yuexingan06.cn

[U66] PHP：设置 Cookie
来源：http://jz.huanxung.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rv.szsharing.cn

[U67] PHP：处理文件上传
来源：http://rx.newstarts.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rk.lnxyls.cn

[U68] PHP：PDO 连接
来源：http://oq.huixinmuqiang.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gb.huixiangedu.cn

[U69] PHP：PDO 预处理
来源：http://dk.yuexingan06.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mu.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://zf.gzmigu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://se.asd995.cn

[U71] PHP：抛出异常
来源：http://xh.yuntaijiaju.cn

throw new RuntimeException("失败", 500);
来源：http://uc.panjiajie.cn

[U72] PHP：写错误日志
来源：http://qk.newstarts.cn

error_log("失败: " . $e->getMessage());
来源：http://sz.shxzskj.cn

[U73] PHP：读取 ini 配置
来源：http://qe.haigaiapp.cn

parse_ini_file("config.ini", true)
来源：http://qx.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://ck.shtwfgs.cn

getenv("APP_ENV") ?: "production"
来源：http://ly.asd995.cn

[U75] PHP：依赖注入
来源：http://be.panjiajie.cn

composer require psr/container
来源：http://je.nszjky.cn

[U76] PHP：简单路由
来源：http://wr.chemitech.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yl.521024.cn

[U77] PHP：模板渲染
来源：http://sf.huixiangedu.cn

composer require twig/twig
来源：http://gf.huanxung.cn

[U78] PHP：单元测试
来源：http://wg.521024.cn

composer require --dev phpunit/phpunit
来源：http://bl.jctech888.com.cn

[U79] PHP：静态分析
来源：http://jj.yuexingan06.cn

composer require --dev phpstan/phpstan
来源：http://tn.colortex.cn

[U80] PHP：代码规范修复
来源：http://zq.bjjhwx.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://al.shtwfgs.cn

[U81] JS：初始化项目
来源：http://qv.szsharing.cn

npm init -y;  npm i express
来源：http://tl.huixiangedu.cn

[U82] JS：package.json 脚本
来源：http://sa.shtwfgs.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mn.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://ec.szxytkj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hf.colortex.cn

[U84] JS：CommonJS 写法
来源：http://jr.shxzskj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zh.muxihuayi.cn

[U85] JS：可选链
来源：http://bx.muxihuayi.cn

a?.b?.c
来源：http://jj.nszjky.cn

[U86] JS：空值合并
来源：http://jm.nicolike.cn

a ?? b
来源：http://bm.shtwfgs.cn

[U87] JS：解构默认值
来源：http://ub.wgjwhj.cn

const { a = 1, b = 2 } = obj;
来源：http://nk.muxihuayi.cn

[U88] JS：对象展开合并
来源：http://sg.huixiangedu.cn

{ ...a, ...b }
来源：http://xl.colortex.cn

[U89] JS：数组去重
来源：http://vw.szsharing.cn

[...new Set(arr)]
来源：http://ww.bjjhwx.cn

[U90] JS：数字数组排序
来源：http://dc.chemitech.net.cn

[...arr].sort((a, b) => a - b)
来源：http://hc.panjiajie.cn

[U91] JS：对象键值遍历
来源：http://hk.yuexingan06.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ko.huixiangedu.cn

[U92] JS：深拷贝
来源：http://hc.nszjky.cn

structuredClone(obj)
来源：http://ue.huixiangedu.cn

[U93] JS：模板字符串
来源：http://gj.jctech888.com.cn

`共 ${n} 条`
来源：http://wy.chemitech.net.cn

[U94] JS：箭头函数
来源：http://rn.bjjhwx.cn

const double = x => x * 2;
来源：http://up.nszjky.cn

[U95] JS：Promise 包装
来源：http://xw.hahajie.cn

new Promise((resolve, reject) => {})
来源：http://aw.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://wt.hnjuh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vb.colortex.cn

[U97] JS：并发请求
来源：http://vs.lnxyls.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hp.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://dr.gzmigu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wy.muxihuayi.cn

[U99] JS：事件监听
来源：http://sk.nicolike.cn

el.addEventListener("click", e => {})
来源：http://wf.gzmigu.cn

[U100] JS：DOM 查询
来源：http://qw.nszjky.cn

document.querySelector(".item")
来源：http://gi.muxihuayi.cn

[U101] JS：classList 操作
来源：http://kb.gzmigu.cn

el.classList.toggle("active")
来源：http://cg.chemitech.net.cn

[U102] JS：本地存储
来源：http://it.gzmigu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://op.lnxyls.cn

[U103] JS：定时器
来源：http://vy.newstarts.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sa.shxzskj.cn

[U104] JS：防抖
来源：http://cj.panjiajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://be.chemitech.net.cn

[U105] JS：节流
来源：http://cu.9csxet.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bq.szsharing.cn

[U106] JS：日期格式化
来源：http://ws.jianghongdianzi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xm.newstarts.cn

[U107] JS：数字千分位
来源：http://wa.jctech888.com.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ak.wgjwhj.cn

[U108] JS：随机整数
来源：http://hv.huanxung.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jv.asd995.cn

[U109] JS：数组分组
来源：http://hd.chemitech.net.cn

Object.groupBy(arr, x => x.type)
来源：http://lu.huixinmuqiang.cn

[U110] JS：数组分块
来源：http://ad.colortex.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jc.nszjky.cn

[U111] JS：对象转 Map
来源：http://sg.jctech888.com.cn

new Map(Object.entries(obj))
来源：http://ki.wgjwhj.cn

[U112] JS：字符串补位
来源：http://bg.szxytkj.cn

"7".padStart(3, "0")
来源：http://hn.wgjwhj.cn

[U113] JS：正则替换全部
来源：http://gm.nszjky.cn

s.replaceAll("a", "b")
来源：http://tt.huixiangedu.cn

[U114] JS：JSON 深比较
来源：http://yo.panjiajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tw.szxytkj.cn

[U115] JS：生成 UUID
来源：http://fh.asd995.cn

crypto.randomUUID()
来源：http://ne.lnxyls.cn

[U116] JS：类型检查（JSDoc）
来源：http://oi.jctech888.com.cn

/** @param {string} name */ function f(name) {}
来源：http://pl.jianghongdianzi.cn

[U117] JS：单元测试
来源：http://zf.yuexingan06.cn

npm i -D vitest;  npx vitest
来源：http://th.nicolike.cn

[U118] JS：开发服务器
来源：http://cd.colortex.cn

npm i -D vite;  npx vite
来源：http://gk.huixinmuqiang.cn

[U119] JS：生产构建
来源：http://ga.colortex.cn

npx vite build
来源：http://qi.asd995.cn

[U120] JS：读取环境变量（Vite）
来源：http://hz.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://tf.521024.cn

================================================================================
来源：http://ya.jianghongdianzi.cn

统计汇总
来源：http://of.jctech888.com.cn

================================================================================
来源：http://ab.jianghongdianzi.cn

按语言统计（条）：
来源：http://ao.asd995.cn

Python ......... 252
来源：http://sm.huixiangedu.cn

PHP ............ 252
来源：http://tg.gzmigu.cn

JavaScript ..... 252
来源：http://yp.asd995.cn

TypeScript ..... 212
来源：http://tz.chemitech.net.cn

Java ........... 212
来源：http://rf.bjjhwx.cn

Go ............. 212
来源：http://bw.asd995.cn

Ruby ........... 212
来源：http://sz.asd995.cn

C# ............. 212
来源：http://wa.huixiangedu.cn

C .............. 30
来源：http://xi.9csxet.cn

C++ ............ 30
来源：http://tc.gzmigu.cn

SQL ............ 90
来源：http://rj.lnxyls.cn

Bash ........... 80
来源：http://mu.gzmigu.cn

Kotlin ......... 15
来源：http://oq.jctech888.com.cn

Swift .......... 15
来源：http://vk.szsharing.cn

Lua ............ 10
来源：http://fp.lnxyls.cn

Perl ........... 10
来源：http://so.jianghongdianzi.cn

Scala .......... 10
来源：http://xo.jctech888.com.cn

------------------------------------
来源：http://rt.huanxung.cn

合计 ........... 2106 条
来源：http://gb.lnxyls.cn

按章节统计：
来源：http://vy.newstarts.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wz.wgjwhj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ft.hnjuh.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kp.huixinmuqiang.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vq.newstarts.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wz.colortex.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://js.colortex.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ad.yuexingan06.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://os.newstarts.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://za.chemitech.net.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gi.newstarts.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://be.colortex.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://de.haigaiapp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bk.nicolike.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://br.asd995.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xh.gzmigu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mw.521024.cn

Q SQL 专题                              90
来源：http://yt.szsharing.cn

R Bash 专题                             80
来源：http://rh.shxzskj.cn

S C / C++ 专题                          60
来源：http://ox.9csxet.cn

T 其他语言补充                          60
来源：http://rb.bjjhwx.cn

U 高频实用片段                         120
来源：http://mh.jianghongdianzi.cn

------------------------------------
来源：http://de.asd995.cn

合计                                  2106 条
来源：http://nq.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://lr.huixiangedu.cn

使用提醒
来源：http://oy.newstarts.cn

--------------------------------------------------------------------------------
来源：http://ow.lnxyls.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ao.huixiangedu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zd.huixiangedu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.shtwfgs.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zu.huixiangedu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xi.asd995.cn

—— 文件结束 ——
来源：http://mk.chemitech.net.cn

================================================================================
来源：http://ms.gzmigu.cn

程序语言常见例子速查手册（2024 版）
来源：http://sm.szxytkj.cn

Common Programming Examples Cheat Book
来源：http://cn.chemitech.net.cn

================================================================================
来源：http://cl.szsharing.cn

【收录内容】
来源：http://nz.9csxet.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://os.asd995.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ib.muxihuayi.cn

SQL · Bash · C · C++
来源：http://ne.shtwfgs.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yz.jianghongdianzi.cn

【使用说明】
来源：http://kt.shxzukj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tv.szsharing.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gi.hahajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ue.9csxet.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://np.jianghongdianzi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wr.colortex.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mi.wgjwhj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://es.newstarts.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ku.nszjky.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gr.jctech888.com.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ag.wgjwhj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qw.asd995.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://em.asd995.cn

【文件统计】
来源：http://xr.shxzukj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fd.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://jd.colortex.cn

目  录
来源：http://xw.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://hc.muxihuayi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wi.521024.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ya.shxzskj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fg.shxzskj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://gm.colortex.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vq.jctech888.com.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fb.newstarts.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://pf.szsharing.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vv.huanxung.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sk.wgjwhj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vn.hnjuh.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jk.bjjhwx.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yt.yuexingan06.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hi.huixinmuqiang.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fw.jctech888.com.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yf.asd995.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ee.wgjwhj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fh.hnjuh.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xu.521024.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ou.haigaiapp.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fw.muxihuayi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://if.jianghongdianzi.cn

================================================================================
来源：http://vx.9csxet.cn

A. 基础语法与类型
来源：http://ry.huixiangedu.cn

================================================================================
来源：http://az.szsharing.cn

[A01] Hello World
来源：http://fg.haigaiapp.cn

Py:   print("Hello, World!")
来源：http://jw.yuexingan06.cn

PHP:  echo "Hello, World!";
来源：http://hh.bjjhwx.cn

JS:   console.log("Hello, World!");
来源：http://rr.chemitech.net.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sv.huixinmuqiang.cn

Java: System.out.println("Hello, World!");
来源：http://io.haigaiapp.cn

Go:   fmt.Println("Hello, World!")
来源：http://yx.panjiajie.cn

Ruby: puts "Hello, World!"
来源：http://vo.szsharing.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://pt.wgjwhj.cn

[A02] 变量声明与赋值
来源：http://ft.bjjhwx.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://el.szsharing.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://tk.hnjuh.cn

JS:   let name = "Alex"; const age = 20;
来源：http://cv.haigaiapp.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bg.huixiangedu.cn

Java: String name = "Alex"; int age = 20;
来源：http://dr.szsharing.cn

Go:   name := "Alex"; age := 20
来源：http://ez.lnxyls.cn

Ruby: name = "Alex"; age = 20
来源：http://ch.huixiangedu.cn


<!-- 参考信息 -->