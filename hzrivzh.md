代发 wailian999

[U25] Py：CSV 按字典读
来源：http://ob.bookmarksfly.cn

csv.DictReader(f)
来源：http://qu.nszjky.cn

[U26] Py：并发下载
来源：http://tl.huixiangedu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yc.nicolike.cn

[U27] Py：异步 HTTP
来源：http://fy.muxihuayi.cn

aiohttp.ClientSession() 配合 async with
来源：http://pm.haigaiapp.cn

[U28] Py：类型别名
来源：http://ij.gzmigu.cn

UserId = int
来源：http://db.panjiajie.cn

[U29] Py：属性校验
来源：http://ig.9csxet.cn

@property 与 @x.setter 配合
来源：http://vd.bjjhwx.cn

[U30] Py：数据类
来源：http://tr.asd995.cn

@dataclass(slots=True)
来源：http://op.newstarts.cn

[U31] Py：单测
来源：http://nx.nszjky.cn

python -m pytest -q
来源：http://so.hnjuh.cn

[U32] Py：代码格式化
来源：http://us.521024.cn

ruff format . && ruff check --fix .
来源：http://qu.hahajie.cn

[U33] Py：打包发布
来源：http://zt.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://fy.hahajie.cn

[U34] Py：判断编码
来源：http://rz.szsharing.cn

chardet.detect(raw)
来源：http://vb.wgjwhj.cn

[U35] Py：发送邮件
来源：http://qd.shxzskj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hk.jianghongdianzi.cn

[U36] Py：定时任务
来源：http://gk.shtwfgs.cn

schedule.every(10).minutes.do(job)
来源：http://mq.shxzukj.cn

[U37] Py：读写 Excel
来源：http://te.huanxung.cn

pandas.read_excel / DataFrame.to_excel
来源：http://eq.shxzskj.cn

[U38] Py：获取脚本所在目录
来源：http://qf.asd995.cn

Path(__file__).resolve().parent
来源：http://ve.asd995.cn

[U39] Py：判断是否在交互环境
来源：http://un.shxzukj.cn

sys.stdout.isatty()
来源：http://bt.shtwfgs.cn

[U40] Py：打印到标准错误
来源：http://zz.9csxet.cn

print("err", file=sys.stderr)
来源：http://nk.chemitech.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://kx.jctech888.com.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cl.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://up.asd995.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fd.9csxet.cn

[U43] PHP：声明命名空间
来源：http://im.shxzskj.cn

namespace App\Http;
来源：http://vm.asd995.cn

[U44] PHP：开启严格类型
来源：http://pl.hnjuh.cn

declare(strict_types=1);
来源：http://eo.chemitech.net.cn

[U45] PHP：类型声明与返回类型
来源：http://yo.chemitech.net.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cu.szxytkj.cn

[U46] PHP：可空类型
来源：http://cj.yuexingan06.cn

?string $name = null
来源：http://fr.bjjhwx.cn

[U47] PHP：联合类型
来源：http://zp.521024.cn

int|string $id
来源：http://le.bjjhwx.cn

[U48] PHP：纯枚举
来源：http://id.gzmigu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wd.asd995.cn

[U49] PHP：只读属性
来源：http://nn.bjjhwx.cn

public readonly string $name
来源：http://ct.lnxyls.cn

[U50] PHP：构造器属性提升
来源：http://ss.bookmarksfly.cn

public function __construct(private int $id) {}
来源：http://jd.shtwfgs.cn

[U51] PHP：数组解构
来源：http://iy.hnjuh.cn

[$a, $b] = $arr;
来源：http://lx.nicolike.cn

[U52] PHP：箭头函数
来源：http://vt.shxzskj.cn

$double = fn($x) => $x * 2;
来源：http://yt.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://yx.lnxyls.cn

$v = $a ?? $b ?? "default";
来源：http://gf.newstarts.cn

[U54] PHP：空安全调用
来源：http://wl.9csxet.cn

$obj?->method()
来源：http://br.szxytkj.cn

[U55] PHP：match 表达式
来源：http://jb.hahajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vr.yuexingan06.cn

[U56] PHP：命名参数
来源：http://tk.bjjhwx.cn

f(a: 1, b: 2)
来源：http://lo.colortex.cn

