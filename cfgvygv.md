代发 wailian999

[U27] Py：异步 HTTP
来源：http://rn.chemitech.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://fq.hahajie.cn

[U28] Py：类型别名
来源：http://pa.bjjhwx.cn

UserId = int
来源：http://ze.bjjhwx.cn

[U29] Py：属性校验
来源：http://hn.nicolike.cn

@property 与 @x.setter 配合
来源：http://ru.szsharing.cn

[U30] Py：数据类
来源：http://jf.huanxung.cn

@dataclass(slots=True)
来源：http://jh.shxzukj.cn

[U31] Py：单测
来源：http://fl.asd995.cn

python -m pytest -q
来源：http://rb.lnxyls.cn

[U32] Py：代码格式化
来源：http://mk.szsharing.cn

ruff format . && ruff check --fix .
来源：http://au.hahajie.cn

[U33] Py：打包发布
来源：http://nn.shtwfgs.cn

python -m build  （依赖 pyproject.toml）
来源：http://oc.szxytkj.cn

[U34] Py：判断编码
来源：http://md.jianghongdianzi.cn

chardet.detect(raw)
来源：http://zv.huixiangedu.cn

[U35] Py：发送邮件
来源：http://zq.panjiajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rd.huixinmuqiang.cn

[U36] Py：定时任务
来源：http://fx.huanxung.cn

schedule.every(10).minutes.do(job)
来源：http://ae.huixiangedu.cn

[U37] Py：读写 Excel
来源：http://jr.nicolike.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kf.bjjhwx.cn

[U38] Py：获取脚本所在目录
来源：http://yc.szsharing.cn

Path(__file__).resolve().parent
来源：http://xr.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://qe.9csxet.cn

sys.stdout.isatty()
来源：http://tt.hahajie.cn

[U40] Py：打印到标准错误
来源：http://ta.muxihuayi.cn

print("err", file=sys.stderr)
来源：http://yh.shxzskj.cn

[U41] PHP：初始化 Composer 项目
来源：http://pt.9csxet.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qt.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://fb.nszjky.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cx.shtwfgs.cn

[U43] PHP：声明命名空间
来源：http://pu.huixinmuqiang.cn

namespace App\Http;
来源：http://ly.yuexingan06.cn

[U44] PHP：开启严格类型
来源：http://pg.haigaiapp.cn

declare(strict_types=1);
来源：http://op.colortex.cn

[U45] PHP：类型声明与返回类型
来源：http://xh.huanxung.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yw.colortex.cn

[U46] PHP：可空类型
来源：http://uf.yuntaijiaju.cn

?string $name = null
来源：http://yl.gzmigu.cn

[U47] PHP：联合类型
来源：http://id.yuexingan06.cn

int|string $id
来源：http://ez.jctech888.com.cn

[U48] PHP：纯枚举
来源：http://md.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uo.huixiangedu.cn

[U49] PHP：只读属性
来源：http://vq.gzmigu.cn

public readonly string $name
来源：http://ws.hnjuh.cn

[U50] PHP：构造器属性提升
来源：http://vp.huanxung.cn

public function __construct(private int $id) {}
来源：http://lu.shxzskj.cn

[U51] PHP：数组解构
来源：http://ut.shxzukj.cn

[$a, $b] = $arr;
来源：http://vo.newstarts.cn

[U52] PHP：箭头函数
来源：http://li.shxzukj.cn

$double = fn($x) => $x * 2;
来源：http://le.haigaiapp.cn

[U53] PHP：空合并运算符
来源：http://tj.szsharing.cn

$v = $a ?? $b ?? "default";
来源：http://ht.nicolike.cn

[U54] PHP：空安全调用
来源：http://dv.yuexingan06.cn

$obj?->method()
来源：http://kj.jianghongdianzi.cn

[U55] PHP：match 表达式
来源：http://rq.huixiangedu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ff.nszjky.cn

[U56] PHP：命名参数
来源：http://yr.shtwfgs.cn

f(a: 1, b: 2)
来源：http://nv.huanxung.cn

[U57] PHP：字符串插值
来源：http://zb.hnjuh.cn

"值: {$a}"
来源：http://vo.9csxet.cn

[U58] PHP：数组三件套
来源：http://ob.szsharing.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fn.asd995.cn

