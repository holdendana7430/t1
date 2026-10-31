代发 wailian999

[U03] Py：加载 .env 配置
来源：http://jn.panjiajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wh.521024.cn

[U04] Py：变量调试打印
来源：http://tq.colortex.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eb.hnjuh.cn

[U05] Py：列表去重且保序
来源：http://ng.bookmarksfly.cn

list(dict.fromkeys(arr))
来源：http://gm.huixiangedu.cn

[U06] Py：合并两个字典
来源：http://yp.9csxet.cn

{**a, **b}
来源：http://wl.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://on.newstarts.cn

{v: k for k, v in d.items()}
来源：http://nc.shxzskj.cn

[U08] Py：展平二维列表
来源：http://pb.shxzskj.cn

[y for x in nested for y in x]
来源：http://rb.newstarts.cn

[U09] Py：字典取最大值的键
来源：http://rx.huanxung.cn

max(d, key=d.get)
来源：http://ji.lnxyls.cn

[U10] Py：按值排序字典
来源：http://sw.bjjhwx.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://iq.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://db.chemitech.net.cn

(x * 2 for x in arr)
来源：http://jw.nszjky.cn

[U12] Py：取出现最多的 3 个元素
来源：http://aa.bookmarksfly.cn

Counter(arr).most_common(3)
来源：http://ej.jianghongdianzi.cn

[U13] Py：固定长度队列
来源：http://bg.9csxet.cn

deque(maxlen=10)
来源：http://zi.bookmarksfly.cn

[U14] Py：分组收集到列表
来源：http://jo.colortex.cn

defaultdict(list)
来源：http://qa.muxihuayi.cn

[U15] Py：高精度计时
来源：http://nr.shxzukj.cn

t = time.perf_counter()
来源：http://hl.wgjwhj.cn

[U16] Py：命令行参数解析
来源：http://qo.nszjky.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dl.521024.cn

[U17] Py：初始化日志
来源：http://gc.wgjwhj.cn

logging.basicConfig(level=logging.INFO)
来源：http://ve.chemitech.net.cn

[U18] Py：预编译正则
来源：http://eg.shxzukj.cn

pat = re.compile(r"\d+")
来源：http://mq.lnxyls.cn

[U19] Py：正则替换带回调
来源：http://vz.haigaiapp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://iq.szxytkj.cn

[U20] Py：缓存函数结果
来源：http://ma.chemitech.net.cn

@functools.lru_cache(maxsize=None)
来源：http://al.521024.cn

[U21] Py：自定义上下文管理器
来源：http://ua.colortex.cn

@contextlib.contextmanager
来源：http://rg.hnjuh.cn

[U22] Py：矩阵转置
来源：http://iq.bjjhwx.cn

list(zip(*m))
来源：http://os.wgjwhj.cn

[U23] Py：分块读取大文件
来源：http://fj.hahajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jo.szxytkj.cn

[U24] Py：路径操作
来源：http://hc.bjjhwx.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ix.yuexingan06.cn

[U25] Py：CSV 按字典读
来源：http://en.bookmarksfly.cn

csv.DictReader(f)
来源：http://op.szxytkj.cn

[U26] Py：并发下载
来源：http://of.jianghongdianzi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zg.szxytkj.cn

[U27] Py：异步 HTTP
来源：http://ku.haigaiapp.cn

aiohttp.ClientSession() 配合 async with
来源：http://jw.shtwfgs.cn

[U28] Py：类型别名
来源：http://zn.asd995.cn

UserId = int
来源：http://wz.shxzukj.cn

[U29] Py：属性校验
来源：http://tg.yuntaijiaju.cn

@property 与 @x.setter 配合
来源：http://dq.hahajie.cn

[U30] Py：数据类
来源：http://uz.newstarts.cn

@dataclass(slots=True)
来源：http://pa.yuntaijiaju.cn

[U31] Py：单测
来源：http://nm.jctech888.com.cn

python -m pytest -q
来源：http://cn.huanxung.cn

[U32] Py：代码格式化
来源：http://oc.huixiangedu.cn

ruff format . && ruff check --fix .
来源：http://br.jctech888.com.cn

[U33] Py：打包发布
来源：http://ym.521024.cn

python -m build  （依赖 pyproject.toml）
来源：http://mh.hahajie.cn

[U34] Py：判断编码
来源：http://ug.wgjwhj.cn

chardet.detect(raw)
来源：http://wa.muxihuayi.cn

[U35] Py：发送邮件
来源：http://nr.jianghongdianzi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://js.lnxyls.cn

[U36] Py：定时任务
来源：http://av.gzmigu.cn

schedule.every(10).minutes.do(job)
来源：http://nj.bookmarksfly.cn

