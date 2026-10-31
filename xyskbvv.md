代发 wailian999

[U19] Py：正则替换带回调
来源：http://sc.bookmarksfly.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ma.hahajie.cn

[U20] Py：缓存函数结果
来源：http://gz.panjiajie.cn

@functools.lru_cache(maxsize=None)
来源：http://ol.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://ux.chemitech.net.cn

@contextlib.contextmanager
来源：http://lo.szsharing.cn

[U22] Py：矩阵转置
来源：http://bp.gzmigu.cn

list(zip(*m))
来源：http://tt.huanxung.cn

[U23] Py：分块读取大文件
来源：http://gu.hahajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nj.yuntaijiaju.cn

[U24] Py：路径操作
来源：http://qb.yuntaijiaju.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xp.lnxyls.cn

[U25] Py：CSV 按字典读
来源：http://up.shxzukj.cn

csv.DictReader(f)
来源：http://hc.muxihuayi.cn

[U26] Py：并发下载
来源：http://kc.jctech888.com.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://et.szsharing.cn

[U27] Py：异步 HTTP
来源：http://cn.bjjhwx.cn

aiohttp.ClientSession() 配合 async with
来源：http://jm.muxihuayi.cn

[U28] Py：类型别名
来源：http://zh.hahajie.cn

UserId = int
来源：http://sv.bookmarksfly.cn

[U29] Py：属性校验
来源：http://tp.nicolike.cn

@property 与 @x.setter 配合
来源：http://nv.nicolike.cn

[U30] Py：数据类
来源：http://pa.muxihuayi.cn

@dataclass(slots=True)
来源：http://ac.9csxet.cn

[U31] Py：单测
来源：http://iw.521024.cn

python -m pytest -q
来源：http://ok.haigaiapp.cn

[U32] Py：代码格式化
来源：http://uw.yuntaijiaju.cn

ruff format . && ruff check --fix .
来源：http://nx.muxihuayi.cn

[U33] Py：打包发布
来源：http://pv.szxytkj.cn

python -m build  （依赖 pyproject.toml）
来源：http://fc.jctech888.com.cn

[U34] Py：判断编码
来源：http://gc.nszjky.cn

chardet.detect(raw)
来源：http://ct.hahajie.cn

[U35] Py：发送邮件
来源：http://up.muxihuayi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ss.huixiangedu.cn

[U36] Py：定时任务
来源：http://kj.lnxyls.cn

schedule.every(10).minutes.do(job)
来源：http://ju.szxytkj.cn

[U37] Py：读写 Excel
来源：http://iw.yuntaijiaju.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qo.9csxet.cn

[U38] Py：获取脚本所在目录
来源：http://gj.hahajie.cn

Path(__file__).resolve().parent
来源：http://va.szxytkj.cn

[U39] Py：判断是否在交互环境
来源：http://qm.huanxung.cn

sys.stdout.isatty()
来源：http://wl.shtwfgs.cn

[U40] Py：打印到标准错误
来源：http://or.panjiajie.cn

print("err", file=sys.stderr)
来源：http://nn.yuexingan06.cn

[U41] PHP：初始化 Composer 项目
来源：http://hb.bjjhwx.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tz.colortex.cn

[U42] PHP：PSR-4 自动加载
来源：http://ue.colortex.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://db.shtwfgs.cn

[U43] PHP：声明命名空间
来源：http://zp.bookmarksfly.cn

namespace App\Http;
来源：http://im.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://gb.chemitech.net.cn

declare(strict_types=1);
来源：http://lb.shxzukj.cn

[U45] PHP：类型声明与返回类型
来源：http://ya.jctech888.com.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bx.521024.cn

[U46] PHP：可空类型
来源：http://hx.panjiajie.cn

?string $name = null
来源：http://ds.shxzskj.cn

[U47] PHP：联合类型
来源：http://zw.asd995.cn

int|string $id
来源：http://ia.szsharing.cn

[U48] PHP：纯枚举
来源：http://lc.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pj.szsharing.cn

[U49] PHP：只读属性
来源：http://ug.shxzskj.cn

public readonly string $name
来源：http://ze.9csxet.cn

[U50] PHP：构造器属性提升
来源：http://jf.bjjhwx.cn

public function __construct(private int $id) {}
来源：http://ic.shtwfgs.cn