[U59] PHP：自定义排序
来源：http://ls.huixinmuqiang.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aj.jctech888.com.cn

[U60] PHP：JSON 编解码
来源：http://ek.nicolike.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://td.lnxyls.cn

[U61] PHP：正则
来源：http://ab.szxytkj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gs.shtwfgs.cn

[U62] PHP：日期对象
来源：http://hb.muxihuayi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zu.muxihuayi.cn

[U63] PHP：文件读写
来源：http://jx.shxzskj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pa.yuntaijiaju.cn

[U64] PHP：目录遍历
来源：http://oj.chemitech.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://gm.jctech888.com.cn

[U65] PHP：会话
来源：http://jk.shxzukj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://aq.hnjuh.cn

[U66] PHP：设置 Cookie
来源：http://lj.hahajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ty.colortex.cn

[U67] PHP：处理文件上传
来源：http://oi.shxzskj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rf.nicolike.cn

[U68] PHP：PDO 连接
来源：http://vm.yuexingan06.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sj.szsharing.cn

[U69] PHP：PDO 预处理
来源：http://hk.jctech888.com.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sx.szsharing.cn

[U70] PHP：PDO 事务
来源：http://qv.9csxet.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lu.hnjuh.cn

[U71] PHP：抛出异常
来源：http://as.nicolike.cn

throw new RuntimeException("失败", 500);
来源：http://kr.lnxyls.cn

[U72] PHP：写错误日志
来源：http://hj.chemitech.net.cn

error_log("失败: " . $e->getMessage());
来源：http://dx.asd995.cn

[U73] PHP：读取 ini 配置
来源：http://fa.wgjwhj.cn

parse_ini_file("config.ini", true)
来源：http://cm.newstarts.cn

[U74] PHP：读取环境变量
来源：http://hy.szxytkj.cn

getenv("APP_ENV") ?: "production"
来源：http://iw.asd995.cn

[U75] PHP：依赖注入
来源：http://bb.chemitech.net.cn

composer require psr/container
来源：http://tu.colortex.cn

[U76] PHP：简单路由
来源：http://ym.gzmigu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ow.panjiajie.cn

[U77] PHP：模板渲染
来源：http://he.lnxyls.cn

composer require twig/twig
来源：http://us.shxzskj.cn

[U78] PHP：单元测试
来源：http://fh.newstarts.cn

composer require --dev phpunit/phpunit
来源：http://uu.huixiangedu.cn

[U79] PHP：静态分析
来源：http://wg.newstarts.cn

composer require --dev phpstan/phpstan
来源：http://pr.hnjuh.cn

[U80] PHP：代码规范修复
来源：http://jq.huixiangedu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ot.jctech888.com.cn

[U81] JS：初始化项目
来源：http://fy.hnjuh.cn

npm init -y;  npm i express
来源：http://va.huixiangedu.cn

[U82] JS：package.json 脚本
来源：http://ca.9csxet.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gb.hahajie.cn

[U83] JS：ES Module 导入导出
来源：http://io.yuexingan06.cn

export const a = 1;  import { a } from "./m.js";
来源：http://sp.9csxet.cn

[U84] JS：CommonJS 写法
来源：http://lv.haigaiapp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hr.huixinmuqiang.cn

[U85] JS：可选链
来源：http://mm.huixinmuqiang.cn

a?.b?.c
来源：http://ib.nicolike.cn

[U86] JS：空值合并
来源：http://ux.gzmigu.cn

a ?? b
来源：http://re.haigaiapp.cn

[U87] JS：解构默认值
来源：http://dy.huixinmuqiang.cn

const { a = 1, b = 2 } = obj;
来源：http://la.521024.cn

[U88] JS：对象展开合并
来源：http://cg.shxzukj.cn

{ ...a, ...b }
来源：http://wf.szxytkj.cn

[U89] JS：数组去重
来源：http://nw.huixiangedu.cn

[...new Set(arr)]
来源：http://zu.huanxung.cn

[U90] JS：数字数组排序
来源：http://ys.nszjky.cn

[...arr].sort((a, b) => a - b)
来源：http://hm.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://uo.huixiangedu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kb.wgjwhj.cn

[U92] JS：深拷贝
来源：http://cz.shxzukj.cn

structuredClone(obj)
来源：http://mn.panjiajie.cn

