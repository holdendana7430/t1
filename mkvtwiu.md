代发 wailian999

[U19] Py：正则替换带回调
来源：http://ff.jctech888.com.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dw.jianghongdianzi.cn

[U20] Py：缓存函数结果
来源：http://xh.colortex.cn

@functools.lru_cache(maxsize=None)
来源：http://ol.szxytkj.cn

[U21] Py：自定义上下文管理器
来源：http://si.bookmarksfly.cn

@contextlib.contextmanager
来源：http://im.asd995.cn

[U22] Py：矩阵转置
来源：http://vc.newstarts.cn

list(zip(*m))
来源：http://ij.hnjuh.cn

[U23] Py：分块读取大文件
来源：http://uv.bookmarksfly.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cs.asd995.cn

[U24] Py：路径操作
来源：http://lc.yuexingan06.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ks.huixiangedu.cn

[U25] Py：CSV 按字典读
来源：http://pf.bjjhwx.cn

csv.DictReader(f)
来源：http://mw.nicolike.cn

[U26] Py：并发下载
来源：http://zd.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oj.muxihuayi.cn

[U27] Py：异步 HTTP
来源：http://yj.lnxyls.cn

aiohttp.ClientSession() 配合 async with
来源：http://na.hnjuh.cn

[U28] Py：类型别名
来源：http://zo.shxzukj.cn

UserId = int
来源：http://di.chemitech.net.cn

[U29] Py：属性校验
来源：http://ee.nicolike.cn

@property 与 @x.setter 配合
来源：http://dt.9csxet.cn

[U30] Py：数据类
来源：http://nv.huixinmuqiang.cn

@dataclass(slots=True)
来源：http://yh.bookmarksfly.cn

[U31] Py：单测
来源：http://hy.521024.cn

python -m pytest -q
来源：http://vr.bjjhwx.cn

[U32] Py：代码格式化
来源：http://py.huanxung.cn

ruff format . && ruff check --fix .
来源：http://ji.szsharing.cn

[U33] Py：打包发布
来源：http://yf.bookmarksfly.cn

python -m build  （依赖 pyproject.toml）
来源：http://lw.szxytkj.cn

[U34] Py：判断编码
来源：http://qs.haigaiapp.cn

chardet.detect(raw)
来源：http://rh.nszjky.cn

[U35] Py：发送邮件
来源：http://fh.bjjhwx.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qx.chemitech.net.cn

[U36] Py：定时任务
来源：http://qp.hnjuh.cn

schedule.every(10).minutes.do(job)
来源：http://bd.hnjuh.cn

[U37] Py：读写 Excel
来源：http://bc.panjiajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dw.nszjky.cn

[U38] Py：获取脚本所在目录
来源：http://om.shtwfgs.cn

Path(__file__).resolve().parent
来源：http://rs.yuexingan06.cn

[U39] Py：判断是否在交互环境
来源：http://fi.nicolike.cn

sys.stdout.isatty()
来源：http://ac.lnxyls.cn

[U40] Py：打印到标准错误
来源：http://hz.muxihuayi.cn

print("err", file=sys.stderr)
来源：http://tz.muxihuayi.cn

[U41] PHP：初始化 Composer 项目
来源：http://pd.yuexingan06.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gm.huixinmuqiang.cn

[U42] PHP：PSR-4 自动加载
来源：http://ir.muxihuayi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wq.bjjhwx.cn

[U43] PHP：声明命名空间
来源：http://yl.huixiangedu.cn

namespace App\Http;
来源：http://tm.huixiangedu.cn

[U44] PHP：开启严格类型
来源：http://ua.shtwfgs.cn

declare(strict_types=1);
来源：http://uf.shxzukj.cn

[U45] PHP：类型声明与返回类型
来源：http://yy.hnjuh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lq.szxytkj.cn

[U46] PHP：可空类型
来源：http://ro.521024.cn

?string $name = null
来源：http://xc.yuexingan06.cn

[U47] PHP：联合类型
来源：http://vu.huixinmuqiang.cn

int|string $id
来源：http://fo.szxytkj.cn

[U48] PHP：纯枚举
来源：http://ny.shxzukj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ln.newstarts.cn

[U49] PHP：只读属性
来源：http://sw.panjiajie.cn

public readonly string $name
来源：http://kh.chemitech.net.cn

[U50] PHP：构造器属性提升
来源：http://zg.hnjuh.cn

