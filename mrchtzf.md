代发 wailian999

[U19] Py：正则替换带回调
来源：http://bf.newstarts.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rw.colortex.cn

[U20] Py：缓存函数结果
来源：http://qd.huanxung.cn

@functools.lru_cache(maxsize=None)
来源：http://fo.huanxung.cn

[U21] Py：自定义上下文管理器
来源：http://da.newstarts.cn

@contextlib.contextmanager
来源：http://nb.lnxyls.cn

[U22] Py：矩阵转置
来源：http://pv.huanxung.cn

list(zip(*m))
来源：http://nt.nicolike.cn

[U23] Py：分块读取大文件
来源：http://fp.bjjhwx.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hc.lnxyls.cn

[U24] Py：路径操作
来源：http://az.shtwfgs.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fe.yuexingan06.cn

[U25] Py：CSV 按字典读
来源：http://ul.newstarts.cn

csv.DictReader(f)
来源：http://aa.muxihuayi.cn

[U26] Py：并发下载
来源：http://ep.nszjky.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vh.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://ya.colortex.cn

aiohttp.ClientSession() 配合 async with
来源：http://ez.shxzskj.cn

[U28] Py：类型别名
来源：http://nl.yuntaijiaju.cn

UserId = int
来源：http://hy.hahajie.cn

[U29] Py：属性校验
来源：http://pd.bjjhwx.cn

@property 与 @x.setter 配合
来源：http://ns.bjjhwx.cn

[U30] Py：数据类
来源：http://dr.jianghongdianzi.cn

@dataclass(slots=True)
来源：http://kt.haigaiapp.cn

[U31] Py：单测
来源：http://ki.panjiajie.cn

python -m pytest -q
来源：http://te.nicolike.cn

[U32] Py：代码格式化
来源：http://sq.haigaiapp.cn

ruff format . && ruff check --fix .
来源：http://aj.521024.cn

[U33] Py：打包发布
来源：http://ir.bjjhwx.cn

python -m build  （依赖 pyproject.toml）
来源：http://vo.shtwfgs.cn

[U34] Py：判断编码
来源：http://yf.haigaiapp.cn

chardet.detect(raw)
来源：http://dj.wgjwhj.cn

[U35] Py：发送邮件
来源：http://ga.jctech888.com.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hl.9csxet.cn

[U36] Py：定时任务
来源：http://kh.huanxung.cn

schedule.every(10).minutes.do(job)
来源：http://xx.gzmigu.cn

[U37] Py：读写 Excel
来源：http://em.yuntaijiaju.cn

pandas.read_excel / DataFrame.to_excel
来源：http://nj.nicolike.cn

[U38] Py：获取脚本所在目录
来源：http://kz.gzmigu.cn

Path(__file__).resolve().parent
来源：http://cd.huixinmuqiang.cn

[U39] Py：判断是否在交互环境
来源：http://rr.huixinmuqiang.cn

sys.stdout.isatty()
来源：http://xg.jianghongdianzi.cn

[U40] Py：打印到标准错误
来源：http://zl.huixinmuqiang.cn

print("err", file=sys.stderr)
来源：http://dt.lnxyls.cn

[U41] PHP：初始化 Composer 项目
来源：http://wn.jctech888.com.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://py.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://yx.hnjuh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cl.lnxyls.cn

[U43] PHP：声明命名空间
来源：http://co.nicolike.cn

namespace App\Http;
来源：http://zw.lnxyls.cn

[U44] PHP：开启严格类型
来源：http://sq.huixinmuqiang.cn

declare(strict_types=1);
来源：http://ek.chemitech.net.cn

[U45] PHP：类型声明与返回类型
来源：http://lp.szxytkj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://kh.asd995.cn

[U46] PHP：可空类型
来源：http://uq.huixiangedu.cn

?string $name = null
来源：http://rz.hahajie.cn

[U47] PHP：联合类型
来源：http://ec.asd995.cn

int|string $id
来源：http://eo.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://wa.shxzskj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wp.yuexingan06.cn

[U49] PHP：只读属性
来源：http://um.shtwfgs.cn

public readonly string $name
来源：http://mf.colortex.cn

[U50] PHP：构造器属性提升
来源：http://id.521024.cn

public function __construct(private int $id) {}
来源：http://ws.wgjwhj.cn

[U51] PHP：数组解构
来源：http://di.yuexingan06.cn

[$a, $b] = $arr;
来源：http://oe.hnjuh.cn