[U93] JS：模板字符串
来源：http://gy.hahajie.cn

`共 ${n} 条`
来源：http://md.nszjky.cn

[U94] JS：箭头函数
来源：http://at.nszjky.cn

const double = x => x * 2;
来源：http://rp.jctech888.com.cn

[U95] JS：Promise 包装
来源：http://oe.panjiajie.cn

new Promise((resolve, reject) => {})
来源：http://rs.yuexingan06.cn

[U96] JS：async/await 与异常
来源：http://zb.shxzskj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ye.chemitech.net.cn

[U97] JS：并发请求
来源：http://vn.yuntaijiaju.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://or.newstarts.cn

[U98] JS：fetch 带 JSON
来源：http://he.newstarts.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://er.nszjky.cn

[U99] JS：事件监听
来源：http://on.hnjuh.cn

el.addEventListener("click", e => {})
来源：http://xf.yuexingan06.cn

[U100] JS：DOM 查询
来源：http://wd.521024.cn

document.querySelector(".item")
来源：http://xz.huanxung.cn

[U101] JS：classList 操作
来源：http://hd.huixiangedu.cn

el.classList.toggle("active")
来源：http://fy.colortex.cn

[U102] JS：本地存储
来源：http://xh.nszjky.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wt.szsharing.cn

[U103] JS：定时器
来源：http://jz.szsharing.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vx.jianghongdianzi.cn

[U104] JS：防抖
来源：http://st.nszjky.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pa.muxihuayi.cn

[U105] JS：节流
来源：http://er.panjiajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tp.szsharing.cn

[U106] JS：日期格式化
来源：http://gj.newstarts.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rt.haigaiapp.cn

[U107] JS：数字千分位
来源：http://ou.newstarts.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wd.shtwfgs.cn

[U108] JS：随机整数
来源：http://xh.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bq.szxytkj.cn

[U109] JS：数组分组
来源：http://bi.szxytkj.cn

Object.groupBy(arr, x => x.type)
来源：http://pu.nicolike.cn

[U110] JS：数组分块
来源：http://ir.bookmarksfly.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ho.bookmarksfly.cn

[U111] JS：对象转 Map
来源：http://uc.panjiajie.cn

new Map(Object.entries(obj))
来源：http://pi.gzmigu.cn

[U112] JS：字符串补位
来源：http://qx.jianghongdianzi.cn

"7".padStart(3, "0")
来源：http://fy.shxzukj.cn

[U113] JS：正则替换全部
来源：http://si.shxzukj.cn

s.replaceAll("a", "b")
来源：http://ry.hahajie.cn

[U114] JS：JSON 深比较
来源：http://iq.huixinmuqiang.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ah.shxzukj.cn

[U115] JS：生成 UUID
来源：http://as.gzmigu.cn

crypto.randomUUID()
来源：http://gx.hnjuh.cn

[U116] JS：类型检查（JSDoc）
来源：http://xq.panjiajie.cn

/** @param {string} name */ function f(name) {}
来源：http://an.shtwfgs.cn

[U117] JS：单元测试
来源：http://zc.bjjhwx.cn

npm i -D vitest;  npx vitest
来源：http://ht.yuexingan06.cn

[U118] JS：开发服务器
来源：http://te.haigaiapp.cn

npm i -D vite;  npx vite
来源：http://qc.yuntaijiaju.cn

[U119] JS：生产构建
来源：http://on.huixiangedu.cn

npx vite build
来源：http://nw.huixiangedu.cn

[U120] JS：读取环境变量（Vite）
来源：http://hf.szxytkj.cn

import.meta.env.VITE_API_URL
来源：http://fs.9csxet.cn

================================================================================
来源：http://qd.hnjuh.cn

统计汇总
来源：http://bo.haigaiapp.cn

================================================================================
来源：http://ng.szsharing.cn

按语言统计（条）：
来源：http://nq.jianghongdianzi.cn

Python ......... 252
来源：http://xb.nicolike.cn

PHP ............ 252
来源：http://hi.yuexingan06.cn

JavaScript ..... 252
来源：http://yd.chemitech.net.cn

TypeScript ..... 212
来源：http://dw.szsharing.cn

Java ........... 212
来源：http://fv.chemitech.net.cn

