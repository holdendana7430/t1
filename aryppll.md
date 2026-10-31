代发 wailian999

[U25] Py：CSV 按字典读
来源：http://ul.hahajie.cn

csv.DictReader(f)
来源：http://zl.colortex.cn

[U26] Py：并发下载
来源：http://so.shxzskj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ws.huixiangedu.cn

[U27] Py：异步 HTTP
来源：http://as.szsharing.cn

aiohttp.ClientSession() 配合 async with
来源：http://jn.colortex.cn

[U28] Py：类型别名
来源：http://iq.jctech888.com.cn

UserId = int
来源：http://yf.yuexingan06.cn

[U29] Py：属性校验
来源：http://cj.szxytkj.cn

@property 与 @x.setter 配合
来源：http://py.panjiajie.cn

[U30] Py：数据类
来源：http://bj.hnjuh.cn

@dataclass(slots=True)
来源：http://tx.jianghongdianzi.cn

[U31] Py：单测
来源：http://ll.nicolike.cn

python -m pytest -q
来源：http://pm.bjjhwx.cn

[U32] Py：代码格式化
来源：http://vb.colortex.cn

ruff format . && ruff check --fix .
来源：http://gm.jianghongdianzi.cn

[U33] Py：打包发布
来源：http://ft.jctech888.com.cn

python -m build  （依赖 pyproject.toml）
来源：http://iw.lnxyls.cn

[U34] Py：判断编码
来源：http://ef.nicolike.cn

chardet.detect(raw)
来源：http://wf.huixinmuqiang.cn

[U35] Py：发送邮件
来源：http://dq.hnjuh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fs.shtwfgs.cn

[U36] Py：定时任务
来源：http://gf.asd995.cn

schedule.every(10).minutes.do(job)
来源：http://rq.szsharing.cn

[U37] Py：读写 Excel
来源：http://pf.yuntaijiaju.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ba.hahajie.cn

[U38] Py：获取脚本所在目录
来源：http://vd.nszjky.cn

Path(__file__).resolve().parent
来源：http://wa.bookmarksfly.cn

[U39] Py：判断是否在交互环境
来源：http://yj.bjjhwx.cn

sys.stdout.isatty()
来源：http://sk.szsharing.cn

[U40] Py：打印到标准错误
来源：http://fj.muxihuayi.cn

print("err", file=sys.stderr)
来源：http://ru.newstarts.cn

[U41] PHP：初始化 Composer 项目
来源：http://ai.hnjuh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xw.huixiangedu.cn

[U42] PHP：PSR-4 自动加载
来源：http://uk.muxihuayi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wh.bookmarksfly.cn

[U43] PHP：声明命名空间
来源：http://kb.gzmigu.cn

namespace App\Http;
来源：http://jy.gzmigu.cn

[U44] PHP：开启严格类型
来源：http://tc.jctech888.com.cn

declare(strict_types=1);
来源：http://gw.shxzskj.cn

[U45] PHP：类型声明与返回类型
来源：http://qv.jianghongdianzi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ml.shxzskj.cn

[U46] PHP：可空类型
来源：http://ar.yuntaijiaju.cn

?string $name = null
来源：http://nj.muxihuayi.cn

[U47] PHP：联合类型
来源：http://iw.szxytkj.cn

int|string $id
来源：http://vr.521024.cn

[U48] PHP：纯枚举
来源：http://gy.huanxung.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://go.shxzukj.cn

[U49] PHP：只读属性
来源：http://gf.muxihuayi.cn

public readonly string $name
来源：http://mh.shtwfgs.cn

[U50] PHP：构造器属性提升
来源：http://qn.shxzskj.cn

public function __construct(private int $id) {}
来源：http://ca.shtwfgs.cn

[U51] PHP：数组解构
来源：http://ep.shxzskj.cn

[$a, $b] = $arr;
来源：http://ab.jianghongdianzi.cn

[U52] PHP：箭头函数
来源：http://xg.9csxet.cn

$double = fn($x) => $x * 2;
来源：http://nr.jctech888.com.cn

[U53] PHP：空合并运算符
来源：http://ix.bjjhwx.cn

$v = $a ?? $b ?? "default";
来源：http://tg.yuexingan06.cn

[U54] PHP：空安全调用
来源：http://pt.szsharing.cn