[U37] Py：读写 Excel
来源：http://gz.panjiajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gd.panjiajie.cn

[U38] Py：获取脚本所在目录
来源：http://jl.yuexingan06.cn

Path(__file__).resolve().parent
来源：http://oz.521024.cn

[U39] Py：判断是否在交互环境
来源：http://qq.nszjky.cn

sys.stdout.isatty()
来源：http://uo.huixiangedu.cn

[U40] Py：打印到标准错误
来源：http://bc.jianghongdianzi.cn

print("err", file=sys.stderr)
来源：http://ee.shxzskj.cn

[U41] PHP：初始化 Composer 项目
来源：http://gs.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://sj.szxytkj.cn

[U42] PHP：PSR-4 自动加载
来源：http://po.szxytkj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sh.yuntaijiaju.cn

[U43] PHP：声明命名空间
来源：http://ql.colortex.cn

namespace App\Http;
来源：http://vv.huanxung.cn

[U44] PHP：开启严格类型
来源：http://gf.shxzskj.cn

declare(strict_types=1);
来源：http://dc.yuexingan06.cn

[U45] PHP：类型声明与返回类型
来源：http://tk.bookmarksfly.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://we.lnxyls.cn

[U46] PHP：可空类型
来源：http://uj.newstarts.cn

?string $name = null
来源：http://ss.colortex.cn

[U47] PHP：联合类型
来源：http://dr.szxytkj.cn

int|string $id
来源：http://nt.wgjwhj.cn

[U48] PHP：纯枚举
来源：http://ou.shxzukj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://om.hnjuh.cn

[U49] PHP：只读属性
来源：http://vw.9csxet.cn

public readonly string $name
来源：http://ys.szsharing.cn

[U50] PHP：构造器属性提升
来源：http://ai.hnjuh.cn

public function __construct(private int $id) {}
来源：http://cs.shxzskj.cn

[U51] PHP：数组解构
来源：http://xi.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://ql.huanxung.cn

[U52] PHP：箭头函数
来源：http://ec.jianghongdianzi.cn

$double = fn($x) => $x * 2;
来源：http://rc.huixiangedu.cn

[U53] PHP：空合并运算符
来源：http://uo.asd995.cn

$v = $a ?? $b ?? "default";
来源：http://fp.521024.cn

[U54] PHP：空安全调用
来源：http://ut.9csxet.cn

$obj?->method()
来源：http://bc.bjjhwx.cn

[U55] PHP：match 表达式
来源：http://fa.hahajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ry.huixinmuqiang.cn

[U56] PHP：命名参数
来源：http://jm.lnxyls.cn

f(a: 1, b: 2)
来源：http://wu.521024.cn

[U57] PHP：字符串插值
来源：http://ue.chemitech.net.cn

"值: {$a}"
来源：http://lc.521024.cn

[U58] PHP：数组三件套
来源：http://nx.szxytkj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zz.shxzukj.cn

[U59] PHP：自定义排序
来源：http://jh.panjiajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ix.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://qe.huixinmuqiang.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dm.jianghongdianzi.cn

[U61] PHP：正则
来源：http://ov.asd995.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hj.9csxet.cn

[U62] PHP：日期对象
来源：http://bq.newstarts.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jn.asd995.cn

[U63] PHP：文件读写
来源：http://bl.hnjuh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://du.yuntaijiaju.cn

[U64] PHP：目录遍历
来源：http://ei.shxzskj.cn

glob("dir/*.php");  scandir("dir");
来源：http://df.shxzskj.cn

[U65] PHP：会话
来源：http://bd.asd995.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rr.colortex.cn

[U66] PHP：设置 Cookie
来源：http://op.bjjhwx.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ql.huanxung.cn

[U67] PHP：处理文件上传
来源：http://yn.panjiajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ss.jianghongdianzi.cn

[U68] PHP：PDO 连接
来源：http://sr.muxihuayi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cq.newstarts.cn

[U69] PHP：PDO 预处理
来源：http://is.panjiajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jm.huixiangedu.cn

[U70] PHP：PDO 事务
来源：http://kt.szxytkj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fr.wgjwhj.cn

[U71] PHP：抛出异常
来源：http://au.wgjwhj.cn

throw new RuntimeException("失败", 500);
来源：http://ti.szsharing.cn

[U72] PHP：写错误日志
来源：http://hl.bookmarksfly.cn

error_log("失败: " . $e->getMessage());
来源：http://ky.wgjwhj.cn

[U73] PHP：读取 ini 配置
来源：http://ml.huixiangedu.cn

parse_ini_file("config.ini", true)
来源：http://fj.hnjuh.cn

