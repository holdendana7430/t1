代发 wailian999

[U15] Py：高精度计时
来源：http://qq.huanxung.cn

t = time.perf_counter()
来源：http://zd.muxihuayi.cn

[U16] Py：命令行参数解析
来源：http://ru.yuexingan06.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fe.yuexingan06.cn

[U17] Py：初始化日志
来源：http://la.yuntaijiaju.cn

logging.basicConfig(level=logging.INFO)
来源：http://xj.9csxet.cn

[U18] Py：预编译正则
来源：http://tl.521024.cn

pat = re.compile(r"\d+")
来源：http://yo.521024.cn

[U19] Py：正则替换带回调
来源：http://mr.panjiajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oj.asd995.cn

[U20] Py：缓存函数结果
来源：http://mz.yuexingan06.cn

@functools.lru_cache(maxsize=None)
来源：http://no.nicolike.cn

[U21] Py：自定义上下文管理器
来源：http://mj.bjjhwx.cn

@contextlib.contextmanager
来源：http://so.huixiangedu.cn

[U22] Py：矩阵转置
来源：http://or.nicolike.cn

list(zip(*m))
来源：http://ll.bjjhwx.cn

[U23] Py：分块读取大文件
来源：http://kg.bjjhwx.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vg.bookmarksfly.cn

[U24] Py：路径操作
来源：http://vp.lnxyls.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rd.hnjuh.cn

[U25] Py：CSV 按字典读
来源：http://ik.panjiajie.cn

csv.DictReader(f)
来源：http://yr.lnxyls.cn

[U26] Py：并发下载
来源：http://rr.huixinmuqiang.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://da.jianghongdianzi.cn

[U27] Py：异步 HTTP
来源：http://ay.nszjky.cn

aiohttp.ClientSession() 配合 async with
来源：http://rz.bjjhwx.cn

[U28] Py：类型别名
来源：http://ld.muxihuayi.cn

UserId = int
来源：http://cy.szxytkj.cn

[U29] Py：属性校验
来源：http://xu.bookmarksfly.cn

@property 与 @x.setter 配合
来源：http://dq.huanxung.cn

[U30] Py：数据类
来源：http://zo.chemitech.net.cn

@dataclass(slots=True)
来源：http://kr.colortex.cn

[U31] Py：单测
来源：http://ke.bjjhwx.cn

python -m pytest -q
来源：http://pl.shxzskj.cn

[U32] Py：代码格式化
来源：http://wx.gzmigu.cn

ruff format . && ruff check --fix .
来源：http://zn.9csxet.cn

[U33] Py：打包发布
来源：http://ou.szxytkj.cn

python -m build  （依赖 pyproject.toml）
来源：http://hd.lnxyls.cn

[U34] Py：判断编码
来源：http://el.colortex.cn

chardet.detect(raw)
来源：http://sd.asd995.cn

[U35] Py：发送邮件
来源：http://cu.newstarts.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cv.nicolike.cn

[U36] Py：定时任务
来源：http://sf.colortex.cn

schedule.every(10).minutes.do(job)
来源：http://ks.bjjhwx.cn

[U37] Py：读写 Excel
来源：http://tc.muxihuayi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://aj.shxzukj.cn

[U38] Py：获取脚本所在目录
来源：http://rr.huanxung.cn

Path(__file__).resolve().parent
来源：http://tf.yuntaijiaju.cn

[U39] Py：判断是否在交互环境
来源：http://xj.bjjhwx.cn

sys.stdout.isatty()
来源：http://ll.haigaiapp.cn

[U40] Py：打印到标准错误
来源：http://le.chemitech.net.cn

print("err", file=sys.stderr)
来源：http://ie.lnxyls.cn

[U41] PHP：初始化 Composer 项目
来源：http://qv.bjjhwx.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bz.chemitech.net.cn

[U42] PHP：PSR-4 自动加载
来源：http://cw.gzmigu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ww.chemitech.net.cn

[U43] PHP：声明命名空间
来源：http://vy.jianghongdianzi.cn

namespace App\Http;
来源：http://hg.jianghongdianzi.cn

[U44] PHP：开启严格类型
来源：http://kn.panjiajie.cn

declare(strict_types=1);
来源：http://ll.shxzukj.cn

[U45] PHP：类型声明与返回类型
来源：http://ju.gzmigu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bo.gzmigu.cn

[U46] PHP：可空类型
来源：http://ya.huanxung.cn

?string $name = null
来源：http://kx.jctech888.com.cn

[U47] PHP：联合类型
来源：http://di.jctech888.com.cn