[U52] PHP：箭头函数
来源：http://fh.muxihuayi.cn

$double = fn($x) => $x * 2;
来源：http://sf.nicolike.cn

[U53] PHP：空合并运算符
来源：http://gh.shxzukj.cn

$v = $a ?? $b ?? "default";
来源：http://mq.szxytkj.cn

[U54] PHP：空安全调用
来源：http://dt.muxihuayi.cn

$obj?->method()
来源：http://xf.huixinmuqiang.cn

[U55] PHP：match 表达式
来源：http://cl.521024.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ng.wgjwhj.cn

[U56] PHP：命名参数
来源：http://jz.yuntaijiaju.cn

f(a: 1, b: 2)
来源：http://um.521024.cn

[U57] PHP：字符串插值
来源：http://qo.yuntaijiaju.cn

"值: {$a}"
来源：http://pn.gzmigu.cn

[U58] PHP：数组三件套
来源：http://lj.yuexingan06.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zz.haigaiapp.cn

[U59] PHP：自定义排序
来源：http://sq.newstarts.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rj.asd995.cn

[U60] PHP：JSON 编解码
来源：http://yo.9csxet.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nx.gzmigu.cn

[U61] PHP：正则
来源：http://ju.jctech888.com.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lz.hahajie.cn

[U62] PHP：日期对象
来源：http://fm.521024.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ox.panjiajie.cn

[U63] PHP：文件读写
来源：http://xq.shxzskj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://iz.yuexingan06.cn

[U64] PHP：目录遍历
来源：http://ae.haigaiapp.cn

glob("dir/*.php");  scandir("dir");
来源：http://kg.wgjwhj.cn

[U65] PHP：会话
来源：http://qj.szsharing.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ii.lnxyls.cn

[U66] PHP：设置 Cookie
来源：http://fc.bjjhwx.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xa.huanxung.cn

[U67] PHP：处理文件上传
来源：http://dq.huanxung.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tt.hahajie.cn

[U68] PHP：PDO 连接
来源：http://bc.shtwfgs.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xc.muxihuayi.cn

[U69] PHP：PDO 预处理
来源：http://qh.szxytkj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fj.haigaiapp.cn

[U70] PHP：PDO 事务
来源：http://gw.colortex.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xp.9csxet.cn

[U71] PHP：抛出异常
来源：http://ar.huixiangedu.cn

throw new RuntimeException("失败", 500);
来源：http://bb.bookmarksfly.cn

[U72] PHP：写错误日志
来源：http://qx.huixinmuqiang.cn

error_log("失败: " . $e->getMessage());
来源：http://hk.huanxung.cn

[U73] PHP：读取 ini 配置
来源：http://wv.lnxyls.cn

parse_ini_file("config.ini", true)
来源：http://qk.colortex.cn

[U74] PHP：读取环境变量
来源：http://ra.jianghongdianzi.cn

getenv("APP_ENV") ?: "production"
来源：http://kb.bookmarksfly.cn

[U75] PHP：依赖注入
来源：http://sq.huanxung.cn

composer require psr/container
来源：http://it.huanxung.cn

[U76] PHP：简单路由
来源：http://fb.wgjwhj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hd.shxzukj.cn

[U77] PHP：模板渲染
来源：http://qv.hnjuh.cn

composer require twig/twig
来源：http://fd.shtwfgs.cn

[U78] PHP：单元测试
来源：http://qz.lnxyls.cn

composer require --dev phpunit/phpunit
来源：http://le.huixinmuqiang.cn

[U79] PHP：静态分析
来源：http://ee.newstarts.cn

composer require --dev phpstan/phpstan
来源：http://ur.gzmigu.cn

[U80] PHP：代码规范修复
来源：http://lq.huixiangedu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ja.huixinmuqiang.cn

[U81] JS：初始化项目
来源：http://ci.colortex.cn

npm init -y;  npm i express
来源：http://mv.huanxung.cn

[U82] JS：package.json 脚本
来源：http://fl.asd995.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://at.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://gz.newstarts.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jm.9csxet.cn

[U84] JS：CommonJS 写法
来源：http://bb.nicolike.cn

module.exports = { a };  const { a } = require("./m");
来源：http://dj.yuexingan06.cn

[U85] JS：可选链
来源：http://bc.newstarts.cn

a?.b?.c
来源：http://rt.hahajie.cn

[U86] JS：空值合并
来源：http://xz.bjjhwx.cn