[U74] PHP：读取环境变量
来源：http://mp.bookmarksfly.cn

getenv("APP_ENV") ?: "production"
来源：http://zu.521024.cn

[U75] PHP：依赖注入
来源：http://tz.jianghongdianzi.cn

composer require psr/container
来源：http://ii.huanxung.cn

[U76] PHP：简单路由
来源：http://yg.nszjky.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ne.asd995.cn

[U77] PHP：模板渲染
来源：http://ce.lnxyls.cn

composer require twig/twig
来源：http://hi.haigaiapp.cn

[U78] PHP：单元测试
来源：http://hh.shxzskj.cn

composer require --dev phpunit/phpunit
来源：http://cx.haigaiapp.cn

[U79] PHP：静态分析
来源：http://as.lnxyls.cn

composer require --dev phpstan/phpstan
来源：http://ed.newstarts.cn

[U80] PHP：代码规范修复
来源：http://zm.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://yv.colortex.cn

[U81] JS：初始化项目
来源：http://fj.jctech888.com.cn

npm init -y;  npm i express
来源：http://tw.hahajie.cn

[U82] JS：package.json 脚本
来源：http://ki.huixinmuqiang.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fl.shxzskj.cn

[U83] JS：ES Module 导入导出
来源：http://yh.yuexingan06.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bs.lnxyls.cn

[U84] JS：CommonJS 写法
来源：http://ez.chemitech.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yd.hahajie.cn

[U85] JS：可选链
来源：http://qs.chemitech.net.cn

a?.b?.c
来源：http://wz.shxzukj.cn

[U86] JS：空值合并
来源：http://tj.yuntaijiaju.cn

a ?? b
来源：http://rn.yuexingan06.cn

[U87] JS：解构默认值
来源：http://jp.9csxet.cn

const { a = 1, b = 2 } = obj;
来源：http://xs.huanxung.cn

[U88] JS：对象展开合并
来源：http://oe.nszjky.cn

{ ...a, ...b }
来源：http://mt.szsharing.cn

[U89] JS：数组去重
来源：http://fh.szsharing.cn

[...new Set(arr)]
来源：http://kj.szxytkj.cn

[U90] JS：数字数组排序
来源：http://db.gzmigu.cn

[...arr].sort((a, b) => a - b)
来源：http://gk.bjjhwx.cn

[U91] JS：对象键值遍历
来源：http://ni.gzmigu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mx.huanxung.cn

[U92] JS：深拷贝
来源：http://qk.szxytkj.cn

structuredClone(obj)
来源：http://yw.wgjwhj.cn

[U93] JS：模板字符串
来源：http://sf.bjjhwx.cn

`共 ${n} 条`
来源：http://gv.hnjuh.cn

[U94] JS：箭头函数
来源：http://ou.jianghongdianzi.cn

const double = x => x * 2;
来源：http://cx.newstarts.cn

[U95] JS：Promise 包装
来源：http://mh.muxihuayi.cn

new Promise((resolve, reject) => {})
来源：http://sx.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://xo.jctech888.com.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ev.lnxyls.cn

[U97] JS：并发请求
来源：http://bq.yuexingan06.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ie.huanxung.cn

[U98] JS：fetch 带 JSON
来源：http://on.asd995.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pr.newstarts.cn

[U99] JS：事件监听
来源：http://xu.colortex.cn

el.addEventListener("click", e => {})
来源：http://yx.szxytkj.cn

[U100] JS：DOM 查询
来源：http://ta.huixiangedu.cn

document.querySelector(".item")
来源：http://uk.panjiajie.cn

[U101] JS：classList 操作
来源：http://le.yuntaijiaju.cn

el.classList.toggle("active")
来源：http://oo.asd995.cn

[U102] JS：本地存储
来源：http://lw.yuntaijiaju.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gn.nszjky.cn

[U103] JS：定时器
来源：http://fo.nicolike.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xz.muxihuayi.cn

[U104] JS：防抖
来源：http://gj.jctech888.com.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hb.9csxet.cn

[U105] JS：节流
来源：http://ck.nicolike.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fc.shxzskj.cn

[U106] JS：日期格式化
来源：http://fa.newstarts.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ii.hahajie.cn

[U107] JS：数字千分位
来源：http://bc.jctech888.com.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ey.hnjuh.cn

[U108] JS：随机整数
来源：http://os.hahajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ld.szsharing.cn

[U109] JS：数组分组
来源：http://nv.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://re.gzmigu.cn

[U110] JS：数组分块
来源：http://ou.asd995.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vr.chemitech.net.cn

[U111] JS：对象转 Map
来源：http://bs.521024.cn