$obj?->method()
来源：http://kn.wgjwhj.cn

[U55] PHP：match 表达式
来源：http://gl.jianghongdianzi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gj.shxzskj.cn

[U56] PHP：命名参数
来源：http://kg.nszjky.cn

f(a: 1, b: 2)
来源：http://nb.newstarts.cn

[U57] PHP：字符串插值
来源：http://zc.hnjuh.cn

"值: {$a}"
来源：http://cr.szxytkj.cn

[U58] PHP：数组三件套
来源：http://vn.shxzukj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zb.wgjwhj.cn

[U59] PHP：自定义排序
来源：http://wd.lnxyls.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ku.colortex.cn

[U60] PHP：JSON 编解码
来源：http://nd.panjiajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mq.huixiangedu.cn

[U61] PHP：正则
来源：http://ms.yuexingan06.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hm.huanxung.cn

[U62] PHP：日期对象
来源：http://qv.szxytkj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tn.shxzskj.cn

[U63] PHP：文件读写
来源：http://rc.521024.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://az.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://cp.szxytkj.cn

glob("dir/*.php");  scandir("dir");
来源：http://bf.jianghongdianzi.cn

[U65] PHP：会话
来源：http://by.lnxyls.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fw.szxytkj.cn

[U66] PHP：设置 Cookie
来源：http://fc.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cp.haigaiapp.cn

[U67] PHP：处理文件上传
来源：http://ff.shxzskj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ue.haigaiapp.cn

[U68] PHP：PDO 连接
来源：http://ot.521024.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nr.521024.cn

[U69] PHP：PDO 预处理
来源：http://io.yuexingan06.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://si.jianghongdianzi.cn

[U70] PHP：PDO 事务
来源：http://tw.huanxung.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jf.wgjwhj.cn

[U71] PHP：抛出异常
来源：http://kq.yuntaijiaju.cn

throw new RuntimeException("失败", 500);
来源：http://sr.gzmigu.cn

[U72] PHP：写错误日志
来源：http://so.muxihuayi.cn

error_log("失败: " . $e->getMessage());
来源：http://ja.asd995.cn

[U73] PHP：读取 ini 配置
来源：http://on.shxzukj.cn

parse_ini_file("config.ini", true)
来源：http://gt.szsharing.cn

[U74] PHP：读取环境变量
来源：http://ai.hnjuh.cn

getenv("APP_ENV") ?: "production"
来源：http://ys.shxzukj.cn

[U75] PHP：依赖注入
来源：http://ou.hnjuh.cn

composer require psr/container
来源：http://jq.huixinmuqiang.cn

[U76] PHP：简单路由
来源：http://yv.shtwfgs.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qn.colortex.cn

[U77] PHP：模板渲染
来源：http://si.colortex.cn

composer require twig/twig
来源：http://sl.521024.cn

[U78] PHP：单元测试
来源：http://yn.yuexingan06.cn

composer require --dev phpunit/phpunit
来源：http://nh.jctech888.com.cn

[U79] PHP：静态分析
来源：http://ur.jctech888.com.cn

composer require --dev phpstan/phpstan
来源：http://lb.521024.cn

[U80] PHP：代码规范修复
来源：http://ea.jctech888.com.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ng.chemitech.net.cn

[U81] JS：初始化项目
来源：http://lt.gzmigu.cn

npm init -y;  npm i express
来源：http://uc.asd995.cn

[U82] JS：package.json 脚本
来源：http://jd.wgjwhj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ah.shxzskj.cn

[U83] JS：ES Module 导入导出
来源：http://jx.huixiangedu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vs.huixinmuqiang.cn

[U84] JS：CommonJS 写法
来源：http://lf.szxytkj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ph.chemitech.net.cn

[U85] JS：可选链
来源：http://tm.haigaiapp.cn

a?.b?.c
来源：http://ts.hnjuh.cn

[U86] JS：空值合并
来源：http://au.huixiangedu.cn

a ?? b
来源：http://ri.hahajie.cn

[U87] JS：解构默认值
来源：http://zk.haigaiapp.cn

const { a = 1, b = 2 } = obj;
来源：http://zc.szsharing.cn

[U88] JS：对象展开合并
来源：http://vw.lnxyls.cn

{ ...a, ...b }
来源：http://yn.jctech888.com.cn

[U89] JS：数组去重
来源：http://oj.chemitech.net.cn