public function __construct(private int $id) {}
来源：http://bb.lnxyls.cn

[U51] PHP：数组解构
来源：http://tj.shtwfgs.cn

[$a, $b] = $arr;
来源：http://hp.hnjuh.cn

[U52] PHP：箭头函数
来源：http://pt.lnxyls.cn

$double = fn($x) => $x * 2;
来源：http://no.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://ww.yuexingan06.cn

$v = $a ?? $b ?? "default";
来源：http://no.nszjky.cn

[U54] PHP：空安全调用
来源：http://pp.chemitech.net.cn

$obj?->method()
来源：http://le.huixinmuqiang.cn

[U55] PHP：match 表达式
来源：http://xo.asd995.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hi.hahajie.cn

[U56] PHP：命名参数
来源：http://gv.muxihuayi.cn

f(a: 1, b: 2)
来源：http://vb.huanxung.cn

[U57] PHP：字符串插值
来源：http://ip.newstarts.cn

"值: {$a}"
来源：http://ge.colortex.cn

[U58] PHP：数组三件套
来源：http://eb.nicolike.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zm.huixiangedu.cn

[U59] PHP：自定义排序
来源：http://kz.bookmarksfly.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pu.shxzskj.cn

[U60] PHP：JSON 编解码
来源：http://hw.hnjuh.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ax.nszjky.cn

[U61] PHP：正则
来源：http://ih.yuntaijiaju.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://iz.jctech888.com.cn

[U62] PHP：日期对象
来源：http://xn.newstarts.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kx.huixiangedu.cn

[U63] PHP：文件读写
来源：http://kl.huixinmuqiang.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bz.9csxet.cn

[U64] PHP：目录遍历
来源：http://ca.huixiangedu.cn

glob("dir/*.php");  scandir("dir");
来源：http://ws.gzmigu.cn

[U65] PHP：会话
来源：http://bl.9csxet.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://aa.asd995.cn

[U66] PHP：设置 Cookie
来源：http://uz.szsharing.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ur.panjiajie.cn

[U67] PHP：处理文件上传
来源：http://jr.panjiajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ur.huixiangedu.cn

[U68] PHP：PDO 连接
来源：http://kr.huixinmuqiang.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uw.shxzskj.cn

[U69] PHP：PDO 预处理
来源：http://lb.gzmigu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pg.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://qo.asd995.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tb.shxzskj.cn

[U71] PHP：抛出异常
来源：http://zp.nicolike.cn

throw new RuntimeException("失败", 500);
来源：http://ax.hnjuh.cn

[U72] PHP：写错误日志
来源：http://aq.newstarts.cn

error_log("失败: " . $e->getMessage());
来源：http://za.huixinmuqiang.cn

[U73] PHP：读取 ini 配置
来源：http://ql.szxytkj.cn

parse_ini_file("config.ini", true)
来源：http://kd.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://os.asd995.cn

getenv("APP_ENV") ?: "production"
来源：http://yx.hnjuh.cn

[U75] PHP：依赖注入
来源：http://ag.panjiajie.cn

composer require psr/container
来源：http://fz.szsharing.cn

[U76] PHP：简单路由
来源：http://xu.shxzukj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mw.jctech888.com.cn

[U77] PHP：模板渲染
来源：http://qt.asd995.cn

composer require twig/twig
来源：http://cf.chemitech.net.cn

[U78] PHP：单元测试
来源：http://qs.wgjwhj.cn

composer require --dev phpunit/phpunit
来源：http://fw.haigaiapp.cn

[U79] PHP：静态分析
来源：http://ds.nszjky.cn

composer require --dev phpstan/phpstan
来源：http://ms.huixiangedu.cn

[U80] PHP：代码规范修复
来源：http://nr.shtwfgs.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pz.shxzukj.cn

[U81] JS：初始化项目
来源：http://id.hnjuh.cn

npm init -y;  npm i express
来源：http://cj.hahajie.cn

[U82] JS：package.json 脚本
来源：http://vx.9csxet.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wj.muxihuayi.cn

[U83] JS：ES Module 导入导出
来源：http://zj.521024.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ce.bookmarksfly.cn

[U84] JS：CommonJS 写法
来源：http://nb.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://og.huixinmuqiang.cn

[U85] JS：可选链
来源：http://wc.huixinmuqiang.cn

a?.b?.c
来源：http://dq.asd995.cn

