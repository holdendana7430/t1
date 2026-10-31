代发 wailian999

[U31] Py：单测
来源：http://gg.yuntaijiaju.cn

python -m pytest -q
来源：http://zp.szsharing.cn

[U32] Py：代码格式化
来源：http://nm.szsharing.cn

ruff format . && ruff check --fix .
来源：http://im.gzmigu.cn

[U33] Py：打包发布
来源：http://bs.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://ui.muxihuayi.cn

[U34] Py：判断编码
来源：http://ko.asd995.cn

chardet.detect(raw)
来源：http://wx.gzmigu.cn

[U35] Py：发送邮件
来源：http://qc.hahajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tl.shtwfgs.cn

[U36] Py：定时任务
来源：http://tn.shxzukj.cn

schedule.every(10).minutes.do(job)
来源：http://co.9csxet.cn

[U37] Py：读写 Excel
来源：http://qf.haigaiapp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://oc.hnjuh.cn

[U38] Py：获取脚本所在目录
来源：http://xu.newstarts.cn

Path(__file__).resolve().parent
来源：http://ea.shxzskj.cn

[U39] Py：判断是否在交互环境
来源：http://si.muxihuayi.cn

sys.stdout.isatty()
来源：http://kj.chemitech.net.cn

[U40] Py：打印到标准错误
来源：http://lq.szsharing.cn

print("err", file=sys.stderr)
来源：http://yq.bookmarksfly.cn

[U41] PHP：初始化 Composer 项目
来源：http://oi.newstarts.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rv.colortex.cn

[U42] PHP：PSR-4 自动加载
来源：http://ok.lnxyls.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ys.9csxet.cn

[U43] PHP：声明命名空间
来源：http://xz.shtwfgs.cn

namespace App\Http;
来源：http://fz.muxihuayi.cn

[U44] PHP：开启严格类型
来源：http://uv.9csxet.cn

declare(strict_types=1);
来源：http://xr.wgjwhj.cn

[U45] PHP：类型声明与返回类型
来源：http://lg.panjiajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ja.panjiajie.cn

[U46] PHP：可空类型
来源：http://pw.huixinmuqiang.cn

?string $name = null
来源：http://to.szxytkj.cn

[U47] PHP：联合类型
来源：http://gr.hahajie.cn

int|string $id
来源：http://al.gzmigu.cn

[U48] PHP：纯枚举
来源：http://ep.colortex.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ci.szsharing.cn

[U49] PHP：只读属性
来源：http://oj.haigaiapp.cn

public readonly string $name
来源：http://fa.huixinmuqiang.cn

[U50] PHP：构造器属性提升
来源：http://ov.huixinmuqiang.cn

public function __construct(private int $id) {}
来源：http://rz.shxzskj.cn

[U51] PHP：数组解构
来源：http://ry.newstarts.cn

[$a, $b] = $arr;
来源：http://vv.nszjky.cn

[U52] PHP：箭头函数
来源：http://ab.9csxet.cn

$double = fn($x) => $x * 2;
来源：http://cz.hahajie.cn

[U53] PHP：空合并运算符
来源：http://hb.szxytkj.cn

$v = $a ?? $b ?? "default";
来源：http://jr.panjiajie.cn

[U54] PHP：空安全调用
来源：http://dn.wgjwhj.cn

$obj?->method()
来源：http://pl.haigaiapp.cn

[U55] PHP：match 表达式
来源：http://vd.huanxung.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ee.521024.cn

[U56] PHP：命名参数
来源：http://gw.9csxet.cn

f(a: 1, b: 2)
来源：http://fv.panjiajie.cn

[U57] PHP：字符串插值
来源：http://ss.gzmigu.cn

"值: {$a}"
来源：http://hb.jctech888.com.cn

[U58] PHP：数组三件套
来源：http://gh.lnxyls.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ap.szxytkj.cn

[U59] PHP：自定义排序
来源：http://yo.shxzukj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wy.jianghongdianzi.cn

[U60] PHP：JSON 编解码
来源：http://xl.bookmarksfly.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ng.9csxet.cn

[U61] PHP：正则
来源：http://cv.colortex.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xo.9csxet.cn

[U62] PHP：日期对象
来源：http://lo.huanxung.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vo.9csxet.cn