[...new Set(arr)]
来源：http://lw.nicolike.cn

[U90] JS：数字数组排序
来源：http://yo.jctech888.com.cn

[...arr].sort((a, b) => a - b)
来源：http://cc.shxzskj.cn

[U91] JS：对象键值遍历
来源：http://yk.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://od.bookmarksfly.cn

[U92] JS：深拷贝
来源：http://jx.huixiangedu.cn

structuredClone(obj)
来源：http://uf.shtwfgs.cn

[U93] JS：模板字符串
来源：http://iw.huixiangedu.cn

`共 ${n} 条`
来源：http://vt.shxzskj.cn

[U94] JS：箭头函数
来源：http://wa.shxzukj.cn

const double = x => x * 2;
来源：http://yz.521024.cn

[U95] JS：Promise 包装
来源：http://fw.nszjky.cn

new Promise((resolve, reject) => {})
来源：http://xp.chemitech.net.cn

[U96] JS：async/await 与异常
来源：http://mj.haigaiapp.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://at.muxihuayi.cn

[U97] JS：并发请求
来源：http://es.asd995.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://je.panjiajie.cn

[U98] JS：fetch 带 JSON
来源：http://sx.wgjwhj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ks.gzmigu.cn

[U99] JS：事件监听
来源：http://dg.gzmigu.cn

el.addEventListener("click", e => {})
来源：http://yd.szxytkj.cn

[U100] JS：DOM 查询
来源：http://ap.yuexingan06.cn

document.querySelector(".item")
来源：http://yu.521024.cn

[U101] JS：classList 操作
来源：http://ml.gzmigu.cn

el.classList.toggle("active")
来源：http://ju.9csxet.cn

[U102] JS：本地存储
来源：http://yv.521024.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mo.gzmigu.cn

[U103] JS：定时器
来源：http://ge.shxzukj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xl.nszjky.cn

[U104] JS：防抖
来源：http://pi.newstarts.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iq.hahajie.cn

[U105] JS：节流
来源：http://ga.bjjhwx.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qg.yuntaijiaju.cn

[U106] JS：日期格式化
来源：http://jf.yuntaijiaju.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qz.nicolike.cn

[U107] JS：数字千分位
来源：http://pn.jctech888.com.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kr.panjiajie.cn

[U108] JS：随机整数
来源：http://yg.nszjky.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hu.huixinmuqiang.cn

[U109] JS：数组分组
来源：http://np.shtwfgs.cn

Object.groupBy(arr, x => x.type)
来源：http://bk.lnxyls.cn

[U110] JS：数组分块
来源：http://to.muxihuayi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xx.nszjky.cn

[U111] JS：对象转 Map
来源：http://ck.chemitech.net.cn

new Map(Object.entries(obj))
来源：http://dz.shtwfgs.cn

[U112] JS：字符串补位
来源：http://al.panjiajie.cn

"7".padStart(3, "0")
来源：http://if.hahajie.cn

[U113] JS：正则替换全部
来源：http://jk.huixiangedu.cn

s.replaceAll("a", "b")
来源：http://ci.bjjhwx.cn

[U114] JS：JSON 深比较
来源：http://wb.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://yw.nicolike.cn

[U115] JS：生成 UUID
来源：http://tk.yuexingan06.cn

crypto.randomUUID()
来源：http://tx.jctech888.com.cn

[U116] JS：类型检查（JSDoc）
来源：http://in.nszjky.cn

/** @param {string} name */ function f(name) {}
来源：http://gw.jctech888.com.cn

[U117] JS：单元测试
来源：http://ba.haigaiapp.cn

npm i -D vitest;  npx vitest
来源：http://dj.wgjwhj.cn

[U118] JS：开发服务器
来源：http://cs.shxzskj.cn

npm i -D vite;  npx vite
来源：http://fj.nicolike.cn

[U119] JS：生产构建
来源：http://hk.chemitech.net.cn

npx vite build
来源：http://ef.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://nz.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://lz.jctech888.com.cn

================================================================================
来源：http://az.hnjuh.cn

统计汇总
来源：http://cn.yuexingan06.cn

================================================================================
来源：http://gc.yuexingan06.cn

按语言统计（条）：
来源：http://kj.szsharing.cn

Python ......... 252
来源：http://dw.jianghongdianzi.cn