[U86] JS：空值合并
来源：http://vm.bjjhwx.cn

a ?? b
来源：http://mm.panjiajie.cn

[U87] JS：解构默认值
来源：http://kw.yuntaijiaju.cn

const { a = 1, b = 2 } = obj;
来源：http://xt.9csxet.cn

[U88] JS：对象展开合并
来源：http://wk.shxzskj.cn

{ ...a, ...b }
来源：http://ke.9csxet.cn

[U89] JS：数组去重
来源：http://ac.szxytkj.cn

[...new Set(arr)]
来源：http://sb.hahajie.cn

[U90] JS：数字数组排序
来源：http://gw.huixiangedu.cn

[...arr].sort((a, b) => a - b)
来源：http://yr.bookmarksfly.cn

[U91] JS：对象键值遍历
来源：http://ht.shxzukj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://de.hahajie.cn

[U92] JS：深拷贝
来源：http://lx.shxzskj.cn

structuredClone(obj)
来源：http://io.haigaiapp.cn

[U93] JS：模板字符串
来源：http://qo.nszjky.cn

`共 ${n} 条`
来源：http://kh.muxihuayi.cn

[U94] JS：箭头函数
来源：http://ye.jctech888.com.cn

const double = x => x * 2;
来源：http://mq.lnxyls.cn

[U95] JS：Promise 包装
来源：http://hp.lnxyls.cn

new Promise((resolve, reject) => {})
来源：http://tr.jctech888.com.cn

[U96] JS：async/await 与异常
来源：http://be.nicolike.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zk.jctech888.com.cn

[U97] JS：并发请求
来源：http://rq.521024.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://sh.yuexingan06.cn

[U98] JS：fetch 带 JSON
来源：http://as.shxzskj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zr.newstarts.cn

[U99] JS：事件监听
来源：http://dv.nicolike.cn

el.addEventListener("click", e => {})
来源：http://tt.shxzukj.cn

[U100] JS：DOM 查询
来源：http://tm.szsharing.cn

document.querySelector(".item")
来源：http://fe.nszjky.cn

[U101] JS：classList 操作
来源：http://vt.huixiangedu.cn

el.classList.toggle("active")
来源：http://xo.chemitech.net.cn

[U102] JS：本地存储
来源：http://nk.hahajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hj.colortex.cn

[U103] JS：定时器
来源：http://ky.wgjwhj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ju.huixinmuqiang.cn

[U104] JS：防抖
来源：http://fx.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ih.panjiajie.cn

[U105] JS：节流
来源：http://yc.panjiajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qc.hahajie.cn

[U106] JS：日期格式化
来源：http://sr.bjjhwx.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://oj.szxytkj.cn

[U107] JS：数字千分位
来源：http://cb.shxzukj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sf.jctech888.com.cn

[U108] JS：随机整数
来源：http://rb.asd995.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ra.gzmigu.cn

[U109] JS：数组分组
来源：http://zw.jianghongdianzi.cn

Object.groupBy(arr, x => x.type)
来源：http://fu.huixiangedu.cn

[U110] JS：数组分块
来源：http://rm.asd995.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lr.gzmigu.cn

[U111] JS：对象转 Map
来源：http://rt.szxytkj.cn

new Map(Object.entries(obj))
来源：http://ec.shxzskj.cn

[U112] JS：字符串补位
来源：http://hw.shxzskj.cn

"7".padStart(3, "0")
来源：http://fr.szxytkj.cn

[U113] JS：正则替换全部
来源：http://qd.521024.cn

s.replaceAll("a", "b")
来源：http://go.huanxung.cn

[U114] JS：JSON 深比较
来源：http://qj.wgjwhj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ce.szsharing.cn

[U115] JS：生成 UUID
来源：http://ok.nicolike.cn

crypto.randomUUID()
来源：http://kf.gzmigu.cn

[U116] JS：类型检查（JSDoc）
来源：http://zv.huixinmuqiang.cn

/** @param {string} name */ function f(name) {}
来源：http://ug.521024.cn

[U117] JS：单元测试
来源：http://tv.huixinmuqiang.cn

npm i -D vitest;  npx vitest
来源：http://gd.9csxet.cn

[U118] JS：开发服务器
来源：http://sx.panjiajie.cn

npm i -D vite;  npx vite
来源：http://ka.muxihuayi.cn

[U119] JS：生产构建
来源：http://ym.shxzukj.cn