[U57] PHP：字符串插值
来源：http://oo.shxzskj.cn

"值: {$a}"
来源：http://aj.huixiangedu.cn

[U58] PHP：数组三件套
来源：http://hu.gzmigu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bw.gzmigu.cn

[U59] PHP：自定义排序
来源：http://iw.asd995.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://db.nszjky.cn

[U60] PHP：JSON 编解码
来源：http://gl.huanxung.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://oa.yuexingan06.cn

[U61] PHP：正则
来源：http://cl.huanxung.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ad.muxihuayi.cn

[U62] PHP：日期对象
来源：http://qw.nicolike.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://am.huanxung.cn

[U63] PHP：文件读写
来源：http://oo.muxihuayi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mi.yuexingan06.cn

[U64] PHP：目录遍历
来源：http://yt.chemitech.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://fo.nszjky.cn

[U65] PHP：会话
来源：http://hr.9csxet.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://nm.huanxung.cn

[U66] PHP：设置 Cookie
来源：http://ls.yuntaijiaju.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://so.huanxung.cn

[U67] PHP：处理文件上传
来源：http://xa.jctech888.com.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cv.jctech888.com.cn

[U68] PHP：PDO 连接
来源：http://uc.huixinmuqiang.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://em.haigaiapp.cn

[U69] PHP：PDO 预处理
来源：http://bv.newstarts.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rv.jianghongdianzi.cn

[U70] PHP：PDO 事务
来源：http://or.shtwfgs.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gj.szsharing.cn

[U71] PHP：抛出异常
来源：http://tr.nicolike.cn

throw new RuntimeException("失败", 500);
来源：http://cg.wgjwhj.cn

[U72] PHP：写错误日志
来源：http://ci.hahajie.cn

error_log("失败: " . $e->getMessage());
来源：http://ek.hnjuh.cn

[U73] PHP：读取 ini 配置
来源：http://sh.muxihuayi.cn

parse_ini_file("config.ini", true)
来源：http://br.hnjuh.cn

[U74] PHP：读取环境变量
来源：http://jv.jctech888.com.cn

getenv("APP_ENV") ?: "production"
来源：http://pu.jianghongdianzi.cn

[U75] PHP：依赖注入
来源：http://oc.hahajie.cn

composer require psr/container
来源：http://wp.hnjuh.cn

[U76] PHP：简单路由
来源：http://qo.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ok.jctech888.com.cn

[U77] PHP：模板渲染
来源：http://fc.muxihuayi.cn

composer require twig/twig
来源：http://iv.szsharing.cn

[U78] PHP：单元测试
来源：http://dh.521024.cn

composer require --dev phpunit/phpunit
来源：http://xo.chemitech.net.cn

[U79] PHP：静态分析
来源：http://xh.yuntaijiaju.cn

composer require --dev phpstan/phpstan
来源：http://pi.szxytkj.cn

[U80] PHP：代码规范修复
来源：http://wg.wgjwhj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nu.panjiajie.cn

[U81] JS：初始化项目
来源：http://hx.9csxet.cn

npm init -y;  npm i express
来源：http://ik.nszjky.cn

[U82] JS：package.json 脚本
来源：http://rk.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pe.chemitech.net.cn

[U83] JS：ES Module 导入导出
来源：http://dl.muxihuayi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kd.szsharing.cn

[U84] JS：CommonJS 写法
来源：http://oh.jianghongdianzi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rm.shxzskj.cn

[U85] JS：可选链
来源：http://jp.yuntaijiaju.cn

a?.b?.c
来源：http://ox.lnxyls.cn

[U86] JS：空值合并
来源：http://iy.hahajie.cn

a ?? b
来源：http://zk.colortex.cn

[U87] JS：解构默认值
来源：http://ih.wgjwhj.cn

const { a = 1, b = 2 } = obj;
来源：http://iq.asd995.cn

[U88] JS：对象展开合并
来源：http://nb.szxytkj.cn

{ ...a, ...b }
来源：http://hv.9csxet.cn

[U89] JS：数组去重
来源：http://gn.chemitech.net.cn

[...new Set(arr)]
来源：http://wj.nszjky.cn

[U90] JS：数字数组排序
来源：http://ws.521024.cn

[...arr].sort((a, b) => a - b)
来源：http://ba.szxytkj.cn