[U63] PHP：文件读写
来源：http://uc.huixiangedu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://uo.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://zn.huixinmuqiang.cn

glob("dir/*.php");  scandir("dir");
来源：http://hk.muxihuayi.cn

[U65] PHP：会话
来源：http://zj.huixiangedu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cn.shxzukj.cn

[U66] PHP：设置 Cookie
来源：http://th.lnxyls.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wb.hnjuh.cn

[U67] PHP：处理文件上传
来源：http://oy.asd995.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jk.shtwfgs.cn

[U68] PHP：PDO 连接
来源：http://mq.yuntaijiaju.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ss.huixinmuqiang.cn

[U69] PHP：PDO 预处理
来源：http://yt.hnjuh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ht.chemitech.net.cn

[U70] PHP：PDO 事务
来源：http://rv.shxzukj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gj.newstarts.cn

[U71] PHP：抛出异常
来源：http://cq.shxzukj.cn

throw new RuntimeException("失败", 500);
来源：http://bf.szxytkj.cn

[U72] PHP：写错误日志
来源：http://co.521024.cn

error_log("失败: " . $e->getMessage());
来源：http://jy.chemitech.net.cn

[U73] PHP：读取 ini 配置
来源：http://zm.wgjwhj.cn

parse_ini_file("config.ini", true)
来源：http://cf.9csxet.cn

[U74] PHP：读取环境变量
来源：http://rt.panjiajie.cn

getenv("APP_ENV") ?: "production"
来源：http://ti.jianghongdianzi.cn

[U75] PHP：依赖注入
来源：http://wc.yuntaijiaju.cn

composer require psr/container
来源：http://hu.bjjhwx.cn

[U76] PHP：简单路由
来源：http://hr.shxzukj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tt.asd995.cn

[U77] PHP：模板渲染
来源：http://nh.521024.cn

composer require twig/twig
来源：http://fx.nicolike.cn

[U78] PHP：单元测试
来源：http://zg.hnjuh.cn

composer require --dev phpunit/phpunit
来源：http://uy.shxzskj.cn

[U79] PHP：静态分析
来源：http://xs.gzmigu.cn

composer require --dev phpstan/phpstan
来源：http://ib.muxihuayi.cn

[U80] PHP：代码规范修复
来源：http://ow.asd995.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hw.huixinmuqiang.cn

[U81] JS：初始化项目
来源：http://jh.bookmarksfly.cn

npm init -y;  npm i express
来源：http://hh.haigaiapp.cn

[U82] JS：package.json 脚本
来源：http://jf.huixinmuqiang.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bc.bookmarksfly.cn

[U83] JS：ES Module 导入导出
来源：http://vo.hnjuh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kf.521024.cn

[U84] JS：CommonJS 写法
来源：http://rj.haigaiapp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zm.newstarts.cn

[U85] JS：可选链
来源：http://rd.shxzskj.cn

a?.b?.c
来源：http://hp.yuexingan06.cn

[U86] JS：空值合并
来源：http://gh.nszjky.cn

a ?? b
来源：http://yo.hahajie.cn

[U87] JS：解构默认值
来源：http://fy.shtwfgs.cn

const { a = 1, b = 2 } = obj;
来源：http://nb.nicolike.cn

[U88] JS：对象展开合并
来源：http://dr.bjjhwx.cn

{ ...a, ...b }
来源：http://ka.yuntaijiaju.cn

[U89] JS：数组去重
来源：http://ib.colortex.cn

[...new Set(arr)]
来源：http://sy.bjjhwx.cn

[U90] JS：数字数组排序
来源：http://yz.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://nr.hahajie.cn

[U91] JS：对象键值遍历
来源：http://hl.newstarts.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cs.lnxyls.cn

[U92] JS：深拷贝
来源：http://uo.bookmarksfly.cn

structuredClone(obj)
来源：http://hj.bookmarksfly.cn

[U93] JS：模板字符串
来源：http://lm.9csxet.cn

`共 ${n} 条`
来源：http://mq.lnxyls.cn

[U94] JS：箭头函数
来源：http://im.9csxet.cn

const double = x => x * 2;
来源：http://hd.jianghongdianzi.cn

[U95] JS：Promise 包装
来源：http://vy.asd995.cn

new Promise((resolve, reject) => {})
来源：http://nx.wgjwhj.cn

