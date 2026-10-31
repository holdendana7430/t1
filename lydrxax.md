代发 wailian999

[U25] Py：CSV 按字典读
来源：http://lf.huixiangedu.cn

csv.DictReader(f)
来源：http://df.yuntaijiaju.cn

[U26] Py：并发下载
来源：http://rm.haigaiapp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wq.9csxet.cn

[U27] Py：异步 HTTP
来源：http://iw.hahajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://lb.lnxyls.cn

[U28] Py：类型别名
来源：http://tp.nszjky.cn

UserId = int
来源：http://cu.haigaiapp.cn

[U29] Py：属性校验
来源：http://uo.nszjky.cn

@property 与 @x.setter 配合
来源：http://ir.asd995.cn

[U30] Py：数据类
来源：http://ng.bjjhwx.cn

@dataclass(slots=True)
来源：http://dl.szxytkj.cn

[U31] Py：单测
来源：http://qr.9csxet.cn

python -m pytest -q
来源：http://ym.huanxung.cn

[U32] Py：代码格式化
来源：http://cn.yuntaijiaju.cn

ruff format . && ruff check --fix .
来源：http://il.nicolike.cn

[U33] Py：打包发布
来源：http://np.jianghongdianzi.cn

python -m build  （依赖 pyproject.toml）
来源：http://ip.shxzukj.cn

[U34] Py：判断编码
来源：http://zq.bjjhwx.cn

chardet.detect(raw)
来源：http://mm.yuntaijiaju.cn

[U35] Py：发送邮件
来源：http://jt.haigaiapp.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://li.shxzskj.cn

[U36] Py：定时任务
来源：http://kq.huixinmuqiang.cn

schedule.every(10).minutes.do(job)
来源：http://sk.yuexingan06.cn

[U37] Py：读写 Excel
来源：http://fo.jianghongdianzi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wz.chemitech.net.cn

[U38] Py：获取脚本所在目录
来源：http://pu.hahajie.cn

Path(__file__).resolve().parent
来源：http://np.haigaiapp.cn

[U39] Py：判断是否在交互环境
来源：http://aq.huixiangedu.cn

sys.stdout.isatty()
来源：http://im.huixiangedu.cn

[U40] Py：打印到标准错误
来源：http://vh.gzmigu.cn

print("err", file=sys.stderr)
来源：http://vd.huixiangedu.cn

[U41] PHP：初始化 Composer 项目
来源：http://jx.huixinmuqiang.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vm.hnjuh.cn

[U42] PHP：PSR-4 自动加载
来源：http://uy.haigaiapp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qb.haigaiapp.cn

[U43] PHP：声明命名空间
来源：http://yh.bookmarksfly.cn

namespace App\Http;
来源：http://sg.nicolike.cn

[U44] PHP：开启严格类型
来源：http://dr.521024.cn

declare(strict_types=1);
来源：http://tb.newstarts.cn

[U45] PHP：类型声明与返回类型
来源：http://nj.colortex.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jn.bookmarksfly.cn

[U46] PHP：可空类型
来源：http://fs.shtwfgs.cn

?string $name = null
来源：http://ot.muxihuayi.cn

[U47] PHP：联合类型
来源：http://sf.szxytkj.cn

int|string $id
来源：http://in.szsharing.cn

[U48] PHP：纯枚举
来源：http://eq.gzmigu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://eg.huixiangedu.cn

[U49] PHP：只读属性
来源：http://rh.hahajie.cn

public readonly string $name
来源：http://gr.hnjuh.cn

[U50] PHP：构造器属性提升
来源：http://ta.nszjky.cn

public function __construct(private int $id) {}
来源：http://yk.521024.cn

[U51] PHP：数组解构
来源：http://wp.shxzukj.cn

[$a, $b] = $arr;
来源：http://an.9csxet.cn

[U52] PHP：箭头函数
来源：http://gn.wgjwhj.cn

$double = fn($x) => $x * 2;
来源：http://qz.szsharing.cn

[U53] PHP：空合并运算符
来源：http://md.szxytkj.cn

$v = $a ?? $b ?? "default";
来源：http://zz.newstarts.cn

[U54] PHP：空安全调用
来源：http://aw.szsharing.cn

$obj?->method()
来源：http://tf.huixiangedu.cn

[U55] PHP：match 表达式
来源：http://ev.gzmigu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fe.huixiangedu.cn

