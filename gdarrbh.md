代发 wailian999

[U03] Py：加载 .env 配置
来源：http://pf.panjiajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jq.nszjky.cn

[U04] Py：变量调试打印
来源：http://up.panjiajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ju.yuexingan06.cn

[U05] Py：列表去重且保序
来源：http://sp.521024.cn

list(dict.fromkeys(arr))
来源：http://aq.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://pi.jianghongdianzi.cn

{**a, **b}
来源：http://dg.bjjhwx.cn

[U07] Py：反转字典键值
来源：http://zx.chemitech.net.cn

{v: k for k, v in d.items()}
来源：http://nf.huixinmuqiang.cn

[U08] Py：展平二维列表
来源：http://bp.huanxung.cn

[y for x in nested for y in x]
来源：http://dj.huanxung.cn

[U09] Py：字典取最大值的键
来源：http://ny.hnjuh.cn

max(d, key=d.get)
来源：http://jh.9csxet.cn

[U10] Py：按值排序字典
来源：http://od.huixinmuqiang.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dt.jctech888.com.cn

[U11] Py：生成器表达式
来源：http://tf.hnjuh.cn

(x * 2 for x in arr)
来源：http://cz.shtwfgs.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mo.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://fe.asd995.cn

[U13] Py：固定长度队列
来源：http://wj.szxytkj.cn

deque(maxlen=10)
来源：http://ej.muxihuayi.cn

[U14] Py：分组收集到列表
来源：http://jn.muxihuayi.cn

defaultdict(list)
来源：http://wc.hahajie.cn

[U15] Py：高精度计时
来源：http://bo.chemitech.net.cn

t = time.perf_counter()
来源：http://ef.szxytkj.cn

[U16] Py：命令行参数解析
来源：http://xl.521024.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ee.newstarts.cn

[U17] Py：初始化日志
来源：http://wy.jianghongdianzi.cn

logging.basicConfig(level=logging.INFO)
来源：http://wt.nicolike.cn

[U18] Py：预编译正则
来源：http://eo.lnxyls.cn

pat = re.compile(r"\d+")
来源：http://jv.panjiajie.cn

[U19] Py：正则替换带回调
来源：http://pg.9csxet.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://iy.colortex.cn

[U20] Py：缓存函数结果
来源：http://fj.wgjwhj.cn

@functools.lru_cache(maxsize=None)
来源：http://wp.szxytkj.cn

[U21] Py：自定义上下文管理器
来源：http://ha.9csxet.cn

@contextlib.contextmanager
来源：http://kt.haigaiapp.cn

[U22] Py：矩阵转置
来源：http://zx.shxzukj.cn

list(zip(*m))
来源：http://in.bookmarksfly.cn

[U23] Py：分块读取大文件
来源：http://jx.9csxet.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kl.muxihuayi.cn

[U24] Py：路径操作
来源：http://mu.huanxung.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ax.huanxung.cn

[U25] Py：CSV 按字典读
来源：http://fy.haigaiapp.cn

csv.DictReader(f)
来源：http://dw.shxzukj.cn

[U26] Py：并发下载
来源：http://sk.muxihuayi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ui.9csxet.cn

[U27] Py：异步 HTTP
来源：http://ia.colortex.cn

aiohttp.ClientSession() 配合 async with
来源：http://pf.gzmigu.cn

[U28] Py：类型别名
来源：http://jg.szxytkj.cn

UserId = int
来源：http://wb.szsharing.cn

[U29] Py：属性校验
来源：http://pu.hnjuh.cn

@property 与 @x.setter 配合
来源：http://pj.bjjhwx.cn

[U30] Py：数据类
来源：http://lh.yuntaijiaju.cn

@dataclass(slots=True)
来源：http://lh.hnjuh.cn

[U31] Py：单测
来源：http://lb.9csxet.cn

python -m pytest -q
来源：http://io.szxytkj.cn

[U32] Py：代码格式化
来源：http://iw.hnjuh.cn

ruff format . && ruff check --fix .
来源：http://az.haigaiapp.cn

[U33] Py：打包发布
来源：http://iw.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://qq.haigaiapp.cn

[U34] Py：判断编码
来源：http://yg.shxzskj.cn

chardet.detect(raw)
来源：http://pn.asd995.cn

[U35] Py：发送邮件
来源：http://nn.bookmarksfly.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vv.szsharing.cn

[U36] Py：定时任务
来源：http://vs.521024.cn

schedule.every(10).minutes.do(job)
来源：http://sj.bookmarksfly.cn

[U37] Py：读写 Excel
来源：http://vr.yuexingan06.cn

pandas.read_excel / DataFrame.to_excel
来源：http://oy.bookmarksfly.cn