[U51] PHP：数组解构
来源：http://ba.nszjky.cn

[$a, $b] = $arr;
来源：http://jc.nicolike.cn

[U52] PHP：箭头函数
来源：http://pw.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://hn.muxihuayi.cn

[U53] PHP：空合并运算符
来源：http://ik.hahajie.cn

$v = $a ?? $b ?? "default";
来源：http://fb.huixinmuqiang.cn

[U54] PHP：空安全调用
来源：http://nx.wgjwhj.cn

$obj?->method()
来源：http://xa.9csxet.cn

[U55] PHP：match 表达式
来源：http://ai.chemitech.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mk.hahajie.cn

[U56] PHP：命名参数
来源：http://en.wgjwhj.cn

f(a: 1, b: 2)
来源：http://zl.shxzukj.cn

[U57] PHP：字符串插值
来源：http://yz.521024.cn

"值: {$a}"
来源：http://tc.bjjhwx.cn

[U58] PHP：数组三件套
来源：http://og.lnxyls.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yo.szsharing.cn

[U59] PHP：自定义排序
来源：http://hy.nicolike.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ut.jianghongdianzi.cn

[U60] PHP：JSON 编解码
来源：http://gg.gzmigu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gw.huixiangedu.cn

[U61] PHP：正则
来源：http://ic.muxihuayi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tz.yuntaijiaju.cn

[U62] PHP：日期对象
来源：http://if.szxytkj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xv.bjjhwx.cn

[U63] PHP：文件读写
来源：http://sd.9csxet.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bd.muxihuayi.cn

[U64] PHP：目录遍历
来源：http://ym.szsharing.cn

glob("dir/*.php");  scandir("dir");
来源：http://wp.muxihuayi.cn

[U65] PHP：会话
来源：http://bs.bjjhwx.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fp.panjiajie.cn

[U66] PHP：设置 Cookie
来源：http://ax.asd995.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qc.huixiangedu.cn

[U67] PHP：处理文件上传
来源：http://oh.hahajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jp.lnxyls.cn

[U68] PHP：PDO 连接
来源：http://ff.huanxung.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vh.huixinmuqiang.cn

[U69] PHP：PDO 预处理
来源：http://va.shxzukj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hk.9csxet.cn

[U70] PHP：PDO 事务
来源：http://ie.shxzukj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://aw.wgjwhj.cn

[U71] PHP：抛出异常
来源：http://vw.szsharing.cn

throw new RuntimeException("失败", 500);
来源：http://qn.shxzskj.cn

[U72] PHP：写错误日志
来源：http://cx.521024.cn

error_log("失败: " . $e->getMessage());
来源：http://gk.jianghongdianzi.cn

[U73] PHP：读取 ini 配置
来源：http://fz.yuexingan06.cn

parse_ini_file("config.ini", true)
来源：http://ny.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://ts.jctech888.com.cn

getenv("APP_ENV") ?: "production"
来源：http://aa.asd995.cn

[U75] PHP：依赖注入
来源：http://nc.jianghongdianzi.cn

composer require psr/container
来源：http://qb.9csxet.cn

[U76] PHP：简单路由
来源：http://vy.hahajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mv.nicolike.cn

[U77] PHP：模板渲染
来源：http://ar.wgjwhj.cn

composer require twig/twig
来源：http://vq.yuntaijiaju.cn

[U78] PHP：单元测试
来源：http://nb.hnjuh.cn

composer require --dev phpunit/phpunit
来源：http://dt.lnxyls.cn

[U79] PHP：静态分析
来源：http://bq.hahajie.cn

composer require --dev phpstan/phpstan
来源：http://uq.asd995.cn

[U80] PHP：代码规范修复
来源：http://or.hnjuh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ob.shxzukj.cn

[U81] JS：初始化项目
来源：http://he.asd995.cn

npm init -y;  npm i express
来源：http://bw.lnxyls.cn

[U82] JS：package.json 脚本
来源：http://mh.haigaiapp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yd.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://ex.lnxyls.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vt.521024.cn

[U84] JS：CommonJS 写法
来源：http://ek.newstarts.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ob.newstarts.cn

[U85] JS：可选链
来源：http://ys.yuexingan06.cn

a?.b?.c
来源：http://wi.jianghongdianzi.cn

[U86] JS：空值合并
来源：http://fe.huanxung.cn

