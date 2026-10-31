代发 wailian999

[U25] Py：CSV 按字典读
来源：http://wv.9csxet.cn

csv.DictReader(f)
来源：http://ms.nszjky.cn

[U26] Py：并发下载
来源：http://uq.shxzskj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wk.chemitech.net.cn

[U27] Py：异步 HTTP
来源：http://cp.newstarts.cn

aiohttp.ClientSession() 配合 async with
来源：http://nl.shtwfgs.cn

[U28] Py：类型别名
来源：http://rw.shxzskj.cn

UserId = int
来源：http://ct.wgjwhj.cn

[U29] Py：属性校验
来源：http://im.lnxyls.cn

@property 与 @x.setter 配合
来源：http://dh.haigaiapp.cn

[U30] Py：数据类
来源：http://ya.gzmigu.cn

@dataclass(slots=True)
来源：http://vk.hahajie.cn

[U31] Py：单测
来源：http://an.hnjuh.cn

python -m pytest -q
来源：http://fa.huixiangedu.cn

[U32] Py：代码格式化
来源：http://au.nicolike.cn

ruff format . && ruff check --fix .
来源：http://dx.wgjwhj.cn

[U33] Py：打包发布
来源：http://eq.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://xi.hahajie.cn

[U34] Py：判断编码
来源：http://ls.szsharing.cn

chardet.detect(raw)
来源：http://qn.panjiajie.cn

[U35] Py：发送邮件
来源：http://et.huixiangedu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oe.gzmigu.cn

[U36] Py：定时任务
来源：http://ux.lnxyls.cn

schedule.every(10).minutes.do(job)
来源：http://nf.haigaiapp.cn

[U37] Py：读写 Excel
来源：http://by.jianghongdianzi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qc.shxzskj.cn

[U38] Py：获取脚本所在目录
来源：http://bk.szsharing.cn

Path(__file__).resolve().parent
来源：http://ek.9csxet.cn

[U39] Py：判断是否在交互环境
来源：http://wc.huixiangedu.cn

sys.stdout.isatty()
来源：http://jz.hahajie.cn

[U40] Py：打印到标准错误
来源：http://yd.colortex.cn

print("err", file=sys.stderr)
来源：http://iy.shxzukj.cn

[U41] PHP：初始化 Composer 项目
来源：http://rl.jctech888.com.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ed.shtwfgs.cn

[U42] PHP：PSR-4 自动加载
来源：http://xh.shtwfgs.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wm.shtwfgs.cn

[U43] PHP：声明命名空间
来源：http://vp.nicolike.cn

namespace App\Http;
来源：http://tt.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://cx.jianghongdianzi.cn

declare(strict_types=1);
来源：http://ln.newstarts.cn

[U45] PHP：类型声明与返回类型
来源：http://cu.jctech888.com.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fe.lnxyls.cn

[U46] PHP：可空类型
来源：http://dk.huixinmuqiang.cn

?string $name = null
来源：http://lo.huanxung.cn

[U47] PHP：联合类型
来源：http://gj.panjiajie.cn

int|string $id
来源：http://wb.colortex.cn

[U48] PHP：纯枚举
来源：http://ss.9csxet.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xz.jctech888.com.cn

[U49] PHP：只读属性
来源：http://re.szsharing.cn

public readonly string $name
来源：http://zb.huixiangedu.cn

[U50] PHP：构造器属性提升
来源：http://ls.asd995.cn

public function __construct(private int $id) {}
来源：http://jk.huixinmuqiang.cn

[U51] PHP：数组解构
来源：http://kg.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://at.asd995.cn

[U52] PHP：箭头函数
来源：http://at.asd995.cn

$double = fn($x) => $x * 2;
来源：http://uo.nicolike.cn

[U53] PHP：空合并运算符
来源：http://lk.szxytkj.cn

$v = $a ?? $b ?? "default";
来源：http://gy.9csxet.cn

[U54] PHP：空安全调用
来源：http://ci.newstarts.cn

$obj?->method()
来源：http://vi.haigaiapp.cn

[U55] PHP：match 表达式
来源：http://rt.shxzskj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://by.szsharing.cn

[U56] PHP：命名参数
来源：http://yk.shxzskj.cn

f(a: 1, b: 2)
来源：http://ql.muxihuayi.cn