[U38] Py：获取脚本所在目录
来源：http://lk.muxihuayi.cn

Path(__file__).resolve().parent
来源：http://fc.colortex.cn

[U39] Py：判断是否在交互环境
来源：http://hn.shxzukj.cn

sys.stdout.isatty()
来源：http://xl.yuexingan06.cn

[U40] Py：打印到标准错误
来源：http://wq.shtwfgs.cn

print("err", file=sys.stderr)
来源：http://eo.asd995.cn

[U41] PHP：初始化 Composer 项目
来源：http://sp.huanxung.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bl.newstarts.cn

[U42] PHP：PSR-4 自动加载
来源：http://qi.shxzskj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ij.bjjhwx.cn

[U43] PHP：声明命名空间
来源：http://yp.huanxung.cn

namespace App\Http;
来源：http://gn.newstarts.cn

[U44] PHP：开启严格类型
来源：http://go.haigaiapp.cn

declare(strict_types=1);
来源：http://ft.haigaiapp.cn

[U45] PHP：类型声明与返回类型
来源：http://kd.asd995.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://gw.hnjuh.cn

[U46] PHP：可空类型
来源：http://nr.szsharing.cn

?string $name = null
来源：http://tr.nicolike.cn

[U47] PHP：联合类型
来源：http://bl.szsharing.cn

int|string $id
来源：http://yo.muxihuayi.cn

[U48] PHP：纯枚举
来源：http://gg.colortex.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gy.colortex.cn

[U49] PHP：只读属性
来源：http://ql.asd995.cn

public readonly string $name
来源：http://ij.shxzukj.cn

[U50] PHP：构造器属性提升
来源：http://xx.colortex.cn

public function __construct(private int $id) {}
来源：http://xy.bookmarksfly.cn

[U51] PHP：数组解构
来源：http://fa.shxzukj.cn

[$a, $b] = $arr;
来源：http://lt.muxihuayi.cn

[U52] PHP：箭头函数
来源：http://ug.bjjhwx.cn

$double = fn($x) => $x * 2;
来源：http://xg.newstarts.cn

[U53] PHP：空合并运算符
来源：http://ny.shtwfgs.cn

$v = $a ?? $b ?? "default";
来源：http://sb.szxytkj.cn

[U54] PHP：空安全调用
来源：http://jw.colortex.cn

$obj?->method()
来源：http://qz.yuexingan06.cn

[U55] PHP：match 表达式
来源：http://bj.huixiangedu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fz.asd995.cn

[U56] PHP：命名参数
来源：http://lu.colortex.cn

f(a: 1, b: 2)
来源：http://qs.muxihuayi.cn

[U57] PHP：字符串插值
来源：http://kc.chemitech.net.cn

"值: {$a}"
来源：http://uv.chemitech.net.cn

[U58] PHP：数组三件套
来源：http://il.wgjwhj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vb.yuntaijiaju.cn

[U59] PHP：自定义排序
来源：http://go.colortex.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sx.jianghongdianzi.cn

[U60] PHP：JSON 编解码
来源：http://ew.hahajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gd.yuexingan06.cn

[U61] PHP：正则
来源：http://ie.huixiangedu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qn.szxytkj.cn

[U62] PHP：日期对象
来源：http://it.asd995.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jk.hnjuh.cn

[U63] PHP：文件读写
来源：http://me.panjiajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zo.nszjky.cn

[U64] PHP：目录遍历
来源：http://ik.hahajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://gc.colortex.cn

[U65] PHP：会话
来源：http://jd.yuntaijiaju.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rf.jianghongdianzi.cn

[U66] PHP：设置 Cookie
来源：http://hz.nszjky.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ui.shxzukj.cn

[U67] PHP：处理文件上传
来源：http://ec.huixiangedu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kp.chemitech.net.cn

[U68] PHP：PDO 连接
来源：http://zn.nszjky.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ro.szsharing.cn

[U69] PHP：PDO 预处理
来源：http://oq.hnjuh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://we.huixiangedu.cn

[U70] PHP：PDO 事务
来源：http://qh.jctech888.com.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ld.nszjky.cn

[U71] PHP：抛出异常
来源：http://zd.huanxung.cn

throw new RuntimeException("失败", 500);
来源：http://ui.haigaiapp.cn

[U72] PHP：写错误日志
来源：http://wq.shxzskj.cn

error_log("失败: " . $e->getMessage());
来源：http://vn.colortex.cn

[U73] PHP：读取 ini 配置
来源：http://dr.shxzukj.cn

parse_ini_file("config.ini", true)
来源：http://vx.nicolike.cn

[U74] PHP：读取环境变量
来源：http://ee.wgjwhj.cn