a ?? b
来源：http://kv.shtwfgs.cn

[U87] JS：解构默认值
来源：http://hh.hahajie.cn

const { a = 1, b = 2 } = obj;
来源：http://gd.huanxung.cn

[U88] JS：对象展开合并
来源：http://hx.nszjky.cn

{ ...a, ...b }
来源：http://bx.newstarts.cn

[U89] JS：数组去重
来源：http://wr.shxzukj.cn

[...new Set(arr)]
来源：http://jt.wgjwhj.cn

[U90] JS：数字数组排序
来源：http://rj.muxihuayi.cn

[...arr].sort((a, b) => a - b)
来源：http://cr.yuntaijiaju.cn

[U91] JS：对象键值遍历
来源：http://wc.panjiajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xi.bookmarksfly.cn

[U92] JS：深拷贝
来源：http://tv.chemitech.net.cn

structuredClone(obj)
来源：http://mu.yuntaijiaju.cn

[U93] JS：模板字符串
来源：http://wj.jctech888.com.cn

`共 ${n} 条`
来源：http://eq.chemitech.net.cn

[U94] JS：箭头函数
来源：http://it.bjjhwx.cn

const double = x => x * 2;
来源：http://cp.9csxet.cn

[U95] JS：Promise 包装
来源：http://lc.colortex.cn

new Promise((resolve, reject) => {})
来源：http://pj.nicolike.cn

[U96] JS：async/await 与异常
来源：http://sr.jctech888.com.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yg.szxytkj.cn

[U97] JS：并发请求
来源：http://we.jianghongdianzi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lg.haigaiapp.cn

[U98] JS：fetch 带 JSON
来源：http://ub.yuntaijiaju.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ht.panjiajie.cn

[U99] JS：事件监听
来源：http://yj.bookmarksfly.cn

el.addEventListener("click", e => {})
来源：http://de.muxihuayi.cn

[U100] JS：DOM 查询
来源：http://lm.gzmigu.cn

document.querySelector(".item")
来源：http://cn.hnjuh.cn

[U101] JS：classList 操作
来源：http://uj.yuexingan06.cn

el.classList.toggle("active")
来源：http://gi.haigaiapp.cn

[U102] JS：本地存储
来源：http://bt.szxytkj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cw.bjjhwx.cn

[U103] JS：定时器
来源：http://av.lnxyls.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wu.jctech888.com.cn

[U104] JS：防抖
来源：http://ib.newstarts.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vw.521024.cn

[U105] JS：节流
来源：http://fn.jctech888.com.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ls.shxzukj.cn

[U106] JS：日期格式化
来源：http://to.newstarts.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://iq.shxzukj.cn

[U107] JS：数字千分位
来源：http://xd.wgjwhj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bh.jianghongdianzi.cn

[U108] JS：随机整数
来源：http://hw.521024.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xe.huanxung.cn

[U109] JS：数组分组
来源：http://km.asd995.cn

Object.groupBy(arr, x => x.type)
来源：http://ew.colortex.cn

[U110] JS：数组分块
来源：http://uh.bookmarksfly.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jw.shxzskj.cn

[U111] JS：对象转 Map
来源：http://ug.newstarts.cn

new Map(Object.entries(obj))
来源：http://uf.haigaiapp.cn

[U112] JS：字符串补位
来源：http://ui.panjiajie.cn

"7".padStart(3, "0")
来源：http://so.hnjuh.cn

[U113] JS：正则替换全部
来源：http://bi.nszjky.cn

s.replaceAll("a", "b")
来源：http://mp.colortex.cn

[U114] JS：JSON 深比较
来源：http://xn.shtwfgs.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nq.bjjhwx.cn

[U115] JS：生成 UUID
来源：http://ed.bookmarksfly.cn

crypto.randomUUID()
来源：http://wi.hahajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://mc.szxytkj.cn

/** @param {string} name */ function f(name) {}
来源：http://ok.huixinmuqiang.cn

[U117] JS：单元测试
来源：http://uh.hnjuh.cn

npm i -D vitest;  npx vitest
来源：http://va.9csxet.cn

[U118] JS：开发服务器
来源：http://ju.newstarts.cn

npm i -D vite;  npx vite
来源：http://lv.panjiajie.cn

[U119] JS：生产构建
来源：http://ep.9csxet.cn

npx vite build
来源：http://mf.yuntaijiaju.cn