[U91] JS：对象键值遍历
来源：http://if.panjiajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hj.jianghongdianzi.cn

[U92] JS：深拷贝
来源：http://qm.shxzukj.cn

structuredClone(obj)
来源：http://vn.colortex.cn

[U93] JS：模板字符串
来源：http://fd.wgjwhj.cn

`共 ${n} 条`
来源：http://gc.shtwfgs.cn

[U94] JS：箭头函数
来源：http://qr.521024.cn

const double = x => x * 2;
来源：http://dh.9csxet.cn

[U95] JS：Promise 包装
来源：http://iy.newstarts.cn

new Promise((resolve, reject) => {})
来源：http://nm.szsharing.cn

[U96] JS：async/await 与异常
来源：http://ul.shtwfgs.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pj.muxihuayi.cn

[U97] JS：并发请求
来源：http://id.wgjwhj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vh.9csxet.cn

[U98] JS：fetch 带 JSON
来源：http://qp.bookmarksfly.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vk.yuntaijiaju.cn

[U99] JS：事件监听
来源：http://tl.hahajie.cn

el.addEventListener("click", e => {})
来源：http://oa.nicolike.cn

[U100] JS：DOM 查询
来源：http://zr.9csxet.cn

document.querySelector(".item")
来源：http://be.nszjky.cn

[U101] JS：classList 操作
来源：http://zu.chemitech.net.cn

el.classList.toggle("active")
来源：http://bf.panjiajie.cn

[U102] JS：本地存储
来源：http://uu.yuexingan06.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gk.huanxung.cn

[U103] JS：定时器
来源：http://aj.nicolike.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lz.huixiangedu.cn

[U104] JS：防抖
来源：http://vv.asd995.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ar.szxytkj.cn

[U105] JS：节流
来源：http://eg.jianghongdianzi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://du.jianghongdianzi.cn

[U106] JS：日期格式化
来源：http://wd.szsharing.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kt.szxytkj.cn

[U107] JS：数字千分位
来源：http://bw.shxzskj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dp.hahajie.cn

[U108] JS：随机整数
来源：http://sk.huanxung.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pf.nicolike.cn

[U109] JS：数组分组
来源：http://cs.nicolike.cn

Object.groupBy(arr, x => x.type)
来源：http://qy.szxytkj.cn

[U110] JS：数组分块
来源：http://cr.bookmarksfly.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lq.huanxung.cn

[U111] JS：对象转 Map
来源：http://wa.wgjwhj.cn

new Map(Object.entries(obj))
来源：http://gj.yuntaijiaju.cn

[U112] JS：字符串补位
来源：http://fs.wgjwhj.cn

"7".padStart(3, "0")
来源：http://uy.gzmigu.cn

[U113] JS：正则替换全部
来源：http://yp.colortex.cn

s.replaceAll("a", "b")
来源：http://yh.muxihuayi.cn

[U114] JS：JSON 深比较
来源：http://ge.jctech888.com.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ia.asd995.cn

[U115] JS：生成 UUID
来源：http://ik.hnjuh.cn

crypto.randomUUID()
来源：http://nf.jianghongdianzi.cn

[U116] JS：类型检查（JSDoc）
来源：http://bm.colortex.cn

/** @param {string} name */ function f(name) {}
来源：http://om.jianghongdianzi.cn

[U117] JS：单元测试
来源：http://au.asd995.cn

npm i -D vitest;  npx vitest
来源：http://vq.muxihuayi.cn

[U118] JS：开发服务器
来源：http://ju.yuntaijiaju.cn

npm i -D vite;  npx vite
来源：http://du.hahajie.cn

[U119] JS：生产构建
来源：http://iq.chemitech.net.cn

npx vite build
来源：http://mq.jianghongdianzi.cn

[U120] JS：读取环境变量（Vite）
来源：http://dj.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://ql.colortex.cn

================================================================================
来源：http://qy.szxytkj.cn

统计汇总
来源：http://hb.muxihuayi.cn

================================================================================
来源：http://xz.nicolike.cn

按语言统计（条）：
来源：http://ln.shxzskj.cn

Python ......... 252
来源：http://st.shtwfgs.cn

PHP ............ 252
来源：http://zv.nszjky.cn