[U56] PHP：命名参数
来源：http://ui.huanxung.cn

f(a: 1, b: 2)
来源：http://dm.9csxet.cn

[U57] PHP：字符串插值
来源：http://bk.yuexingan06.cn

"值: {$a}"
来源：http://vy.bookmarksfly.cn

[U58] PHP：数组三件套
来源：http://jj.yuexingan06.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://om.colortex.cn

[U59] PHP：自定义排序
来源：http://zm.shxzukj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fd.bookmarksfly.cn

[U60] PHP：JSON 编解码
来源：http://ph.nszjky.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vc.shtwfgs.cn

[U61] PHP：正则
来源：http://iz.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lh.nicolike.cn

[U62] PHP：日期对象
来源：http://kk.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rj.yuntaijiaju.cn

[U63] PHP：文件读写
来源：http://ux.gzmigu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dw.muxihuayi.cn

[U64] PHP：目录遍历
来源：http://ji.panjiajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://ca.gzmigu.cn

[U65] PHP：会话
来源：http://fd.521024.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vz.gzmigu.cn

[U66] PHP：设置 Cookie
来源：http://dc.yuexingan06.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nl.shxzskj.cn

[U67] PHP：处理文件上传
来源：http://ba.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kp.nszjky.cn

[U68] PHP：PDO 连接
来源：http://iy.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hy.yuexingan06.cn

[U69] PHP：PDO 预处理
来源：http://cb.muxihuayi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wb.huanxung.cn

[U70] PHP：PDO 事务
来源：http://ui.lnxyls.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://iq.lnxyls.cn

[U71] PHP：抛出异常
来源：http://jw.szsharing.cn

throw new RuntimeException("失败", 500);
来源：http://mj.shxzskj.cn

[U72] PHP：写错误日志
来源：http://wf.asd995.cn

error_log("失败: " . $e->getMessage());
来源：http://vs.newstarts.cn

[U73] PHP：读取 ini 配置
来源：http://gi.gzmigu.cn

parse_ini_file("config.ini", true)
来源：http://mi.szsharing.cn

[U74] PHP：读取环境变量
来源：http://so.haigaiapp.cn

getenv("APP_ENV") ?: "production"
来源：http://zr.shxzukj.cn

[U75] PHP：依赖注入
来源：http://do.hnjuh.cn

composer require psr/container
来源：http://jl.shxzukj.cn

[U76] PHP：简单路由
来源：http://ru.panjiajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fz.lnxyls.cn

[U77] PHP：模板渲染
来源：http://ob.muxihuayi.cn

composer require twig/twig
来源：http://ab.shtwfgs.cn

[U78] PHP：单元测试
来源：http://fa.szsharing.cn

composer require --dev phpunit/phpunit
来源：http://tn.bookmarksfly.cn

[U79] PHP：静态分析
来源：http://kt.hnjuh.cn

composer require --dev phpstan/phpstan
来源：http://zs.huanxung.cn

[U80] PHP：代码规范修复
来源：http://rp.lnxyls.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://yu.huixinmuqiang.cn

[U81] JS：初始化项目
来源：http://ju.newstarts.cn

npm init -y;  npm i express
来源：http://md.yuexingan06.cn

[U82] JS：package.json 脚本
来源：http://vy.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tq.nicolike.cn

[U83] JS：ES Module 导入导出
来源：http://yd.9csxet.cn

export const a = 1;  import { a } from "./m.js";
来源：http://oh.muxihuayi.cn

[U84] JS：CommonJS 写法
来源：http://as.asd995.cn

module.exports = { a };  const { a } = require("./m");
来源：http://sf.huanxung.cn

[U85] JS：可选链
来源：http://kw.9csxet.cn

a?.b?.c
来源：http://uj.huanxung.cn

[U86] JS：空值合并
来源：http://fx.wgjwhj.cn

a ?? b
来源：http://jz.newstarts.cn

[U87] JS：解构默认值
来源：http://cp.szxytkj.cn

const { a = 1, b = 2 } = obj;
来源：http://dl.newstarts.cn

[U88] JS：对象展开合并
来源：http://ml.nszjky.cn

{ ...a, ...b }
来源：http://kc.hahajie.cn

[U89] JS：数组去重
来源：http://hk.huanxung.cn

[...new Set(arr)]
来源：http://av.wgjwhj.cn