new Map(Object.entries(obj))
来源：http://hu.haigaiapp.cn

[U112] JS：字符串补位
来源：http://yy.yuexingan06.cn

"7".padStart(3, "0")
来源：http://rr.szxytkj.cn

[U113] JS：正则替换全部
来源：http://hu.nszjky.cn

s.replaceAll("a", "b")
来源：http://fk.huanxung.cn

[U114] JS：JSON 深比较
来源：http://ph.chemitech.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vc.shxzukj.cn

[U115] JS：生成 UUID
来源：http://to.shxzukj.cn

crypto.randomUUID()
来源：http://vk.shxzukj.cn

[U116] JS：类型检查（JSDoc）
来源：http://sv.gzmigu.cn

/** @param {string} name */ function f(name) {}
来源：http://gj.haigaiapp.cn

[U117] JS：单元测试
来源：http://te.chemitech.net.cn

npm i -D vitest;  npx vitest
来源：http://fh.newstarts.cn

[U118] JS：开发服务器
来源：http://ot.jianghongdianzi.cn

npm i -D vite;  npx vite
来源：http://ia.szsharing.cn

[U119] JS：生产构建
来源：http://ow.shxzskj.cn

npx vite build
来源：http://ni.shtwfgs.cn

[U120] JS：读取环境变量（Vite）
来源：http://su.asd995.cn

import.meta.env.VITE_API_URL
来源：http://qq.bookmarksfly.cn

================================================================================
来源：http://pm.wgjwhj.cn

统计汇总
来源：http://mg.9csxet.cn

================================================================================
来源：http://yd.521024.cn

按语言统计（条）：
来源：http://dy.hahajie.cn

Python ......... 252
来源：http://ud.haigaiapp.cn

PHP ............ 252
来源：http://al.huixiangedu.cn

JavaScript ..... 252
来源：http://ll.nszjky.cn

TypeScript ..... 212
来源：http://wb.yuexingan06.cn

Java ........... 212
来源：http://ul.asd995.cn

Go ............. 212
来源：http://ro.shxzukj.cn

Ruby ........... 212
来源：http://mo.jianghongdianzi.cn

C# ............. 212
来源：http://ft.jctech888.com.cn

C .............. 30
来源：http://ou.nszjky.cn

C++ ............ 30
来源：http://vg.colortex.cn

SQL ............ 90
来源：http://bm.jianghongdianzi.cn

Bash ........... 80
来源：http://nf.colortex.cn

Kotlin ......... 15
来源：http://ou.jctech888.com.cn

Swift .......... 15
来源：http://ov.newstarts.cn

Lua ............ 10
来源：http://xw.gzmigu.cn

Perl ........... 10
来源：http://jw.shtwfgs.cn

Scala .......... 10
来源：http://ai.shxzukj.cn

------------------------------------
来源：http://cw.asd995.cn

合计 ........... 2106 条
来源：http://er.huanxung.cn

按章节统计：
来源：http://rd.szxytkj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://oy.jctech888.com.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fa.huanxung.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jx.shtwfgs.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qc.colortex.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://km.newstarts.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ip.shxzskj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dr.newstarts.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ht.9csxet.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kd.hnjuh.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fn.yuntaijiaju.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pl.bookmarksfly.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rz.szxytkj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nt.shxzukj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jk.szxytkj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sm.chemitech.net.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ug.asd995.cn

Q SQL 专题                              90
来源：http://uc.huixiangedu.cn

R Bash 专题                             80
来源：http://cx.9csxet.cn

S C / C++ 专题                          60
来源：http://xz.nicolike.cn

T 其他语言补充                          60
来源：http://rh.newstarts.cn

U 高频实用片段                         120
来源：http://cm.panjiajie.cn

------------------------------------
来源：http://ty.szsharing.cn

合计                                  2106 条
来源：http://ci.nicolike.cn

--------------------------------------------------------------------------------
来源：http://ew.asd995.cn

使用提醒
来源：http://gi.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://ki.9csxet.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rs.521024.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tq.chemitech.net.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zt.bjjhwx.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qi.huixinmuqiang.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://js.shxzukj.cn

—— 文件结束 ——
来源：http://wl.huixinmuqiang.cn

================================================================================
来源：http://ft.lnxyls.cn

程序语言常见例子速查手册（2024 版）
来源：http://eh.hnjuh.cn

Common Programming Examples Cheat Book
来源：http://hm.huanxung.cn

================================================================================
来源：http://ru.wgjwhj.cn

【收录内容】
来源：http://aw.nszjky.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ev.szxytkj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yx.huixinmuqiang.cn

SQL · Bash · C · C++
来源：http://vt.haigaiapp.cn


<!-- 参考信息 -->