PHP ............ 252
来源：http://vq.chemitech.net.cn

JavaScript ..... 252
来源：http://wb.shtwfgs.cn

TypeScript ..... 212
来源：http://wb.yuexingan06.cn

Java ........... 212
来源：http://wy.yuntaijiaju.cn

Go ............. 212
来源：http://uy.shxzskj.cn

Ruby ........... 212
来源：http://mn.shtwfgs.cn

C# ............. 212
来源：http://qx.jctech888.com.cn

C .............. 30
来源：http://oz.gzmigu.cn

C++ ............ 30
来源：http://do.gzmigu.cn

SQL ............ 90
来源：http://dx.jctech888.com.cn

Bash ........... 80
来源：http://hp.9csxet.cn

Kotlin ......... 15
来源：http://mf.shtwfgs.cn

Swift .......... 15
来源：http://fx.huixinmuqiang.cn

Lua ............ 10
来源：http://fm.yuexingan06.cn

Perl ........... 10
来源：http://lo.hnjuh.cn

Scala .......... 10
来源：http://jt.bookmarksfly.cn

------------------------------------
来源：http://th.lnxyls.cn

合计 ........... 2106 条
来源：http://lu.bjjhwx.cn

按章节统计：
来源：http://vx.muxihuayi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://oc.shxzskj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ob.huixinmuqiang.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uv.panjiajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zm.9csxet.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ua.huixinmuqiang.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cu.9csxet.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://iu.yuexingan06.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sv.newstarts.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tn.hnjuh.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://aw.chemitech.net.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cl.bjjhwx.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bd.szsharing.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bw.9csxet.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ci.shxzskj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ib.yuntaijiaju.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ax.shxzskj.cn

Q SQL 专题                              90
来源：http://vv.yuexingan06.cn

R Bash 专题                             80
来源：http://ii.szsharing.cn

S C / C++ 专题                          60
来源：http://fy.hahajie.cn

T 其他语言补充                          60
来源：http://uc.colortex.cn

U 高频实用片段                         120
来源：http://mx.nszjky.cn

------------------------------------
来源：http://sx.bjjhwx.cn

合计                                  2106 条
来源：http://cf.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://on.chemitech.net.cn

使用提醒
来源：http://dm.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://tc.jctech888.com.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://go.bjjhwx.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mk.newstarts.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rc.huixinmuqiang.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qh.shxzukj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ay.shxzskj.cn

—— 文件结束 ——
来源：http://ki.szsharing.cn

================================================================================
来源：http://gc.chemitech.net.cn

程序语言常见例子速查手册（2024 版）
来源：http://yz.gzmigu.cn

Common Programming Examples Cheat Book
来源：http://vw.szxytkj.cn

================================================================================
来源：http://mb.szxytkj.cn

【收录内容】
来源：http://wy.haigaiapp.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://tr.gzmigu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qi.shxzukj.cn

SQL · Bash · C · C++
来源：http://lp.shxzukj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tj.muxihuayi.cn

【使用说明】
来源：http://ye.wgjwhj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tv.huixiangedu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jp.szsharing.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zf.hahajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xt.hahajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xy.lnxyls.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zg.szsharing.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wy.szsharing.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ph.nszjky.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ba.shtwfgs.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lt.szxytkj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gf.asd995.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vb.chemitech.net.cn

【文件统计】
来源：http://so.9csxet.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ui.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://fb.wgjwhj.cn

目  录
来源：http://ms.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://qc.shxzskj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ij.jctech888.com.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://yp.yuexingan06.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yk.huixinmuqiang.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jo.hnjuh.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cv.nszjky.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jy.yuexingan06.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://en.huixinmuqiang.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xq.huixiangedu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qz.lnxyls.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qn.huixiangedu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pq.jctech888.com.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fb.wgjwhj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mk.jctech888.com.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://uj.shxzskj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nm.9csxet.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qd.huixiangedu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sn.hnjuh.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vz.yuntaijiaju.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ha.jianghongdianzi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uf.wgjwhj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fz.newstarts.cn

================================================================================
来源：http://dy.hnjuh.cn

A. 基础语法与类型
来源：http://yj.szxytkj.cn

================================================================================
来源：http://rt.nszjky.cn

[A01] Hello World
来源：http://kz.nicolike.cn


<!-- 参考信息 -->