[U96] JS：async/await 与异常
来源：http://nz.wgjwhj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xu.shtwfgs.cn

[U97] JS：并发请求
来源：http://dh.colortex.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://oh.shxzukj.cn

[U98] JS：fetch 带 JSON
来源：http://ip.shxzskj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pl.hahajie.cn

[U99] JS：事件监听
来源：http://kh.jianghongdianzi.cn

el.addEventListener("click", e => {})
来源：http://to.szxytkj.cn

[U100] JS：DOM 查询
来源：http://cj.huixinmuqiang.cn

document.querySelector(".item")
来源：http://rm.huanxung.cn

[U101] JS：classList 操作
来源：http://ug.jianghongdianzi.cn

el.classList.toggle("active")
来源：http://zp.newstarts.cn

[U102] JS：本地存储
来源：http://wj.shtwfgs.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xd.panjiajie.cn

[U103] JS：定时器
来源：http://yn.muxihuayi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uy.shxzskj.cn

[U104] JS：防抖
来源：http://be.haigaiapp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uj.bjjhwx.cn

[U105] JS：节流
来源：http://km.colortex.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vg.yuexingan06.cn

[U106] JS：日期格式化
来源：http://hd.haigaiapp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ai.nicolike.cn

[U107] JS：数字千分位
来源：http://py.panjiajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ti.hnjuh.cn

[U108] JS：随机整数
来源：http://co.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mm.haigaiapp.cn

[U109] JS：数组分组
来源：http://be.hnjuh.cn

Object.groupBy(arr, x => x.type)
来源：http://wa.hahajie.cn

[U110] JS：数组分块
来源：http://gg.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zk.chemitech.net.cn

[U111] JS：对象转 Map
来源：http://jg.colortex.cn

new Map(Object.entries(obj))
来源：http://mg.haigaiapp.cn

[U112] JS：字符串补位
来源：http://ax.newstarts.cn

"7".padStart(3, "0")
来源：http://iq.521024.cn

[U113] JS：正则替换全部
来源：http://il.jianghongdianzi.cn

s.replaceAll("a", "b")
来源：http://wo.shxzukj.cn

[U114] JS：JSON 深比较
来源：http://jf.asd995.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qi.9csxet.cn

[U115] JS：生成 UUID
来源：http://dl.hnjuh.cn

crypto.randomUUID()
来源：http://xe.asd995.cn

[U116] JS：类型检查（JSDoc）
来源：http://ft.huixinmuqiang.cn

/** @param {string} name */ function f(name) {}
来源：http://kz.yuntaijiaju.cn

[U117] JS：单元测试
来源：http://cd.panjiajie.cn

npm i -D vitest;  npx vitest
来源：http://kz.gzmigu.cn

[U118] JS：开发服务器
来源：http://cd.521024.cn

npm i -D vite;  npx vite
来源：http://hn.szxytkj.cn

[U119] JS：生产构建
来源：http://kq.haigaiapp.cn

npx vite build
来源：http://bl.yuntaijiaju.cn

[U120] JS：读取环境变量（Vite）
来源：http://vc.asd995.cn

import.meta.env.VITE_API_URL
来源：http://uz.huixinmuqiang.cn

================================================================================
来源：http://fq.jianghongdianzi.cn

统计汇总
来源：http://br.szsharing.cn

================================================================================
来源：http://ao.huixinmuqiang.cn

按语言统计（条）：
来源：http://cl.muxihuayi.cn

Python ......... 252
来源：http://pr.shxzskj.cn

PHP ............ 252
来源：http://gy.hahajie.cn

JavaScript ..... 252
来源：http://hz.nszjky.cn

TypeScript ..... 212
来源：http://lk.haigaiapp.cn

Java ........... 212
来源：http://nl.nicolike.cn

Go ............. 212
来源：http://mt.yuntaijiaju.cn

Ruby ........... 212
来源：http://eh.nszjky.cn

C# ............. 212
来源：http://yp.colortex.cn

C .............. 30
来源：http://ma.gzmigu.cn

C++ ............ 30
来源：http://lh.colortex.cn

SQL ............ 90
来源：http://my.wgjwhj.cn

Bash ........... 80
来源：http://gq.asd995.cn