[U57] PHP：字符串插值
来源：http://oe.bookmarksfly.cn

"值: {$a}"
来源：http://vr.9csxet.cn

[U58] PHP：数组三件套
来源：http://yb.huixinmuqiang.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gk.521024.cn

[U59] PHP：自定义排序
来源：http://wn.yuexingan06.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ro.szxytkj.cn

[U60] PHP：JSON 编解码
来源：http://fj.nszjky.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://se.jianghongdianzi.cn

[U61] PHP：正则
来源：http://hr.521024.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xz.haigaiapp.cn

[U62] PHP：日期对象
来源：http://pa.huixiangedu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gt.huanxung.cn

[U63] PHP：文件读写
来源：http://bb.huixinmuqiang.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ww.yuexingan06.cn

[U64] PHP：目录遍历
来源：http://qj.gzmigu.cn

glob("dir/*.php");  scandir("dir");
来源：http://zb.wgjwhj.cn

[U65] PHP：会话
来源：http://mh.hnjuh.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dg.hnjuh.cn

[U66] PHP：设置 Cookie
来源：http://ev.huanxung.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qi.shxzukj.cn

[U67] PHP：处理文件上传
来源：http://fs.panjiajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vu.nicolike.cn

[U68] PHP：PDO 连接
来源：http://xb.shtwfgs.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ja.521024.cn

[U69] PHP：PDO 预处理
来源：http://zf.bookmarksfly.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jf.gzmigu.cn

[U70] PHP：PDO 事务
来源：http://qu.hahajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ji.jctech888.com.cn

[U71] PHP：抛出异常
来源：http://ye.szsharing.cn

throw new RuntimeException("失败", 500);
来源：http://jd.yuntaijiaju.cn

[U72] PHP：写错误日志
来源：http://zm.9csxet.cn

error_log("失败: " . $e->getMessage());
来源：http://ls.shtwfgs.cn

[U73] PHP：读取 ini 配置
来源：http://vd.lnxyls.cn

parse_ini_file("config.ini", true)
来源：http://zc.muxihuayi.cn

[U74] PHP：读取环境变量
来源：http://bp.panjiajie.cn

getenv("APP_ENV") ?: "production"
来源：http://ei.newstarts.cn

[U75] PHP：依赖注入
来源：http://zn.huixinmuqiang.cn

composer require psr/container
来源：http://df.bookmarksfly.cn

[U76] PHP：简单路由
来源：http://yi.jianghongdianzi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ae.panjiajie.cn

[U77] PHP：模板渲染
来源：http://cn.chemitech.net.cn

composer require twig/twig
来源：http://lu.9csxet.cn

[U78] PHP：单元测试
来源：http://le.bookmarksfly.cn

composer require --dev phpunit/phpunit
来源：http://dj.lnxyls.cn

[U79] PHP：静态分析
来源：http://xf.jctech888.com.cn

composer require --dev phpstan/phpstan
来源：http://vj.huanxung.cn

[U80] PHP：代码规范修复
来源：http://aj.9csxet.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://uu.colortex.cn

[U81] JS：初始化项目
来源：http://na.yuexingan06.cn

npm init -y;  npm i express
来源：http://tn.bjjhwx.cn

[U82] JS：package.json 脚本
来源：http://fr.shxzskj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rw.jianghongdianzi.cn

[U83] JS：ES Module 导入导出
来源：http://qn.asd995.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hv.wgjwhj.cn

[U84] JS：CommonJS 写法
来源：http://vi.hnjuh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://of.muxihuayi.cn

[U85] JS：可选链
来源：http://hd.newstarts.cn

a?.b?.c
来源：http://uo.9csxet.cn

[U86] JS：空值合并
来源：http://ob.szsharing.cn

a ?? b
来源：http://je.bookmarksfly.cn

[U87] JS：解构默认值
来源：http://xf.yuntaijiaju.cn

const { a = 1, b = 2 } = obj;
来源：http://fw.huanxung.cn

[U88] JS：对象展开合并
来源：http://ab.bjjhwx.cn

{ ...a, ...b }
来源：http://ue.panjiajie.cn

[U89] JS：数组去重
来源：http://pb.panjiajie.cn

[...new Set(arr)]
来源：http://ip.bjjhwx.cn

[U90] JS：数字数组排序
来源：http://mt.colortex.cn