[U90] JS：数字数组排序
来源：http://ch.9csxet.cn

[...arr].sort((a, b) => a - b)
来源：http://fb.nszjky.cn

[U91] JS：对象键值遍历
来源：http://hw.chemitech.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://eu.huixiangedu.cn

[U92] JS：深拷贝
来源：http://jg.nicolike.cn

structuredClone(obj)
来源：http://ce.yuntaijiaju.cn

[U93] JS：模板字符串
来源：http://er.bjjhwx.cn

`共 ${n} 条`
来源：http://rd.haigaiapp.cn

[U94] JS：箭头函数
来源：http://wj.wgjwhj.cn

const double = x => x * 2;
来源：http://jp.nicolike.cn

[U95] JS：Promise 包装
来源：http://ju.asd995.cn

new Promise((resolve, reject) => {})
来源：http://sw.521024.cn

[U96] JS：async/await 与异常
来源：http://bw.jianghongdianzi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sr.yuexingan06.cn

[U97] JS：并发请求
来源：http://ax.huanxung.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ye.newstarts.cn

[U98] JS：fetch 带 JSON
来源：http://fz.shxzskj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ae.haigaiapp.cn

[U99] JS：事件监听
来源：http://ts.colortex.cn

el.addEventListener("click", e => {})
来源：http://el.hnjuh.cn

[U100] JS：DOM 查询
来源：http://pu.jianghongdianzi.cn

document.querySelector(".item")
来源：http://kt.bookmarksfly.cn

[U101] JS：classList 操作
来源：http://ys.hnjuh.cn

el.classList.toggle("active")
来源：http://zg.asd995.cn

[U102] JS：本地存储
来源：http://cw.gzmigu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sq.huanxung.cn

[U103] JS：定时器
来源：http://hi.wgjwhj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bo.huixinmuqiang.cn

[U104] JS：防抖
来源：http://wh.bookmarksfly.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gf.bjjhwx.cn

[U105] JS：节流
来源：http://kn.szxytkj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gf.chemitech.net.cn

[U106] JS：日期格式化
来源：http://dc.newstarts.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://if.shxzskj.cn

[U107] JS：数字千分位
来源：http://sb.huanxung.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gn.haigaiapp.cn

[U108] JS：随机整数
来源：http://nm.bjjhwx.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ba.szsharing.cn

[U109] JS：数组分组
来源：http://uy.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://jd.panjiajie.cn

[U110] JS：数组分块
来源：http://mu.huixiangedu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wp.bjjhwx.cn

[U111] JS：对象转 Map
来源：http://om.shtwfgs.cn

new Map(Object.entries(obj))
来源：http://jx.yuntaijiaju.cn

[U112] JS：字符串补位
来源：http://jm.bjjhwx.cn

"7".padStart(3, "0")
来源：http://gm.newstarts.cn

[U113] JS：正则替换全部
来源：http://fv.hahajie.cn

s.replaceAll("a", "b")
来源：http://sj.nicolike.cn

[U114] JS：JSON 深比较
来源：http://kk.nicolike.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://md.hahajie.cn

[U115] JS：生成 UUID
来源：http://hs.nicolike.cn

crypto.randomUUID()
来源：http://da.szsharing.cn

[U116] JS：类型检查（JSDoc）
来源：http://ad.yuntaijiaju.cn

/** @param {string} name */ function f(name) {}
来源：http://ge.huixinmuqiang.cn

[U117] JS：单元测试
来源：http://lw.shxzskj.cn

npm i -D vitest;  npx vitest
来源：http://ln.huixiangedu.cn

[U118] JS：开发服务器
来源：http://ut.shxzukj.cn

npm i -D vite;  npx vite
来源：http://yz.bjjhwx.cn

[U119] JS：生产构建
来源：http://qv.yuntaijiaju.cn

npx vite build
来源：http://nh.jctech888.com.cn

[U120] JS：读取环境变量（Vite）
来源：http://vc.szxytkj.cn

import.meta.env.VITE_API_URL
来源：http://hi.yuexingan06.cn

================================================================================
来源：http://ds.gzmigu.cn

统计汇总
来源：http://lm.yuntaijiaju.cn

================================================================================
来源：http://el.hnjuh.cn

按语言统计（条）：
来源：http://vp.bookmarksfly.cn

Python ......... 252
来源：http://cs.nicolike.cn