getenv("APP_ENV") ?: "production"
来源：http://kt.shxzskj.cn

[U75] PHP：依赖注入
来源：http://gj.yuexingan06.cn

composer require psr/container
来源：http://jn.muxihuayi.cn

[U76] PHP：简单路由
来源：http://qq.jctech888.com.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hy.huanxung.cn

[U77] PHP：模板渲染
来源：http://pi.hahajie.cn

composer require twig/twig
来源：http://al.colortex.cn

[U78] PHP：单元测试
来源：http://mx.jianghongdianzi.cn

composer require --dev phpunit/phpunit
来源：http://wk.haigaiapp.cn

[U79] PHP：静态分析
来源：http://rf.colortex.cn

composer require --dev phpstan/phpstan
来源：http://qk.9csxet.cn

[U80] PHP：代码规范修复
来源：http://jf.asd995.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qz.9csxet.cn

[U81] JS：初始化项目
来源：http://xw.yuntaijiaju.cn

npm init -y;  npm i express
来源：http://gv.panjiajie.cn

[U82] JS：package.json 脚本
来源：http://gx.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sx.haigaiapp.cn

[U83] JS：ES Module 导入导出
来源：http://cx.lnxyls.cn

export const a = 1;  import { a } from "./m.js";
来源：http://oy.huixinmuqiang.cn

[U84] JS：CommonJS 写法
来源：http://gt.panjiajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://kc.jianghongdianzi.cn

[U85] JS：可选链
来源：http://aa.jctech888.com.cn

a?.b?.c
来源：http://vk.yuntaijiaju.cn

[U86] JS：空值合并
来源：http://gy.haigaiapp.cn

a ?? b
来源：http://xy.huanxung.cn

[U87] JS：解构默认值
来源：http://qe.huanxung.cn

const { a = 1, b = 2 } = obj;
来源：http://fr.haigaiapp.cn

[U88] JS：对象展开合并
来源：http://lt.szsharing.cn

{ ...a, ...b }
来源：http://pc.newstarts.cn

[U89] JS：数组去重
来源：http://dg.jianghongdianzi.cn

[...new Set(arr)]
来源：http://rq.szsharing.cn

[U90] JS：数字数组排序
来源：http://yj.chemitech.net.cn

[...arr].sort((a, b) => a - b)
来源：http://jc.yuntaijiaju.cn

[U91] JS：对象键值遍历
来源：http://hf.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fu.gzmigu.cn

[U92] JS：深拷贝
来源：http://fz.haigaiapp.cn

structuredClone(obj)
来源：http://lb.wgjwhj.cn

[U93] JS：模板字符串
来源：http://mz.huixiangedu.cn

`共 ${n} 条`
来源：http://sp.szxytkj.cn

[U94] JS：箭头函数
来源：http://dc.huanxung.cn

const double = x => x * 2;
来源：http://qr.bjjhwx.cn

[U95] JS：Promise 包装
来源：http://ok.jianghongdianzi.cn

new Promise((resolve, reject) => {})
来源：http://ai.huixiangedu.cn

[U96] JS：async/await 与异常
来源：http://pf.lnxyls.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://op.huixinmuqiang.cn

[U97] JS：并发请求
来源：http://lm.yuexingan06.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yv.bookmarksfly.cn

[U98] JS：fetch 带 JSON
来源：http://ef.9csxet.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gk.hahajie.cn

[U99] JS：事件监听
来源：http://yw.wgjwhj.cn

el.addEventListener("click", e => {})
来源：http://qx.shxzskj.cn

[U100] JS：DOM 查询
来源：http://ck.huixiangedu.cn

document.querySelector(".item")
来源：http://en.shxzukj.cn

[U101] JS：classList 操作
来源：http://gk.huanxung.cn

el.classList.toggle("active")
来源：http://ow.bjjhwx.cn

[U102] JS：本地存储
来源：http://bs.shtwfgs.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://yc.asd995.cn

[U103] JS：定时器
来源：http://xq.huixinmuqiang.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://le.shxzukj.cn

[U104] JS：防抖
来源：http://hm.muxihuayi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nt.hnjuh.cn

[U105] JS：节流
来源：http://db.panjiajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cr.hahajie.cn

[U106] JS：日期格式化
来源：http://ea.jianghongdianzi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ly.lnxyls.cn

[U107] JS：数字千分位
来源：http://wz.jianghongdianzi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lj.yuexingan06.cn

[U108] JS：随机整数
来源：http://oc.muxihuayi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://og.hahajie.cn

[U109] JS：数组分组
来源：http://zs.shxzskj.cn

Object.groupBy(arr, x => x.type)
来源：http://yz.yuexingan06.cn

[U110] JS：数组分块
来源：http://js.asd995.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nl.yuntaijiaju.cn