a ?? b
来源：http://kk.jianghongdianzi.cn

[U87] JS：解构默认值
来源：http://ab.asd995.cn

const { a = 1, b = 2 } = obj;
来源：http://zl.yuntaijiaju.cn

[U88] JS：对象展开合并
来源：http://pw.huixiangedu.cn

{ ...a, ...b }
来源：http://in.bjjhwx.cn

[U89] JS：数组去重
来源：http://hj.panjiajie.cn

[...new Set(arr)]
来源：http://xf.chemitech.net.cn

[U90] JS：数字数组排序
来源：http://xy.yuexingan06.cn

[...arr].sort((a, b) => a - b)
来源：http://bm.shxzukj.cn

[U91] JS：对象键值遍历
来源：http://ay.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://md.panjiajie.cn

[U92] JS：深拷贝
来源：http://fc.newstarts.cn

structuredClone(obj)
来源：http://xw.bookmarksfly.cn

[U93] JS：模板字符串
来源：http://gu.szxytkj.cn

`共 ${n} 条`
来源：http://az.huixinmuqiang.cn

[U94] JS：箭头函数
来源：http://zs.huixinmuqiang.cn

const double = x => x * 2;
来源：http://io.9csxet.cn

[U95] JS：Promise 包装
来源：http://yt.panjiajie.cn

new Promise((resolve, reject) => {})
来源：http://rn.yuexingan06.cn

[U96] JS：async/await 与异常
来源：http://xw.colortex.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cw.nicolike.cn

[U97] JS：并发请求
来源：http://qt.hnjuh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://cn.newstarts.cn

[U98] JS：fetch 带 JSON
来源：http://ut.lnxyls.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ud.wgjwhj.cn

[U99] JS：事件监听
来源：http://ok.shxzskj.cn

el.addEventListener("click", e => {})
来源：http://xm.hahajie.cn

[U100] JS：DOM 查询
来源：http://kr.haigaiapp.cn

document.querySelector(".item")
来源：http://js.9csxet.cn

[U101] JS：classList 操作
来源：http://uf.muxihuayi.cn

el.classList.toggle("active")
来源：http://yi.szsharing.cn

[U102] JS：本地存储
来源：http://vr.huixiangedu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ao.wgjwhj.cn

[U103] JS：定时器
来源：http://oz.nszjky.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qk.szxytkj.cn

[U104] JS：防抖
来源：http://bs.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fq.521024.cn

[U105] JS：节流
来源：http://qw.shxzskj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gv.muxihuayi.cn

[U106] JS：日期格式化
来源：http://qt.panjiajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tl.bjjhwx.cn

[U107] JS：数字千分位
来源：http://rx.muxihuayi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jt.shxzukj.cn

[U108] JS：随机整数
来源：http://pg.chemitech.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cr.jctech888.com.cn

[U109] JS：数组分组
来源：http://sg.nicolike.cn

Object.groupBy(arr, x => x.type)
来源：http://sv.muxihuayi.cn

[U110] JS：数组分块
来源：http://qg.colortex.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zl.huixiangedu.cn

[U111] JS：对象转 Map
来源：http://pe.jianghongdianzi.cn

new Map(Object.entries(obj))
来源：http://ni.huixinmuqiang.cn

[U112] JS：字符串补位
来源：http://kj.bjjhwx.cn

"7".padStart(3, "0")
来源：http://oe.yuntaijiaju.cn

[U113] JS：正则替换全部
来源：http://fj.chemitech.net.cn

s.replaceAll("a", "b")
来源：http://ly.panjiajie.cn

[U114] JS：JSON 深比较
来源：http://am.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://uo.shxzskj.cn

[U115] JS：生成 UUID
来源：http://cu.shxzukj.cn

crypto.randomUUID()
来源：http://le.jianghongdianzi.cn

[U116] JS：类型检查（JSDoc）
来源：http://iy.gzmigu.cn

/** @param {string} name */ function f(name) {}
来源：http://ny.nszjky.cn

[U117] JS：单元测试
来源：http://qy.chemitech.net.cn

npm i -D vitest;  npx vitest
来源：http://gj.lnxyls.cn

[U118] JS：开发服务器
来源：http://fi.nicolike.cn

npm i -D vite;  npx vite
来源：http://pj.jctech888.com.cn

[U119] JS：生产构建
来源：http://th.haigaiapp.cn