Go ............. 212
来源：http://po.521024.cn

Ruby ........... 212
来源：http://il.hahajie.cn

C# ............. 212
来源：http://si.nicolike.cn

C .............. 30
来源：http://ip.wgjwhj.cn

C++ ............ 30
来源：http://od.szsharing.cn

SQL ............ 90
来源：http://dd.muxihuayi.cn

Bash ........... 80
来源：http://xm.hnjuh.cn

Kotlin ......... 15
来源：http://is.nszjky.cn

Swift .......... 15
来源：http://qm.jctech888.com.cn

Lua ............ 10
来源：http://cv.jianghongdianzi.cn

Perl ........... 10
来源：http://vu.huixiangedu.cn

Scala .......... 10
来源：http://wr.9csxet.cn

------------------------------------
来源：http://ow.asd995.cn

合计 ........... 2106 条
来源：http://vu.colortex.cn

按章节统计：
来源：http://az.yuntaijiaju.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://iz.szsharing.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ml.wgjwhj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://oz.asd995.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tj.shxzskj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://at.panjiajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://if.lnxyls.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nq.jctech888.com.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sv.shxzskj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ew.521024.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bo.yuexingan06.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pv.haigaiapp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vy.bookmarksfly.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ix.chemitech.net.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sl.wgjwhj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ek.hahajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bx.huixinmuqiang.cn

Q SQL 专题                              90
来源：http://kx.lnxyls.cn

R Bash 专题                             80
来源：http://bb.jianghongdianzi.cn

S C / C++ 专题                          60
来源：http://vg.chemitech.net.cn

T 其他语言补充                          60
来源：http://lr.shxzskj.cn

U 高频实用片段                         120
来源：http://re.9csxet.cn

------------------------------------
来源：http://rv.haigaiapp.cn

合计                                  2106 条
来源：http://bc.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://dt.nszjky.cn

使用提醒
来源：http://ss.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://qz.hnjuh.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cn.lnxyls.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yv.nicolike.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yp.shxzukj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://hf.shtwfgs.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://oa.haigaiapp.cn

—— 文件结束 ——
来源：http://zj.bjjhwx.cn

================================================================================
来源：http://vk.huixiangedu.cn

程序语言常见例子速查手册（2024 版）
来源：http://in.hnjuh.cn

Common Programming Examples Cheat Book
来源：http://na.yuntaijiaju.cn

================================================================================
来源：http://bm.nicolike.cn

【收录内容】
来源：http://me.shtwfgs.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://dm.bjjhwx.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ov.bjjhwx.cn

SQL · Bash · C · C++
来源：http://oc.bjjhwx.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yn.yuexingan06.cn

【使用说明】
来源：http://ab.asd995.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hn.shxzukj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dk.shxzskj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ho.lnxyls.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://up.hnjuh.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ii.muxihuayi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mo.muxihuayi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yj.nicolike.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dv.jctech888.com.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://eo.lnxyls.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jg.wgjwhj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fu.yuexingan06.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jd.haigaiapp.cn

【文件统计】
来源：http://jl.hahajie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qq.nszjky.cn

--------------------------------------------------------------------------------
来源：http://hj.szsharing.cn

目  录
来源：http://ux.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://ar.nicolike.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fq.lnxyls.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sk.newstarts.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sd.szsharing.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pw.hnjuh.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jy.bookmarksfly.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gs.521024.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kq.gzmigu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fh.muxihuayi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lf.bookmarksfly.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fb.gzmigu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zz.wgjwhj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nx.nszjky.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vi.haigaiapp.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pj.chemitech.net.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yu.wgjwhj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wo.yuexingan06.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dj.hahajie.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://py.shxzukj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://eh.szxytkj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://na.shtwfgs.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jv.haigaiapp.cn

================================================================================
来源：http://ks.shxzskj.cn

A. 基础语法与类型
来源：http://wd.gzmigu.cn

================================================================================
来源：http://al.wgjwhj.cn

[A01] Hello World
来源：http://dl.lnxyls.cn

Py:   print("Hello, World!")
来源：http://is.shxzskj.cn

PHP:  echo "Hello, World!";
来源：http://eb.wgjwhj.cn

JS:   console.log("Hello, World!");
来源：http://vc.hahajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ce.hahajie.cn


<!-- 参考信息 -->