int|string $id
来源：http://uv.nicolike.cn

[U48] PHP：纯枚举
来源：http://xm.9csxet.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://iw.nszjky.cn

[U49] PHP：只读属性
来源：http://bn.chemitech.net.cn

public readonly string $name
来源：http://gi.lnxyls.cn

[U50] PHP：构造器属性提升
来源：http://gx.yuexingan06.cn

public function __construct(private int $id) {}
来源：http://kt.hnjuh.cn

[U51] PHP：数组解构
来源：http://dj.szxytkj.cn

[$a, $b] = $arr;
来源：http://sz.jctech888.com.cn

[U52] PHP：箭头函数
来源：http://mf.huixiangedu.cn

$double = fn($x) => $x * 2;
来源：http://ms.szxytkj.cn

[U53] PHP：空合并运算符
来源：http://kf.bjjhwx.cn

$v = $a ?? $b ?? "default";
来源：http://yr.haigaiapp.cn

[U54] PHP：空安全调用
来源：http://gn.haigaiapp.cn

$obj?->method()
来源：http://oo.huanxung.cn

[U55] PHP：match 表达式
来源：http://nf.bjjhwx.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uv.panjiajie.cn

[U56] PHP：命名参数
来源：http://ex.jctech888.com.cn

f(a: 1, b: 2)
来源：http://bp.szsharing.cn

[U57] PHP：字符串插值
来源：http://ce.huixiangedu.cn

"值: {$a}"
来源：http://wo.huixiangedu.cn

[U58] PHP：数组三件套
来源：http://tj.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zn.nicolike.cn

[U59] PHP：自定义排序
来源：http://vg.9csxet.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xh.haigaiapp.cn

[U60] PHP：JSON 编解码
来源：http://md.521024.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ha.nicolike.cn

[U61] PHP：正则
来源：http://ty.huanxung.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://db.muxihuayi.cn

[U62] PHP：日期对象
来源：http://wn.jctech888.com.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vs.jianghongdianzi.cn

[U63] PHP：文件读写
来源：http://yc.huanxung.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kj.shtwfgs.cn

[U64] PHP：目录遍历
来源：http://vv.newstarts.cn

glob("dir/*.php");  scandir("dir");
来源：http://xd.shxzskj.cn

[U65] PHP：会话
来源：http://ve.yuntaijiaju.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mk.jctech888.com.cn

[U66] PHP：设置 Cookie
来源：http://kj.shxzskj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fm.muxihuayi.cn

[U67] PHP：处理文件上传
来源：http://ja.shxzskj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://oe.huanxung.cn

[U68] PHP：PDO 连接
来源：http://le.wgjwhj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://na.521024.cn

[U69] PHP：PDO 预处理
来源：http://bp.bjjhwx.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://em.gzmigu.cn

[U70] PHP：PDO 事务
来源：http://rw.chemitech.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hm.huanxung.cn

[U71] PHP：抛出异常
来源：http://cw.colortex.cn

throw new RuntimeException("失败", 500);
来源：http://vs.bookmarksfly.cn

[U72] PHP：写错误日志
来源：http://fy.shxzukj.cn

error_log("失败: " . $e->getMessage());
来源：http://vj.asd995.cn

[U73] PHP：读取 ini 配置
来源：http://tf.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://ki.bjjhwx.cn

[U74] PHP：读取环境变量
来源：http://ig.newstarts.cn

getenv("APP_ENV") ?: "production"
来源：http://tq.haigaiapp.cn

[U75] PHP：依赖注入
来源：http://um.shxzskj.cn

composer require psr/container
来源：http://uj.newstarts.cn

[U76] PHP：简单路由
来源：http://nm.bookmarksfly.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yo.gzmigu.cn

[U77] PHP：模板渲染
来源：http://fx.nszjky.cn

composer require twig/twig
来源：http://pd.chemitech.net.cn

[U78] PHP：单元测试
来源：http://qc.colortex.cn

composer require --dev phpunit/phpunit
来源：http://hf.bjjhwx.cn

[U79] PHP：静态分析
来源：http://ei.9csxet.cn

composer require --dev phpstan/phpstan
来源：http://ke.shtwfgs.cn

[U80] PHP：代码规范修复
来源：http://hy.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://po.nszjky.cn

[U81] JS：初始化项目
来源：http://xo.jctech888.com.cn

npm init -y;  npm i express
来源：http://dq.yuexingan06.cn

[U82] JS：package.json 脚本
来源：http://tt.yuntaijiaju.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ga.hnjuh.cn