PHP ............ 252
来源：http://bi.bookmarksfly.cn

JavaScript ..... 252
来源：http://ps.huanxung.cn

TypeScript ..... 212
来源：http://vw.huanxung.cn

Java ........... 212
来源：http://vn.shxzskj.cn

Go ............. 212
来源：http://ob.9csxet.cn

Ruby ........... 212
来源：http://bc.huanxung.cn

C# ............. 212
来源：http://ug.wgjwhj.cn

C .............. 30
来源：http://fh.panjiajie.cn

C++ ............ 30
来源：http://ts.yuntaijiaju.cn

SQL ............ 90
来源：http://lh.gzmigu.cn

Bash ........... 80
来源：http://bi.asd995.cn

Kotlin ......... 15
来源：http://hv.bookmarksfly.cn

Swift .......... 15
来源：http://qz.bookmarksfly.cn

Lua ............ 10
来源：http://pa.panjiajie.cn

Perl ........... 10
来源：http://io.bjjhwx.cn

Scala .......... 10
来源：http://va.gzmigu.cn

------------------------------------
来源：http://zp.szsharing.cn

合计 ........... 2106 条
来源：http://hr.huixiangedu.cn

按章节统计：
来源：http://sf.szsharing.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://id.wgjwhj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ye.yuexingan06.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mz.bookmarksfly.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dg.szsharing.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jz.bookmarksfly.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xs.yuexingan06.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lu.bjjhwx.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://re.nicolike.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jp.muxihuayi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dw.jianghongdianzi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hq.muxihuayi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ah.nicolike.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tn.gzmigu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qt.szxytkj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://az.huanxung.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lz.bjjhwx.cn

Q SQL 专题                              90
来源：http://lq.newstarts.cn

R Bash 专题                             80
来源：http://at.haigaiapp.cn

S C / C++ 专题                          60
来源：http://rl.jctech888.com.cn

T 其他语言补充                          60
来源：http://fd.hnjuh.cn

U 高频实用片段                         120
来源：http://mk.bjjhwx.cn

------------------------------------
来源：http://wc.lnxyls.cn

合计                                  2106 条
来源：http://kg.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://vh.huixinmuqiang.cn

使用提醒
来源：http://my.hahajie.cn

--------------------------------------------------------------------------------
来源：http://by.521024.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mh.nicolike.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nn.nicolike.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vv.szsharing.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vi.panjiajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ev.shtwfgs.cn

—— 文件结束 ——
来源：http://mz.huixiangedu.cn

================================================================================
来源：http://qf.bjjhwx.cn

程序语言常见例子速查手册（2024 版）
来源：http://wh.shxzskj.cn

Common Programming Examples Cheat Book
来源：http://ty.szxytkj.cn

================================================================================
来源：http://xx.hnjuh.cn

【收录内容】
来源：http://vh.colortex.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zj.hahajie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wy.hahajie.cn

SQL · Bash · C · C++
来源：http://cp.szsharing.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qm.yuexingan06.cn

【使用说明】
来源：http://ol.huixinmuqiang.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cw.shtwfgs.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ja.jctech888.com.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://us.asd995.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yw.shxzskj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qc.yuexingan06.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://va.hahajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yd.chemitech.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hv.hnjuh.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dv.nicolike.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ch.521024.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://eh.asd995.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://by.huanxung.cn

【文件统计】
来源：http://bc.bjjhwx.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ny.colortex.cn

--------------------------------------------------------------------------------
来源：http://rl.bjjhwx.cn

目  录
来源：http://ea.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://ay.chemitech.net.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qg.huanxung.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://py.jianghongdianzi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kw.hnjuh.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nb.nicolike.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ec.chemitech.net.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hb.yuntaijiaju.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yj.asd995.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ys.hahajie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bz.bookmarksfly.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qh.nicolike.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ez.yuexingan06.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kw.gzmigu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hj.jctech888.com.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gn.colortex.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ga.panjiajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://be.szxytkj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tk.wgjwhj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://qg.gzmigu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lm.gzmigu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vu.colortex.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yi.yuntaijiaju.cn

================================================================================
来源：http://qa.panjiajie.cn

A. 基础语法与类型
来源：http://kd.newstarts.cn

================================================================================
来源：http://jw.muxihuayi.cn

[A01] Hello World
来源：http://bb.hahajie.cn


<!-- 参考信息 -->