npx vite build
来源：http://pr.nszjky.cn

[U120] JS：读取环境变量（Vite）
来源：http://rf.nszjky.cn

import.meta.env.VITE_API_URL
来源：http://oj.shtwfgs.cn

================================================================================
来源：http://sl.nszjky.cn

统计汇总
来源：http://tk.panjiajie.cn

================================================================================
来源：http://tk.hnjuh.cn

按语言统计（条）：
来源：http://an.jctech888.com.cn

Python ......... 252
来源：http://fg.shxzukj.cn

PHP ............ 252
来源：http://sl.muxihuayi.cn

JavaScript ..... 252
来源：http://uv.chemitech.net.cn

TypeScript ..... 212
来源：http://gk.bjjhwx.cn

Java ........... 212
来源：http://ob.hnjuh.cn

Go ............. 212
来源：http://qm.hnjuh.cn

Ruby ........... 212
来源：http://mh.bjjhwx.cn

C# ............. 212
来源：http://fe.asd995.cn

C .............. 30
来源：http://ku.szsharing.cn

C++ ............ 30
来源：http://zg.haigaiapp.cn

SQL ............ 90
来源：http://fg.panjiajie.cn

Bash ........... 80
来源：http://kg.wgjwhj.cn

Kotlin ......... 15
来源：http://ak.huixinmuqiang.cn

Swift .......... 15
来源：http://mi.9csxet.cn

Lua ............ 10
来源：http://zw.haigaiapp.cn

Perl ........... 10
来源：http://rv.shxzskj.cn

Scala .......... 10
来源：http://su.yuntaijiaju.cn

------------------------------------
来源：http://zj.shxzskj.cn

合计 ........... 2106 条
来源：http://pp.hnjuh.cn

按章节统计：
来源：http://vk.huanxung.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pi.muxihuayi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ow.nszjky.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dv.szsharing.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zt.bookmarksfly.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qo.hnjuh.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dq.asd995.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ve.hnjuh.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zt.bookmarksfly.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uu.jianghongdianzi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rp.shxzukj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bq.nszjky.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ui.bjjhwx.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wy.szxytkj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sr.wgjwhj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://js.9csxet.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tz.yuexingan06.cn

Q SQL 专题                              90
来源：http://fe.shxzskj.cn

R Bash 专题                             80
来源：http://xq.nicolike.cn

S C / C++ 专题                          60
来源：http://gc.nicolike.cn

T 其他语言补充                          60
来源：http://it.gzmigu.cn

U 高频实用片段                         120
来源：http://wq.shxzskj.cn

------------------------------------
来源：http://bm.yuntaijiaju.cn

合计                                  2106 条
来源：http://or.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://jx.shtwfgs.cn

使用提醒
来源：http://he.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://dk.bjjhwx.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ej.9csxet.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qr.jianghongdianzi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dn.panjiajie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://cx.nicolike.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ju.gzmigu.cn

—— 文件结束 ——
来源：http://kb.muxihuayi.cn

================================================================================
来源：http://pt.shxzskj.cn

程序语言常见例子速查手册（2024 版）
来源：http://nh.wgjwhj.cn

Common Programming Examples Cheat Book
来源：http://wc.521024.cn

================================================================================
来源：http://ag.nszjky.cn

【收录内容】
来源：http://pr.muxihuayi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://br.hnjuh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vk.shxzukj.cn

SQL · Bash · C · C++
来源：http://mu.panjiajie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cr.wgjwhj.cn

【使用说明】
来源：http://xh.lnxyls.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://md.jctech888.com.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ta.huixiangedu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vk.huixiangedu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://db.wgjwhj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ls.9csxet.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gf.asd995.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tx.huixiangedu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ox.9csxet.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://br.bookmarksfly.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jp.521024.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://au.nicolike.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xo.huanxung.cn

【文件统计】
来源：http://yb.lnxyls.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ri.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://zx.nszjky.cn

目  录
来源：http://rk.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://zc.shxzskj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qx.9csxet.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ge.asd995.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zx.huixinmuqiang.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://so.szxytkj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pp.shxzskj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mt.bookmarksfly.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vu.chemitech.net.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sj.jctech888.com.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://yd.gzmigu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://aj.wgjwhj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xl.bookmarksfly.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ct.lnxyls.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xo.asd995.cn


<!-- 参考信息 -->