Kotlin ......... 15
来源：http://af.jctech888.com.cn

Swift .......... 15
来源：http://vu.521024.cn

Lua ............ 10
来源：http://vq.shxzukj.cn

Perl ........... 10
来源：http://ti.shxzukj.cn

Scala .......... 10
来源：http://vm.nszjky.cn

------------------------------------
来源：http://is.wgjwhj.cn

合计 ........... 2106 条
来源：http://ja.jianghongdianzi.cn

按章节统计：
来源：http://oa.newstarts.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://om.bookmarksfly.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vn.jianghongdianzi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ks.haigaiapp.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xx.yuntaijiaju.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fp.panjiajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wb.chemitech.net.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ix.szsharing.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tn.szsharing.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ek.shxzskj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mz.bookmarksfly.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zt.shxzskj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dk.bookmarksfly.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://te.shxzskj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zs.yuntaijiaju.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mi.bjjhwx.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xa.nicolike.cn

Q SQL 专题                              90
来源：http://me.9csxet.cn

R Bash 专题                             80
来源：http://ua.szxytkj.cn

S C / C++ 专题                          60
来源：http://cm.colortex.cn

T 其他语言补充                          60
来源：http://zk.bookmarksfly.cn

U 高频实用片段                         120
来源：http://so.szxytkj.cn

------------------------------------
来源：http://ko.huixiangedu.cn

合计                                  2106 条
来源：http://eb.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://io.huixinmuqiang.cn

使用提醒
来源：http://in.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://ez.huixinmuqiang.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rp.huixiangedu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wf.jianghongdianzi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://oy.gzmigu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://em.yuexingan06.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rd.huixiangedu.cn

—— 文件结束 ——
来源：http://kj.gzmigu.cn

================================================================================
来源：http://qy.nicolike.cn

程序语言常见例子速查手册（2024 版）
来源：http://mw.asd995.cn

Common Programming Examples Cheat Book
来源：http://fe.asd995.cn

================================================================================
来源：http://hs.szsharing.cn

【收录内容】
来源：http://gy.gzmigu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://wh.haigaiapp.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rj.yuntaijiaju.cn

SQL · Bash · C · C++
来源：http://do.szsharing.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pk.panjiajie.cn

【使用说明】
来源：http://ex.szsharing.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ul.wgjwhj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wc.szsharing.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ha.haigaiapp.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xg.huixinmuqiang.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xz.gzmigu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nc.bookmarksfly.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ss.colortex.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rf.haigaiapp.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tn.yuexingan06.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sg.yuexingan06.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xt.gzmigu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gx.huixiangedu.cn

【文件统计】
来源：http://an.szxytkj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dg.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://ck.521024.cn

目  录
来源：http://az.521024.cn

--------------------------------------------------------------------------------
来源：http://hp.panjiajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gl.gzmigu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ch.muxihuayi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zx.jctech888.com.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mc.hahajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rn.yuexingan06.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ku.szxytkj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cj.huanxung.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jy.jctech888.com.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kl.colortex.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cr.shxzukj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ez.asd995.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sx.nicolike.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ko.szsharing.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ip.jianghongdianzi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uw.nszjky.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://oy.panjiajie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pq.asd995.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://iu.szxytkj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xt.jctech888.com.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://oo.huixiangedu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gu.asd995.cn

================================================================================
来源：http://fw.shxzukj.cn

A. 基础语法与类型
来源：http://jz.huixinmuqiang.cn

================================================================================
来源：http://uz.jctech888.com.cn

[A01] Hello World
来源：http://yn.yuntaijiaju.cn

Py:   print("Hello, World!")
来源：http://gj.9csxet.cn

PHP:  echo "Hello, World!";
来源：http://he.hahajie.cn

JS:   console.log("Hello, World!");
来源：http://ce.chemitech.net.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ho.yuntaijiaju.cn

Java: System.out.println("Hello, World!");
来源：http://cj.shtwfgs.cn

Go:   fmt.Println("Hello, World!")
来源：http://ve.huixinmuqiang.cn

Ruby: puts "Hello, World!"
来源：http://zn.szxytkj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ok.521024.cn

[A02] 变量声明与赋值
来源：http://ji.szxytkj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ve.asd995.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ej.shxzskj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ya.haigaiapp.cn


<!-- 参考信息 -->