[...arr].sort((a, b) => a - b)
来源：http://nc.szxytkj.cn

[U91] JS：对象键值遍历
来源：http://yq.wgjwhj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hs.nszjky.cn

[U92] JS：深拷贝
来源：http://nf.shxzskj.cn

structuredClone(obj)
来源：http://xg.colortex.cn

[U93] JS：模板字符串
来源：http://ld.hnjuh.cn

`共 ${n} 条`
来源：http://fe.huixiangedu.cn

[U94] JS：箭头函数
来源：http://oi.huanxung.cn

const double = x => x * 2;
来源：http://hf.gzmigu.cn

[U95] JS：Promise 包装
来源：http://fa.haigaiapp.cn

new Promise((resolve, reject) => {})
来源：http://kq.hahajie.cn

[U96] JS：async/await 与异常
来源：http://kc.wgjwhj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kc.huixinmuqiang.cn

[U97] JS：并发请求
来源：http://kx.huixiangedu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ro.jianghongdianzi.cn

[U98] JS：fetch 带 JSON
来源：http://pp.huixiangedu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tc.shtwfgs.cn

[U99] JS：事件监听
来源：http://ek.nicolike.cn

el.addEventListener("click", e => {})
来源：http://bo.lnxyls.cn

[U100] JS：DOM 查询
来源：http://hf.lnxyls.cn

document.querySelector(".item")
来源：http://zy.jianghongdianzi.cn

[U101] JS：classList 操作
来源：http://lj.yuexingan06.cn

el.classList.toggle("active")
来源：http://uo.lnxyls.cn

[U102] JS：本地存储
来源：http://xs.gzmigu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wn.gzmigu.cn

[U103] JS：定时器
来源：http://sr.wgjwhj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fu.szxytkj.cn

[U104] JS：防抖
来源：http://lg.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://in.bjjhwx.cn

[U105] JS：节流
来源：http://uh.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ah.521024.cn

[U106] JS：日期格式化
来源：http://qc.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ch.huanxung.cn

[U107] JS：数字千分位
来源：http://lg.huixinmuqiang.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xg.huixiangedu.cn

[U108] JS：随机整数
来源：http://zs.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bz.bjjhwx.cn

[U109] JS：数组分组
来源：http://ms.wgjwhj.cn

Object.groupBy(arr, x => x.type)
来源：http://vn.yuexingan06.cn

[U110] JS：数组分块
来源：http://le.bjjhwx.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xu.newstarts.cn

[U111] JS：对象转 Map
来源：http://mp.panjiajie.cn

new Map(Object.entries(obj))
来源：http://pc.hahajie.cn

[U112] JS：字符串补位
来源：http://zy.newstarts.cn

"7".padStart(3, "0")
来源：http://sd.hnjuh.cn

[U113] JS：正则替换全部
来源：http://zb.yuntaijiaju.cn

s.replaceAll("a", "b")
来源：http://hn.shxzskj.cn

[U114] JS：JSON 深比较
来源：http://pu.huixiangedu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gt.jianghongdianzi.cn

[U115] JS：生成 UUID
来源：http://ft.lnxyls.cn

crypto.randomUUID()
来源：http://ch.bookmarksfly.cn

[U116] JS：类型检查（JSDoc）
来源：http://tr.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://nw.huixiangedu.cn

[U117] JS：单元测试
来源：http://dj.huanxung.cn

npm i -D vitest;  npx vitest
来源：http://ul.szsharing.cn

[U118] JS：开发服务器
来源：http://jp.huixinmuqiang.cn

npm i -D vite;  npx vite
来源：http://un.wgjwhj.cn

[U119] JS：生产构建
来源：http://xr.colortex.cn

npx vite build
来源：http://fj.newstarts.cn

[U120] JS：读取环境变量（Vite）
来源：http://wq.shxzukj.cn

import.meta.env.VITE_API_URL
来源：http://hb.jctech888.com.cn

================================================================================
来源：http://gv.colortex.cn

统计汇总
来源：http://pw.huixiangedu.cn

================================================================================
来源：http://iz.szxytkj.cn

按语言统计（条）：
来源：http://dh.9csxet.cn

Python ......... 252
来源：http://wv.huixiangedu.cn

PHP ............ 252
来源：http://bq.jianghongdianzi.cn