[U111] JS：对象转 Map
来源：http://qs.wgjwhj.cn

new Map(Object.entries(obj))
来源：http://wc.panjiajie.cn

[U112] JS：字符串补位
来源：http://dy.521024.cn

"7".padStart(3, "0")
来源：http://jl.huixiangedu.cn

[U113] JS：正则替换全部
来源：http://kb.9csxet.cn

s.replaceAll("a", "b")
来源：http://fq.haigaiapp.cn

[U114] JS：JSON 深比较
来源：http://yb.gzmigu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jy.shxzskj.cn

[U115] JS：生成 UUID
来源：http://bo.nicolike.cn

crypto.randomUUID()
来源：http://zm.gzmigu.cn

[U116] JS：类型检查（JSDoc）
来源：http://mm.huixinmuqiang.cn

/** @param {string} name */ function f(name) {}
来源：http://yp.shxzskj.cn

[U117] JS：单元测试
来源：http://be.gzmigu.cn

npm i -D vitest;  npx vitest
来源：http://ni.bookmarksfly.cn

[U118] JS：开发服务器
来源：http://hx.521024.cn

npm i -D vite;  npx vite
来源：http://vz.bookmarksfly.cn

[U119] JS：生产构建
来源：http://qc.huixiangedu.cn

npx vite build
来源：http://dg.hahajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://lq.nicolike.cn

import.meta.env.VITE_API_URL
来源：http://dm.yuntaijiaju.cn

================================================================================
来源：http://zs.jctech888.com.cn

统计汇总
来源：http://xr.nszjky.cn

================================================================================
来源：http://mm.shxzukj.cn

按语言统计（条）：
来源：http://ax.newstarts.cn

Python ......... 252
来源：http://nh.9csxet.cn

PHP ............ 252
来源：http://kh.shxzskj.cn

JavaScript ..... 252
来源：http://oh.bjjhwx.cn

TypeScript ..... 212
来源：http://ca.shxzskj.cn

Java ........... 212
来源：http://eq.szxytkj.cn

Go ............. 212
来源：http://nj.gzmigu.cn

Ruby ........... 212
来源：http://jv.shtwfgs.cn

C# ............. 212
来源：http://jl.gzmigu.cn

C .............. 30
来源：http://zc.haigaiapp.cn

C++ ............ 30
来源：http://de.szsharing.cn

SQL ............ 90
来源：http://yk.jctech888.com.cn

Bash ........... 80
来源：http://eu.lnxyls.cn

Kotlin ......... 15
来源：http://wg.yuntaijiaju.cn

Swift .......... 15
来源：http://ua.yuexingan06.cn

Lua ............ 10
来源：http://sr.shtwfgs.cn

Perl ........... 10
来源：http://su.shxzukj.cn

Scala .......... 10
来源：http://hz.nicolike.cn

------------------------------------
来源：http://xo.nicolike.cn

合计 ........... 2106 条
来源：http://ua.muxihuayi.cn

按章节统计：
来源：http://pb.shtwfgs.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ll.shxzukj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wv.yuntaijiaju.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hi.huixiangedu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fu.muxihuayi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ky.muxihuayi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lq.asd995.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://go.bookmarksfly.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yx.shtwfgs.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ar.haigaiapp.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://la.jianghongdianzi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tl.chemitech.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hi.huanxung.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yo.bookmarksfly.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://io.colortex.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xr.9csxet.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ch.9csxet.cn

Q SQL 专题                              90
来源：http://hz.asd995.cn

R Bash 专题                             80
来源：http://vl.huanxung.cn

S C / C++ 专题                          60
来源：http://qw.muxihuayi.cn

T 其他语言补充                          60
来源：http://ng.muxihuayi.cn

U 高频实用片段                         120
来源：http://cn.hnjuh.cn

------------------------------------
来源：http://lt.9csxet.cn

合计                                  2106 条
来源：http://pj.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://fd.yuexingan06.cn

使用提醒
来源：http://ui.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://hd.colortex.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mr.shxzskj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ur.szsharing.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ea.wgjwhj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://py.nszjky.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kw.huanxung.cn

—— 文件结束 ——
来源：http://yd.bookmarksfly.cn

================================================================================
来源：http://ps.hnjuh.cn

程序语言常见例子速查手册（2024 版）
来源：http://sz.bookmarksfly.cn

Common Programming Examples Cheat Book
来源：http://za.muxihuayi.cn

================================================================================
来源：http://vt.shxzukj.cn

【收录内容】
来源：http://op.shxzukj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ml.szxytkj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zm.colortex.cn

SQL · Bash · C · C++
来源：http://qn.shxzskj.cn


<!-- 参考信息 -->