[U120] JS：读取环境变量（Vite）
来源：http://zi.nicolike.cn

import.meta.env.VITE_API_URL
来源：http://ps.haigaiapp.cn

================================================================================
来源：http://pe.hahajie.cn

统计汇总
来源：http://kr.hnjuh.cn

================================================================================
来源：http://hq.shxzskj.cn

按语言统计（条）：
来源：http://kr.szxytkj.cn

Python ......... 252
来源：http://wd.lnxyls.cn

PHP ............ 252
来源：http://uz.newstarts.cn

JavaScript ..... 252
来源：http://sz.521024.cn

TypeScript ..... 212
来源：http://wh.huanxung.cn

Java ........... 212
来源：http://el.haigaiapp.cn

Go ............. 212
来源：http://wj.shtwfgs.cn

Ruby ........... 212
来源：http://ip.jctech888.com.cn

C# ............. 212
来源：http://uv.hnjuh.cn

C .............. 30
来源：http://mk.hnjuh.cn

C++ ............ 30
来源：http://rp.szsharing.cn

SQL ............ 90
来源：http://pb.bookmarksfly.cn

Bash ........... 80
来源：http://ss.9csxet.cn

Kotlin ......... 15
来源：http://cs.jianghongdianzi.cn

Swift .......... 15
来源：http://hk.muxihuayi.cn

Lua ............ 10
来源：http://mv.gzmigu.cn

Perl ........... 10
来源：http://yf.yuexingan06.cn

Scala .......... 10
来源：http://ff.shtwfgs.cn

------------------------------------
来源：http://sp.521024.cn

合计 ........... 2106 条
来源：http://sb.9csxet.cn

按章节统计：
来源：http://be.jianghongdianzi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ae.jctech888.com.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nh.szsharing.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yt.bjjhwx.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vw.newstarts.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yh.chemitech.net.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sg.hahajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ae.bookmarksfly.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rc.shxzskj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vf.chemitech.net.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rr.szxytkj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ve.huanxung.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pp.yuexingan06.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pd.lnxyls.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gj.bookmarksfly.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hu.bookmarksfly.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pr.9csxet.cn

Q SQL 专题                              90
来源：http://io.colortex.cn

R Bash 专题                             80
来源：http://yg.shxzukj.cn

S C / C++ 专题                          60
来源：http://dm.shxzskj.cn

T 其他语言补充                          60
来源：http://cf.hnjuh.cn

U 高频实用片段                         120
来源：http://yl.gzmigu.cn

------------------------------------
来源：http://lj.9csxet.cn

合计                                  2106 条
来源：http://jh.szsharing.cn

--------------------------------------------------------------------------------
来源：http://cy.haigaiapp.cn

使用提醒
来源：http://dt.colortex.cn

--------------------------------------------------------------------------------
来源：http://kw.newstarts.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qq.hnjuh.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ia.gzmigu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tj.huanxung.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ad.muxihuayi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mv.jianghongdianzi.cn

—— 文件结束 ——
来源：http://bb.lnxyls.cn

================================================================================
来源：http://qj.huanxung.cn

程序语言常见例子速查手册（2024 版）
来源：http://lz.nszjky.cn

Common Programming Examples Cheat Book
来源：http://dc.bjjhwx.cn

================================================================================
来源：http://dl.bjjhwx.cn

【收录内容】
来源：http://ff.szxytkj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zc.521024.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ky.colortex.cn

SQL · Bash · C · C++
来源：http://td.521024.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tr.huanxung.cn

【使用说明】
来源：http://df.521024.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ri.szxytkj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://iv.yuexingan06.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://aa.wgjwhj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fh.jctech888.com.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://gu.haigaiapp.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jl.chemitech.net.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zf.huanxung.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mf.chemitech.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qn.huixiangedu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://is.szxytkj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://eb.shtwfgs.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ph.haigaiapp.cn

【文件统计】
来源：http://eh.muxihuayi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://np.huanxung.cn

--------------------------------------------------------------------------------
来源：http://rx.jianghongdianzi.cn

目  录
来源：http://na.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://xx.colortex.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kv.panjiajie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ru.shtwfgs.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vl.chemitech.net.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bu.huanxung.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wq.nszjky.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vi.lnxyls.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sb.shxzskj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dc.panjiajie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zx.huanxung.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gr.huanxung.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vs.shxzukj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cw.huixinmuqiang.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kw.shxzskj.cn


<!-- 参考信息 -->