[U83] JS：ES Module 导入导出
来源：http://rv.chemitech.net.cn

export const a = 1;  import { a } from "./m.js";
来源：http://gq.yuexingan06.cn

[U84] JS：CommonJS 写法
来源：http://um.panjiajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nl.shxzukj.cn

[U85] JS：可选链
来源：http://ff.gzmigu.cn

a?.b?.c
来源：http://so.newstarts.cn

[U86] JS：空值合并
来源：http://ob.jctech888.com.cn

a ?? b
来源：http://uu.bookmarksfly.cn

[U87] JS：解构默认值
来源：http://kq.szsharing.cn

const { a = 1, b = 2 } = obj;
来源：http://bn.lnxyls.cn

[U88] JS：对象展开合并
来源：http://bd.gzmigu.cn

{ ...a, ...b }
来源：http://pe.lnxyls.cn

[U89] JS：数组去重
来源：http://vf.bjjhwx.cn

[...new Set(arr)]
来源：http://dn.szxytkj.cn

[U90] JS：数字数组排序
来源：http://lq.shxzskj.cn

[...arr].sort((a, b) => a - b)
来源：http://ua.huanxung.cn

[U91] JS：对象键值遍历
来源：http://pv.shxzukj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://to.szxytkj.cn

[U92] JS：深拷贝
来源：http://bf.lnxyls.cn

structuredClone(obj)
来源：http://uj.muxihuayi.cn

[U93] JS：模板字符串
来源：http://qe.huanxung.cn

`共 ${n} 条`
来源：http://tt.yuexingan06.cn

[U94] JS：箭头函数
来源：http://mz.wgjwhj.cn

const double = x => x * 2;
来源：http://xq.yuexingan06.cn

[U95] JS：Promise 包装
来源：http://bs.shxzskj.cn

new Promise((resolve, reject) => {})
来源：http://za.huixinmuqiang.cn

[U96] JS：async/await 与异常
来源：http://fe.521024.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ic.hahajie.cn

[U97] JS：并发请求
来源：http://oa.nicolike.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zz.yuntaijiaju.cn

[U98] JS：fetch 带 JSON
来源：http://wj.jianghongdianzi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gi.jctech888.com.cn

[U99] JS：事件监听
来源：http://kr.hnjuh.cn

el.addEventListener("click", e => {})
来源：http://jv.huanxung.cn

[U100] JS：DOM 查询
来源：http://kt.panjiajie.cn

document.querySelector(".item")
来源：http://di.nszjky.cn

[U101] JS：classList 操作
来源：http://jl.nszjky.cn

el.classList.toggle("active")
来源：http://xk.wgjwhj.cn

[U102] JS：本地存储
来源：http://ra.yuexingan06.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://oc.jianghongdianzi.cn

[U103] JS：定时器
来源：http://tj.hnjuh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nq.521024.cn

[U104] JS：防抖
来源：http://ip.hahajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://df.shxzukj.cn

[U105] JS：节流
来源：http://iv.huixinmuqiang.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ls.szxytkj.cn

[U106] JS：日期格式化
来源：http://hu.bjjhwx.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zm.shtwfgs.cn

[U107] JS：数字千分位
来源：http://qx.9csxet.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dh.shtwfgs.cn

[U108] JS：随机整数
来源：http://xu.lnxyls.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cj.shxzskj.cn

[U109] JS：数组分组
来源：http://gg.9csxet.cn

Object.groupBy(arr, x => x.type)
来源：http://jv.hahajie.cn

[U110] JS：数组分块
来源：http://sr.hahajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://li.huixinmuqiang.cn

[U111] JS：对象转 Map
来源：http://ae.shxzukj.cn

new Map(Object.entries(obj))
来源：http://th.521024.cn

[U112] JS：字符串补位
来源：http://qk.szxytkj.cn

"7".padStart(3, "0")
来源：http://dl.shtwfgs.cn

[U113] JS：正则替换全部
来源：http://sa.yuexingan06.cn

s.replaceAll("a", "b")
来源：http://ee.hahajie.cn

[U114] JS：JSON 深比较
来源：http://tn.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://kh.bjjhwx.cn

[U115] JS：生成 UUID
来源：http://ki.hahajie.cn

crypto.randomUUID()
来源：http://mn.shxzskj.cn

[U116] JS：类型检查（JSDoc）
来源：http://bo.lnxyls.cn

/** @param {string} name */ function f(name) {}
来源：http://kb.hnjuh.cn

[U117] JS：单元测试
来源：http://za.muxihuayi.cn