JavaScript ..... 252
来源：http://rt.gzmigu.cn

TypeScript ..... 212
来源：http://mt.muxihuayi.cn

Java ........... 212
来源：http://bq.shtwfgs.cn

Go ............. 212
来源：http://og.lnxyls.cn

Ruby ........... 212
来源：http://ih.colortex.cn

C# ............. 212
来源：http://cq.haigaiapp.cn

C .............. 30
来源：http://dr.bjjhwx.cn

C++ ............ 30
来源：http://ev.jctech888.com.cn

SQL ............ 90
来源：http://bk.jctech888.com.cn

Bash ........... 80
来源：http://qy.szxytkj.cn

Kotlin ......... 15
来源：http://qz.shxzukj.cn

Swift .......... 15
来源：http://tk.bookmarksfly.cn

Lua ............ 10
来源：http://nk.colortex.cn

Perl ........... 10
来源：http://ay.bjjhwx.cn

Scala .......... 10
来源：http://wd.jctech888.com.cn

------------------------------------
来源：http://bw.yuexingan06.cn

合计 ........... 2106 条
来源：http://bu.lnxyls.cn

按章节统计：
来源：http://xt.huanxung.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yw.gzmigu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ag.bjjhwx.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qf.nszjky.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vr.asd995.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vf.gzmigu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gz.huixiangedu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zi.wgjwhj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wj.chemitech.net.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jv.huixinmuqiang.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gv.9csxet.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://je.jianghongdianzi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rw.jctech888.com.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ez.nszjky.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ie.bookmarksfly.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ui.muxihuayi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bh.yuntaijiaju.cn

Q SQL 专题                              90
来源：http://pw.shxzukj.cn

R Bash 专题                             80
来源：http://rp.haigaiapp.cn

S C / C++ 专题                          60
来源：http://xz.nszjky.cn

T 其他语言补充                          60
来源：http://uh.huixinmuqiang.cn

U 高频实用片段                         120
来源：http://kz.lnxyls.cn

------------------------------------
来源：http://yd.haigaiapp.cn

合计                                  2106 条
来源：http://gx.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://ii.yuexingan06.cn

使用提醒
来源：http://wn.nicolike.cn

--------------------------------------------------------------------------------
来源：http://jt.huixinmuqiang.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fe.hnjuh.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fk.jianghongdianzi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ug.huixiangedu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zy.nicolike.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://in.yuexingan06.cn

—— 文件结束 ——
来源：http://od.shxzukj.cn

================================================================================
来源：http://so.521024.cn

程序语言常见例子速查手册（2024 版）
来源：http://sn.hnjuh.cn

Common Programming Examples Cheat Book
来源：http://vb.lnxyls.cn

================================================================================
来源：http://dz.gzmigu.cn

【收录内容】
来源：http://yc.hnjuh.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ph.panjiajie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ci.wgjwhj.cn

SQL · Bash · C · C++
来源：http://du.asd995.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pr.521024.cn

【使用说明】
来源：http://mh.gzmigu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jh.nicolike.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cc.chemitech.net.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rm.huixinmuqiang.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://sl.bookmarksfly.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ej.newstarts.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pv.szsharing.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dt.szsharing.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yx.9csxet.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://oj.yuntaijiaju.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jl.szsharing.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://al.haigaiapp.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kz.colortex.cn

【文件统计】
来源：http://wn.colortex.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yc.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://cs.huanxung.cn

目  录
来源：http://ls.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://vn.jctech888.com.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://iv.9csxet.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://af.nszjky.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qi.hahajie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://oi.huixinmuqiang.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kp.gzmigu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fq.hnjuh.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dk.haigaiapp.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xt.nicolike.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lg.chemitech.net.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://um.hahajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zx.nszjky.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sz.panjiajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lk.chemitech.net.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://je.huanxung.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yb.bjjhwx.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bd.gzmigu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jf.bjjhwx.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://yg.haigaiapp.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wl.jianghongdianzi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dd.panjiajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cc.huixinmuqiang.cn

================================================================================
来源：http://fb.huanxung.cn

A. 基础语法与类型
来源：http://ka.colortex.cn

================================================================================
来源：http://ku.bjjhwx.cn

[A01] Hello World
来源：http://ep.hahajie.cn


<!-- 参考信息 -->