npx vite build
来源：http://zx.lnxyls.cn

[U120] JS：读取环境变量（Vite）
来源：http://be.asd995.cn

import.meta.env.VITE_API_URL
来源：http://bm.bjjhwx.cn

================================================================================
来源：http://no.nszjky.cn

统计汇总
来源：http://hr.huanxung.cn

================================================================================
来源：http://qa.szsharing.cn

按语言统计（条）：
来源：http://nh.huixiangedu.cn

Python ......... 252
来源：http://kv.szsharing.cn

PHP ............ 252
来源：http://us.huixiangedu.cn

JavaScript ..... 252
来源：http://kj.haigaiapp.cn

TypeScript ..... 212
来源：http://vu.nicolike.cn

Java ........... 212
来源：http://et.hahajie.cn

Go ............. 212
来源：http://hq.9csxet.cn

Ruby ........... 212
来源：http://kw.huixinmuqiang.cn

C# ............. 212
来源：http://if.nszjky.cn

C .............. 30
来源：http://sv.gzmigu.cn

C++ ............ 30
来源：http://st.lnxyls.cn

SQL ............ 90
来源：http://ru.yuntaijiaju.cn

Bash ........... 80
来源：http://xb.huanxung.cn

Kotlin ......... 15
来源：http://od.521024.cn

Swift .......... 15
来源：http://ud.shxzukj.cn

Lua ............ 10
来源：http://uj.yuntaijiaju.cn

Perl ........... 10
来源：http://zs.jctech888.com.cn

Scala .......... 10
来源：http://rs.hnjuh.cn

------------------------------------
来源：http://gw.newstarts.cn

合计 ........... 2106 条
来源：http://fe.szsharing.cn

按章节统计：
来源：http://kc.jianghongdianzi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bj.asd995.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ci.nszjky.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xb.chemitech.net.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tr.9csxet.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wy.shtwfgs.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vd.bookmarksfly.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ub.wgjwhj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ne.521024.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qd.szxytkj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pr.shtwfgs.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gw.jctech888.com.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sc.hnjuh.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sw.shtwfgs.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pm.hahajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zx.bookmarksfly.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qo.shxzskj.cn

Q SQL 专题                              90
来源：http://cl.muxihuayi.cn

R Bash 专题                             80
来源：http://ca.shxzukj.cn

S C / C++ 专题                          60
来源：http://mt.szxytkj.cn

T 其他语言补充                          60
来源：http://xg.jianghongdianzi.cn

U 高频实用片段                         120
来源：http://dw.huanxung.cn

------------------------------------
来源：http://zi.hnjuh.cn

合计                                  2106 条
来源：http://xr.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://ja.haigaiapp.cn

使用提醒
来源：http://av.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://pw.9csxet.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ze.nszjky.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kl.lnxyls.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://di.jianghongdianzi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://kp.gzmigu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jo.hnjuh.cn

—— 文件结束 ——
来源：http://sd.muxihuayi.cn

================================================================================
来源：http://ru.wgjwhj.cn

程序语言常见例子速查手册（2024 版）
来源：http://bk.wgjwhj.cn

Common Programming Examples Cheat Book
来源：http://ft.asd995.cn

================================================================================
来源：http://gy.huixinmuqiang.cn

【收录内容】
来源：http://gu.huanxung.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://cw.gzmigu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rm.bookmarksfly.cn

SQL · Bash · C · C++
来源：http://ko.haigaiapp.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cv.asd995.cn

【使用说明】
来源：http://pb.chemitech.net.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ow.panjiajie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://li.huixiangedu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ll.huanxung.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://my.gzmigu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://br.yuntaijiaju.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zx.lnxyls.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ti.panjiajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ah.chemitech.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ol.panjiajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nh.newstarts.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ku.newstarts.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hs.521024.cn

【文件统计】
来源：http://tk.huanxung.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nb.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://sl.bookmarksfly.cn

目  录
来源：http://jt.colortex.cn

--------------------------------------------------------------------------------
来源：http://kg.asd995.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://eg.huixinmuqiang.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wy.asd995.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fn.asd995.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://eu.bjjhwx.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://sv.shxzukj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dz.lnxyls.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://pu.muxihuayi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lj.hahajie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://im.jianghongdianzi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fj.muxihuayi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sa.nicolike.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mm.asd995.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wy.hahajie.cn


<!-- 参考信息 -->