npm i -D vitest;  npx vitest
来源：http://fk.hnjuh.cn

[U118] JS：开发服务器
来源：http://vp.newstarts.cn

npm i -D vite;  npx vite
来源：http://um.nszjky.cn

[U119] JS：生产构建
来源：http://kl.panjiajie.cn

npx vite build
来源：http://kh.chemitech.net.cn

[U120] JS：读取环境变量（Vite）
来源：http://zu.shxzskj.cn

import.meta.env.VITE_API_URL
来源：http://tc.asd995.cn

================================================================================
来源：http://pv.yuexingan06.cn

统计汇总
来源：http://en.bookmarksfly.cn

================================================================================
来源：http://ah.nicolike.cn

按语言统计（条）：
来源：http://do.nszjky.cn

Python ......... 252
来源：http://nd.shxzukj.cn

PHP ............ 252
来源：http://jl.gzmigu.cn

JavaScript ..... 252
来源：http://af.bjjhwx.cn

TypeScript ..... 212
来源：http://hb.panjiajie.cn

Java ........... 212
来源：http://wh.nszjky.cn

Go ............. 212
来源：http://xv.nicolike.cn

Ruby ........... 212
来源：http://pz.hnjuh.cn

C# ............. 212
来源：http://lw.chemitech.net.cn

C .............. 30
来源：http://xa.9csxet.cn

C++ ............ 30
来源：http://gm.gzmigu.cn

SQL ............ 90
来源：http://pl.colortex.cn

Bash ........... 80
来源：http://lz.szxytkj.cn

Kotlin ......... 15
来源：http://ly.haigaiapp.cn

Swift .......... 15
来源：http://pj.yuexingan06.cn

Lua ............ 10
来源：http://zu.nicolike.cn

Perl ........... 10
来源：http://jq.huixinmuqiang.cn

Scala .......... 10
来源：http://mf.newstarts.cn

------------------------------------
来源：http://io.asd995.cn

合计 ........... 2106 条
来源：http://yw.bjjhwx.cn

按章节统计：
来源：http://aw.yuexingan06.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lv.shxzskj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cu.wgjwhj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ls.hnjuh.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://je.colortex.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://is.lnxyls.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kv.jctech888.com.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xd.521024.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.hahajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nu.bjjhwx.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cy.muxihuayi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nv.yuexingan06.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://it.hnjuh.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sf.lnxyls.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mr.chemitech.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://eh.nicolike.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jb.asd995.cn

Q SQL 专题                              90
来源：http://if.hnjuh.cn

R Bash 专题                             80
来源：http://rr.521024.cn

S C / C++ 专题                          60
来源：http://qj.nicolike.cn

T 其他语言补充                          60
来源：http://ho.jianghongdianzi.cn

U 高频实用片段                         120
来源：http://nm.huanxung.cn

------------------------------------
来源：http://og.jctech888.com.cn

合计                                  2106 条
来源：http://ym.newstarts.cn

--------------------------------------------------------------------------------
来源：http://tc.colortex.cn

使用提醒
来源：http://jw.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://ex.huanxung.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nx.nicolike.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pz.shxzukj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pp.hnjuh.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://rm.gzmigu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://er.lnxyls.cn

—— 文件结束 ——
来源：http://ld.gzmigu.cn

================================================================================
来源：http://nm.szsharing.cn

程序语言常见例子速查手册（2024 版）
来源：http://ws.newstarts.cn

Common Programming Examples Cheat Book
来源：http://br.gzmigu.cn

================================================================================
来源：http://wi.gzmigu.cn

【收录内容】
来源：http://cr.9csxet.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://bd.colortex.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://av.huanxung.cn

SQL · Bash · C · C++
来源：http://qs.huixiangedu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://le.chemitech.net.cn

【使用说明】
来源：http://dk.panjiajie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cp.yuexingan06.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://od.hnjuh.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ax.huanxung.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vb.nicolike.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://yx.yuntaijiaju.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hw.yuexingan06.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vw.huixiangedu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ky.shxzskj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wu.haigaiapp.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pf.muxihuayi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ta.haigaiapp.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ki.jctech888.com.cn

【文件统计】
来源：http://ei.9csxet.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kh.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://lh.jctech888.com.cn

目  录
来源：http://lr.9csxet.cn

--------------------------------------------------------------------------------
来源：http://qs.bookmarksfly.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dq.muxihuayi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zq.panjiajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cu.huixinmuqiang.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://us.shtwfgs.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://iq.chemitech.net.cn


<!-- 参考信息 -->