JavaScript ..... 252
来源：http://js.nicolike.cn

TypeScript ..... 212
来源：http://id.muxihuayi.cn

Java ........... 212
来源：http://gm.hnjuh.cn

Go ............. 212
来源：http://nw.yuexingan06.cn

Ruby ........... 212
来源：http://on.shxzskj.cn

C# ............. 212
来源：http://bj.bookmarksfly.cn

C .............. 30
来源：http://kq.yuntaijiaju.cn

C++ ............ 30
来源：http://fd.bookmarksfly.cn

SQL ............ 90
来源：http://xq.hnjuh.cn

Bash ........... 80
来源：http://bm.hnjuh.cn

Kotlin ......... 15
来源：http://ch.jianghongdianzi.cn

Swift .......... 15
来源：http://lf.yuexingan06.cn

Lua ............ 10
来源：http://gb.newstarts.cn

Perl ........... 10
来源：http://cj.wgjwhj.cn

Scala .......... 10
来源：http://tf.huixiangedu.cn

------------------------------------
来源：http://cz.shxzukj.cn

合计 ........... 2106 条
来源：http://zy.huixiangedu.cn

按章节统计：
来源：http://bs.huixiangedu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qz.521024.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fr.szsharing.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lm.shxzskj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lm.bookmarksfly.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bf.huanxung.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ji.jctech888.com.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fo.lnxyls.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rr.szxytkj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uq.huanxung.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tp.shtwfgs.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xo.bjjhwx.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gm.shxzskj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tn.newstarts.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ty.panjiajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kk.huixiangedu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pl.shxzskj.cn

Q SQL 专题                              90
来源：http://kp.szxytkj.cn

R Bash 专题                             80
来源：http://lj.asd995.cn

S C / C++ 专题                          60
来源：http://lo.nszjky.cn

T 其他语言补充                          60
来源：http://sy.huixiangedu.cn

U 高频实用片段                         120
来源：http://yi.szsharing.cn

------------------------------------
来源：http://tn.haigaiapp.cn

合计                                  2106 条
来源：http://tt.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://vn.chemitech.net.cn

使用提醒
来源：http://tu.9csxet.cn

--------------------------------------------------------------------------------
来源：http://ll.newstarts.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ik.chemitech.net.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qp.huixinmuqiang.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://eo.hnjuh.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://yj.nicolike.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ci.haigaiapp.cn

—— 文件结束 ——
来源：http://go.yuntaijiaju.cn

================================================================================
来源：http://qq.9csxet.cn

程序语言常见例子速查手册（2024 版）
来源：http://hs.asd995.cn

Common Programming Examples Cheat Book
来源：http://fe.hnjuh.cn

================================================================================
来源：http://uv.haigaiapp.cn

【收录内容】
来源：http://qx.lnxyls.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rx.nicolike.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zb.panjiajie.cn

SQL · Bash · C · C++
来源：http://bx.szsharing.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://te.jctech888.com.cn

【使用说明】
来源：http://ax.gzmigu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://iu.szsharing.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hh.9csxet.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zo.shtwfgs.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lu.huanxung.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://us.huanxung.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lo.huixiangedu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://of.huixiangedu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ao.asd995.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rf.hahajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lo.shxzskj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rl.9csxet.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kz.huanxung.cn

【文件统计】
来源：http://ld.shxzskj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://va.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://sx.huixiangedu.cn

目  录
来源：http://kf.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://et.wgjwhj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xo.shxzskj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ck.hahajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zm.yuexingan06.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ux.gzmigu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qp.hahajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://iz.nicolike.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ue.yuexingan06.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tu.hnjuh.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bb.muxihuayi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kf.lnxyls.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dc.panjiajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zr.bjjhwx.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ig.shtwfgs.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://if.shxzukj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bj.nicolike.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ef.huixinmuqiang.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yt.wgjwhj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://jx.jctech888.com.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ob.chemitech.net.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dx.huixiangedu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vt.newstarts.cn

================================================================================
来源：http://ds.jctech888.com.cn

A. 基础语法与类型
来源：http://uz.chemitech.net.cn

================================================================================
来源：http://dc.wgjwhj.cn

[A01] Hello World
来源：http://rx.yuntaijiaju.cn


<!-- 参考信息 -->